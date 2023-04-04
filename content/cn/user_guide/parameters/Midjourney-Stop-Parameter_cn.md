---
title: Stop
weight: 6
---
使用`--stop`参数可以在作业处理过程中提前结束，但是在较早的百分比处停止作业会造成模糊，缺乏细节的结果。

`--stop`接受值: 10-100。默认的`--stop`值为100。在[放大](https://docs.midjourney.com/upscalers)期间，不起作用。

---

## 停止比较

提示示例：`/imagine prompt` `splatter art painting of acorns --stop 90`

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_10.png)

\--stop 10

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_20.png)

\--stop 20

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_30.png)

\--stop 30

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_40.png)

\--stop 40

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_50.png)

\--stop 50

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_60.png)

\--stop 60

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_70.png)

\--stop 70

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_80.png)

\--stop 80

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_90.png)

\--stop 90

![Midjourney Stop参数示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_stop_100.png)

\--stop 100

---

## 停止参数对放大的影响

`--stop`参数不影响放大作业。但是，停止将生成一个较为柔和，缺乏细节的初始图像，这将影响最终放大结果的详细程度。以下放大图像使用[Beta Upscaler](https://docs.midjourney.com/v1/docs/upscalers)。

![使用停止20进行初始网格图像和图像放大后的比较](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_Up_20.png)

\--stop 20

![使用停止80进行初始网格图像和图像放大后的比较](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_Up_80.png)

\--stop 80

![使用停止90进行初始网格图像和图像放大后的比较](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_Up_90.png)

\--stop 90

![使用停止100进行初始网格图像和图像放大后的比较](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stop_Up_100.png)

\--stop 100

---

## 如何更改停止百分比

### 使用`--stop`参数

在提示的结尾添加`--stop <value>`。

![Midjourney Stop参数的输入示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Parameter_Stop.gif)



本文是否有帮助？