---
tags:
    - "osu"
    - "更新日志"
title: "mfosu更新日志"
categories:
    - "日常"
excerpt: "暂无描述"
header:
  image: /assets/Images/Header/1.jpg
  teaser: /assets/Images/Header/1.jpg
  #caption: "水印: [**源**](https:/lcoalhost)"
---
此文档会随着项目变更滚动更新，在每一次汉化版更新后开始记录，在记录的版本被推送至stable后清空。推荐使用**强制刷新(一般为Ctrl+F5)**来查看最新内容。
{: .notice--info}

# **▪ Android**

`aaa98b8` - 修复*M.Resources*在打开*osu.Android*时报错找不到的问题

# **▪ 项目维护**

`0274901` - 移除tau残留文件

`df26cdb` - 将*osu!mania*模式设置中的*下落时间*翻译更改为*下落速度*

# **▪ Mvis播放器**

`82cfc5a` - 只在`CollectionPanel`的谱面缩略图中显示背景

`82cfc5a` - BeatmapCover: 只在`BackgroundBox`为`true`时添加背景Box

`82cfc5a` - 缩小`CollectionInfo`中收藏夹信息上下两侧的留白

`6c196a2` - 削弱`BeatmapPiece`的闪烁效果

<div>
当前<b>不处于</b>歌曲高潮时, 只会在第4拍(四分之一拍节奏)或第3拍(三分之一)节奏闪烁。<br/>
当前<b>处于</b>歌曲高潮时, 则在每一拍都闪烁
</div>
{: .notice}

`6c196a2` - 当选择的收藏夹不是当前收藏夹时，将`CollectionInfo`的谱面列表滚动到头

`ed4baaa` - 修复当`MvisScreen`中`桌面背景模式`按钮被按下时，收藏夹选择界面不会关闭的bug

`cfa7a35` - 修复游戏启动时`CollectionFilterDropdown`会报错的问题 *(汉化版功能导致的bug)*

`cfa7a35` - 将`CollectionInfo`的谱面列表提取出来，单独作为一个class

`cfa7a35` - 将`CollectionInfo`谱面刷新作为异步任务执行

`cfa7a35` - 为`CollectionPanel`的谱面缩略图列表添加一个最大缩略图数量限制

`aa557f6` - `BeatmapList`: 第一次滚动时不要播放动画

`aa557f6` - 为`BeatmapPiece`添加光标悬浮时的动画效果

`aa557f6` - `CollectionPanel`：修复无法显示第一张谱面背景图的问题

`aa557f6` - `CollectionPanel`：修复当收藏夹数量正好为15个时，缩略图最后一个会显示"+0"的bug

`0f5ce7b` - `BeatmapCover`：默认调用`Cover`而非`BeatmapBackground`用作谱面背景显示，减少内存占用

`cb8fc98` - 优化`BackgroundStoryBoardLoader`加载故事版的流程

`89ddf44` - 修复在点击`桌面背景模式`按钮后收藏夹按钮异常的问题

`3019bc3` - 修复commit `89ddf44`导致的新bug

`3019bc3` - `CollectionSelectPanel`: 添加关闭按钮

`3019bc3` - 移动`collectionPanel`到`Content Container`中

`dec1c0e` - 修复故事版加载bug

# **▪ Bug/Todo**

## **▪ Mvis播放器**
- ~~**bug** - 在故事版未完全加载时更换谱面会导致已加载的故事版贴图不会自动释放直到退出mvis播放器界面~~ (已在`dec1c0e`修复)
- **bug** - 在快速换曲时, 故事版会有几率留在`BackgroundStoryboardLoader`中
- **牢骚** - 这故事版我咋就怎么整都整不好呢(´・_・`)