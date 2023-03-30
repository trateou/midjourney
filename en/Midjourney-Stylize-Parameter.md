#### This Midjourney Bot has been trained to produce images that favor artistic color, composition, and forms. The `--stylize` or `--s` parameter influences how strongly this training is applied. Low stylization values produce images that closely match the prompt but are less artistic. High stylization values create images that are very artistic but less connected to the prompt.

`--stylize`'s default value is 100 and accepts integer values 0–1000 when using the default \[V4 model\].

Different [Midjourney Version Models](https://docs.midjourney.com/models) have different stylize ranges.

|  | Version 5 | Version 4 | Version 3 | Test / Testp | niji |
| --- | --- | --- | --- | --- | --- |
| Stylize default | 100 | 100 | 2500 | 2500 | NA |
| Stylize Range | 0–1000 | 0–1000 | 625–60000 | 1250–5000 | NA |

___

## Common Stylize Settings

### Midjourney Model V4

prompt example: `/imagine prompt` `illustrated figs --s 100`

##### `--stylize 50`

![Midjourney style parameter example. Image of the prompt illustrated figs with style=50](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stylize_0.jpg)

`🖌️ Style Low`

##### `--stylize 100` (default)

![Midjourney stylize parameter example. Image of the prompt illustrated figs with style=100](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stylize_100.jpg)

`🖌️ Style Med`

##### `--stylize 250`

![Midjourney stylize parameter example. Image of the prompt illustrated figs with style=250](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stylize_250.jpg)

`🖌️ Style High`

##### `--stylize 750`

![Midjourney stylize parameter example. Image of the prompt illustrated figs with style=750](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Stylize_750.jpg)

`🖌️ Style Very High`

___

### Midjourney Model V5

prompt example: `/imagine prompt` `colorful risograph of a fig --s 100`

##### `--stylize 0`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=0](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_0.jpg)

##### `--stylize 50`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=50](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_50.jpg)

##### `--stylize 100` (default)

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=100](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_100.jpg)

##### `--stylize 250`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=250](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_250.jpg)

##### `--stylize 750`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=750](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_750.jpg)

##### `--stylize 1000`

![Midjourney style parameter example. Image of the prompt colorful risograph of a fig stylize=1000](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_V5_Stylize_1000.jpg)

___

## How to Switch Stylization Values

### Use the Stylize Parameter

Add `--stylize <value>` or `--s <value>` to the end of your prompt.

![Animated Gif showing how to use the Midjourney style parameter.](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Parameter_Style.gif)

  

### Use the Settings Command

Type `/settings` and select your preferred stylize value from the menu.

`🖌️ Style Low` `🖌️ Style Med` `🖌️ Style High` `🖌️ Style Very High`

Was this article helpful?