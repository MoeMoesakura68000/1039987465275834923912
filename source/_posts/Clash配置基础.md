---
title: Clash配置文件·基础篇
date: 2021-07-01
tags: [internet]
---
*庆祝Chinese Communist Party 100th Anniversary*
<!-- more -->

Clash是一个基于规则的跨平台网络代理工具，支持诸如Shadowsocks/V2Ray/Trojan等协议，功能强大，界面美观。

与传统的网络代理工具不同，Clash需要依赖配置文件（其他软件也得用，所以这话相当于废话）但是Clash不像一般的代理工具，无法在图形化前端上直接配置，不够直观，也就劝退了一堆小白。

好在，对于机场及付费服务用户来说，只要导入机场提供的订阅Url就完事了；对于自建用户，网络上也有很多“订阅转换”工具，能够满足基本要求。

然而，如果需要更好的**个性化设置**，那么只能对Clash的配置文件进行处理才能更好的让Clash**“为我所用”**。

（Q:Clash For Windows没有中文么？A:要不第三方汉化版，要不Google翻译去，总有一款适合你）

Clash的配置文件基于Yaml格式，也正应此，配置文件可读性很高。

Yaml有如下优点：

- 大小写敏感
- 缩进只能使用空格（不能用tab）
- 以缩进指示层级关系
- 支持注释（因此比json可读性就高了不是一星半点）



闲话少叙，下面进入正题。

（Ps:本文使用模板文件来自[此处](https://hijk.pw/clash_template.yaml))

Clash配置文件分成多段，

首先是客户端设置：

```Yaml

port: 7890

socks-port: 7891

allow-lan: false

mode: Rule

log-level: info

external-controller: 127.0.0.1:9090

experimental:
  ignore-resolve-fail: true 
```



这是一些基础选项，

port与socks-port无须多论，就是本地的http及socks5代理端口（

allow-lan：允许局域网共享，设置成true时发挥作用

bind-address:当allow-lan设置true时发挥作用，设置"*"时绑定所有ip（包括v4及v6）

当然也可以单个v4或者v6。

mode：相当于Shadowrocket（或者桌面版ss/ssr/v2rayn）的模式

可选rule（按规则放行）/Global（全局走Clash）/Direct（全不走Clash）

log-level：日志选项

可选silent（完全不输出日志）/warning（仅warning等级日志）/error（仅error等级日志）/info（正常输出）/debug（调试模式/嘈杂模式，输出最详细）

external-controller：用不着不管（不是很懂）

experimental：实验性功能

ignore-resolve-fail：忽略DNS解析失败（默认开）



Hosts设置：

```Yaml
hosts:
  'mtalk.google.com': 108.177.125.188
```

这里支持通配符，但是请注意静态（即完整域名）优先级是高于使用通配符的域名的。

（即定义了*.example.com又定义了foo.example.com会优先考虑foo.example.com）
（神马？不会用Hosts？Pls Google it.）



然后是DNS设置：

```Yaml
 dns:
   enable: true 
   ipv6: false 
   listen: 0.0.0.0:53

   enhanced-mode: fake-ip
   fake-ip-filter: 
     - '*.lan'
     - localhost.ptlogin2.qq.com
     - tplogin.cn
     - routerlogin.net
   nameserver:
     - tls://dns.adguard.com:853 
     - https://1.1.1.1/dns-query
   fallback:
     - tcp://1.1.1.1
     - tcp://8.8.4.4
     - tcp://8.8.8.8
     - tcp://9.9.9.9
   fallback-filter:
     geoip: true 
     ipcidr:
       - 240.0.0.0/4

```

enhanced-mode设置为fake-ip或者redir-host模式
（以下内容来自某段网络资料）

如果是不使用 Fake-IP 的 redir 情况下，由于操作系统、浏览器或者应用程序中的任何一个缓存了 DNS 解析结果，因此 TCP 连接可以直接根据缓存的解析结果的 IP 建立，代理客户端并没有预先收到对应的 DNS question。在这种情况下，代理客户端有可能直接将这个连接视为和 IP 连接而不是和域名连接，根据域名规则的分流可能就会因此失效，不过根据 IP 分流的规则没有失效。

如果为了避免域名分流规则失效，你可以设法阻止操作系统或者浏览器缓存 DNS 解析结果，这样每次建立 TCP 连接之前都会发送 DNS question 使代理客户端探测到域名。但是这意味着每次 TCP 连接建立都需要代理客户端进行一次 DNS 解析请求（当然代理客户端可以对 DNS 解析进行缓存避免出现延时激增）。

Fake-IP 模式下，浏览器、应用程序都是对 Fake IP 发起连接，如果没有代理客户端对连接进行重新封转，那么这部分流量就不能被发往真实的目的 IP，因此所有流量都必须经过代理客户端，而根据端口、设备的分流就需要由代理客户端自己实现。（PS:坏处也是有的，如果Clash崩了你的网就全断了）

下面的fake-ip-filter：虚假ip过滤器(过滤本地地址)
这玩意的用处：比如不处理qq的快速登录（原理：QQ/TIM本地客户端打开服务器与网页交互）（腾讯远端可没这个服务器）或者Tplink路由器的Tplogin.cn，网件路由器的routerlogin.net等。

nameserver：设置DNS（支持DNS-over-TLS以及DNS-over-HTTPS）

fallback:当选择全部不可用时，故障恢复。



然后是Proxies一节（虽然鬼都不会手填）

```Yaml
proxies:

- name: "ss"
  type: ss
  server: server
  port: 443
  cipher: chacha20-ietf-poly1305
  password: "password"
  # udp: true
```

在这里我们手动定义了一个Shadowsocks服务器。

name:不用说都明白

type:ss表示是个Shadowsocks服务器。

以下都很好懂

udp:是否允许udp连接。



当然V2Ray 和Trojan也可以

```Yaml
- name: "v2ray"
  type: vmess
  server: server
  port: 443
  uuid: a3482e88-686a-4a58-8126-99c9df64b7bf
  alterId: 64
  cipher: auto
  #udp: true
  tls: true
  #skip-cert-verify: true
  network: ws
  ws-path: /path
  ws-headers: 
  Host: v2ray.com 
  
  # Trojan
- name: "trojan"
  type: trojan
  server: server
  port: 443
  password: password
  # udp: true
  # sni: example.com # aka server name
  alpn:
     - h2
     - http/1.1
  # skip-cert-verify: true
```

(友情提示：请勿打开skip-cert-verify（跳过证书验证）否则会带来严重安全性问题：比如来自GFW的MITM(中间人攻击))

（不过一般都不会手填，要不然，，）



接下来是代理组策略：

可以在此定义切换节点，它与下一节的Rule（策略）都很重要。



假设你已经在上一节（proxies）定义过了

- HK2
- HK1
- US1
- TW1
- KR1

这五个节点

Clash共四种代理方式：分别是自主选择，延迟最低，故障转移，负载均衡

自主选择：

```Yaml
proxy-groups:

- name: "自选"
  type: select
  proxies:
    - "HK1"
    - "HK2"
    - "US1"
    - "TW1"
    - "KR1"

```

name不用多讲

type为select表示自选，

proxies以下内容为存在于此组内的节点列表。

关于自选很简单，比如我们选择了HK1这个节点，那么所有分流到这组的都需要走HK1这个节点。



延迟最低：

```Yaml
- name: "LowDelay"
  type: url-test
  proxies:
    - "HK1"
    - "HK2"
    - "TW1"
  url: 'http://www.gstatic.com/generate_204'
  interval: 300

```



type:模式选择

在这里使用了url-test模式

（以下内容摘自某Clash文档）

很多刚接触这类分流软件的用户往往会犯一个**常识性错误**，那就是当他们得知自动选择是**自动选择一个最快的节点**，就很可能认为这个策略组选择的是速度最快的节点，然而显然不是如此。自动选择选出的节点是**批量测延迟过后延迟最低的那个节点**，而非许多人认为的**速度最快的节点**。clash没有内置一个策略组类型以供获取速度最快的节点。
根据我的理解，自动选择将选出**组内一个能连的上且延迟最低的节点**，这个节点不一定**速度快**，也不一定**稳定**，但是毫无疑问是这次批量测延迟中**延迟最低**的节点。

（比如iplc本来是给你打游戏用的，去下Google Drive还拉满速度岂不是多少有点那啥）

补充：这种低延迟的节点特别适合给Telegram或者Whatsapp用（尤其是语音通话的时候）；或者是游戏用（低延迟硬性要求）

比如在Telegram/Clubhouse开语音电话的时候延迟太高这语音电话就会非常不稳定（乃至听了半天一句话听不到，无疑是非常致命的）

其他选项说明：

interval：间隔时间，单位秒（s）

tolerance：批量检测完后切换节点所需的延迟差

比如：



第一次：

| HK1  | HK2  | TW1  |
| ---- | ---- | ---- |
| 300  | 350  | 345  |

(延迟，单位毫秒（ms），下同)

过了300秒，第二次检测：

| HK1  | HK2  | TW1  |
| ---- | ---- | ---- |
| 325  | 300  | 325  |

因为 325 - 300 = 25 < 75

所以不做切换（仍旧保持HK1节点）

又过了三百秒，第三次：

| HK1  | HK2  | TW1  |
| ---- | ---- | ---- |
| 400  | 275  | 310  |

因为 400 - 275 = 125 > 75

所以切换至HK2节点。



故障转移：

这个模式与自动选择逻辑相近：都用测延迟选择节点，区别在与选择模式；

```Yaml

 - name: "Fallback"
   type: fallback
   proxies:
     - "HK1"
     - "TW1"
     - "HK2"
   url: 'http://www.gstatic.com/generate_204'
   interval: 300
```

type:模式选择；这里选择了failback模式

interval:同上



说明：



第一次（当你夜里用不稳定的移动光纤家宽上网）

| HK1         | HK2  | TW1  |
| ----------- | ---- | ---- |
| No Response | 1000 | 1500 |

（延迟，单位毫秒(ms)）

此时选择HK2节点



过了三百秒第二次检测：

| TW1  | HK1  | HK2  |
| ---- | ---- | ---- |
| 450  | 375  | 1500 |

此时依旧选择HK2节点联网



又过了三百秒：

| TW1  | HK1  | HK2         |
| ---- | ---- | ----------- |
| 300  | 290  | No Response |

此时才会使用HK1节点



此模式虽有用但不一定完全可用

（延迟高到10^3ms可用吗？）



负载均衡：

与前面的工作方式也很类似，同样测延迟，但是并非只是单独一个节点，而是不同网站使用不同节点。



```Yaml
 load-balance: 
 - name: "负载均衡"
   type: load-balance
   proxies:
     - "1"
     - "2"
     - "3"
     - "4"
   url: 'http://www.gstatic.com/generate_204'
   interval: 300

```

type为load-balance表示此（负载均衡模式）

url及interval见上。

这也就是为何称作“负载均衡”：不同流量不同代理，（理论）可以减轻服务器负载。

stragery:关键参数；

选项有叁：

1. 不填
2. consistent-hashing
3. round-robin



第二项大致是对于同一个ip/网址下的请求都使用同一个节点。

（比如Google只用Hk1）



C项则是轮换；（爬虫事务有效——一直用一个节点会被拉清单的）



（友情提示：**如果你的机场禁止批量测速/测延迟，那么以上三种策略请勿使用，否则会因为违反TOS被机场拉清单**）



链式代理：

简单讲就是套娃；

比如你在校内找到了无线网，但是无线网需要认证啊，

这时候你发现不认证的时候校内有一台机器可以直连，这时候你“挪为私用”，在上面配置好Nodejs与npm，装好了SS-nodejs(ps:电信网直连npm不算慢)

可是你的机场只用v2ray啊，他不支持前置代理，这就很内啥，，

这时候Clash的链式代理就可以出场了。

```Yaml

- name: "OUTSIDE"
  type: relay
  proxies:
  - "出口"
  - "自选"
```

“出口”当然是你的自己搭建的ss

“自选”就是你选定的连接外网的节点组。



（ps:**安全性很抱歉我们不能确保，就像你搭的SS如果被学校抓了，很难说不会出一个处分。这个问题不是一个clash客户端该讨论的，而是相对于这个协议来讨论的**）

接下来是Rule部分：

这一部分可以说是Clash的关键：<br>

*Clash 是一款用Go 语言编写的、基于规则的隧道（Tunnel ）程序，它支持多种加密通信协议和跨平台*

```Yaml
Rule:
- DOMAIN-SUFFIX,google.cn,DIRECT
```

此句定义了一个规则：

DOMAIN-SUFFIX:按域名前缀匹配，此处即"*.google.cn"

DIRECT:直连

```Yaml
- DOMAIN-KEYWORD,twitter,自选
```

DOMAIN-KEYWORD:以关键词匹配，本例中匹配“twitter"（即凡是遇到twitter都走“自选”）

```Yaml
- USER-AGENT,niconico*,自选
```
USER-AGENT:用[useragent字符串](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Headers/User-Agent)进行匹配；（在本例中凡是遇到有niconico就走“自选”）


```Yaml
- DOMAIN,www.flash.cn,REJECT
```

DOMAIN:对www.flash.cn精准匹配

REJECT:拒绝连接


```Yaml
- IP-CIDR,91.108.4.0/22,LowDelay,no-resolve
```

IP-CIDR:此句为[CIDR语法](https://zh.wikipedia.org/zh-hans/%E6%97%A0%E7%B1%BB%E5%88%AB%E5%9F%9F%E9%97%B4%E8%B7%AF%E7%94%B1)
,可以使用[此计算器](https://zh.rakko.tools/tools/27/)来确定范围。

no-resolve:告诉Clash不要去尝试解析来匹配这条规则，只处理「直接IP 访问」的请求。




```Yaml

- MATCH,Final

```

该句只能放在末尾，指定漏网之🐟该走哪个代理。


通过结合以上内容可以很方便的拉出来一份代理清单。<br>
Such As Telegram：

```Yaml
- DOMAIN-SUFFIX,t.me,PROXY
- DOMAIN-SUFFIX,tlanyan.me,PROXY
- DOMAIN-SUFFIX,tdesktop.com,PROXY
- DOMAIN-SUFFIX,telegra.ph,PROXY
- DOMAIN-SUFFIX,telegram.me,PROXY
- DOMAIN-SUFFIX,telegram.org,PROXY
- DOMAIN-SUFFIX,telesco.pe,PROXY
- IP-CIDR,91.108.4.0/22,PROXY,no-resolve
- IP-CIDR,91.108.8.0/22,PROXY,no-resolve
- IP-CIDR,91.108.12.0/22,PROXY,no-resolve
- IP-CIDR,91.108.16.0/22,PROXY,no-resolve
- IP-CIDR,91.108.56.0/22,PROXY,no-resolve
- IP-CIDR,149.154.160.0/20,PROXY,no-resolve
- IP-CIDR,2001:b28:f23d::/48,PROXY,no-resolve
- IP-CIDR,2001:b28:f23f::/48,PROXY,no-resolve
- IP-CIDR,2001:67c:4e8::/48,PROXY,no-resolve
```

以上就是本期内容，我们下期再见（
