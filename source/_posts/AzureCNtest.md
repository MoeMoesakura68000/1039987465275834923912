title: Azure中国评测
date: 2020-11-10
tags: [internet]
---


[聿纾](https://www.zhihu.com/people/deepdarkfantastic)

INTP/马猴烧酒/智性恋/128的弱智/腹黑/毒舌/死傲娇/科技控/战忽时评员




## Update 2019/12/6：



# 这家默认自带 1TB 双向流量的促销没了，在流量、价格都没有优势的情况下，大伙儿都散了吧……



[价格详情 - 数据传输（Data Transfer）-Azure](https://link.zhihu.com/?target=https%3A//www.azure.cn/zh-cn/pricing/details/bandwidth)

![img](https://pic2.zhimg.com/80/v2-e8e42a94600788cd6690947c1aff0189_hd.jpg)

## Update 2019/5/2：




经评论区知友提醒，现更新 Azure 的服务价格和收费标准：

[优惠详情 | Azure](https://www.azure.cn/zh-cn/offers/ms-mc-arz-33p/)

> Azure 支持三种支付方式：支付宝，银联在线以及电汇。支付宝和银联的最低充值金额为人民币 1,000 元，电汇的最低支付金额为人民币 5,000 元。Azure 服务使用额度有效期为 12 个月。



看来 Azure 走的仍然是大客户策略，“首充 1000”的门槛，让不少个人用户望而却步，有效期只有 12 个月的订阅充值余额使用限制，这一点感觉跟众多 VPS 商或月付或季付或年付，且可以根据自己购买的产品灵活选择充值余额的计费模式相差很多。微软许多服务都有“订阅”这种概念，对于不少个人用户而言，“订阅”这种概念很不太容易理解，执行起来也比较繁琐，可能人家没花太多心思，做跟“个人”有关的生意吧。

------

## 有关中国大陆服务器流量费极其高昂的疑问和原因探究[优惠详情 | Azure](https://link.zhihu.com/?target=https%3A//www.azure.cn/zh-cn/offers/ms-mc-arz-33p/)



玩 VPS 这么久，国内的机器和国外的机器都有玩过，至今让我无法理解的是，国内的 VPS 为什么统一采用按宽带计价的方式，而且费用极高，一方面这和我国的某些特殊的互联网政策导致，过于严厉的实名制，使 Web 服务器的 80、443 端口不实名就没法使用，过于繁琐的备案流程和 Content Censorship 使众人唯恐不及，热门地域大多由一线 VPS 上垄断；另一方面，则是来自电信运营商和 policy 的垄断，国外商家和用户都进不来，竞争完全不够充分。



在“提速降费”深入人心的今天，在能说的和不能说的因素共同作用下，无论优惠喊得又多震天响，国内服务器厂商，什么阿里云、腾讯云、华为云、青云、百度云等等，全按固定入站速率算，一看带宽全1M的，真是脑子有包。



![img](https://pic2.zhimg.com/80/v2-9392c67cbdbd12cd4ae54cdab8dfdbb9_hd.jpg)<br>2M 带宽，跑你妈呢？



![img](https://pic4.zhimg.com/80/v2-224f4b354c158e4d494761afc4f75c7b_hd.jpg)<br>让 VPS 商多让点带宽，比让资本家妥协点利润还难受



![img](https://pic2.zhimg.com/80/v2-8a1d64a36d31e88590fa16f9583c15d1_hd.jpg)<br>机器不到 28元/月，流量费 980元/月，就问你怕不怕



![img](https://pic4.zhimg.com/80/v2-bd25f196c42184b2a91be2c73f8fdbd7_hd.jpg)<br>阿里云国际一键购买套餐，同样流量，就中国大陆区的流量费最贵，15.5刀/月，比除香港地区之外贵了 15.5 倍！



想在阿里云国际购买中国大陆节点的 VPS，要提交账号注册地区所在国家的签证页，除非你到过对方国家，不然也没法买。



![img](https://pic3.zhimg.com/80/v2-95d3b80b61659eb21be771c8ecf6fb06_hd.jpg)<br>香港地区的流量包价格也居高不下，不开放给国人购买，没点特别手段还弄不到，东亚真他妈内卷！



![img](https://pic4.zhimg.com/80/v2-8f9aa9158dea1a43ed0121dcfea62b93_hd.jpg)<br>凡事都喊着与国际接轨，有种你流量费也和国际接轨啊？



1M 带宽能干什么？就举个例子，一个带图片，1M 大小的网页，一百个人同时访问，每个人平均都要等待 800 秒。什么用都没有，真的，你们千万别光图什么“拼团”、“节日优惠”一窝蜂去买阿里云、腾讯云的 VPS 了，反正买的也是一堆吃灰的垃圾，对服务器来说，最重要的网络通信流畅性都无法保障，那无论是建站、还是吃鸡，都玩不起来。



这种计价方式另外一点让我无法理解的是，1M 不限量，但问题是使用互联网的主体是“人”啊，人都是有作息时间的，白天访问量自然大一些，凌晨访问量自然几乎为零，用这种“计划经济一刀切”的方式，让用户去使用所谓的“不限量”，对全网资源来说本身也是一种浪费。



所以，1M 带宽 7x24 不间断占满，每个月也要通过 300G 左右的流量，为什么不直接给用户 300G 的流量，按需跑，跑完即止呢？访问者访问量大一些的时候，流量耗得快一些，访问者访问量小一些的时候，流量耗得少一些。用户的流量耗完了，数据没法传送了，要么超出套餐的部分继续掏钱使用，要么等下个月或是升级套餐，这样既不会损害 VPS 商的利益，也不会让用户在应付服务器访问上焦头烂额，必须选择高价的大带宽不限量套餐。



卡死流量的后果，就是让不少人选择出海购买 VPS，众所周知，由于国内完全建设了一套自成体系的网络服务，并不怎么依赖国外网站的服务，不少国外网站因为一些特殊的原因，也没法在中国大陆架设本地服务器，所以中国大陆连接海外的国际出口海缆建设长期处于总量不足，人均极低的现状，这就导致出海线路常年保持“爆炸”的境地。从短期来看，这种现状似乎是无解的。



有许多同学会说，我可以利用家里的宽带，把自己家里的 NAS，或是智能家居设备，映射到公网上，方便我异地用手机、Pad、Laptop 访问啊，这样来看，我自己家里的宽带，配合路由器/软路由，就可以当一台小型的 VPS 用了，而且家用宽带蛮便宜的，上传/下载流量给的也足，比商用 VPS 划算多了。



嗯，这个主意蛮不错的，但中国幅员辽阔，不同运营商的宽带所能提供的资源可能千差万别，我敢保证，向上面这么干的同学，你至少会遭遇以下几种困难：



1. 就比如说，给公网 IP 比较大方的联通，部分地区确实是能保证单宽带用户拥有一个独立的公网 IP 地址，当然这个 IP 肯定不是独享的，所以就必须要用 [DDNS](https://link.zhihu.com/?target=https%3A//en.wikipedia.org/wiki/Dynamic_DNS)（Dynamic DNS：动态 DNS 解析），来对绑定该宽带的域名指向的 IP 地址，做实时动态解析。



我自己有玩过这个，用的是[花生壳](https://link.zhihu.com/?target=https%3A//www.oray.com/)的 DDNS 服务，一般来说，免费用户宽带重拨，等新的 IP 地址的 DNS 解析重新生效，并扩散到全网 DNS 服务器（即被我们在外网络环境的 DNS 服务器所相应），延迟大概得有 10 分钟左右吧，家用宽带一天会有若干次重拨的情况出现，也就是说平均一天大概得有近一个小时的时间是服务不可访问的状态，这样的可用性对我而言是完全不能接受的。



2. 除了联通嘛，用户数量多，内卷旺盛的电信、破烂固网铁通（移动），还有各种战五渣的长城、鹏博士等宽带，别看只花小几百就能享受 100M/年，甚至移动还天天送宽带，但这些个宽带，大多都是 [NAT 映射](https://www.zhihu.com/question/31332694)，一个公网 IP Address A:Port B 就能给某个小区里几百个用户一起用，还想独享公网 IP 地址？别想太美。



不然为什么这些宽带那么便宜，所以我就是想在公网上的其他地址，去访问家里的网络，怎么办？请出门右拐，自行购买 1M 带宽的，专门用来做[内网穿透](https://link.zhihu.com/?target=https%3A//blog.csdn.net/zhangguo5/article/details/77848658)的商用VPS。



3. 开头我们谈到中国互联网实名政策的一些弊病，以此类推，即使拥有动态独立的 IP 地址，家用宽带的 80、443 端口也是默认禁用的，即使这个宽带是你实名办理的，这两个端口也不开放给你，你去电信营业厅跟客服肛道理，人家也不会给你开放这两个端口。大部分 Web 服务都需要通过这两种端口通信，这两个端口没法用，你的宽带服务器也是个半残。



什么？又想要固定独立的 IP 地址，又想要实名认证后可开放 80、443 端口？你怎么要求这么多呢？要这要那的。行，满足你需求的产品不是没有，[电信企业宽带](https://link.zhihu.com/?target=https%3A//item.jd.com/31462416434.html)了解一下：



月付仅需 2388 哦，心动了吗？

![img](https://pic1.zhimg.com/80/v2-d65eb05920fd26deca251ac67f827268_hd.jpg)



![img](https://pic2.zhimg.com/80/v2-eaa05bc181ddf4907a09c800d8cefb25_hd.jpg)<br>200M 仅需不到 16万/年，目测国内端自带中国电信出口 CN2 精品网络，世界加钱可及



![img](https://pic1.zhimg.com/80/v2-1c42b2e1cd1e6bcc4546d9898dca87e8_hd.jpg)<br>这宽带起配都比鹤岗的房子还贵，当然，硬件资源比普通家宽好太多。啧啧，土豪随意上！



所以，你要问我，为什么国内的商用网络，服务端的上行链路为什么价格如此昂贵？（这是导致国内商用 VPS 价格高昂，带宽给得死扣的直接原因）我只是发现了这一现象，至于本源是什么？或许就是开头所说的吧。



一个封闭、自 high 的市场，注定无法诞生优质的产品。



## 中国大陆 VPS 市场的一股清流 —— 世纪互联 Azure



因为一些特殊需求（以后我会说），我的诉求很简单，就是需要一台流量充足，不限速的 VPS，难道真的没有选择了吗？



实际上，经过一番探寻，选择还是有的，就是 Azure 中国，与国际 Azure 不同的是，[中国区的 Azure](https://link.zhihu.com/?target=https%3A//www.azure.cn/zh-cn/) 是由[世纪互联](https://link.zhihu.com/?target=http%3A//www.21vianet.com/)代理运营的，微软提供技术支持。



看了一下 Azure 中国的[数据传输价格表](https://link.zhihu.com/?target=https%3A//www.azure.cn/zh-cn/pricing/details/data-transfer/)，简直是一股清流啊：

![img](https://pic3.zhimg.com/80/v2-0b0d98cb636fe99f37aa1db4c87fee32_hd.jpg)



![img](https://pic1.zhimg.com/80/v2-563a8ff07b44d8aaa06de7ee81486f2c_hd.jpg)<br>和客服沟通确认过，每个月 1TB 流量，含出站和入站



价格最低的 A0 套餐，一个月折合 81.84￥，跟阿里云腾讯云那些妖艳贱货比，最大的优势，就是附赠的 1TB 出入站流量额度，超出部分的流量传输费用，也比青云要低，这一点其实已经可以秒杀其他一众了。



## Azure 试用账户申请流程



搜遍全网，竟然找不到一家评测 Azure 的 VPS，这着实让我大跌眼镜，不如，就由我来做吧。



登陆 [Azure 首页](https://link.zhihu.com/?target=https%3A//www.azure.cn/)，申请试用：

![img](https://pic2.zhimg.com/80/v2-fc3b41b97d4f1249cad14ccc6ff505f1_hd.jpg)



填手机，接收验证码，填接收试用申请的邮箱，上传身份证照：

![img](https://pic3.zhimg.com/80/v2-2d24a91d9c811e6506a233763be00a16_hd.jpg)



然后跳到欢迎页面，填写相关信息：

![img](https://pic1.zhimg.com/80/v2-481c5e43ec4857cb7411ca67b221bc34_hd.jpg)



点击“继续”，登陆：

![img](https://pic3.zhimg.com/80/v2-c0ca30abb11c68f8c7c7de641c500cc2_hd.jpg)



如果弹出这个页面，说明实名验证还没完成，需要等待一段时间：

![img](https://pic4.zhimg.com/80/v2-d8859dc994935c2ddc6f8dd58aa01283_hd.jpg)



只要邮箱里接收到了这个邮件，就说明试用申请提交成功了：

![img](https://pic4.zhimg.com/80/v2-f2a9362d4fbef6f76fffde2cd02786c7_hd.jpg)



试用申请成功后，会自动创建 Active Directory 域：

![img](https://pic3.zhimg.com/80/v2-f5ae2d5cc69b4eb1feda6ec0b9f484a2_hd.jpg)



付款信息：地址行 1 填住的地址，市/县如实填写，省/直辖市/自治区如实填写，邮政编码必填；协议：两个都勾选。再点击“购买”按钮：

![img](https://pic3.zhimg.com/80/v2-90b1ca9cc25b7d81d1e6a456b7c385f2_hd.jpg)



如果弹出这个，点击“查看您的现有订阅”：

![img](https://pic1.zhimg.com/80/v2-48c06991165071ca1fac8f9bb31f0560_hd.jpg)



点击这个链接：

![img](https://pic1.zhimg.com/80/v2-4d9e8a4dc2b85d5ef700db89c3783bfc_hd.jpg)



扫码付款：

![img](https://pic1.zhimg.com/80/v2-2c50eec310b782f2dc1b5ddcadad9064_hd.jpg)



验证付款：

![img](https://pic2.zhimg.com/80/v2-7cd7ae915336a6bd58682168174546a1_hd.jpg)



订购成功：

![img](https://pic1.zhimg.com/80/v2-ad3f7e029c9aae63d601c075e4ebeff0_hd.jpg)



1 元试用套餐摘要：

![img](https://pic4.zhimg.com/80/v2-19c43e03d0142904dff38335fb2bcdb7_hd.jpg)



付款完成后，进入后面板，点击左侧栏“虚拟机”：

![img](https://pic2.zhimg.com/80/v2-f59aa6365b769b47d51c3b5f6390b269_hd.jpg)



点击“创建虚拟机”：

![img](https://pic2.zhimg.com/80/v2-217fb77332dd9cfb9dca1b097a7b6dc9_hd.jpg)



试用版套餐，只能最高使用 E4_v3 型号的机器：

![img](https://pic2.zhimg.com/80/v2-2816caafba2684fea84eebec1cd51189_hd.jpg)



管理员账户选择使用账户密码登陆，用户名不允许使用 root、admin、guest 等保留字，入站端口，把 HTTP、HTTPS、SSH、RDP 都勾上：

![img](https://pic4.zhimg.com/80/v2-67a07730eb1dfc32db09330f44ca135b_hd.jpg)



检查没有问题，创建：

![img](https://pic1.zhimg.com/80/v2-1f7b4a46cd10f17329b55c0779f5381c_hd.jpg)



除了虚拟机，它的磁盘、网络接口也被当做逻辑上的硬件资源被创建：

![img](https://pic4.zhimg.com/80/v2-1de3ccbd717ae547eabdf62ce338e583_hd.jpg)



创建完成后，还需要为其开放入站访问权限，点击“虚拟机” → 设置（网络）→ 添加入站端口规则：

![img](https://pic2.zhimg.com/80/v2-8ad1c06ecc1a5b99a10854f8c9641cbd_hd.jpg)



源选择“Any”，源端口范围“*”，目标“Any”，目标端口范围“1-65535”，协议“Any”，优先级和名称自定，点击“添加”，即可允许外网任何 IP 地址在任何端口对该虚拟机的访问：

![img](https://pic4.zhimg.com/80/v2-342a0d279dc923ba93715af2a81c6d17_hd.jpg)



## 基础测试



1. **秋水逸冰的测试脚本，linux 界鲁大师：**

```text
wget -qO- bench.sh | bash
```



![img](https://pic4.zhimg.com/80/v2-4a758708887fe6565d3efa3747e93aff_hd.jpg)

```text
----------------------------------------------------------------------
CPU model            : Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz
Number of cores      : 4
CPU frequency        : 2294.686 MHz
Total size of Disk   : 129.0 GB (2.4 GB Used)
Total amount of Mem  : 32169 MB (212 MB Used)
Total amount of Swap : 0 MB (0 MB Used)
System uptime        : 13 days, 1 hour 40 min
Load average         : 0.00, 0.00, 0.00
OS                   : Ubuntu 16.04.6 LTS
Arch                 : x86_64 (64 Bit)
Kernel               : 4.15.0-1041-azure
----------------------------------------------------------------------
I/O speed(1st run)   : 11.9 MB/s
I/O speed(2nd run)   : 11.9 MB/s
I/O speed(3rd run)   : 11.9 MB/s
Average I/O speed    : 11.9 MB/s
----------------------------------------------------------------------
Node Name                       IPv4 address            Download Speed
CacheFly                        204.93.150.152          22.5MB/s      
Linode, Tokyo, JP               106.187.96.148          21.4MB/s      
Linode, Singapore, SG           139.162.23.4            15.6MB/s      
Linode, London, UK              176.58.107.39           5.14MB/s       
Linode, Frankfurt, DE           139.162.130.8           6.80MB/s      
Linode, Fremont, CA             50.116.14.9             8.39MB/s      
Softlayer, Dallas, TX           173.192.68.18           5.21MB/s      
Softlayer, Seattle, WA          67.228.112.250          2.40MB/s      
Softlayer, Frankfurt, DE        159.122.69.4            604KB/s
Softlayer, Singapore, SG        119.81.28.170           2.85MB/s
Softlayer, HongKong, CN         119.81.130.170          15.3MB/s
----------------------------------------------------------------------
```



2. **UnixBench**，基本方法参照[初探CloudGarage（二）——节点网络、硬件性能测试](https://zhuanlan.zhihu.com/p/30686416)文章中的 UnixBench 部分，**如果你在执行“make”命令的时候接连二三出现了错误，按以下方式逐一排查**：



安装这些组件：

```text
apt-get install make make-guile gcc libx11-dev mesa-common-dev libgl1-mesa-dev libglu1-mesa-dev -y
```



由于 ubgears.c 组件要调用数学函数，而实际运行时找不到对应的数学函数，只需要在显示调用函数函数库即可，把 /byte-unixbench-5.1.3/UnixBench/ 目录中的 Makefile 文件中的 GL_LIBS 变量后指定 -lm 参数：

![img](https://pic3.zhimg.com/80/v2-ca1e733a87f6416b97699e48c138d15a_hd.png)



再次运行 make 命令，就不会有错误了，然后我们直接放结果：



![img](https://pic2.zhimg.com/80/v2-8c1c9ff15ecf5ab891e8ec5ae0d385c9_hd.jpg)

![img](https://pic3.zhimg.com/80/v2-143b262193d369abddb880b5368e5fae_hd.jpg)



```text
========================================================================
   BYTE UNIX Benchmarks (Version 5.1.3)

   System: testguest: GNU/Linux
   OS: GNU/Linux -- 4.15.0-1041-azure -- #45-Ubuntu SMP Fri Mar 15 14:41:00 UTC 2019
   Machine: x86_64 (x86_64)
   Language: en_US.utf8 (charmap="UTF-8", collate="UTF-8")
   CPU 0: Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz (4589.4 bogomips)
          Hyper-Threading, x86-64, MMX, Physical Address Ext, SYSENTER/SYSEXIT, SYSCALL/SYSRET, Intel virtualization
   CPU 1: Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz (4589.4 bogomips)
          Hyper-Threading, x86-64, MMX, Physical Address Ext, SYSENTER/SYSEXIT, SYSCALL/SYSRET, Intel virtualization
   CPU 2: Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz (4589.4 bogomips)
          Hyper-Threading, x86-64, MMX, Physical Address Ext, SYSENTER/SYSEXIT, SYSCALL/SYSRET, Intel virtualization
   CPU 3: Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz (4589.4 bogomips)
          Hyper-Threading, x86-64, MMX, Physical Address Ext, SYSENTER/SYSEXIT, SYSCALL/SYSRET, Intel virtualization
   07:01:14 up 13 days,  3:28,  1 user,  load average: 0.00, 0.00, 0.00; runlevel 5

------------------------------------------------------------------------
Benchmark Run: Sun May 12 2019 07:01:14 - 07:29:20
4 CPUs in system; running 1 parallel copy of tests

Dhrystone 2 using register variables       28680691.8 lps   (10.0 s, 7 samples)
Double-Precision Whetstone                     4521.6 MWIPS (9.9 s, 7 samples)
Execl Throughput                               3652.5 lps   (30.0 s, 2 samples)
File Copy 1024 bufsize 2000 maxblocks        630179.3 KBps  (30.0 s, 2 samples)
File Copy 256 bufsize 500 maxblocks          163341.5 KBps  (30.0 s, 2 samples)
File Copy 4096 bufsize 8000 maxblocks       2088191.0 KBps  (30.0 s, 2 samples)
Pipe Throughput                              919266.7 lps   (10.0 s, 7 samples)
Pipe-based Context Switching                  37560.3 lps   (10.0 s, 7 samples)
Process Creation                               6900.3 lps   (30.0 s, 2 samples)
Shell Scripts (1 concurrent)                   8868.4 lpm   (60.0 s, 2 samples)
Shell Scripts (8 concurrent)                   2130.8 lpm   (60.0 s, 2 samples)
System Call Overhead                         861117.0 lps   (10.0 s, 7 samples)

System Benchmarks Index Values               BASELINE       RESULT    INDEX
Dhrystone 2 using register variables         116700.0   28680691.8   2457.6
Double-Precision Whetstone                       55.0       4521.6    822.1
Execl Throughput                                 43.0       3652.5    849.4
File Copy 1024 bufsize 2000 maxblocks          3960.0     630179.3   1591.4
File Copy 256 bufsize 500 maxblocks            1655.0     163341.5    987.0
File Copy 4096 bufsize 8000 maxblocks          5800.0    2088191.0   3600.3
Pipe Throughput                               12440.0     919266.7    739.0
Pipe-based Context Switching                   4000.0      37560.3     93.9
Process Creation                                126.0       6900.3    547.6
Shell Scripts (1 concurrent)                     42.4       8868.4   2091.6
Shell Scripts (8 concurrent)                      6.0       2130.8   3551.3
System Call Overhead                          15000.0     861117.0    574.1
                                                                   ========
System Benchmarks Index Score                                        1038.4

------------------------------------------------------------------------
Benchmark Run: Sun May 12 2019 07:29:20 - 07:57:33
4 CPUs in system; running 4 parallel copies of tests

Dhrystone 2 using register variables       65669824.6 lps   (10.0 s, 7 samples)
Double-Precision Whetstone                    15228.2 MWIPS (10.1 s, 7 samples)
Execl Throughput                               9292.8 lps   (30.0 s, 2 samples)
File Copy 1024 bufsize 2000 maxblocks        761964.9 KBps  (30.0 s, 2 samples)
File Copy 256 bufsize 500 maxblocks          194725.9 KBps  (30.0 s, 2 samples)
File Copy 4096 bufsize 8000 maxblocks       2501797.4 KBps  (30.0 s, 2 samples)
Pipe Throughput                             2568780.6 lps   (10.0 s, 7 samples)
Pipe-based Context Switching                 409905.0 lps   (10.0 s, 7 samples)
Process Creation                              17765.3 lps   (30.0 s, 2 samples)
Shell Scripts (1 concurrent)                  16830.8 lpm   (60.0 s, 2 samples)
Shell Scripts (8 concurrent)                   2451.6 lpm   (60.0 s, 2 samples)
System Call Overhead                        2602293.6 lps   (10.0 s, 7 samples)

System Benchmarks Index Values               BASELINE       RESULT    INDEX
Dhrystone 2 using register variables         116700.0   65669824.6   5627.2
Double-Precision Whetstone                       55.0      15228.2   2768.8
Execl Throughput                                 43.0       9292.8   2161.1
File Copy 1024 bufsize 2000 maxblocks          3960.0     761964.9   1924.2
File Copy 256 bufsize 500 maxblocks            1655.0     194725.9   1176.6
File Copy 4096 bufsize 8000 maxblocks          5800.0    2501797.4   4313.4
Pipe Throughput                               12440.0    2568780.6   2064.9
Pipe-based Context Switching                   4000.0     409905.0   1024.8
Process Creation                                126.0      17765.3   1409.9
Shell Scripts (1 concurrent)                     42.4      16830.8   3969.5
Shell Scripts (8 concurrent)                      6.0       2451.6   4086.1
System Call Overhead                          15000.0    2602293.6   1734.9
                                                                   ========
System Benchmarks Index Score                                        2344.7
```



3. **总体点评：**

- 这个 I/O…… 有点惨，12MB/s 的读写速度，跟我多年珍藏的 USB 2.0 U 盘表现差不多，怎么能差成这样，这数据对得起“标准 SSD”名号吗？难不成 Azure 的母鸡用的 SSD 是传说中的“[黑片](https://zhuanlan.zhihu.com/p/54722345)”颗粒？

![img](https://pic2.zhimg.com/80/v2-ada4af3d5833c0a0a00d1e7f69b851f5_hd.jpg)



- [E5-2673](https://link.zhihu.com/?target=https%3A//ark.intel.com/content/www/us/en/ark/products/79930/intel-xeon-processor-e5-2673-v2-25m-cache-3-30-ghz.html)，6 年前的 Ivy Bridge 产品，也蛮老的了，不能要求过高，不过好歹 4 核，配合 4GB 的内存，当中型企业的 Web 服务器用，性能不差；
- 下载速度嘛，距离中国最近的 [cachefly](https://link.zhihu.com/?target=https%3A//www.cachefly.com/) 亚太地区节点的速度还行，差不多 200 - 300 Mbps 带宽的水准，没有 CN2 加持的中美、中欧速度就一般般了。不过有一点没搞太懂，就是 40MB/s 的下载速度，这 SSD 的 I/O 顶不住啊，可能脚本用的是把内存虚拟成临时硬盘做的下载速度测试吧，这样不会因为 I/O 的性能限制而影响了带宽测试的真实水准，实际应用中，就这惨不忍睹的 I/O 速度，网口再快也真没啥用了……
- UnixBench 里呈现的结果，文件拷贝项（I/O）显示的水平并不比我之前测的 CloudGarage 的性能差太多，难道是秋水逸冰的脚本数据有误？这个确实搞不太清楚。



## 网络测试



出于安全问题，Azure **禁用了所有基于 ICMP 协议的通信**，所以我们必须使用 TCP 协议来测试 PING 值和 TraceRoute 值，**如果你所使用的 VPS 服务商也做了类似的限制，基本方法是共通的，请触类旁通，活学活用**。



1. **TCP 版路由追踪功能的使用：**



Linux 下的 TraceRoute 工具依旧属 besttrace 最好用，部署方式请参见：[初探CloudGarage（二）——节点网络、硬件性能测试](https://zhuanlan.zhihu.com/p/30686416)中“测试”一节的“2.回程现路”小节。

如果需要强制使用 TCP 协议进行 TraceRoute 测试，需要在命令中附加 -T 参数：

```text
./besttrace -q1 -T -g cn 42.159.136.107
```

如果需要输出 json 格式的数据，需要在命令中附加 -J 参数：

```text
./besttrace -q1 -J -T -g cn 42.159.136.107
```



如非特殊情况，我们站在该台测试机器的视角，默认“回程”即其他服务器至本测试服务器的路由，“去程”即本测试服务器至其他服务器的路由，看一看 Azure 上海节点的通信线路怎么样。



2. **TraceRoute 回程测试：**



- 搬瓦工 CN2 GT DC8洛杉矶 → Azure 上海：

![img](https://pic1.zhimg.com/80/v2-15d4e6d2b9fe73ffa04911fb1207f648_hd.jpg)
按搬瓦工这个套餐的描述（Direct route via CN2 and China Unicom），应该双网（电信/联通）走CN2 GT的，实际上是动态从北京/广州联通返回，就是不直接从上海回来。



格式化 Json 数据：

```text
{"trace":"42.159.136.107","response":"42.159.136.107","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"192.254.81.134","host":"te-2-0-6.cr2.lax2.us.zenlayer.net","location":"美国 加利福尼亚州 洛杉矶 zenlayer.com","as":"AS62610","elapse":5.26}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"192.254.84.86","location":"ZENLAYER.COM 骨干网 zenlayer.com","as":"AS62610","elapse":1.17}]}
{"hop":5,"data":[{"ip":"192.254.84.86","location":"ZENLAYER.COM 骨干网 zenlayer.com","as":"AS62610","elapse":1.57}]}
{"hop":6,"data":[{"ip":"219.158.104.17","location":"中国 北京 联通","as":"AS4837","elapse":162.76}]}
{"hop":7,"data":[{"ip":"219.158.3.145","location":"中国 北京 联通","as":"AS4837","elapse":162.95}]}
{"hop":8,"data":[{"ip":"219.158.3.145","location":"中国 北京 联通","as":"AS4837","elapse":160.32}]}
{"hop":9,"data":[{"ip":"219.158.6.170","location":"中国 上海 联通","as":"AS4837","elapse":187.44}]}
{"hop":10,"data":[{"ip":"139.226.210.62","location":"中国 上海 联通","as":"AS17621","elapse":181.84}]}
{"hop":11,"data":[{"ip":"139.226.210.62","location":"中国 上海 联通","as":"AS17621","elapse":185.96}]}
{"hop":12,"data":[{"ip":"112.64.245.230","location":"中国 上海 联通","as":"AS17621","elapse":181.48}]}
{"hop":13,"data":[{"ip":"139.226.225.118","location":"中国 上海 联通","as":"AS17621","elapse":182.5}]}
{"hop":14,"data":[{"ip":"42.159.128.85","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":158.71}]}
{"hop":15,"data":[{"ip":"*"}]}
{"hop":16,"data":[{"ip":"*"}]}
{"hop":17,"data":[{"ip":"*"}]}
{"hop":18,"data":[{"ip":"*"}]}
{"hop":19,"data":[{"ip":"*"}]}
{"hop":20,"data":[{"ip":"*"}]}
{"hop":21,"data":[{"ip":"*"}]}
{"hop":22,"data":[{"ip":"*"}]}
{"hop":23,"data":[{"ip":"*"}]}
{"hop":24,"data":[{"ip":"*"}]}
{"hop":25,"data":[{"ip":"42.159.136.107","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":159.58}]}
```



- 搬瓦工 QNET DC2 洛杉矶 → Azure 上海

![img](https://pic3.zhimg.com/80/v2-f3233d2335ee67344ab186a92c9e6cd2_hd.jpg)
DC2 是搬瓦工很老的一个机房了，动态从北京/广州联通返回 Azure，就是不直接从上海回来，众所周知，联通线路因为总出口量仅次于电信，且用户数比电信少很多，所以人均出口量比电信要宽裕，拥堵和丢包状况比 CN1 网络稍微好一些，不如纯 CN2。



格式化 Json 数据：

```text
{"trace":"42.159.136.107","response":"42.159.136.107","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"*"}]}
{"hop":3,"data":[{"ip":"69.12.70.234","host":"lax1-fatpipe-1.it7.net","location":"美国 加利福尼亚州 洛杉矶 quadranet.com","as":"AS8100","elapse":0.41}]}
{"hop":4,"data":[{"ip":"204.152.204.2","host":"china.unicom","location":"美国 加利福尼亚州 洛杉矶 quadranet.com","as":"AS8100","elapse":0.92}]}
{"hop":5,"data":[{"ip":"207.254.191.102","location":"美国 加利福尼亚州 洛杉矶 chinaunicom.com","as":"AS19174","elapse":3.98}]}
{"hop":6,"data":[{"ip":"207.254.191.89","location":"美国 加利福尼亚州 洛杉矶 chinaunicom.com","as":"AS19174","elapse":0.99}]}
{"hop":7,"data":[{"ip":"219.158.3.181","location":"中国 北京 联通","as":"AS4837","elapse":153.18}]}
{"hop":8,"data":[{"ip":"219.158.5.157","location":"中国 北京 联通","as":"AS4837","elapse":147.78}]}
{"hop":9,"data":[{"ip":"219.158.6.170","location":"中国 上海 联通","as":"AS4837","elapse":170.32}]}
{"hop":10,"data":[{"ip":"219.158.6.245","location":"中国 上海 联通","as":"AS4837","elapse":171.94}]}
{"hop":11,"data":[{"ip":"139.226.214.38","location":"中国 上海 联通","as":"AS17621","elapse":176.73}]}
{"hop":12,"data":[{"ip":"139.226.214.38","location":"中国 上海 联通","as":"AS17621","elapse":171.41}]}
{"hop":13,"data":[{"ip":"*"}]}
{"hop":14,"data":[{"ip":"42.159.128.85","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":148.81}]}
{"hop":15,"data":[{"ip":"42.159.128.85","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":148.73}]}
{"hop":16,"data":[{"ip":"*"}]}
{"hop":17,"data":[{"ip":"*"}]}
{"hop":18,"data":[{"ip":"*"}]}
{"hop":19,"data":[{"ip":"*"}]}
{"hop":20,"data":[{"ip":"*"}]}
{"hop":21,"data":[{"ip":"*"}]}
{"hop":22,"data":[{"ip":"*"}]}
{"hop":23,"data":[{"ip":"*"}]}
{"hop":24,"data":[{"ip":"42.159.136.107","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":149.64}]}
```



- 搬瓦工 CN2 GIA DC9 洛杉矶 → Azure 上海：

![img](https://pic1.zhimg.com/80/v2-a485eab72050bece593c1a78a9dc21bc_hd.jpg)
这才是中美之间真正意义上的高速直连，全程 CN2 网络，经过的路由节点数量少，延迟低，且 CN2 网络的负载不高，丢包少，质量非常好，全天不炸，价格你们也高攀不起。



格式化 Json 数据：

```text
{"trace":"42.159.136.107","response":"42.159.136.107","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"218.30.49.97","location":"美国 ctamericas.com","as":"AS4134","elapse":1.85}]}
{"hop":3,"data":[{"ip":"59.43.189.33","location":"中国 上海 电信","as":"*","elapse":127.64}]}
{"hop":4,"data":[{"ip":"59.43.182.182","location":"中国 上海 电信","as":"*","elapse":132.38}]}
{"hop":5,"data":[{"ip":"59.43.138.53","location":"中国 上海 电信","as":"*","elapse":128.99}]}
{"hop":6,"data":[{"ip":"59.43.138.49","location":"中国 上海 电信","as":"*","elapse":142.2}]}
{"hop":7,"data":[{"ip":"101.95.88.58","location":"中国 上海 电信","as":"AS4812","elapse":134.19}]}
{"hop":8,"data":[{"ip":"101.95.207.102","location":"中国 上海 电信","as":"AS4812","elapse":132.29}]}
{"hop":9,"data":[{"ip":"180.153.24.106","location":"中国 上海 电信","as":"AS4812","elapse":128.34}]}
{"hop":10,"data":[{"ip":"*"}]}
{"hop":11,"data":[{"ip":"*"}]}
{"hop":12,"data":[{"ip":"*"}]}
{"hop":13,"data":[{"ip":"*"}]}
{"hop":14,"data":[{"ip":"*"}]}
{"hop":15,"data":[{"ip":"*"}]}
{"hop":16,"data":[{"ip":"*"}]}
{"hop":17,"data":[{"ip":"*"}]}
{"hop":18,"data":[{"ip":"*"}]}
{"hop":19,"data":[{"ip":"42.159.136.107","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":128.8}]}
```



- 标准互联 CN2 GIA 圣何塞 → Azure 上海：

![img](https://pic4.zhimg.com/80/v2-dbe437dc9a6c0f43079813b0d1304193_hd.jpg)
标准互联的 CN2 GIA 线路还是不错的，电信和联通线路都走 CN2，移动直连，就是母鸡超售有点严重，高峰期磁盘 I/O 会低得令人发指。



格式化 Json 数据：

```text
{"trace":"42.159.136.107","response":"42.159.136.107","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"104.233.238.158","location":"美国 加利福尼亚州 圣何塞 petaexpress.com","as":"AS54600","elapse":8.1}]}
{"hop":2,"data":[{"ip":"10.255.255.100","location":"局域网","as":"*","elapse":2.1}]}
{"hop":3,"data":[{"ip":"218.30.49.73","location":"美国 ctamericas.com","as":"AS4134","elapse":17.34}]}
{"hop":4,"data":[{"ip":"59.43.182.142","location":"中国 上海 电信","as":"*","elapse":157.78}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"59.43.138.49","location":"中国 上海 电信","as":"*","elapse":151.55}]}
{"hop":7,"data":[{"ip":"101.95.88.58","location":"中国 上海 电信","as":"AS4812","elapse":137.04}]}
{"hop":8,"data":[{"ip":"124.74.166.138","location":"中国 上海 电信","as":"AS4812","elapse":148.94}]}
{"hop":9,"data":[{"ip":"124.74.232.238","location":"中国 上海 电信","as":"AS4812","elapse":137.95}]}
{"hop":10,"data":[{"ip":"180.153.24.102","location":"中国 上海 电信","as":"AS4812","elapse":148.16}]}
{"hop":11,"data":[{"ip":"*"}]}
{"hop":12,"data":[{"ip":"*"}]}
{"hop":13,"data":[{"ip":"*"}]}
{"hop":14,"data":[{"ip":"*"}]}
{"hop":15,"data":[{"ip":"*"}]}
{"hop":16,"data":[{"ip":"*"}]}
{"hop":17,"data":[{"ip":"*"}]}
{"hop":18,"data":[{"ip":"*"}]}
{"hop":19,"data":[{"ip":"*"}]}
{"hop":20,"data":[{"ip":"42.159.136.107","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":138.38}]}
```



- 阿里云国际香港 → Azure 上海：

![img](https://pic3.zhimg.com/80/v2-b97e49f471531b098e50c6f0d3db16e6_hd.jpg)
很意外地，竟然不是 CN2，而是走 PCCW 线路，电信家用宽带去回都是走纯 CN2 GIA 的，即使这样，炸的概率比阿里云轻量要低。



格式化 Json 数据：

```text
{"trace":"42.159.136.107","response":"42.159.136.107","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"11.52.240.49","location":"美国 defense.gov","as":"*","elapse":0.69}]}
{"hop":3,"data":[{"ip":"11.52.240.2","location":"美国 defense.gov","as":"*","elapse":5.14}]}
{"hop":4,"data":[{"ip":"*"}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"63.217.237.157","host":"ten-0-6-0-13.246.br03.hkg12.pccwbtn.net","location":"中国 香港 pccw.com","as":"AS3491","elapse":1.51}]}
{"hop":7,"data":[{"ip":"63.223.15.174","host":"TenGE0-5-0-0.br02.hkg15.pccwbtn.net","location":"中国 香港 pccw.com","as":"AS3491","elapse":2.59}]}
{"hop":8,"data":[{"ip":"202.97.121.230","location":"中国 香港 电信","as":"AS4134","elapse":2.73}]}
{"hop":9,"data":[{"ip":"202.97.121.230","location":"中国 香港 电信","as":"AS4134","elapse":2.38}]}
{"hop":10,"data":[{"ip":"202.97.6.49","location":"中国 上海 电信","as":"AS4134","elapse":34.87}]}
{"hop":11,"data":[{"ip":"202.97.94.201","location":"中国 上海 电信","as":"AS4134","elapse":89.15}]}
{"hop":12,"data":[{"ip":"202.97.94.201","location":"中国 上海 电信","as":"AS4134","elapse":68.57}]}
{"hop":13,"data":[{"ip":"101.95.120.193","location":"中国 上海 电信","as":"AS4812","elapse":29.98}]}
{"hop":14,"data":[{"ip":"101.95.120.193","location":"中国 上海 电信","as":"AS4812","elapse":27.68}]}
{"hop":15,"data":[{"ip":"101.95.225.218","location":"中国 上海 电信","as":"AS4812","elapse":28.81}]}
{"hop":16,"data":[{"ip":"101.95.225.218","location":"中国 上海 电信","as":"AS4812","elapse":28.08}]}
{"hop":17,"data":[{"ip":"180.153.24.106","location":"中国 上海 电信","as":"AS4812","elapse":29.69}]}
{"hop":18,"data":[{"ip":"*"}]}
{"hop":19,"data":[{"ip":"*"}]}
{"hop":20,"data":[{"ip":"*"}]}
{"hop":21,"data":[{"ip":"*"}]}
{"hop":22,"data":[{"ip":"*"}]}
{"hop":23,"data":[{"ip":"*"}]}
{"hop":24,"data":[{"ip":"*"}]}
{"hop":25,"data":[{"ip":"*"}]}
{"hop":26,"data":[{"ip":"*"}]}
{"hop":27,"data":[{"ip":"42.159.136.107","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":29.41}]}
```



- 阿里云轻量香港 → Azure 上海：

![img](https://pic2.zhimg.com/80/v2-2fde818d1aae04646fe4a0cd44b7150d_hd.jpg)
回程经过的路由和阿里云国际香港差不多，也是 PCCW，但延迟和丢包总是比阿里云国际香港要高，白天还好，从下午就开始炸，炸的时候上150ms都很常见。



格式化 Json 数据：

```text
{"trace":"42.159.136.107","response":"42.159.136.107","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"11.56.8.69","location":"美国 defense.gov","as":"*","elapse":0.22}]}
{"hop":3,"data":[{"ip":"11.52.252.14","location":"美国 defense.gov","as":"*","elapse":4.98}]}
{"hop":4,"data":[{"ip":"11.131.180.242","location":"美国 defense.gov","as":"*","elapse":1.44}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"63.216.176.73","host":"63-216-176-73.static.pccwglobal.net","location":"中国 香港 pccw.com","as":"AS3491","elapse":1.44}]}
{"hop":7,"data":[{"ip":"63.223.15.190","host":"HundredGE0-6-0-0.br02.hkg15.pccwbtn.net","location":"中国 香港 pccw.com","as":"AS3491","elapse":1.97}]}
{"hop":8,"data":[{"ip":"63.223.17.94","host":"HundredGE0-7-0-0.br02.hkg15.pccwbtn.net","location":"中国 香港 pccw.com","as":"AS3491","elapse":1.93}]}
{"hop":9,"data":[{"ip":"202.97.121.230","location":"中国 香港 电信","as":"AS4134","elapse":56.65}]}
{"hop":10,"data":[{"ip":"202.97.61.61","location":"中国 上海 电信","as":"AS4134","elapse":56.54}]}
{"hop":11,"data":[{"ip":"202.97.61.61","location":"中国 上海 电信","as":"AS4134","elapse":54.26}]}
{"hop":12,"data":[{"ip":"202.97.90.34","location":"中国 上海 电信","as":"AS4134","elapse":55.08}]}
{"hop":13,"data":[{"ip":"202.97.50.149","location":"中国 上海 电信","as":"AS4134","elapse":65.88}]}
{"hop":14,"data":[{"ip":"101.95.206.22","location":"中国 上海 电信","as":"AS4812","elapse":95.2}]}
{"hop":15,"data":[{"ip":"101.95.206.10","location":"中国 上海 电信","as":"AS4812","elapse":67.59}]}
{"hop":16,"data":[{"ip":"124.74.232.62","location":"中国 上海 电信","as":"AS4812","elapse":58.7}]}
{"hop":17,"data":[{"ip":"180.153.24.102","location":"中国 上海 电信","as":"AS4812","elapse":61.97}]}
{"hop":18,"data":[{"ip":"*"}]}
{"hop":19,"data":[{"ip":"*"}]}
{"hop":20,"data":[{"ip":"*"}]}
{"hop":21,"data":[{"ip":"*"}]}
{"hop":22,"data":[{"ip":"*"}]}
{"hop":23,"data":[{"ip":"*"}]}
{"hop":24,"data":[{"ip":"*"}]}
{"hop":25,"data":[{"ip":"*"}]}
{"hop":26,"data":[{"ip":"*"}]}
{"hop":27,"data":[{"ip":"42.159.136.107","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":57.48}]}
```



- Cloud Garage 东京 → Azure 上海：

![img](https://pic2.zhimg.com/80/v2-beb588ce412389bb49b9bad71d87c2e1_hd.jpg)
走的是动态路由，KDDI/IIJ 混着跑，白天还好，从下午就开始炸，炸的时候上 200ms 都很常见，总体质量比 NTT 线路略好一丁点。



格式化 Json 数据：

```text
{"trace":"42.159.136.107","response":"42.159.136.107","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"192.168.0.1","location":"局域网","as":"*","elapse":0.45}]}
{"hop":2,"data":[{"ip":"169.254.30.253","location":"本地链路","as":"*","elapse":1.82}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"203.104.199.20","host":"203-104-199-20.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":1.09}]}
{"hop":5,"data":[{"ip":"203.174.64.5","host":"203-174-64-5.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":0.62}]}
{"hop":6,"data":[{"ip":"203.174.66.249","host":"203-174-66-249.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":0.89}]}
{"hop":7,"data":[{"ip":"125.6.112.1","host":"125-6-112-1.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":18.01}]}
{"hop":8,"data":[{"ip":"203.174.64.94","host":"ex-mx480-1-ae0.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":0.9}]}
{"hop":9,"data":[{"ip":"210.130.134.53","location":"日本 iij.ad.jp","as":"AS2497","elapse":1.32}]}
{"hop":10,"data":[{"ip":"58.138.105.53","host":"tky008bb01.IIJ.Net","location":"日本 东京都 东京 iij.ad.jp","as":"AS2497","elapse":1.85}]}
{"hop":11,"data":[{"ip":"27.85.134.162","location":"日本 东京都 kddi.com","as":"AS2516","elapse":1.2}]}
{"hop":12,"data":[{"ip":"202.232.1.14","location":"日本 iij.ad.jp","as":"AS2497","elapse":2.44}]}
{"hop":13,"data":[{"ip":"63.218.147.13","host":"63-218-147-13.static.pccwglobal.net","location":"日本 东京都 东京 pccw.com","as":"AS3491","elapse":2.05}]}
{"hop":14,"data":[{"ip":"63.223.17.94","host":"HundredGE0-7-0-0.br02.hkg15.pccwbtn.net","location":"中国 香港 pccw.com","as":"AS3491","elapse":48.81}]}
{"hop":15,"data":[{"ip":"202.97.121.230","location":"中国 香港 电信","as":"AS4134","elapse":55.83}]}
{"hop":16,"data":[{"ip":"202.97.121.230","location":"中国 香港 电信","as":"AS4134","elapse":56.02}]}
{"hop":17,"data":[{"ip":"202.97.6.49","location":"中国 上海 电信","as":"AS4134","elapse":57.72}]}
{"hop":18,"data":[{"ip":"202.97.6.49","location":"中国 上海 电信","as":"AS4134","elapse":63.34}]}
{"hop":19,"data":[{"ip":"202.97.57.158","location":"中国 上海 电信","as":"AS4134","elapse":60.25}]}
{"hop":20,"data":[{"ip":"61.152.86.41","location":"中国 上海 电信","as":"AS4812","elapse":59.47}]}
{"hop":21,"data":[{"ip":"61.152.86.41","location":"中国 上海 电信","as":"AS4812","elapse":57.51}]}
{"hop":22,"data":[{"ip":"101.95.207.254","location":"中国 上海 电信","as":"AS4812","elapse":60.24}]}
{"hop":23,"data":[{"ip":"124.74.232.62","location":"中国 上海 电信","as":"AS4812","elapse":57.74}]}
{"hop":24,"data":[{"ip":"180.153.24.106","location":"中国 上海 电信","as":"AS4812","elapse":58.15}]}
{"hop":25,"data":[{"ip":"*"}]}
{"hop":26,"data":[{"ip":"*"}]}
{"hop":27,"data":[{"ip":"*"}]}
{"hop":28,"data":[{"ip":"*"}]}
{"hop":29,"data":[{"ip":"*"}]}
{"hop":30,"data":[{"ip":"*"}]}
```



- Host Hatch 斯德哥尔摩 → Azure 上海：

![img](https://pic1.zhimg.com/80/v2-b3491e0f008c1911611a3ccc548cb4dc_hd.jpg)
不像其他东南亚国家一样，出去了要从美国过去，中欧之间有直连的专线，且中欧 CN2 的网络比中美 CN2 更贵，这条线就是普通的 163 网。



格式化 Json 数据：

```text
{"trace":"42.159.136.107","response":"42.159.136.107","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"185.213.24.1","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 hosthatch.com","as":"AS63473","elapse":4.2}]}
{"hop":2,"data":[{"ip":"80.67.0.168","host":"vl-121.pe1.sto1.se.portlane.net","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 portlane.com","as":"AS42708","elapse":0.37}]}
{"hop":3,"data":[{"ip":"80.67.4.192","host":"be-4.cr1.sto1.se.portlane.net","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 portlane.com","as":"AS42708","elapse":0.58}]}
{"hop":4,"data":[{"ip":"80.67.4.227","host":"be-1.cr2.sto1.se.portlane.net","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 portlane.com","as":"AS42708","elapse":0.76}]}
{"hop":5,"data":[{"ip":"62.115.61.246","host":"glesys-ic-341360-s-b5.c.telia.net","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 telia.com","as":"AS1299","elapse":26.69}]}
{"hop":6,"data":[{"ip":"62.115.114.166","host":"s-bb3-link.telia.net","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 telia.com","as":"AS1299","elapse":5.87}]}
{"hop":7,"data":[{"ip":"62.115.138.237","host":"ffm-bb3-link.telia.net","location":"德国 黑森州 法兰克福 telia.com","as":"AS1299","elapse":25.61}]}
{"hop":8,"data":[{"ip":"62.115.120.0","host":"ffm-b4-link.telia.net","location":"德国 黑森州 法兰克福 telia.com","as":"AS1299","elapse":23.05}]}
{"hop":9,"data":[{"ip":"213.248.68.71","host":"pccw-ic-319976-ffm-b4.c.telia.net","location":"德国 黑森州 法兰克福 telia.com","as":"AS1299","elapse":50.55}]}
{"hop":10,"data":[{"ip":"63.223.15.98","host":"tenge0-0-0-22.br02.hkg15.pccwbtn.net","location":"中国 香港 pccw.com","as":"AS3491","elapse":326.6}]}
{"hop":11,"data":[{"ip":"202.97.121.230","location":"中国 香港 电信","as":"AS4134","elapse":315.41}]}
{"hop":12,"data":[{"ip":"202.97.121.229","location":"中国 香港 电信","as":"AS4134","elapse":316.49}]}
{"hop":13,"data":[{"ip":"202.97.63.1","location":"中国 上海 电信","as":"AS4134","elapse":296.49}]}
{"hop":14,"data":[{"ip":"202.97.90.30","location":"中国 上海 电信","as":"AS4134","elapse":288.08}]}
{"hop":15,"data":[{"ip":"202.97.50.141","location":"中国 上海 电信","as":"AS4134","elapse":286.28}]}
{"hop":16,"data":[{"ip":"101.95.120.157","location":"中国 上海 电信","as":"AS4812","elapse":314.69}]}
{"hop":17,"data":[{"ip":"101.95.207.254","location":"中国 上海 电信","as":"AS4812","elapse":327.58}]}
{"hop":18,"data":[{"ip":"101.95.225.218","location":"中国 上海 电信","as":"AS4812","elapse":282.05}]}
{"hop":19,"data":[{"ip":"180.153.24.110","location":"中国 上海 电信","as":"AS4812","elapse":275.13}]}
{"hop":20,"data":[{"ip":"*"}]}
{"hop":21,"data":[{"ip":"*"}]}
{"hop":22,"data":[{"ip":"*"}]}
{"hop":23,"data":[{"ip":"*"}]}
{"hop":24,"data":[{"ip":"*"}]}
{"hop":25,"data":[{"ip":"*"}]}
{"hop":26,"data":[{"ip":"*"}]}
{"hop":27,"data":[{"ip":"*"}]}
{"hop":28,"data":[{"ip":"*"}]}
{"hop":29,"data":[{"ip":"42.159.136.107","location":"中国 上海 microsoft.com 电信/联通/移动","as":"AS58593","elapse":273.5}]}
```



3. **TraceRoute 去程测试：**



- Azure 上海 → 搬瓦工 CN2 GT DC8洛杉矶：

![img](https://pic3.zhimg.com/80/v2-7033d8575446edaed925003a52c11bce_hd.jpg)
标准 CN2 GT 应有的表现，表现为国内电信网络的机器走向出海口的一段，一定是电信 163 网，随后走太平洋的海底光缆，才并入到 CN2 网络，最终到达目的地，表现跟CN2 GIA 相比，坚而不挺，持而不久。



格式化 Json 数据：

```text
{"trace":"97.64.*.*","response":"97.64.*.*","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"*"}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"*"}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"180.153.24.97","location":"中国 上海 电信","as":"AS4812","elapse":0.56}]}
{"hop":7,"data":[{"ip":"124.74.232.53","location":"中国 上海 电信","as":"AS4812","elapse":1.88}]}
{"hop":8,"data":[{"ip":"101.95.207.253","location":"中国 上海 电信","as":"AS4812","elapse":5.49}]}
{"hop":9,"data":[{"ip":"61.152.24.50","location":"中国 上海 电信","as":"AS4812","elapse":9.43}]}
{"hop":10,"data":[{"ip":"202.97.61.6","location":"中国 上海 电信","as":"AS4134","elapse":48.84}]}
{"hop":11,"data":[{"ip":"202.97.63.229","location":"中国 上海 电信","as":"AS4134","elapse":50.14}]}
{"hop":12,"data":[{"ip":"59.43.244.117","location":"中国 上海 电信","as":"*","elapse":62.16}]}
{"hop":13,"data":[{"ip":"59.43.189.34","location":"美国 加利福尼亚州 洛杉矶 电信","as":"*","elapse":129.81}]}
{"hop":14,"data":[{"ip":"59.43.182.58","location":"美国 加利福尼亚州 洛杉矶 电信","as":"*","elapse":131.83}]}
{"hop":15,"data":[{"ip":"*"}]}
{"hop":16,"data":[{"ip":"192.254.84.245","location":"ZENLAYER.COM 骨干网 zenlayer.com","as":"AS62610","elapse":171.91}]}
{"hop":17,"data":[{"ip":"*"}]}
{"hop":18,"data":[{"ip":"97.64.*.*","host":"97.64.*.*.16clouds.com","location":"美国 加利福尼亚州 洛杉矶 it7.net","as":"AS25820","elapse":159.28}]}
```



- Azure 上海 → 搬瓦工 QNET DC2 洛杉矶：

![img](https://pic4.zhimg.com/80/v2-96ddf0da7a8409ce39089bcbd319d5c7_hd.jpg)
这个有点牛啤哈，看起来平平无奇的 QNET 机房，竟然去程被设定为半程 CN2 网络（本来我以为应该是全程 163 网来着），结合去程的路由来看，高峰时段 QNET 机房的访问体验一点都不比 DC8 机房差。



格式化 Json 数据：

```text
{"trace":"67.216.*.*","response":"67.216.*.*","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"*"}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"*"}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"180.153.24.97","location":"中国 上海 电信","as":"AS4812","elapse":0.86}]}
{"hop":7,"data":[{"ip":"124.74.232.61","location":"中国 上海 电信","as":"AS4812","elapse":2.23}]}
{"hop":9,"data":[{"ip":"101.95.120.154","location":"中国 上海 电信","as":"AS4812","elapse":3.43}]}
{"hop":9,"data":[{"ip":"202.101.63.242","location":"中国 上海 电信","as":"AS4812","elapse":4.53}]}
{"hop":10,"data":[{"ip":"202.97.24.154","location":"中国 上海 电信","as":"AS4134","elapse":56.69}]}
{"hop":11,"data":[{"ip":"202.97.91.34","location":"中国 上海 电信","as":"AS4134","elapse":6.85}]}
{"hop":12,"data":[{"ip":"59.43.244.117","location":"中国 上海 电信","as":"*","elapse":49.31}]}
{"hop":13,"data":[{"ip":"59.43.246.238","location":"美国 加利福尼亚州 洛杉矶 电信","as":"*","elapse":150.31}]}
{"hop":14,"data":[{"ip":"218.30.48.146","location":"美国 加利福尼亚州 洛杉矶 ctamericas.com","as":"AS4134","elapse":156.4}]}
{"hop":15,"data":[{"ip":"*"}]}
{"hop":16,"data":[{"ip":"*"}]}
{"hop":17,"data":[{"ip":"67.216.*.*","host":"67.216.*.*.16clouds.com","location":"美国 加利福尼亚州 洛杉矶 it7.net","as":"AS25820","elapse":148.43}]}
```



- Azure 上海 → 搬瓦工 CN2 GIA DC9 洛杉矶：

![img](https://pic3.zhimg.com/80/v2-810ad4e464e1d411bf9ba516b15a4cca_hd.jpg)
真 · CN2 还是很秀的，去程和回程都丝毫不令人失望。



格式化 Json 数据：

```text
{"trace":"67.230.*.*","response":"67.230.*.*","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"*"}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"*"}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"180.153.24.109","location":"中国 上海 电信","as":"AS4812","elapse":0.76}]}
{"hop":7,"data":[{"ip":"101.95.225.157","location":"中国 上海 电信","as":"AS4812","elapse":2.18}]}
{"hop":8,"data":[{"ip":"101.95.207.245","location":"中国 上海 电信","as":"AS4812","elapse":9.48}]}
{"hop":9,"data":[{"ip":"101.95.120.174","location":"中国 上海 电信","as":"AS4812","elapse":4.94}]}
{"hop":10,"data":[{"ip":"59.43.80.81","location":"中国 上海 电信","as":"*","elapse":2.2}]}
{"hop":11,"data":[{"ip":"*"}]}
{"hop":12,"data":[{"ip":"59.43.187.66","location":"中国 上海 电信","as":"*","elapse":52.92}]}
{"hop":13,"data":[{"ip":"59.43.189.38","location":"美国 加利福尼亚州 洛杉矶 电信","as":"*","elapse":128.98}]}
{"hop":14,"data":[{"ip":"*"}]}
{"hop":15,"data":[{"ip":"67.230.*.*","host":"67.230.*.*.16clouds.com","location":"美国 加利福尼亚州 洛杉矶 it7.net","as":"AS25820","elapse":128.9}]}
```



- Azure 上海 → 标准互联 CN2 GIA 圣何塞：

![img](https://pic3.zhimg.com/80/v2-bf80accf1f0575c69a66dbc8977f2f9e_hd.jpg)
表现和搬瓦工 DC9 机房一样，线路不错



格式化 Json 数据：

```text
{"trace":"103.126.*.*","response":"103.126. *.*","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"*"}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"*"}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"180.153.24.109","location":"中国 上海 电信","as":"AS4812","elapse":0.62}]}
{"hop":7,"data":[{"ip":"124.74.232.57","location":"中国 上海 电信","as":"AS4812","elapse":1.42}]}
{"hop":8,"data":[{"ip":"124.74.166.137","location":"中国 上海 电信","as":"AS4812","elapse":2.85}]}
{"hop":9,"data":[{"ip":"101.95.88.6","location":"中国 上海 电信","as":"AS4812","elapse":4.92}]}
{"hop":10,"data":[{"ip":"59.43.80.89","location":"中国 上海 电信","as":"*","elapse":3.23}]}
{"hop":11,"data":[{"ip":"*"}]}
{"hop":12,"data":[{"ip":"59.43.246.218","location":"中国 上海 电信","as":"*","elapse":2.78}]}
{"hop":13,"data":[{"ip":"59.43.182.145","location":"美国 加利福尼亚州 圣何塞 电信","as":"*","elapse":205.73}]}
{"hop":14,"data":[{"ip":"218.30.49.74","location":"美国 加利福尼亚州 圣何塞 ctamericas.com","as":"AS4134","elapse":127.03}]}
{"hop":15,"data":[{"ip":"*"}]}
{"hop":16,"data":[{"ip":"103.126.*.*","location":"美国 加利福尼亚州 圣何塞","as":"AS54600","elapse":132.86}]}
```



- Azure 上海 → 阿里云轻量服务器香港：

![img](https://pic3.zhimg.com/80/v2-0d93be7f292053029886d90643defad2_hd.jpg)
说实话这个去程相当不咋地了，走 163 网绕日不说，还走 NTT，NTT 不但最容易炸，高峰还炸的厉害是众所周知的，晚高峰表现甚至会比中美 163 线路还差



格式化 Json 数据：

```text
{"trace":"149.129. *.*","response":"149.129. *.*","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"*"}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"*"}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"180.153.24.101","location":"中国 上海 电信","as":"AS4812","elapse":1.11}]}
{"hop":7,"data":[{"ip":"124.74.232.57","location":"中国 上海 电信","as":"AS4812","elapse":1.53}]}
{"hop":8,"data":[{"ip":"124.74.166.141","location":"中国 上海 电信","as":"AS4812","elapse":8.43}]}
{"hop":9,"data":[{"ip":"61.152.24.46","location":"中国 上海 电信","as":"AS4812","elapse":6.29}]}
{"hop":10,"data":[{"ip":"*"}]}
{"hop":11,"data":[{"ip":"202.97.90.33","location":"中国 上海 电信","as":"AS4134","elapse":52}]}
{"hop":12,"data":[{"ip":"202.97.51.62","location":"日本 东京都 东京 电信","as":"AS4134","elapse":54.33}]}
{"hop":13,"data":[{"ip":"129.250.2.11","host":"ae-0.r30.tokyjp05.jp.bb.gin.ntt.net","location":"日本 东京都 东京 ntt.com","as":"AS2914","elapse":91.56}]}
{"hop":14,"data":[{"ip":"129.250.2.97","host":"ae-5.r24.tkokhk01.hk.bb.gin.ntt.net","location":"中国 香港 ntt.com","as":"AS2914","elapse":114.23}]}
{"hop":15,"data":[{"ip":"129.250.6.98","host":"ae-1.r03.tkokhk01.hk.bb.gin.ntt.net","location":"中国 香港 ntt.com","as":"AS2914","elapse":59.2}]}
{"hop":16,"data":[{"ip":"129.250.5.69","host":"ae-1.a00.newthk03.hk.bb.gin.ntt.net","location":"中国 香港 ntt.com","as":"AS2914","elapse":57.23}]}
{"hop":17,"data":[{"ip":"203.131.247.234","host":"prod06.x.hkg.fullmeshnetworks.com","location":"中国 香港 ntt.com","as":"AS2914","elapse":133.48}]}
{"hop":18,"data":[{"ip":"116.251.82.177","location":"中国 香港 阿里云","as":"AS45102","elapse":77.42}]}
{"hop":19,"data":[{"ip":"*"}]}
{"hop":20,"data":[{"ip":"*"}]}
{"hop":21,"data":[{"ip":"149.129.*.*","location":"中国 香港 阿里云","as":"AS45102","elapse":96.79}]}
```



- Azure 上海 → 阿里云国际香港：

![img](https://pic2.zhimg.com/80/v2-4aab627ba61f13e49bbb5c1b367809f1_hd.jpg)
去程是标准的 CN2 GIA 线路，结合返程来看，表现比阿里云轻量服务器香港要好不少了



格式化 Json 数据：

```text
{"trace":"47.52.*.*","response":"47.52.*.* ","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"*"}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"*"}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"180.153.24.97","location":"中国 上海 电信","as":"AS4812","elapse":0.62}]}
{"hop":7,"data":[{"ip":"124.74.232.53","location":"中国 上海 电信","as":"AS4812","elapse":2.17}]}
{"hop":8,"data":[{"ip":"101.95.207.101","location":"中国 上海 电信","as":"AS4812","elapse":7.64}]}
{"hop":9,"data":[{"ip":"61.152.24.6","location":"中国 上海 电信","as":"AS4812","elapse":8.37}]}
{"hop":10,"data":[{"ip":"59.43.80.105","location":"中国 上海 电信","as":"*","elapse":8.91}]}
{"hop":11,"data":[{"ip":"*"}]}
{"hop":12,"data":[{"ip":"59.43.187.70","location":"中国 上海 电信","as":"*","elapse":3.11}]}
{"hop":13,"data":[{"ip":"59.43.183.82","location":"中国 香港 电信","as":"*","elapse":27.18}]}
{"hop":14,"data":[{"ip":"59.43.247.230","location":"中国 香港 电信","as":"*","elapse":32.96}]}
{"hop":15,"data":[{"ip":"203.100.54.150","location":"中国 香港 电信","as":"AS4809","elapse":104.84}]}
{"hop":16,"data":[{"ip":"*"}]}
{"hop":17,"data":[{"ip":"*"}]}
{"hop":18,"data":[{"ip":"*"}]}
{"hop":19,"data":[{"ip":"47.52.*.*","location":"中国 香港 阿里云","as":"AS45102","elapse":80.57}]}
```



- Azure 上海 → Cloud Garage 东京：

![img](https://pic2.zhimg.com/80/v2-33fd9fbce09db64a161e4581b4f87e59_hd.jpg)
IIJ 线路是大部分日本本土 VPS 商与中国之间连接的标配，去程国内到出海都走 163 网，进入日本本土才走 IIJ 自己的线路，怎么说呢？白天还好，晚上肯定是要炸的



格式化 Json 数据：

```text
{"trace":"203.104. *.*","response":"203.104.*.*","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"*"}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"*"}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"180.153.24.109","location":"中国 上海 电信","as":"AS4812","elapse":0.6}]}
{"hop":7,"data":[{"ip":"124.74.232.65","location":"中国 上海 电信","as":"AS4812","elapse":1.3}]}
{"hop":8,"data":[{"ip":"124.74.166.133","location":"中国 上海 电信","as":"AS4812","elapse":8.67}]}
{"hop":9,"data":[{"ip":"101.95.120.158","location":"中国 上海 电信","as":"AS4812","elapse":6.77}]}
{"hop":10,"data":[{"ip":"202.97.24.146","location":"中国 上海 电信","as":"AS4134","elapse":47.02}]}
{"hop":11,"data":[{"ip":"202.97.90.29","location":"中国 上海 电信","as":"AS4134","elapse":35.24}]}
{"hop":12,"data":[{"ip":"202.97.6.46","location":"日本 东京都 东京 电信","as":"AS4134","elapse":158.36}]}
{"hop":13,"data":[{"ip":"58.138.102.205","host":"tky001bb11.IIJ.Net","location":"日本 东京都 东京 iij.ad.jp","as":"AS2497","elapse":160.03}]}
{"hop":14,"data":[{"ip":"58.138.102.234","host":"tky001ip58.IIJ.Net","location":"日本 东京都 东京 iij.ad.jp","as":"AS2497","elapse":83.8}]}
{"hop":15,"data":[{"ip":"210.130.134.54","location":"日本 iij.ad.jp","as":"AS2497","elapse":126.75}]}
{"hop":16,"data":[{"ip":"203.174.64.97","host":"rr-mx480-2-ae0.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":172.82}]}
{"hop":17,"data":[{"ip":"125.6.112.6","host":"125-6-112-6.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":83.04}]}
{"hop":18,"data":[{"ip":"203.174.66.242","host":"203-174-66-242.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":118.86}]}
{"hop":19,"data":[{"ip":"203.174.64.222","host":"203-174-64-222.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":77.1}]}
{"hop":20,"data":[{"ip":"*"}]}
{"hop":21,"data":[{"ip":"203.104.213.30","host":"static.203-104-213-30.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":60.42}]}
{"hop":22,"data":[{"ip":"*"}]}
{"hop":23,"data":[{"ip":"203.104.*.*","host":"static.203-104-*-*.data-hotel.net","location":"日本 东京都 东京 data-hotel.net","as":"AS17707","elapse":75.85}]}
```



- Azure 上海 → Host Hatch 斯德哥尔摩：

![img](https://pic1.zhimg.com/80/v2-fe8c95a8bd14d9df31c9ccf417c8c748_hd.jpg)
标准的中欧 163 直连网络，晚高峰必抽风



格式化 Json 数据：

```text
{"trace":"185.213.*.*","response":"185.213. *.*","hops":30,"packets":60}
{"hop":1,"data":[{"ip":"*"}]}
{"hop":2,"data":[{"ip":"*"}]}
{"hop":3,"data":[{"ip":"*"}]}
{"hop":4,"data":[{"ip":"*"}]}
{"hop":5,"data":[{"ip":"*"}]}
{"hop":6,"data":[{"ip":"180.153.24.109","location":"中国 上海 电信","as":"AS4812","elapse":0.61}]}
{"hop":7,"data":[{"ip":"124.74.232.237","location":"中国 上海 电信","as":"AS4812","elapse":1.19}]}
{"hop":8,"data":[{"ip":"124.74.166.149","location":"中国 上海 电信","as":"AS4812","elapse":5.12}]}
{"hop":9,"data":[{"ip":"61.152.24.10","location":"中国 上海 电信","as":"AS4812","elapse":5.86}]}
{"hop":10,"data":[{"ip":"202.97.57.25","location":"中国 上海 电信","as":"AS4134","elapse":55.65}]}
{"hop":11,"data":[{"ip":"*"}]}
{"hop":12,"data":[{"ip":"202.97.73.218","location":"中国 电信","as":"*","elapse":184.72}]}
{"hop":13,"data":[{"ip":"202.97.58.150","location":"德国 黑森州 法兰克福 电信","as":"AS4134","elapse":255.72}]}
{"hop":14,"data":[{"ip":"62.115.116.159","host":"ffm-bb4-link.telia.net","location":"德国 黑森州 法兰克福 telia.com","as":"AS1299","elapse":393.19}]}
{"hop":15,"data":[{"ip":"62.115.138.236","host":"s-bb3-link.telia.net","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 telia.com","as":"AS1299","elapse":363.45}]}
{"hop":16,"data":[{"ip":"62.115.136.21","host":"s-b6-link.telia.net","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 telia.com","as":"AS1299","elapse":335.35}]}
{"hop":17,"data":[{"ip":"62.115.61.247","location":"TELIA.COM 骨干网 telia.com","as":"AS1299","elapse":364.14}]}
{"hop":18,"data":[{"ip":"62.115.61.247","location":"TELIA.COM 骨干网 telia.com","as":"AS1299","elapse":400.44}]}
{"hop":19,"data":[{"ip":"80.67.4.193","host":"po-1.pe1.sto1.se.portlane.net","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 portlane.com","as":"AS42708","elapse":366.79}]}
{"hop":20,"data":[{"ip":"80.67.4.193","host":"po-1.pe1.sto1.se.portlane.net","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 portlane.com","as":"AS42708","elapse":396.49}]}
{"hop":21,"data":[{"ip":"188.126.92.25","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 glesys.se","as":"AS42708","elapse":405.33}]}
{"hop":22,"data":[{"ip":"185.213.*.*","location":"瑞典 斯德哥尔摩省 斯德哥尔摩 hosthatch.com","as":"AS63473","elapse":309.78}]}
```



**4. Ping 去回程测试：**



由于 Ping 工具也是基于 ICMP 协议的，所以无法直接向 Azure 测试 Ping，在提供结果前，先传授一个采用 TCP 协议做 Ping 测试的方法：



安装 traceroute 组件：

```text
apt-get install traceroute -y
```



如果报错，修复一下软件包依赖关系：

```text
apt --fix-broken install
```



下载并安装 tcpping：

```text
wget -O /usr/bin/tcpping https://raw.githubusercontent.com/deajan/tcpping/master/tcpping
```



赋予权限：

chmod +x /usr/bin/tcpping



使用范例：

```text
tcpping -x 100 42.159.136.107（IP 地址） 443（通讯端口）
```



以上命令中，100 表示需要进行的 ping 次数，42.159.136.107 表示要 ping 的对方主机的 IP 地址，443 表示 ping 对方主机的某个端口，按实际需要自己更改相关参数。



以下所有 ping 测试我只做了 100 次，值仅供参考，嫌太长不看的，可直接查看该表格，然后直接跳过 ping 测试部分：

![img](https://pic4.zhimg.com/80/v2-5d650c0ebc1d8f36d7cbddc598a99eb3_hd.png)



**4.1 ping 回程测试：**



- 搬瓦工 CN2 GT DC8 洛杉矶 → Azure 上海：

![img](https://pic4.zhimg.com/80/v2-7c63d81c6c75abe7102986497c274157_hd.jpg)
158.532 ms



- 搬瓦工 QNET DC2 洛杉矶 → Azure 上海

![img](https://pic4.zhimg.com/80/v2-a247e0c02ed5bdc336213a139a7b1c0b_hd.jpg)
153.958 ms



- 搬瓦工 CN2 GIA DC9 洛杉矶 → Azure 上海：

![img](https://pic4.zhimg.com/80/v2-19a9343acde3565a31b5303d137add17_hd.jpg)
128.890 ms



- 标准互联 CN2 GIA 圣何塞 → Azure 上海：

![img](https://pic2.zhimg.com/80/v2-c19a300ec4cb2f98b350e357fc37afed_hd.jpg)
137.237 ms



- 阿里云国际香港 → Azure 上海：

![img](https://pic3.zhimg.com/80/v2-c460dedd888c393d7bfde11dd372d346_hd.jpg)
32.567 ms



- 阿里云轻量香港 → Azure 上海：

![img](https://pic3.zhimg.com/80/v2-019c80d0b4cbadd9077982f1138c7ffa_hd.jpg)
62.304 ms



- Cloud Garage 东京 → Azure 上海：

![img](https://pic3.zhimg.com/80/v2-a83ed514b340c6ae56417703586dcb8e_hd.jpg)
58.036 ms



- Host Hatch 斯德哥尔摩 → Azure 上海：

![img](https://pic1.zhimg.com/80/v2-4b128a96cb3a7321047258d3afa68d44_hd.jpg)
353.898 ms



**4.2 ping 回程测试：**



- Azure 上海 → 搬瓦工 CN2 GT DC8洛杉矶：

![img](https://pic1.zhimg.com/80/v2-cb85a73acad4befc850307b23ea48f10_hd.jpg)
159.240 ms



- Azure 上海 → 搬瓦工 QNET DC2 洛杉矶：

![img](https://pic3.zhimg.com/80/v2-24e2889a23f9ba3d6eb0a0bb4f735fee_hd.jpg)
149.705 ms



- Azure 上海 → 搬瓦工 CN2 GIA DC9 洛杉矶：

![img](https://pic4.zhimg.com/80/v2-e2513c84582e5d4ae24bf1f7ef5a71d7_hd.jpg)
129.769 ms



- Azure 上海 → 标准互联 CN2 GIA 圣何塞：

![img](https://pic1.zhimg.com/80/v2-57150e3b90c0a1e5e9b4d56f881a4740_hd.jpg)
150.951 ms



- Azure 上海 → 阿里云轻量服务器香港：

![img](https://pic2.zhimg.com/80/v2-dbf3f725d4d893e8d31aa1aad018bad9_hd.jpg)
98.431 ms



- Azure 上海 → 阿里云国际香港：

![img](https://pic4.zhimg.com/80/v2-c18c5104cd123f187d1796c405f0b163_hd.jpg)
29.728 ms



- Azure 上海 → Cloud Garage 东京：

![img](https://pic3.zhimg.com/80/v2-ddf15a4c454355f4010fc2a90f0a50ce_hd.jpg)
126.979 ms



- Azure 上海 → Host Hatch 斯德哥尔摩：

![img](https://pic3.zhimg.com/80/v2-428f9cbdc5892be097c51bfbf505d0a6_hd.jpg)
350.522 ms





**5. 总结：**



由此可见，无论是当做代理，还是 Web 服务、下载服务器等用途。顾名思义，“服务器”的作用，就是凸出“服务”二字，即向客户机提供送去数据之用，所以回（返）程的意义，要比去程更大一些，回程路由路径的好坏，直接影响到客户机所在地域用户们的访问体验。所以我们在今后选购 VPS 产品时，不但要测去程，必须还要想办法（购置试用）在远程服务器中，以客户机 IP 地址为目标，测试返程路由性能。

由于受成本限制（VPS 商与某地域 ISP 签订的路由线路），远程服务器与本地之间的往返路由路径，有的时候天差地别。而且测去程很容易（找到一个测试 IP 即可），测回程比较麻烦（必须有对面地域的机器，即网络环境才可以），但我们并不能因为嫌麻烦，而忽视了回程的重要性。大部分 VPS 商都提供了退款功能，如果对回程不满意，发起退款申请即可（按用户条款，Azure 中国的不支持退款，所以本次测评做得尽可能详尽一些，尽可能花较低成本让大家知道，Azure 中国虚拟机的水准如何）。



虽然继承了 Microsoft 技术的衣钵，但 Azure 中国的虚拟机的硬件型号较老、线路一般（不像 Azure 国际版不同地域的虚拟机连接国际线路走 Microsoft 专线）、复杂的操作流程、死板的计费方式、中档价格，并没有太多出彩的地方。唯一的亮点就是自带 1TB 出入网双向计费的流量包，和不限速的外网通信速度，对于十分依赖微软技术线的企、事业单位而言，或许是一个不错的选择。

