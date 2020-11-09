---
tags:
    - "mfosu"
title: "mfosu Mvis音乐播放器皮肤制作"
categories:
    - "mfosu"
excerpt: "音乐播放器皮肤手册"
gallery:
  - url: /assets/Images/Posts/mvis-skinning/osu_2020-11-09_23-39-07.png
    image_path: /assets/Images/Posts/mvis-skinning/osu_2020-11-09_23-39-07.png
  - url: /assets/Images/Posts/mvis-skinning/osu_2020-11-09_23-39-11.png
    image_path: /assets/Images/Posts/mvis-skinning/osu_2020-11-09_23-39-11.png
  - url: /assets/Images/Posts/mvis-skinning/osu_2020-11-10_00-00-39.png
    image_path: /assets/Images/Posts/mvis-skinning/osu_2020-11-10_00-00-39.png
---

# 简要
截至`2020.1109.0`版本, Mvis播放器对皮肤的支持程度如下：

- [x] 播放器前景
- [x] 底栏背景
- [x] 底栏按钮背景
- [x] 侧边栏底部条
- [x] 侧边栏背景
- [x] 收藏夹界面背景
- [x] 收藏夹刷新按钮
- [ ] 动画支持

## 播放器前景

| 材质名 | 尺寸 |
| :----: | :----: |
| MPlayer-foreground | *建议根据目标屏幕比例制定* |
| | 16:9(标准大小) 1366x768 |
| | 16:9(2x) 2732x1536 |

- 更多信息:
  - 该材质将会覆盖在故事版和M-vis播放器面板的上方。
  - 该材质将会根据较小的一边缩放以填充屏幕。
  - 锚点为屏幕的正中心，向四周扩散。
  
**个人建议：**<br>
制作前景时可以根据自身需要在左右两边各多弄一些，这样在显示工具栏(顶栏)时能让前景看上去更自然些_(:3 」∠)_

{% include figure image_path="/assets/Images/Posts/mvis-skinning/osu_2020-11-09_23-50-12.png" caption="红框大小:1440x768, 黑框大小:1366x768" %}

## 底栏背景

| 材质名 | 尺寸 |
| :----: | :----: |
| MBottomBar-background | *建议根据目标屏幕比例制定* |
| | 16:9(标准大小) 1366x100 |
| | 16:9(2x) 2732x200 |

- 更多信息:
  - 该材质将会覆盖任何处于底栏下方的界面(换句话说，除了底栏其他的都会被覆盖)
  - 该材质会跟随底栏显示/隐藏
  - **背景高度为100，请留意图像尺寸**
    ![ ](/assets/Images/Posts/mvis-skinning/bottomBarBgHeight.png)
  - 该材质将会根据较小的一边缩放以填充高度。
  - 锚点为屏幕的正中心，向四周扩散。
  
## 底栏标准按钮背景

| 材质名 | 尺寸 |
| :----: | :----: |
| MButtonSquare-background | 1:1尺寸即可 |

- 更多信息:
  - 该材质将会覆盖在按钮背景的上方。
  - 该材质将会根据较大的一边缩放以填充高度。
  - 锚点为按钮的左上角，向右侧扩散。

## 底栏切换按钮背景

| 材质名 | 尺寸 |
| :----: | :----: |
| 关: MButtonSwitchOff-background | 1:1尺寸即可 |
| 开: MButtonSwitchOn-background | 1:1尺寸即可 |

- 更多信息:
  - 见[底栏标准按钮背景](#底栏标准按钮背景)

## 底栏宽按钮背景

| 材质名 | 尺寸 |
| :----: | :----: |
| MButtonWide-background | 5:3比例即可 |

- 更多信息:
  - 见[底栏标准按钮背景](#底栏标准按钮背景)

## 底栏歌曲进度按钮背景

| 材质名 | 尺寸 |
| :----: | :----: |
| 关: MButtonProgressOff-background | (>=11):3 |
| 开: MButtonProgressOn-background | (>=11):3 |

- 更多信息:
  - 见[底栏标准按钮背景](#底栏标准按钮背景)

## 侧边栏底部条

| 材质名 | 尺寸 |
| :----: | :----: |
| MSidebar-BottomBox | *建议根据目标屏幕比例制定* |

* 更多信息:
  - 该材质将会根据较小的一边缩放以填充高度。
  - **背景高度为50，请留意图像尺寸**
    ![ ](/assets/Images/Posts/mvis-skinning/MSidebar-BottomBox.png)
  - 锚点为侧边栏底部的右下角，向左侧扩散。

## 侧边栏背景

| 材质名 | 尺寸 |
| :----: | :----: |
| MSidebar-background | *建议根据目标屏幕比例制定* |
| | 16:9(标准大小) 1366x718 |
| | 16:9(2x) 2732x1436 |

* 更多信息:
  - 该材质将会根据较小的一边缩放以填充高度。
  - 锚点为侧边栏内容的右下角，向左侧扩散。

## 收藏夹界面背景

| 材质名 | 尺寸 |
| :----: | :----: |
| MSidebar-Collection-background | *建议根据目标屏幕比例制定* |
| | 16:9(标准大小) 1366x718 |
| | 16:9(2x) 2732x1436 |

* 更多信息:
  - 该材质将会根据较小的一边缩放以填充高度。
  - 锚点为收藏夹界面的右下角，向左侧扩散。

## 收藏夹刷新按钮

| 材质名 | 尺寸 |
| :----: | :----: |
| MButtonRefreshCollection-background | 3:1 |

- 更多信息:
  - 见[底栏标准按钮背景](#底栏标准按钮背景)

{% include gallery caption="收藏夹背景稍微调教一下放个壁纸也不是不可能" %}