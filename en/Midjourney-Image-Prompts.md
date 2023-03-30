#### You can use images as part of a prompt to influence a Job's composition, style, and colors. Images prompts can be used alone or with text prompts—experiment with combining images with different styles for the most exciting results.

To add images to a prompt, type or paste the web address where the image is stored online. The address must end in an extension like .png, .gif, or .jpg. After adding image addresses, add any additional text and parameters to complete the prompt.

![Image showing the Midjourney prompt structure.](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ%20Prompt.png)

Image prompts go at the front of a prompt.  
Prompts must have two images or one image and additional text to work.  
An image URL must be a direct link to an online image.  
In most browsers, right-click or long-press an image and select Copy Image Address to get the URL.  
The [`/blend` command](https://docs.midjourney.com/blend) is a simplified image prompting process optimized for mobile users.

___

## Upload an image to Discord

To use a personal image as part of a prompt, upload it to Discord. To upload an image, click the **Plus** sign next to where messages are typed. Select **Upload a File**, select an image, and send the message. To add this image to a prompt, begin typing `/imagine` as usual. After the prompt box appears, drag the image file into the prompt box to add the image's URL. Alternatively, right-click the image, select **Copy Link**, and then paste the link within the prompt box.

![Discord_FHZfwDLhLY.gif](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/Discord_FHZfwDLhLY.gif)

Privacy Notes

Upload images in your Direct Messages with the Midjourney Bot to prevent other server users from seeing an image.  
Image prompts are visible on the Midjourney website unless a user has Stealth Mode.

___

## Examples

### Starting Images

![Cropped image of the Bust of Apollo](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_ImagePrompt_Statue.png)

Statue of Apollo

![Cropped image of vintage flower illustraiton](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_ImagePrompt_Flowers.png)

Vintage Flower Illustration

![Cropped image of Ernst Haeckel's Jellyfish](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_ImagePrompt_Jelly.jpg)

Ernst Haeckel's Jellyfish

![Cropped image of Ernst Haeckel's Lichen](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_ImagePrompt_Lichen.png)

Ernst Haeckel's Lichen

![Cropped image of The Great Wave off Kanagawa](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_ImagePrompt_Wave.png)

Hokusai's The Great Wave

### Midjourney Model Version 4

___

### Midjourney Model Version 5

Aspect Ratio Tip

Crop images to the same aspect ratio as your final image for the best results.

___

## Image Prompts in V3

Image prompts in earlier [Midjourney Model Versions](https://docs.midjourney.com/models) are more abstract inspirations than in current models. An image prompt is not the same as building on top of (or "initializing" from) a starting input image. Image prompts are used as visual inspiration, not as a starting point.

### Image Weight, --iw

Earlier [Midjourney Model Versions](https://docs.midjourney.com/models) can use the image weight parameter `--iw` to adjust the importance of the image URLs vs. the text. `--iw 0.25` is the default and is used when no `--iw` is specified. Higher `--iw` values mean the image prompt will have more impact on the finished job.  
See the [Multi Prompts](https://docs.midjourney.com/multi-prompts) page for more information about the relative importance between parts of a prompt.

`--iw` accepts integers -10,000–10,000.

Example 1: The text prompt `vibrant California poppies` combined with an image prompt of a Kandinsky painting.  
**prompt: `http://kandinsky.png vibrant California poppies --v 3 --iw <value>`**

**Image Prompt** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/Kandinsky.png)

**`--iw .25`** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_IW2_025.png)

Image weight = .25

(the default image weight)

**`--iw 1`** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_IW2_1.png)

Image weight = 1

**`--iw 2`** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_IW2_2.png)

Image weight = 2

**`--iw 5`** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_IW2_5.png)

Image weight = 5

Example 2: The text prompt `vibrant California poppies` combined with an image prompt of Van Gogh's Sunflowers.  
**prompt: `http://sunflowers.png vibrant California poppies --v 3 --iw <value>`**

**Image Prompt** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/Vangogh.png)

**`--iw .25`** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_IW_025.png)

Image weight = .25

(the default image weight)

**`--iw 1`** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_IW_1.png)

Image weight = 1

**`--iw 2`** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_IW_2.png)

Image weight = 2

**`--iw 5`** ![](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_IW_5.png)

Image weight = 5

Subscribers can work one-on-one with the Midjourney Bot in Discord's Direct Messages instead of a public channel. Images made within your direct messages are still subject to content and moderation rules and will be visible on your Midjourney website gallery.

Was this article helpful?