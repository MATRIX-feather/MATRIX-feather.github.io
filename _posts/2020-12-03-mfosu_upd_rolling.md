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
[2020.1203.0 已同步更新](/mfosu_update_log/mfosu_20201203_update)
{: .notice--info}

# 44fc206
## Mvis播放器
- 更改播放器设置和收藏夹选择的默认快捷键

在lazer换成SDL之后Menu键好像不管用了
{: .notice}

- `BeatmapList`: 更改maskBox的颜色

- `CollectionInfo`: 移除默认背景; 移除收藏夹封面显示; 移除flashBox

- `Footer`: 移除阴影效果; 在顶部添加- highLightBox

- `Sidebar`: 暗化背景色; 调整淡入、淡出动画

<br>

# d06289b
## Toolbar
- `ToolbarTimeButton`: 代码维护; 不要在点击时隐藏Tooltip

<br>

# e23aa6d
## Mvis播放器
- `BeatmapList`: 代码维护

- `CollectionInfo`: 添加默认背景

<br>

# 525c739
## Mvis播放器
- `Sidebar`: **只在用户需要时添加并显示侧边栏内容，否则移除它**

- `CollectionSelectPanel`: 修复单线程模式下的小概率报错

<br>

# 3ad1d9c
## Mvis播放器
- `BeatmapList`: 精简逻辑; 列表显示非当前收藏夹时也不要滚动到顶部

- `BeatmapPiece`: 优化交互效果

- `TabHeader`: 移除滚动容器

- `Sidebar`: 去除Masking设定

- `BackgroundStoryBoardLoader`: 将更新故事版函数设置为private, 移除`StoryboardState.Failed`

<br>

# 9ea028b
## Mvis播放器
- `CollectionSelectPanel`: 修复bug