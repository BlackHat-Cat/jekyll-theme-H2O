---
layout: post
title: '生命游戏'
subtitle: 'Unity游戏开发心得'
date: 2017-11-10
categories: Unity3d
cover: '/assets/img/lang.jpg'
tags: 游戏
---
# 生命游戏

> 在方格中模拟生命的更替

---
## 游戏介绍

生命游戏是一款零玩家游戏，由英国数学家约翰·何顿·康威在1970年发明，在一个平面面网格中模拟生命

每个方格代表一个细胞，绿色代表生，蓝色代表死，可以通过点击来更改生死状态

点击箭头按钮进入下一轮更替

细胞的生死遵循以下规律：
1. 周围有3个细胞活着，则该细胞为生（若原本为生则不变）
2. 周围有2个细胞，则生死状态保持不变
3. 其他情况下，该细胞为死

---
通过不同的初始设置，可以观察的奇妙的图形变化

**过于分散** 这种模式下，细胞会向中间靠拢，并快速消亡

**过于集中** 内层细胞大面积死亡，周围的细胞则向外扩张，这种模式有时会出现从一小簇细胞团迅速长大的情况

**静态稳定** 根据第二条规则，一些模式可以达成 *每个细胞都有两个细胞* 的这种静态稳定，但是
> 有些人活着，但他已经死了

这些模式虽然是生的状态，但是表现出的则是死寂

**动态稳定** 一些模式可以循环固定的图案，实际上是他们新生成的图案和原来的图案在数学上相等，只是几何上不断旋转，这是一种思路：把握初心，但是要改变视角

---
## 开发后记

游戏在构思阶段相当完善，遇到的问题也都很快的解决了，从中学到了很多东西，几次迭代更新也都很顺利，美中不足的是在发布到网页时出现了一些错误，导致在本地可以完美的游戏在网页上无法工作

暂时还无法修复这个问题

**收获：**
- 开发了第一个完全自主的游戏
- 专注于代码，更高效的解决问题，排除图形渲染等的干扰
- 尝试了UI、音效等等

**不足：**
- 在发布方面遇到的问题依然没有很好的解决
- 发布版的UI没能很好的适应屏幕
