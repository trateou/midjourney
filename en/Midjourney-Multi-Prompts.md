#### It is possible to have the Midjourney Bot consider two or more separate concepts individually using `::` as a separator. Separating prompts allows you to assign relative importance to parts of a prompt.

## Multi-Prompt Basics

Adding a double colon `::` to a prompt indicates to the Midjourney Bot that it should consider each part of the prompt separately.  
In the example below, for the prompt `hot dog` all words are considered together, and the Midjourney Bot produces images of tasty hotdogs. If the prompt is separated into two parts, `hot:: dog` both concepts are considered separately, creating a picture of a dog that is warm.

There is no space between the double colons `::`  
Multi-prompts work with [Model Versions](https://docs.midjourney.com/models) `1`, `2`, `3`, `4` and `niji`  
Any [parameters](https://docs.midjourney.com/parameter-list) are still added to the very end of the prompt.

### `hot dog`

![Image of the Midjourney Prompt hotdog](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_hotdog.jpg)

_Hot dog_ is considered as a single thought.

### `hot:: dog`

![Image of the Midjourney Prompt hot:: dog](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_hot-dog.jpg)

_Hot_ and _dog_ Hot and dog are considered separate thoughts

`cup cake illustration`

![Image of the Midjourney Prompt cup:: cake illustration](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_cupCakeIllustration.jpg)

_Cup cake illustration_ is considered together producing illustrated images of cup cakes.

`cup:: cake illustration`

![Image of the Midjourney Prompt cup:: cake illustration::](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_cup-cakeIllustration.jpg)

_Cup_ is considered separately from _cake illustration_ producing images of cakes in cups.

`cup:: cake:: illustration`

![Image of the Midjourney Prompt cup:: cake:: illustration::](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_cup-cake-illustration.jpg)

_Cup_, _cake_, and _illustration_ are considered separately, producing a cake in a cup with common illustration elements like flowers and butterflies.

## Prompt Weights

When a double colon `::` is used to separate a prompt into different parts, you can add a number immediately after the double colon to assign the relative importance to that part of the prompt.

In the example below, the prompt `hot:: dog` produced a dog that is hot. Changing the prompt to `hot::2 dog` makes the word **hot** twice as important as the word dog, producing an image of a dog that is _very hot!_

\[Model Versions\] `1`, `2`, `3` only accept whole numbers as weights  
\[Model Versions\] `4` can accept decimal places for weights  
Non-specified weights default to 1.

### `hot:: dog`

![Image of the Midjourney Prompt hot:: dog](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_hot-dog.jpg)

_Hot_ and _dog_ are considered as separate thoughts

### `hot::2 dog`

![Image of the Midjourney Prompt hot::2 dog](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_hot2-dog.jpg)

_Hot_ is twice as important as _Dog_

**Weights are normalized:**  
`hot:: dog` is the same as `hot::1 dog`, `hot:: dog::1`,`hot::2 dog::2`, `hot::100 dog::100`, etc.  
`cup::2 cake` is the same as `cup::4 cake::2`, `cup::100 cake::50` etc.  
`cup:: cake:: illustration` is the same as `cup::1 cake::1 illustration::1`, `cup::1 cake:: illustration::`, `cup::2 cake::2 illustration::2` etc.

### Negative Prompt Weights

Negative weights can be added to prompts to remove unwanted elements.  
The sum of all weights must be a positive number.

`vibrant tulip fields`

![Image of the Midjourney Prompt vibrant tulip fields](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_Tulips.jpg)

A range of colored tulips are produced.

`vibrant tulip fields:: red::-.5`

![Image showing the results of negative weights when multi prompting in Midjourney](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Multi_Tulips_NoRed.jpg)

_Tulip fields are less likely to contain the color red._

**Weights are normalized so:**  
`tulips:: red::-.5` is the same as `tulips::2 red::-1`, `tulips::200 red::-100`, etc.

### The `--no` Parameter

The `--no` [parameter](https://docs.midjourney.com/v1/docs/parameter-list) is the same as weighing part of a multi prompt to "-.5" `vibrant tulip fields:: red::-.5` is the same as `vibrant tulip fields --no red`.

Was this article helpful?