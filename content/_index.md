+++
toc = true
+++


# INTRODUCTION

* * *
* * *
\
\
老渔夫是我和朋友们一起制作的一款横版闯关解密游戏，玩家将会在游戏中扮演一个渔夫，使用渔枪在梦境中穿梭，找寻自己失去的记忆并解开困在其心中对于海洋的恐惧。  

游戏由三个关卡构成，分别是沙滩、洞窟森林以及海底世界,下面是游戏内容的演示。  
\
\
{{< bilibili src="//player.bilibili.com/player.html?aid=641041346&bvid=BV1BY4y187fJ&cid=585273719&page=1" >}}
\
\
# Role & Responsibility
***
***
## 我在团队中负责的部分

* 玩法的设计与实现
* 沙滩、洞窟森林的关卡设计与搭建
* 粒子特效&蓝图编程

\
\

***
## 操作方式与蓝图
\
由于游戏的制作时间较短，我选择了蓝图作为游戏玩法的实现方式，操作上同时支持手柄与键鼠  
\
\
手柄操作方式的示意图
\
\
![test](images/controller2.png)
\
\
\
控制玩家行动的蓝图
\
\
![test](images/mainBP.png)
\
\
\
\
***
## 渔枪
\
渔枪的设计灵感来源于《unreval》(毛线小精灵)中摆荡跳跃玩法  
玩家使用鼠标左键射出鱼钩，"A","D"键左右摆动，并通过数字键"1","2"来控制绳子的长度  
\
\
(按下"1"后角色加速上升，摆荡后跳跃至船上)
\
\
![test](images/fishhook.gif)  
\
\
\
由于网络上能够搜寻到的横板钩爪相关蓝图教程很少，渔枪是我在实现玩法过程中遇到最大的困难。  
在参考了[相关视频](https://www.youtube.com/watch?v=zzp-HSOcemU&list=PL-ItXi7X4B2MTLcP0nioF1smJWau_kg0_&index=23&t=168s)后，我修改了角色摆荡受力的计算方式并增
加了角色运动方向的判定，使得渔枪的摆荡能够成功运行并更加自然
\
\
![test](images/swing.png)  
\
\
\
***
## 地图编辑
\
\
为了方便关卡的搭建，我制作了一个包含四种地形材质以及一个方便快速调整物品材质的材质球  
并为场景制作添加浮动的光点、鱼群等特效
\
\
![test](images/land.png) 
\
\
\
地面效果以及特效效果
\
\
![test](images/levelbuild.png) 
\
\
![test](images/levelingame.gif)

***
* The game was made by UE4 and coding by Blueprint

