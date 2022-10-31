---
title: Chromebook初体验与解决问题
date: 2022-10-29
tags: [internet]
---


# chromebook初体验与解决问题

在TG某二手频道捡了一台Dell Chromebook

配置（总之就是能用而已）：Celeron N2030,4G DDR3,16G EMMC 5.1(没内置硬盘)

## 1.上手

机器黑色，屏幕及主体一圈用橡胶条包裹。

A面有一个经典的dell标和一个Chrome Logo。机身左侧一个电源插口，一个SD卡卡槽，两个USB与一个HDMI插口，右侧则是耳机口，电源按键与音量键。

本来是chromeos (Chrome v103)，于2022.6 EOL（终止支持），于是卖家提前刷好了MrChromeBox并安装了Ubuntu Mate。

电池寿命到我手上还有32%，但是续航时间竟然还有5 hrs +（不得不说这就是低功耗处理器的好处（笑））

非常轻便，到处拿着也不嫌厚重（而且续航时间长的优点非常显著）

键盘的布局与正常笔记本稍有不同（F1-F10变成了各种图标，本来capslock的位置变成了搜索键（经过实测为Super键（也即win键））

不过大体键盘录入毫无妨碍（不得不说这个键盘可能还得比Thinkpad的浮岛键盘键程长点）

对了，还有块触摸屏（还挺好用）但是Mate桌面只有单击没有任何优化（长按动作不识别）

## 2.问题

本来一切安好，但是我测试一圈才发现，压根一点声音没有（但是右下角有音频显示）

于是打开Google一通乱搜出来一堆结果（很明显这是个通病），然而没有一个顶用的回答（硬件特殊?）

无计可想，写入一个Xubuntu LiveCD到U盘里，尝试安装

结果又是没声音。 

非常恼火，我直接创建了一个Chromebook恢复盘，将Mrchromebox恢复成出场UEFI Bios后开始系统恢复。

令人意外的是Chrome OS里却是有声音的（我差点以为瞎搞把音频输出烧了）

（根据Wikipedia-zh-computer-science群里某位ChromeBook用户反映：Chromebook将声卡与功放结合，如果配置错误有烧毁功放的危险）

## 3.解决

开始准备使用提取大法，从ChromeOS中直接提取当前系统的音频输出内核驱动模块

怎奈何不甚管用

最终从chromeos developer mode下重新刷写了Mrchromebox并且安装Kubuntu 22.04后声卡开始工作正常。

（看来20.04可能内核略老并不能支持chromebook音频硬件）

## 4.总结

我们可以很轻易的知道chromebook在国内为什么不能风行：

因为很多时候并没有那么好的网络条件（单就FydeOS也不太可能风行，毕竟很多条件在那里）

顺带一提：KDE的触摸操作事实上挺不错的（相比Xfce跟mate等桌面）而wayland更进一步优化了体验。
