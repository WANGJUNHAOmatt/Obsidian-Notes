
契机是萌萌想知道一个游戏是如何开发出来的，刚好我们两个人之前有玩过这个冰球的双人游戏。

我感觉这个游戏的机制不是特别复杂，所以准备试着开发一下，准备使用 Swift 开发一个 IOS 的应用，也算是借着这个契机学习一下 Swift 的游戏开发。


## 开发日志
2022-12-27 19:15 - 发现这个游戏的名字叫 Airhockey
2022-12-28 00:23 - 制作了简单的 游戏场地
2022-12-29 更新了游戏UI，在王雨辰帮助下，有了好看的 碟子 和 小球
2022-12-30 03:23 - 实现了触摸的控制逻辑，可以让小球被碟子击打，但击打后的速度存在问题

![[AirHockey-Day00.jpeg]]


## 游戏玩法

### 游戏简介

两名玩家，分别控制一个「碟子」在各自半场内击打「小球」，小球碰到场地内的「墙壁」可以反弹，到达对方缺口即小局获胜，记一分，小球到达「输球玩家」半场的发球点位上，率先达到特定分数的玩家获胜。

### 多种玩法

1. 趣味玩法
	1. 加电桩
		1. 【2】加沼泽：降低移动速度
		2. 【2】加速区：增加小球速度
	2. 加道具
		1. 冰冻法术：降低碟子移动速度
		2. 变大变小：改变 puck 速度
		3. 分裂球：一个球分裂成2个
		4. 碟子变化：
			1. 变形状：条形
			2. 变大小
	3. 改变场上道具属性
		1. 超弹墙
		2. 零摩擦模式
2. 多球模式

## 触摸逻辑

1. [x] 划分屏幕为上下两部分，分别为两个玩家所有
2. [x] 触摸碟子方可开始控制碟子
3. [x] 一个碟子只能被一个手指（触摸点）控制
4. [x] 允许玩家在控制碟子的过程中，达到对方半场，但碟子无法到达对方半场

## 碰撞模拟

1. [x] 计算碟子速度
2. [x] 计算小球速度
3. [x] 判断小球和碟子是否有接触
4. [ ] 计算碰撞后的小球速度

## 开发需求

- [ ] 首页界面导航
- [ ] 游戏 AI，支持单人游戏

## Bug to Fixed

- [ ] 存在碟子穿透下方 banner 和四周墙壁的问题
- [ ] 碰撞后速度异常，偶尔会突然变快
