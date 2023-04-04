---
title: Quality
weight: 4
---
`--quality`或`--q`参数改变了生成图像所需的时间。高质量的设置需要较长的处理时间并生成更多细节。更高的数值也意味着每个作业使用的GPU分钟数更多。质量设置不影响分辨率。

默认的`--quality`值为1。更高的值会使用更多您的订阅GPU分钟。
`--quality`接受值：.25、.5和1，适用于默认模型。较大的值将舍入到1。
`--quality`仅影响初始图像生成。
`--quality`适用于[Model Versions](https://docs.midjourney.com/models) 1、2、3、4、5和niji。

___

## 质量设置

更高的`--quality`设置并不总是更好。有时，较低的`--quality`设置可以产生更好的结果-这取决于您试图创建的图像。较低的`--quality`设置可能最适合于手势抽象外观。更高的`--quality`值可以改善从许多细节中受益的建筑图像的外观。选择与您希望创建的图像类型最匹配的设置。

提示示例：`/imagine prompt` `木版画桦树林 --q .25`

### 版本 4

##### `--quality .25`

![Quality设置为0.25的Midjourney生成的图像示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Quality_025.jpg)

`-`

最快的结果，最少的细节

_4倍的速度和四分之一的GPU分钟数。_

##### `--quality .5`

![Quality设置为0.5的Midjourney生成的图像示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Quality_05.jpg)

`🔥 半质量`

较少的细节

_2倍的速度和一半的GPU分钟数。_

##### `--quality 1`

![Quality设置为1的Midjourney生成的图像示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Quality_1.jpg)

`🔥 基础质量`

默认设置

在详细程度和速度之间取得了良好的平衡。

### 版本 5

##### `--quality .25`

![Quality设置为0.25的Midjourney生成的图像示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Quality_025.jpg)

`-`

最快的结果，最少的细节

_4倍的速度和四分之一的GPU分钟数。_

##### `--quality .5`

![Quality设置为0.5的Midjourney生成的图像示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Quality_05.jpg)

`🔥 半质量`

较少的细节

_2倍的速度和一半的GPU分钟数。_

##### `--quality 1`

![Quality设置为1的Midjourney生成的图像示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Quality_1.jpg)

`🔥 基础质量`

默认设置

在详细程度和速度之间取得了良好的平衡。

___

### 版本质量兼容性

| 模型版本 | 质量 0.25 | 质量 0.5 | 质量 1 | 质量 2 |
| --- | --- | --- | --- | --- |
| 版本 5 | ✓ | ✓ | ✓ | \- |
| **版本 4** | ✓ | ✓ | ✓ | \- |
| 版本 3 | ✓ | ✓ | ✓ | ✓ |
| 版本 2 | ✓ | ✓ | ✓ | ✓ |
| 版本 1 | ✓ | ✓ | ✓ | ✓ |
| niji | ✓ | ✓ | ✓ | \- |

___

## 如何使用质量参数

### 使用`--quality`或`--q`参数

在提示的末尾添加`--quality <value>`或`--q <value>`。

![动画GIF显示Midjourney品质参数是如何键入的](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Parameter_Quality.gif)



### 使用设置命令

键入`/settings`，并从菜单中选择首选的`quality`值。

`🔥 半质量` `🔥 基础质量` `🔥 高质量 (2倍成本)`

Midjourney Bot会在高端GPU上处理作业。完成作业所需的每一分钟都是一个**GPU分钟**。在**快速模式**中，您拥有有限的GPU分钟数。因为图像生成可能在多个GPU上同时处理，GPU分钟与您等待图像生成的时间没有直接联系。

本文有帮助吗？