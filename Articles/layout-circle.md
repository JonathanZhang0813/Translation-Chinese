﻿*** Machine Translated
`layout-circle`是一种基元，它将主体集合或海龟列表移动到给定半径的均匀间隔的圆中。语法为：

`layout-circle agentset radius`

它通常与使用链接的模型一起使用，因为它可以轻松查看哪些海龟与哪些海龟相连。海龟将在世界中心周围形成圆圈，并将全部面向外。`layout-circle`是一个观察者命令（不在`ask`块中调用），因为它“一次”作用于所有海龟，而不是一次作用于所有海龟。使用主体集合，海龟的顺序是随机的，但与海龟列表一起使用时，海龟以给定的顺序顺时针排列，从圆的顶部开始。

下面的模型显示了网络图中`layout-circle`的典型用法。