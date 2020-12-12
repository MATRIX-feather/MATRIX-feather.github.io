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

断更好久了...🤔

# 游戏本体
## de29f34
### 设置
- 实现Locale设置

<br>

## c32b93c
### osu!
- **添加osu!CursorDance**

来自[TechnoJo4/osu](https://github.com/TechnoJo4/osu)<br>
同样看看[PercyDan54/osu](https://github.com/PercyDan54/osu/tree/custom)的CorsorDance！
{: .notice--info}

## 52ff8d3
### osu!
- 补全osu!CursorDance设置翻译

## 8d58131
### API
- 添加当api请求失败信息的翻译(*Error occurred while handling an API request. -> 处理API请求时出现了问题。*)

## 94404f9
### 杂项
- 修复代码错误

## 7c5ae26
### 翻译支持
- **添加`英语(美国)`及`中文(简体)`的翻译文件**

### 杂项
- 初步添加对自定义框架的引用

### 歌曲选择
- `SetPanelContent`: 使用旧版方案(以原语言显示歌曲信息; ShowUnicode)

## 1d35783
### 翻译支持
- 添加`火星文`的翻译文件
- 更新`英语(美国)`和`中文(简体)`的语言翻译
- **实现`MLocaleManager`**

### M.Resources
- 修复翻译文件没有被囊括进资源的问题

## fbe3f42
### 杂项
- **添加对自定义框架的引用**

## 66bf096
### README
- 添加项目克隆教程以及翻译相关教程

## d6d910f
### README
- 修正文案错误

## 5da615b
### 翻译支持
- 更新翻译模板
- 更新`英语(美国)`和`中文(简体)`的语言翻译

意外解决了一些困扰已久的翻译问题(如何能让一些框架设置项也显示中文)
{: .notice--info}

## 76e4247
### README
- 更新文案

## 8be6ed4
### osu!
- 修复编辑器报错

# 框架
## b6b758c
### 翻译支持
- 实现基本的翻译支持

## 052cde4
### 翻译支持
- `LocalisedBindableString`: 对翻译获取添加`text.ShouldLocalise`条件
- `LocalisedString`: 当`text.original`为空时赋值为`text.Msgid`的值

## a5d2e43
### 翻译支持
- **移除对M.Resources的依赖**
- `SpriteText`: 添加`UseLegacyUnicode`属性
- `ILocalisedBindableString`: 添加`UseLegacyUnicode`属性

UseLegacyUnicode: 是否使用之前的Unicode方案，即是否以原语言显示歌曲信息(在osu!lazer中)<br>
PS: 这时候我还不知道要如何将这个属性通过SpriteText传到ILocalisedBindableString那里，所以就放在那里成待办事项了。
{: .notice}

- `LocalisationManager`: 通过`SetCatalog()`函数来获取mo翻译文件
- `LocalisedBindableString`: 适应新的变动

## b37c3ba
### 翻译支持
- `LocalisedBindableString`: 修复逻辑问题

## `2f99e95`
### 翻译支持
- `SpriteText`: 将`UseLegacyUnicode`作为参数传给`localisation.GetLocalisedString()`
- `LocalisationManager`: 通过参数设置`LocalisedBindableString`的`UseLegacyUnicode`属性
- `LocalisedBindableString`: 适应新的变动

## `9adf2d2`
### 翻译支持
- `SpriteText`: bug修复

因为实现方式，在某些情况下会出现文本不更新的情况
{: .notice}