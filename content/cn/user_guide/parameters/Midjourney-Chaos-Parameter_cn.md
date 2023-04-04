---
title: Chaos
weight: 3
---
`--chaos`或`--c`参数影响初始图像网格的差异程度。高`--chaos`值将生成更不寻常和意外的结果和构图，低`--chaos`值则会产生更可靠和可重复的结果。

`--chaos`接受0-100的值。
默认的`--chaos`值为0。

___

## 混沌对作业的影响

### 低`--chaos`值

使用较低的`--chaos`值，或者不指定值，将产生每次运行Job时略微变化的初始图像网格。

提示示例：`imagine/ prompt` `watermelon owl hybrid`

### 高`--chaos`值

使用较高的`--chaos`值将生成每次运行作业时更加多样化和意外的初始图像网格。

提示示例：`imagine/ prompt` `watermelon owl hybrid --c 50`

### 非常高的`--chaos`值

使用极高的`--chaos`值将生成具有意外构图或艺术媒介的初始图像网格，每次运行作业时变化非常多样化。

提示示例：`imagine/ prompt` `watermelon owl hybrid --c 100`

___

## 如何更改混沌值

### 使用`--chaos`或`--c`参数

将`--chaos<value>`或`--c<value>`添加到提示的末尾。

![Animated Gif showing how the Midjourney chaos parameter is typed](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Parameter_Chaos.gif)

**作业**是使用Midjourney机器人执行的任何操作。 **作业**包括使用`/imagine`创建初始图像网格，提高图像分辨率和创建图像变化。

这篇文章有用吗？