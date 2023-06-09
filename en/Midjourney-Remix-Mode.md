#### Use Remix Mode to change prompts, parameters, model versions, or aspect ratios between variations. Remix will take the general composition of your starting image and use it as part of the new Job. Remixing can help change the setting or lighting of an image, evolve a subject, or achieve tricky compositions.

`Remix` is an experimental feature that may change or be removed at any time.

___

## Using Remix

Activate Remix mode with the `/prefer remix` command or by using the `/settings` command and toggling the `🎛️ Remix Mode` button. Remix changes the behavior of the variation buttons (V1, V2, V3, V4) under image grids. When Remix is enabled, it allows you to edit your prompt during each variation. To Remix an upscale select `🪄 Make Variations`.

When `Remix` is enabled, Variation buttons turn green when used instead of blue.  
You can switch [Model Versions](https://docs.midjourney.com/models) when using Remix.  
When you are done with Remix use the `/settings` or `/prefer remix` command to turn it off.  
Create a standard image variation when Remix is active by not modifying the prompt in the pop-up window.

### Step 1

`line-art stack of pumpkins`

![Image of the Midjourney Make Variation Button](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Remix_1.png)

**Turn on Remix mode.**

Select an image grid or upscaled image to Remix.

### Step 2

`Remix`

![image showing the midjourney remix functionality and remix prompt dialog box.](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Remix2.png)

**Select "Make Variations."**

Modify or enter a new prompt in the pop-up.

### Results

`pile of cartoon owls`

![Image of a pile of owls, generated by using remix mode in Midjourney](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Remix3.png)

The Midjourney Bot generates an image using the new prompt with influence from the original image.

### Starting Image

![Midjourney image of a stack of pumpkins](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Remix_StackPumpkins.jpg)

line-art stack of pumpkins

### Model Change

![iImage showing an image of stacked pumpkins changed to with Midjourney Image Remix from the v4 to test model.](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Remix_testp.jpg)

line-art stack of pumpkins --test

### Subject Change

![Image showing an image of stacked pumpkins changed with Midjourney Image Remix from an illustration to balloon-animals](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Remix_Balloons.jpg)

balloon-animal shaped stack of pumpkins"

### Medium Change

![Image showing an image of stacked pumpkins changed with Midjourney Image Remix from the pumpkins to fruit](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Remix_Fruit.jpg)

vibrant illustrated stack of fruit

___

### Using Parameters with Remix

You can add or remove [Parameters](https://docs.midjourney.com/parameter-list) while using Remix mode, but you must use valid parameter combinations. Changing `/imagine prompt` `illustrated stack of pumpkins --version 3 --stylize 10000` to `illustrated stack of pumpkins --version 4 --stylize 10000` will return an error because Midjourney Model Version 4 is incompatible with the Stylize parameter.

Only parameters that normally influence variations will work while using Remix:

|  | Affects Initial  
Generation | Affects Variations  
and Remix |
| --- | --- | --- |
| Aspect Ratio\* | ✓ | ✓ |
| Chaos | ✓ |  |
| Image Weight | ✓ |  |
| No | ✓ | ✓ |
| Quality | ✓ |  |
| Seed | ✓ |  |
| Same Seed | ✓ |  |
| Stop | ✓ | ✓ |
| Stylize | ✓ |  |
| Tile | ✓ | ✓ |
| Video | ✓ | ✓ |

-   Changing aspect ratios with Remix will _stretch_ an image. It will not extend the canvas, add missing details, or fix a bad crop.

___

## How to Activate Remix

### Use the Settings Command

Type `/settings` and select `Remix` from the pop-up.  
`🎛️ Remix`

### Use the Prefer Remix Command

Type `/prefer remix` to toggle Remix mode on and off.  
![Image showing the Midjourney Prefer Remix Command](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_preferRemix.png)

Was this article helpful?