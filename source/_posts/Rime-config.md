---
title: rime的调校
date: 2021-07-22
tags: [internet]
---
Rime精雕细琢

Rime（中州韵/小狼毫/鼠须管），很快，很精简，但是很不方便（毕竟不是可视化的配置界面）
不过如果调校好了，那将非常流畅与爽快（比我的Google Pinyin 2.7甚至还快）

换在平时我当然更喜欢图形化，傻瓜化的操作。那么今天为什么会用到这个输入法呢，因为谷歌拼音在某次TG Desktop更新（2.8.11）之后就无法选词了（很明显这是老输入法问题了，毕竟2014年就停更的东西）。
![cao](https://imgcdn-git.littleneko.cf/img032034/126481424-a02251d7-79f8-49a2-88cf-21469fc51dd3.png)

rime默认的输入方式是非常违和的

![](https://imgcdn-git.littleneko.cf/img032034/image-20210722205542140.png)

(毕竟现在的输入法都默认横排选字)

同时，rime毕竟是个纯本地输入法，在词库等方面相当欠缺。

所以我们需要好好调校一番，让它能够物尽其用。

# 导入词库

## 导出其他输入法里的词库

(看到没，设置里点导出就行，google不知道比你们简洁到哪里去了，各位国产输入法学学人家“Don't Be Evil",别天天塞点什么东西)

![image-20210722211112891](https://imgcdn-git.littleneko.cf/img032034/202107222114609.png)

然后你需要一个神奇的东西：[imewlconverter](https://github.com/studyzy/imewlconverter)

这东西可以将你导出的词库转化成rime可用的词库，使用很简单。

![image-20210722221414591](https://imgcdn-git.littleneko.cf/img032034/202107222214614.png)

选择之后点转换即可生成rime的词库。

然后去你的开始菜单里选择导入词库：

![image-20210722221642834](https://imgcdn-git.littleneko.cf/img032034/202107222216043.png)

选中默认词库列表，点击“導入文本碼表”导入词库

![image-20210722221826032](https://imgcdn-git.littleneko.cf/img032034/202107222218906.png)

你就获得了一份非常爽的词库（

# 外观配置

默认的图上面有了（很明显不符合现代输入法习惯）

所以我们需要手动写配置：）

打开用户文件夹（即上方导入用户词典下一个）然后打开weasel.custom.yaml进行配置：

```yaml
patch:

  
  
  "preset_color_schemes/Wii2":
    author: PYatoo
    back_color: 0xefefef
    border_color: 0xefefef
    candidate_text_color: 0x575759
    comment_text_color: 0xcac9c8
    hilited_back_color: 0xefefef
    hilited_candidate_back_color: 0xED9564
    hilited_candidate_text_color: 0xffffff
    hilited_comment_text_color: 0xffffff
    hilited_text_color: 0xED9564
    label_color: 0xcac9c8
    name: Wii2
    text_color: 0x575759
  "style/color_scheme": Wii2
  "style/display_tray_icon": true
  "style/font_face": "Microsoft Yahei UI"
  "style/font_point": 12
  "style/horizontal": true
  "style/inline_preedit": false
  "style/layout/border": 0
  "style/layout/border_width": 0
  "style/layout/candidate_spacing": 12
  "style/layout/hilite_padding": 8
  "style/layout/hilite_spacing": 3
  "style/layout/margin_x": 8
  "style/layout/margin_y": 8
  "style/layout/round_corner": 7
  "style/layout/spacing": 10
```

这是我用的主题，看着观感尚佳（芜湖）

![image-20210727225458566](https://imgcdn-git.littleneko.cf/img032034/202107272300900.png) 

切记：此文件中的Patch只能出现一次，不能重复。

#### 关于颜色

rime主题里的16进制颜色为‘蓝’‘绿’‘红’排序，并未是常规的‘红’‘绿’‘蓝’

比如说我需要的是‘#66CCFF’这一颜色(懂得都懂），则写为：‘#FFCC66’

（按：是不是有什么大病）
