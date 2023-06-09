---
title: Aspect Radio
weight: 2
---
#### `--aspect`或`--ar`参数会改变生成图像的宽高比。图像的宽高比是它的宽度与高度的比率，通常用冒号分隔的两个数字表示，例如7:4或4:3。

正方形的图像宽高相等，通常被描述为1:1的宽高比。该图像可以是1000px × 1000px，也可以是1500px × 1500px，但其宽高比仍为1:1。计算机屏幕通常为16:10的比率，即宽度是高度的1.6倍。因此该图像可以是1600px × 1000px，4000px × 2000px，320px x 200px等。

默认的宽高比为1:1.
`--aspect`只能使用整数。请使用139:100而不是1.39:1。
宽高比影响生成图像的形状和构图。
在放大时，某些宽高比可能会略有改变。

___

### 最大宽高比

不同的[Midjourney版本模型](https://docs.midjourney.com/models)具有不同的最大宽高比。

|  | 版本5 | 版本4c (默认) | 版本4a或4b | 版本3 | 测试 / 测试p | niji |
| --- | --- | --- | --- | --- | --- | --- |
| 宽高比 | 任何\* | 1:2到2:1 | 仅：1:1、2:3或3:2 | 5:2到2:5 | 3:2到2:3 | 1:2到2:1 |

`--ar`参数将接受1:1（正方形）到每个模型的最大宽高比之间的任何宽高比。但是，在生成或放大图像期间，最终输出可能会略微修改。例如：使用`--ar 16:9`（1.78）的提示会创建具有`7:4`（1.75）宽高比的图像。

\* 宽高比大于2:1是实验性的，并可能产生不可预测的结果。

![常见Midjourney宽高比的比较图](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_AspectRatioChart.png)

提示示例：`想象 / 提示` `鲜艳的加利福尼亚罂粟 --ar 5:4`

### 常见Midjourney宽高比

`--aspect 1:1` 默认宽高比。
`--aspect 5:4` 常用的框架和印刷宽高比。
`--aspect 3:2` 印刷摄影中常见。
`--aspect 7:4` 接近高清电视屏幕和智能手机屏幕。

___

## 如何改变宽高比

### 使用宽高比参数

在提示的结尾添加`--aspect <值>:<值>`或`--ar <值>:<值>`。
![动图显示Midjourney版本参数的输入方式](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Parameter_Aspect.gif)

本文有帮助吗？