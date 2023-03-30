#### Parameters are options added to a prompt that change how an image generates. Parameters can change an image's [Aspect Ratios](https://docs.midjourney.com/aspect-ratios), switch between Midjourney [Model Versions](https://docs.midjourney.com/models), change which [Upscaler](https://docs.midjourney.com/upscalers) is used, and lots more.

Parameters are always added to the end of a prompt. You can add multiple parameters to each prompt.

![Example of how Midjourney parameters are used.](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Parameters_example.png)

Using an Apple device?

Many apple devices automatically change double hyphens (--) to an em-dash (—). Midjourney accepts both!

___

## Basic Parameters

### [Aspect Ratios](https://docs.midjourney.com/aspect-ratios)

`--aspect`, or `--ar` Change the aspect ratio of a generation.

### [Chaos](https://docs.midjourney.com/chaos)

`--chaos <number 0–100>` Change how varied the results will be. Higher values produce more unusual and unexpected generations.

### [No](https://docs.midjourney.com/multi-prompts)

`--no` Negative prompting, `--no plants` would try to remove plants from the image.

### [Quality](https://docs.midjourney.com/quality)

`--quality <.25, .5, 1, or 2>`, or `--q <.25, .5, 1, or 2>` How much rendering quality time you want to spend. The default value is 1. Higher values cost more and lower values cost less.

### [Seed](https://docs.midjourney.com/seeds)

`--seed <integer between 0–4294967295>` The Midjourney bot uses a seed number to create a field of visual noise, like television static, as a starting point to generate the initial image grids. Seed numbers are generated randomly for each image but can be specified with the --seed or --sameseed parameter. Using the same seed number and prompt will produce similar ending images.

### [Stop](https://docs.midjourney.com/stop)

`--stop <integer between 10–100>` Use the `--stop` parameter to finish a Job partway through the process. Stopping a Job at an earlier percentage can create blurrier, less detailed results.

### [Style](https://docs.midjourney.com/models)

`--style <4a, 4b or 4c>` Switch between versions of the Midjourney [Model Version](https://docs.midjourney.com/docs/models) 4

### [Stylize](https://docs.midjourney.com/stylize)

`--stylize <number>`, or `--s <number>` parameter influences how strongly Midjourney's default aesthetic style is applied to Jobs.

### [Uplight](https://docs.midjourney.com/upscalers)

`--uplight` Use an alternative "light" upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image is less detailed and smoother.

### [Upbeta](https://docs.midjourney.com/upscalers)

`--upbeta` Use an alternative beta upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image has significantly fewer added details.

### Default Values (Model Version 4)

|  | Aspect Ratio | Chaos | Quality | Seed | Stop | Style | Stylize |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Default Value  
 | 1:1 | 0 | 1 | Random | 100 | 4c | 100 |
| Range  
 | 1:2–2:1 | 0–100 | .25 .5 or 1 | whole numbers 0–4294967295 | 10–100 | 4a, 4b, or 4c | 0–1000 |

### Default Values (Model Version 5)

|  | Aspect Ratio | Chaos | Quality | Seed | Stop | Stylize |
| --- | --- | --- | --- | --- | --- | --- |
| Default Value  
 | 1:1 | 0 | 1 | Random | 100 | 100 |
| Range  
 | any | 0–100 | .25 .5, or 1 | whole numbers 0–4294967295 | 10–100 | 0–1000 |

-   Aspect ratios greater than 2:1 are experimental and may produce unpredicatble results.

## Model Version Parameters

Midjourney routinely releases new model versions to improve efficiency, coherency, and quality. Different models excel at different types of images.

### [Niji](https://docs.midjourney.com/models)

`--niji` An alternative model focused on anime style images.

### [High Definition](https://docs.midjourney.com/models)

`--hd` Use an early alternative [Model](https://docs.midjourney.com/models) that produces larger, less consistent images. This algorithm may be suitable for abstract and landscape images.

### [Test](https://docs.midjourney.com/models)

`--test` Use the Midjourney special test model.

### [Testp](https://docs.midjourney.com/models)

`--testp` Use the Midjourney special photography-focused test model.

### [Version](https://docs.midjourney.com/models)

`--version <1, 2, 3, 4, or 5>` or `--v <1, 2, 3, 4, or 5>` Use a different version of the Midjourney algorithm. The current algorithm (V4) is the default setting.

## Upscaler Parameters

Midjourney starts by generating a grid of low-resolution image options for each Job. You can use a Midjourney upscaler on any grid image to increase the size and add additional details. There are multiple upscale models available for upscaling an image.

### [Uplight](https://docs.midjourney.com/upscalers)

`--uplight` Use an alternative "light" upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image is less detailed and smoother.

### [Upbeta](https://docs.midjourney.com/upscalers)

`--upbeta` Use an alternative beta upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image has significantly fewer added details.

### [Upanime](https://docs.midjourney.com/upscalers)

Use an alternative upscaler trained to work with the when selecting the U buttons. This upscaler was specifically created to work with the `--niji` Midjourney Model.

## Other Parameters

These parameters only work with specific earlier Midjourney Models

### [Creative](https://docs.midjourney.com/models)

`--creative` Modify the `test` and `testp` models to be more varied and creative.

### [Image Weight](https://docs.midjourney.com/image-prompts)

`--iw` Sets image prompt weight relative to text weight. The default value is --iw 0.25.

### [Sameseed](https://docs.midjourney.com/seeds)

`--sameseed` Seed values create a single large random noise field applied across all images in the initial grid. When --sameseed is specified, all images in the initial grid use the same starting noise and will produce very similar generated images.

### [Video](https://docs.midjourney.com/video)

`--video` Saves a progress video of the initial image grid being generated. Emoji react to the completed image grid with ✉️ to trigger the video being sent to your direct messages. `--video` does not work when upscaling an image.

___

## Compatibility

### Model Version & Parameter Compatability

|  | Affects initial generation | Affects variations + remix | Version 5 | Version 4 | Version 3 | Test / Testp | Niji |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Max Aspect Ratio | ✓ | ✓ | any | 1:2 or 2:1 | 5:2 or 2:5 | 3:2 or 2:3 | 1:2 or 2:1 |
| Chaos | ✓ |  | ✓ | ✓ | ✓ | ✓ | ✓ |
| Image Weight | ✓ |  | ✓ |  | ✓ | ✓ |  |
| No | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Quality | ✓ |  | ✓ | ✓ | ✓ |  | ✓ |
| Seed | ✓ |  | ✓ | ✓ | ✓ | ✓ | ✓ |
| Sameseed | ✓ |  |  |  | ✓ |  |  |
| Stop | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Style |  |  |  | 4a and 4b |  |  |  |
| Stylize | ✓ |  | 0–1000  
default=100 | 0–1000  
default=100 | 625–60000  
default=2500) | 1250–5000  
default=2500) |  |
| Tile | ✓ | ✓ | ✓ |  | ✓ |  |  |
| Video | ✓ |  |  |  | ✓ |  |  |
| Number of Grid Images | \- | \- | 4 | 4 | 4 | 2 (1 when aspect ratio≠1:1) |  |

___

### Deprecated Parameters

\--width and --w (replaced with --aspect)  
\--height and --h (replaced with --aspect)  
\--fast (replaced with --quality)  
\--vibe (now known as V1)  
\--hq  
\--newclip  
\--nostretch  
\--old  
\--beta

Was this article helpful?