---
title: Stylize
weight: 7
---
这个Midjourney Bot已经训练出能够支持艺术色彩、构图和形式的图像。`-stylize` 或 `-s` 参数会影响训练的强度。低的stylization值会产生与提示匹配度高但不太艺术的图像。而高的stylization值则会产生艺术感非常强但与提示联系不太紧密的图像。

`-stylize` 的默认值为100，在使用默认的\[V4模型\]时接受0-1000的整数值。

不同的[Midjourney版本模型](https://docs.midjourney.com/models)有不同的stylize范围：

|  | 版本5 | 版本4 | 版本3 | Test / Testp | niji |
| --- | --- | --- | --- | --- | --- |
| 默认的stylize值 | 100 | 100 | 2500 | 2500 | NA |
| stylize范围 | 0-1000 | 0-1000 | 625-60000 | 1250-5000 | NA |

___

## 常见的Stylize设置

### Midjourney模型V4

提示示例: `/imagine prompt` `illustrated figs --s 100`

##### `--stylize 50`

![Midjourney style parameter example. Image of the prompt illustrated figs with style=50](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stylize_0.jpg)

`🖌️ 低调的风格`

##### `--stylize 100` (默认)

![Midjourney stylize parameter example. Image of the prompt illustrated figs with style=100](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stylize_100.jpg)

`🖌️ 中等的风格`

##### `--stylize 250`

![Midjourney stylize parameter example. Image of the prompt illustrated figs with style=250](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stylize_250.jpg)

`🖌️ 高调的风格`

##### `--stylize 750`

![Midjourney stylize parameter example. Image of the prompt illustrated figs with style=750](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stylize_750.jpg)

`🖌️ 非常高调的风格`

___

### Midjourney模型V5

提示示例: `/imagine prompt` `colorful risograph of a fig --s 100`

##### `--stylize 0`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=0](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_0.jpg)

##### `--stylize 50`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=50](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_50.jpg)

##### `--stylize 100` (默认)

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=100](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_100.jpg)

##### `--stylize 250`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=250](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_250.jpg)

##### `--stylize 750`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=750](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_750.jpg)

##### `--stylize 1000`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=1000](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_1000.jpg)

___

## 如何切换Stylization值

### 使用Stylize参数

在您的提示末尾添加 `--stylize <value>` 或 `--s <value>`。

![Animated Gif showing how to use the Midjourney style parameter.](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Parameter_Style.gif)

### 使用设置命令

输入 `/settings` 并从菜单中选择您喜欢的Stylize值。

`🖌️ 低调的风格` `🖌️ 中等的风格` `🖌️ 高调的风格` `🖌️ 非常高调的风格`

本文是否有所帮助？