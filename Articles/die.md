﻿*** Machine Translated
`Die`由海龟和链接使用，以将其从模型中移除。当要求海龟或链接`die` ，该海龟或链将不再存在于模型中，将不再执行任何代码，并且将从其所在的任何主体集合消失。例如，如果`count turtles`返回了10个，则`ask one-of turtles [die]`被叫来了，现在`count turtles`会返回9。

在下面的模型中，一群绵羊到处走动，吃草来获取能量。绵羊移动时会失去能量；如果绵羊的能量为0，它将死亡并从模型中删除。因此，我们包含以下代码来删除这些绵羊：

`if energy <= 0 [ die ]`