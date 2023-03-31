---
title:  多个 prompts
weight: 2
---
使用`::`作为分隔符，Midjourney Bot可以将两个或更多单独的概念分别考虑。分离提示允许您将相对重要性分配给提示的部分。

## 多提示基础

在提示中添加双冒号`::`表示Midjourney Bot应考虑提示的每个部分。在下面的示例中，对于提示`热狗`，所有单词都被视为一体，Midjourney Bot会生成美味热狗的图片。如果将提示分为两个部分`热 :: 狗`，则会分别考虑两个概念，从而创建一个温暖狗的图片。

双冒号`::`之间没有空格
多提示适用于[模型版本](https://docs.midjourney.com/models)`1`、`2`、`3`、`4`和`niji`
任何[参数](https://docs.midjourney.com/parameter-list)仍添加到提示的末尾。

### `热狗`

![Midjourney提示热狗的图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_hotdog.jpg)

“热狗”被视为一个单独的想法。

### `热:: 狗`

![Midjourney提示热::狗的图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_hot-dog.jpg)

“热”和“狗”被分别认为是单独的想法

`蛋糕插图`

![Midjourney提示蛋糕插图的图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_cupCakeIllustration.jpg)

“蛋糕插图”被认为是一个整体，生成杯形蛋糕的图像。

`杯:: 蛋糕插图`

![Midjourney提示杯::蛋糕插图的图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_cup-cakeIllustration.jpg)

“杯”被认为与“蛋糕插图”分开，生成杯中的蛋糕的图像。

`杯:: 蛋糕:: 插图`

![Midjourney提示杯::蛋糕::插图的图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_cup-cake-illustration.jpg)

“杯”、“蛋糕”和“插图”被分别考虑，生成带有共同插图元素（如花和蝴蝶）的果冻杯蛋糕。

## 提示权重

当使用双冒号`::`将提示分为不同部分时，您可以在双冒号后立即添加数字，以指定该提示部分的相对重要性。

在下面的示例中，提示`热::狗`生成一个热狗。将提示更改为`热::2狗`使单词“热”的重要性是单词“狗”的两倍，从而生成一张非常“热”的狗的图片！

\[模型版本\] `1`、`2`、`3`只接受整数权重
\[模型版本\] `4` 可以接受带小数的权重
未指定的权重默认为1。

### `热:: 狗`

![Midjourney提示热::狗的图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_hot-dog.jpg)

“热”和“狗”被视为单独的想法

### `热::2狗`

![Midjourney提示热::2狗的图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_hot2-dog.jpg)

“热”的重要性是“狗”的两倍

**权重被标准化：**
`热::狗`与`热::1狗`、`热::狗::1`、`热::2狗::2`、`热:: 100狗::100`等相同。
`杯::2蛋糕`与`杯::4蛋糕::2`、`杯::100蛋糕::50`等相同。
`杯::蛋糕::插图`与`杯::1蛋糕::1插图::1`、`杯::1蛋糕::插图::`、`杯::2蛋糕::2插图::2`等相同。

### 负提示权重

可以在提示中添加负权重以删除不需要的元素。所有权重之和必须为正数。

`充满活力的郁金香田`

![Midjourney提示充满活力的郁金香田的图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_Tulips.jpg)

生成一系列彩色的郁金香。

`充满活力的郁金香田::红色::-0.5`

![显示Midjourney多提示中负权重的结果的图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_Tulips_NoRed.jpg)

少量红色减少出现的机会。

**权重被标准化，所以：**
`tulips::red::- 0.5`等同于`tulips::2 red::-1`、`tulips::200 red::-100`等。

### `--no`参数

`--no` [参数](https://docs.midjourney.com/v1/docs/parameter-list)与将多提示的部分权重设置为“-0.5”的情况相同`充满活力的郁金香田::红色::-0.5`等同于`充满活力的郁金香田--no red`。