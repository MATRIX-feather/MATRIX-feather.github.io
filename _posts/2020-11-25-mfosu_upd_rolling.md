---
tags:
    - "osu"
    - "更新日志"
title: "mfosu更新日志"
categories:
    - "daily"
excerpt: "暂无描述"
header:
  image: /assets/Images/Header/1.jpg
  teaser: /assets/Images/Header/1.jpg
  #caption: "水印: [**源**](https:/lcoalhost)"
---
此文档会随着项目变更滚动更新，在每一次汉化版更新后开始记录，在记录的版本被推送至stable后清空。推荐使用**强制刷新(一般为Ctrl+F5)**来查看最新内容。<br>
[2020.1121.0 已同步更新](/mfosu_update_log/mfosu_20201121_update)
{: .notice--info}

## 杂项
`b0ca7a2` - 添加`BottomBarButton`的TestScene

`b0ca7a2` - 调整`MvisScreen`的TestScene

`709e452` - 移动Mvis播放器各组件的位置

`4813bee` - 移除用不上的代码

## 文件导入
`80a2542` - 简化文件导入屏幕，删除过滤功能

详见 [https://github.com/ppy/osu/pull/10882#pullrequestreview-537122319](https://github.com/ppy/osu/pull/10882#pullrequestreview-537122319)
{: .notice}

## Mvis播放器
`b0ca7a2` - `CollectionHelper`: 在收藏夹有变动时更新列表

`b0ca7a2` - **调整皮肤功能，使用`SkinnableComponent`**

简化界面皮肤功能的实现方式<br>
{: .notice}

`b0ca7a2` - `BeatmapList`: 让图谱列表填充整个CellContainer

`b0ca7a2` - `BeatmapPiece`: 在歌曲、艺术家名过长时截短文本

`b0ca7a2` - 修复一些奇怪的界面外观问题

比方说收藏夹界面状态栏那里，在某些特殊窗口尺寸下顶端会漏一两个像素(???)
{: .notice}

`b0ca7a2` - 削弱`CollectionPanel`的圆角大小

`b0ca7a2` - `CollectionSelectPanel`: 缩小整体宽度

`b0ca7a2` - `CollectionSelectPanel`: 在收藏夹有变动时更新信息

`b0ca7a2` - `SkinnableSprite`: 让`SpriteComponent`从private变为public

TODO: 改回private
{: .notice}

`3adf45d` - `BackgroundStoryboardLoader`: 简化故事版加载方式

`d08b89f` - 将空闲时背景亮度的默认值更改为90%

`7e0f935` - 清理`MvisEnableSBOverlayProxy`设置项

在未来的一段时间内这个功能都不会再去弄了，难顶
{: .notice}

`22432c1` - 调整故事版加载方式

`39e81d3` - `BackgroundStoryboardLoader`: 将更多步骤丢进异步部分执行