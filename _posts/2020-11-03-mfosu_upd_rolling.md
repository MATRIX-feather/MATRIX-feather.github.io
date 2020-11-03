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
此文档会随着项目变更滚动更新，在每一次汉化版更新后开始记录，在记录的版本被推送至stable后清空。推荐使用**强制刷新(一般为Ctrl+F5)**来查看最新内容。<br>
[2020.1031.0 已同步更新](/更新日志/mfosu_20201031_update)
{: .notice--info}

合并上游代码的提交一般不会记录，除非该提交包含了汉化版的改动
{: .notice--info}

# **▪ 项目维护**

`d59ada1` - `MvisScreen`: 解决commit `a425a17`导致的代码缩进问题

`1aabb49` - `BeatmapList`: 移除多余的注释

`1aabb49` - `MvisScreen`: 将`colourProvider`标记为`[Cached]`

`1aabb49` - `CollectionInfo`: 将`colourProvider`变为对`MvisScreen.colourProvider`的一个依赖

`1aabb49` - `SidebarContainer`: 将`colourProvider`变为对`MvisScreen.colourProvider`的一个依赖

`1aabb49` - `CollectionSelectPanel`: 移除对`OverlayColourProvider`的依赖

`6631edc` - `OverlayColourProvider`: 移除不再需要的配色方案

# **▪ Mvis播放器**

`98c2acd` - 调整`BeatmapList`四周的留白大小，让`beatmapScroll`能在水平方向上填满整个区域

`98c2acd` - `CollectionPanel`: 只在选中或激活时显示谱面预览图

`98c2acd` - 减少`CollectionPanel`的谱面预览图数量至8个

`98c2acd` - `CollectionSelectPanel`: 缩小圆角和收藏夹选择界面的宽度，增大收藏夹信息界面的宽度

`98c2acd` - `CollectionSelectPanel`: 缩短弹入、弹出动画的时间，削弱缩放效果

`3d6a150` - `CollectionSelectPanel`: 用`collectionsFillFlow.AddRange(collectionManager.Collections.Select...`代替原来的`foreach ... Add`为收藏夹列表添加`CollectionPanel`

`a8c2472` - **实现新的侧边栏方案**

`a8c2472` - 增加`CollectionPanel`的谱面预览图数量至10个

`a8c2472` - 将`CollectionSelectPanel`添加到新的侧边栏中

`a8c2472` - `CollectionSelectPanel`: 适应新的侧边栏方案，去除关闭按钮

`a8c2472` - 将原有的"侧边栏"按钮改为"播放器设置按钮"

`f1587fb` - `SidebarContainer`: 优化切换动画流程

流程对比(从a切换到b): <br>
之前: 将a淡出，同时b淡入、根据b的`ResizeWidth`和`ResizeHight`分别调整宽度和高度<br>
现在: *先*将a淡出，*然后*将b淡入，同时根据b的`ResizeWidth`和`ResizeHight`分别调整宽度和高度
{: .notice--info}

`a425a17` - `CollectionPanel`: 添加在加载完毕时的淡入动画

`a425a17` - `CollectionPanel`: 只在第一次点击后设置`AutoSizeDuration`和`AutoSizeEasing`属性

`a425a17` - 移除侧边栏在屏幕切换时的隐藏功能

`a425a17` - `SidebarContainer`: 添加弹入、弹出音效

`a425a17` - `SidebarContainer`: 如果`resizeFor`在侧边栏隐藏时被调用，则将调整大小动画时间设置为0

`a425a17` - `SidebarContainer`: 如果为当前显示的内容重复调用`resizeFor`函数，将只会设置`IsHidden`为`false`

`d59ada1` - `CollectionInfo`: 限制收藏夹预览图在界面上的大小，并添加渐变效果

`d59ada1` - `CollectionInfo & CollectionPanel`: 修复当当前收藏夹为空时会引发数组越界的问题

虽然这个解决方案导致了`CollectionPanel`在收藏夹为空时也会显示默认封面...但我感觉这个问题无关紧要，所以暂时就这样吧
{: .notice}

`d59ada1` - `CollectionSelectPanel`: 只在当前收藏夹包含谱面时设置已选择的收藏夹面板

`d59ada1` - `SidebarContainer`: 移除弹入、弹出音效

`d59ada1` - `SidebarContainer`: 为通过`AddDrawableToList`添加的组件添加`Alpha = 0`属性

`1aabb49` - `BottomBarButton`: 优化加载逻辑，移除阴影效果，与界面中其他元素的主题色保持一致

`1aabb49` - `BottomBarSwitchButton`: 优化加载逻辑，与界面中其他元素的主题色保持一致

`1aabb49` - `HoverableProgressBarContainer`: 与界面中其他元素的主题色保持一致

~~现在整个mvis界面除了`CollectionPanel`和`CollectionInfo`有一部分没弄以外其他地方的主题色都一致了，这两个我还没想好要如何配主题色(如何用一个主题色表示选中、激活和不可用这三种状态)~~
{: .notice--info}

`1aabb49` - 将单曲循环和歌曲进度按钮主体分离至单独的文件中，移除原有的`BottomBarSongProgressInfo`

`1aabb49` - `BottomBarOverlayLockSwitchButton & ToggleLoopButton`: 在激活时播放图标动画

`1aabb49` - `CollectionSelectPanel`: 更改刷新列表按钮的大小

`1aabb49` - 将播放器设置按钮的图标更改为齿轮

`6631edc` - `OverlayColourProvider`: 添加Mvis主题色

~~暂时和Blue1是一样的, 正在研究如何实现自定义主题色~~
{: .notice--info}

`6631edc` - 将主题色改为`OverlayColourScheme.Mvis`

`6631edc` - `SidebarContainer`: 修复因界面缩放导致界面残留在屏幕上的bug

`e3c3e0a & 225db8f` - **实现Mvis自定义主题色功能**

__颜色返回逻辑和配色方面，`CustomColourProvider`是基于`OverlayColourProvider`更改来的，主要是想让播放器界面和osu!其他界面的观尽可能保持一致。<br>
__原本的想法是根据RGB返回颜色，但因为暂时没有想出从RGB直接转换亮度、饱和度的方法~~(我懒)~~，就暂时搁置了<br>
__并且由于`OverlayColourProvider`根据色相返回颜色的逻辑，直接从RGB是没办法的。<br>
__所以现在自定义颜色的实现方案是先从配置获取用户给予的颜色(RGB)，然后用`Color4.ToHsl(R,G,B,1).X`获取对应的色相，再赋值给`HueColour`<br>
__接着颜色被其他组件调用时，由于`HueColour`的值已被改变，返回的就是更新后的颜色了。
{: .notice--info}

# **▪ 主界面**
`e3c3e0a` - 不要预加载`MvisScreen`

暂时用以解决在主界面设置完主题色后进入播放器，播放器界面颜色不更改的问题
{: .notice--info}

# **▪ MfConfigManager**
`1aabb49` - 添加3个设置键
  - `MvisInterfaceRed` - 界面主题色(红)
  - `MvisInterfaceGreen` - 界面主题色(蓝)
  - `MvisInterfaceBlue` - 界面主题色(绿)

~~暂时不会用到，但之后就说不定了。~~
{: .notice--info}