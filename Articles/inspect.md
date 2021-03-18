﻿*** Machine Translated
`inspect`是用于打开给定主体的检查器面板的内置命令。这是打开检查器面板的几种方法之一，我们将在后面讨论。作为介绍，检查器面板提供了一种快速的方法来查看和更改给定主体的所有属性（海龟，格子，链）。NetLogo知道的有关主体的所有基础信息都是可见的，并且（几乎）都是可编辑的。

![检查器面板在绿色背景上显示一只白羊，然后显示许多标记为“谁”，“颜色”，“标题”等的可编辑文本字段。](/static/img/grass.png)

要从代码打开检查器面板，请使用`inspect <agent>` 。实际上，这通常看起来像是`inspect turtle 0` ，`inspect patch 0 0`或`inspect one-of turtles with [color = red]` 。但是，更常见的是，您需要从界面打开检查器面板。为此，请在给定的格子或给定的海龟上单击鼠标右键（对于MacOS，单击或单击鼠标，对于Windows，按住Control单击。）在选项列表中，有一个选项可以`inspect patch <x> <y>` ，如果在鼠标单击下有任何海龟，可以输入`turtle <number>` （您可以将其悬停以显示更多选项），第一个是将`inspect turtle <number>` 。

打开后，检查器面板允许您编辑主体的几乎所有属性的值，包括使用`turtles-own` ，`patches-own` ，`links-own`和`<breed>-own`通过代码内置和定义的属性。`<breed>-own` 。例如，您可以编辑海龟的`size` ，格子的`pcolor`或链的图形。请注意，任何更改都会立即应用到您正在检查的特定主体上，但是请记住，如果通过代码（例如，`setup`过程）创建了主体，则您下次在此处进行的所有更改都不会被记住创建。