---
tags:
    - "mfosu"
title: "mfosu音乐播放器使用手册"
categories:
    - "日常"
excerpt: "音乐播放器使用手册"
#header:
#  image: /assets/Images/Header/1.jpg
#  teaser: /assets/Images/Header/1.jpg
#caption: "水印: [**源**](https:/lcoalhost)"

gallery:
  - url: /assets/Images/Posts/Mvis/sidebar_1.png
    image_path: /assets/Images/Posts/Mvis/sidebar_1.png
  - url: /assets/Images/Posts/Mvis/sidebar_2.png
    image_path: /assets/Images/Posts/Mvis/sidebar_2.png

gallery_songSelect:
  - url: /assets/Images/Posts/Mvis/sidebar_songSelect.png
    image_path: /assets/Images/Posts/Mvis/sidebar_songSelect.png
  - url: /assets/Images/Posts/Mvis/mvis_songSelect.png
    image_path: /assets/Images/Posts/Mvis/mvis_songSelect.png
---

# 简要
Mvis音乐播放器是mf-osu基于[EVAST9919/lazer-m-vis](https://github.com/EVAST9919/lazer-m-vis)打造的一个界面，目的是~~让osu成为一个真正的音乐播放器~~提供一个更好的osu!挂机体验。

本手册可以帮助您快速上手该界面

# 跳转目录

[底栏](#底栏)

[侧边栏](#侧边栏)
- [播放器设置](#播放器设置)
- [进入选歌界面](#进入选歌界面)
- [选择收藏夹](#选择收藏夹)

[故事版](#故事版)


# 底栏
底栏在整个界面中承载了所有的基础功能，几乎所有的界面功能都可以通过底栏直接或间接被调用。

![bottomBar](/assets/Images/Posts/Mvis/bottomBar.png)

### 各按钮的功能

![bb_exit](/assets/Images/Posts/Mvis/bb_exit.png)
退出按钮，点按可以退出界面

![bb_help](/assets/Images/Posts/Mvis/bb_help.png)
帮助按钮，点按可以查看快捷提示

![bb_control](/assets/Images/Posts/Mvis/bb_control.png)
控制按钮，从左到右分别为`上一首、从头开始`,`暂停、播放`和`下一首`

![bb_lock](/assets/Images/Posts/Mvis/bb_lock.png)
锁定按钮，激活后可以阻止界面自动影隐藏

默认按`h`可以激活强制锁定，在此状态下界面将无视任何情况一直保持显示或隐藏状态
{: .notice--info}

![bb_collection](/assets/Images/Posts/Mvis/bb_collection.png)
收藏夹按钮，点按可以从侧边栏调出收藏夹界面

![bb_bgmode](/assets/Images/Posts/Mvis/bb_bgmode.png)
桌面背景模式按钮，点按可以激活强制锁定(仅桌面端可用)并隐藏界面。**和[OSU-Desktop](https://github.com/TGSAN/OSU-Desktop)搭配食用更佳**

![bb_loop](/assets/Images/Posts/Mvis/bb_loop.png)
单曲循环按钮，点按可以激活单曲循环模式

![bb_invokeSolo](/assets/Images/Posts/Mvis/bb_invokeSolo.png)
查看按钮，点按可以在选歌界面中查看当前曲目的详细信息

![bb_settings](/assets/Images/Posts/Mvis/bb_settings.png)
设置按钮，点按可以从侧边栏调出播放器设置界面

![bb_progress](/assets/Images/Posts/Mvis/bb_progress.png)
歌曲进度条，进度条怎么用的相信各位网上冲浪的人都知道了吧...

# 侧边栏
侧边栏充当了功能扩展的作用，所有后期加入的、较复杂的功能都会添加到侧边栏中，当前可用的功能有`播放器设置`、`进入选歌界面`和`选择收藏夹`三个

{% include gallery caption="侧边栏一览" %}

## 播放器设置
您可以在这里更方便地管理播放器的偏好设置，包括背景模糊、界面主题色调等，省去了从设置界面前往播放器设置的过程<br>

## 进入选歌界面
在播放器设置菜单翻到最下面即可看见`歌曲选择`按钮，点按可以进入mvis选歌界面

{% include gallery  id="gallery_songSelect" caption="入口及界面样式" %}

点按`选择该谱面`按钮或者按照往常在选歌界面选图的方式即可选中一张图并返回播放器。<br>
点按`返回`按钮或直接退出该界面将从`当前曲目`的`当前时间`继续播放而非继续播放进入界面时播放的曲目
{: .notice--info}

## 选择收藏夹
*前提条件*: 在[播放器设置](#播放器设置)中勾选`从收藏夹播放音乐`选项

您可以在这里决定要将哪一个收藏夹作为播放器播放歌曲的歌单。

在`收藏夹选择界面`中单击一个收藏夹以将其选中并在旁边的`收藏夹信息界面`中预览当前收藏夹包含的所有谱面。

再次单击选中的收藏夹即可切换到该收藏夹并将其作为歌单播放音乐。

如果当前显示的收藏夹**是**正在播放的收藏夹，则收藏夹信息界面的顶端状态条会显示较**鲜艳**的颜色(右)，反之则会显示较**浅**的颜色(左)。

![collection_state](/assets/Images/Posts/Mvis/collection_state.png)

对于`收藏夹信息界面`中的谱面显示(图谱面板)也是一样

{% include figure image_path="/assets/Images/Posts/Mvis/collection_panelState.png" caption="左: 未播放 | 右: 正在播放" %}

图谱面板有两种状态，分别是*正在播放*和*未播放*，点按图谱面板可以跳转到其对应的谱面。<br>
当状态为*正在播放*时，边框会变为*高亮颜色*并将背景上的遮罩淡化，同时该面板还会随着歌曲的节奏闪光，非高潮时期是*每4拍一闪或3拍一闪*，高潮时期则是*一拍一闪*。<br>
当状态为*未播放*时，边框则会变为*背景颜色*并恢复背景上的遮罩。<br>
如果当前显示的收藏夹**不是当前正在播放的收藏夹**，则*正在播放*时边框只会和顶端状态条一样显示一个较浅的颜色，并且点按图谱面板不会有任何反应。
{: .notice--info}

点按`收藏夹选择界面`下方的`刷新列表`按钮可以刷新收藏夹列表和信息。

# 故事版
通过[播放器设置](#播放器设置)的`启用故事版/背景视频(默认开启)`可以启用该功能。

启用后播放器将会根据当前播放**曲目所属的谱面**加载对应的故事版。

在故事版加载期间，界面上会出现一个加载图标![loadingSpinner](/assets/Images/Posts/Mvis/loadingSpinner.png)来表示当前故事版的加载状态。

该图标将在故事版加载成功时自动隐藏。