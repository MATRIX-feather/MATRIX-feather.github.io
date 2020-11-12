---
tags:
    - "mfosu"
title: "mfosu Mvis音乐播放器皮肤指南"
categories:
    - "mfosu"
excerpt: "音乐播放器皮肤手册"
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

`MPlayer-foreground`

![ ](/assets/Images/Posts/mvis-skinning/osu_2020-11-09_23-50-12.png){: .align-center}

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| MPlayer-foreground  | 暂不支持 | 1366*768 | 屏幕中心 | 根据较小的一边缩放以填充屏幕 |

更多信息:
  - 该材质将会覆盖在故事版和M-vis播放器面板的上方

## 底栏背景
`MBottomBar-background`

![ ](/assets/Images/Posts/mvis-skinning/bottomBarBgHeight.png){: .align-center}

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| MBottomBar-background | 暂不支持 | 1366*100 | 底部中心 | 根据较小的一边缩放以填充空间 |

更多信息:
  - 该材质将会覆盖任何处于底栏下方的界面(换句话说，除了底栏其他的都会被覆盖)
  - 该材质会跟随底栏显示/隐藏
  
## 底栏标准按钮背景
`MButtonSquare-background`

![ ](/assets/Images/Posts/Mvis/bb_settings.png){: .align-center}

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| MButtonSquare-background | 暂不支持 | 无(1:1图像即可) | 左上角 | 根据较大的一边缩放以填充空间 |

## 底栏切换按钮背景

`MButtonSwitchOff-background`、`MButtonSwitchOn-background`

![ ](/assets/Images/Posts/Mvis/bb_lock.png){: .align-center}

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| 关: MButtonSwitchOff-background | 暂不支持 | 无(1:1图像即可) | 左上角 | 根据较大的一边缩放以填充空间 |
| 开: MButtonSwitchOn-background | 暂不支持 | 无(1:1图像即可) | 左上角 | 根据较大的一边缩放以填充空间 |

更多信息:
  - 见[底栏标准按钮背景](#底栏标准按钮背景)

## 底栏宽按钮背景

`MButtonWide-background`

![ ](/assets/Images/Posts/mvis-skinning/bb_wide.png){: .align-center}

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| MButtonWide-background | 暂不支持 | 无(5:3图像即可) | 左上角 | 根据较大的一边缩放以填充空间 |

更多信息:
  - 宽按钮背景现只用于上一首/下一首按钮
  - 见[底栏标准按钮背景](#底栏标准按钮背景)

## 底栏歌曲进度按钮背景
`MButtonProgressOff-background`、`MButtonProgressOn-background`

![ ](/assets/Images/Posts/mvis-skinning/bb_progress.png){: .align-center}

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| 关: MButtonProgressOff-background | 暂不支持 | (≥110)*30 | 左上角 | **不缩放** |
| 开: MButtonProgressOn-background | 暂不支持 | (≥110)*30 | 左上角 | **不缩放** |

更多信息:
  - 见[底栏标准按钮背景](#底栏标准按钮背景)

## 侧边栏底部
`MSidebar-BottomBox`

![ ](/assets/Images/Posts/mvis-skinning/MSidebar-BottomBox.png){: .align-center}

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| MSidebar-BottomBox | 暂不支持 | 1366*50 | 右下角 | 根据较小的一边缩放以填充空间 |

## 侧边栏背景
`MSidebar-background`

<!-- ![ ](/assets/Images/Posts/mvis-skinning/MSidebar-BottomBox.png){: .align-center} -->

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| MSidebar-background | 暂不支持 | 1366*718 | 右下角 | 根据较小的一边缩放以填充空间 |

## 收藏夹界面背景
`MSidebar-Collection-background`

<!-- ![ ](/assets/Images/Posts/mvis-skinning/MSidebar-BottomBox.png){: .align-center} -->

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| MSidebar-Collection-background | 暂不支持 | 1366*718 | 右下角 | 根据较小的一边缩放以填充空间 |

## 收藏夹刷新按钮
`MButtonRefreshCollection-background`

<!-- ![ ](/assets/Images/Posts/mvis-skinning/MSidebar-BottomBox.png){: .align-center} -->

| 材质名 | 支持动画  | 建议大小(SD) | 位置 | 缩放方式 |
| :----: | :----: | :----: | :----: | :----: |
| MButtonRefreshCollection-background | 暂不支持 | 无(≥3:1图像即可) | 右下角 | 根据较大的一边缩放以填充空间 |

更多信息:
  - 见[底栏标准按钮背景](#底栏标准按钮背景)