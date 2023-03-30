Midjourney机器人使用种子数字创建一个视觉噪声领域，例如电视静态，作为生成初始图像网格的起点。为每个图像随机生成种子数字，但可以使用“--seed”或“--sameseed”参数指定。使用相同的种子数字和提示将产生类似的结束图像。

“--seed”接受0-4294967295的整数。
“--seed”值仅影响初始图像网格。
“--seed”值[模型版本](https://docs.midjourney.com/models)1，“2”，“3”，“test”和“testp”是非确定性的，将生成类似的但不完全相同的图像。
在[模型版本](https://docs.midjourney.com/models)4，5和niji中使用相同的提示+种子+参数将产生相同的图像。

___

## 种子参数

如果未指定种子，则Midjourney将使用随机生成的种子数字，每次使用提示时产生各种各样的选项。

### 随机种子运行三次作业：

提示示例：`/imagine prompt celadon owl pitcher`


### 使用“--seed 123”运行两次作业:

提示示例：`/ imagine prompt celadon owl pitcher --seed 123`

![在midjourney V4中使用随机种子制作的图像网格示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Seed-123_V4_.png)

![在midjourney V4中使用随机种子制作的图像网格示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Seed-123_V4_.png)

___

## Sameseed参数

“--sameseed”参数值创建单个随机噪声场，应用于初始网格中的所有图像。当指定“--sameseed”时，初始网格中的所有图像都使用相同的起始噪声，将生成非常相似的生成图像。

“--sameseed”接受0-4294967295的整数。
“--sameseed”仅与[模型版本](https://docs.midjourney.com/models)1，“2”，“3”，“test”和“testp”兼容。

##### 来自--sameseed的早期视觉噪声

![使用Midjourney参数sameseed生成图像时使用的早期噪声场的示例图像](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Sameseed_Stop10.png)

`--sameseed 12345`

##### 使用--sameseed制作的完成作业

![使用Midjourney参数sameseed制作的图像示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Sameseed.png)

`--sameseed 12345`

##### 没有--sameseed的早期视觉噪声

![使用Midjourney生成图像时使用的早期噪声场的示例图片](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_seed_Stop10.png)

`--seed 12345`

##### 没有--sameseed制作的完成作业

![使用Midjourney制作的图像示例](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_seed.png)

`--seed 12345`

___

## 如何查找作业的种子数字

### 使用Discord Emoji Reaction

通过对作业使用✉️信封表情符号进行反应，在Discord中查找作业的种子数字。

![动画Gif显示如何在Discord中使用Emoji React与Envelop查找作业的种子数字](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_JobID_EmojiReact.gif)

### 使用Show命令恢复旧作业

要获取某个旧图像的种子号码，请[复制作业ID](https://docs.midjourney.com/docs/show-job)，然后使用该ID键入`/show <Job ID #>`命令来恢复该作业。然后可以对新生成的作业使用✉️信封表情符号进行反应。

___

## 如何更改种子数字

使用“--seed”或“--sameseed”参数，在提示的末尾添加“--seed <value>”或“--sameseed <value>”。

![动画Gif显示Midjourney Seed参数的输入方式](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Seed_Gif.gif)

**作业**是使用Midjourney Bot的任何操作。**作业**包括使用“/imagine”创建初始图像网格，升级图像和创建图像的变化。

本文有帮助吗？