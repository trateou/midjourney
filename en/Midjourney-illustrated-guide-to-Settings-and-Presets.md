#### The Settings command provides toggle buttons for common options like model version, style value, quality value, and upscaler version. Settings also has toggle buttons for the `/stealth` and `/public` commands.

![Image showing the interface of the Midjourney settings command](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_settings.jpg)

___

`1️⃣ MJ Version 1` `2️⃣ MJ Version 2` `3️⃣ MJ Version 3` `4️⃣ MJ Version 4` `5️⃣ MJ Version 5`

`🌈 Niji Mode` `🤖MJ Test` `📷 MJ Test Photo`

`🔥 Half Quality` `🔥 Base Quality` `🔥 High Quality (2x cost)`

Sets the [Quality Parameter](https://docs.midjourney.com/quality) used for jobs.  
Half Quality = `--q .5`, Base Quality = `--q 1`, High Quality = `--q 2`.

`🖌️ Style Low` `🖌️ Style Med` `🖌️ Style High` `🖌️ Style Very High`

Sets the [Stylize Parameter](https://docs.midjourney.com/stylize) used for jobs.  
Style Low = `--s 50`, Style Med = `--s 100`, Style High = `--s 250`, Style Very High = `--s 750`,

`🧍♂️Public` `🕵️ Stealth`

`🎛️ Remix`

`🐇 Fast` `🐢 Relax`

Settings Note

Parameters added to the end of a prompt will override selections made using `/settings`.

___

## Custom Preferences

Create custom options using prefer commands to add commonly used parameters to the end of prompts automatically.  
`/prefer auto_dm` Completed Jobs are automatically sent to Direct Message  
`/prefer option` Create or manage a custom option.  
`/prefer option list` View your current custom options.  
`/prefer suffix` specify a suffix to add to the end of every prompt.

___

### Prefer Option

`/prefer option set <name> <value>` Creates a custom parameter that you can use to add multiple parameters to the end of prompts quickly.

![PreferOptionSet.png](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/PreferOptionSet.png)

`/prefer option set` `mine` `--hd --ar 7:4` creates an option called "mine" that translates to `--hd --ar 7:4`.

![PreferOptionSet_Used.jpg](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/PreferOptionSet_Used.jpg)

Using `/imagine prompt` `vibrant California poppies --mine`, is interpreted as `/imagine prompt` `vibrant California poppies --hd --ar 7:4`.

Leave the "value" field empty to delete an option.

`/prefer option list` list all options created with `prefer option set.` Users can have up to 20 custom options.

![PreferOptionList.png](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/PreferOptionList.png)

To delete a custom option, use `/prefer option set` `<name to delete>` and leave the value field blank.

___

### Prefer Suffix

`/prefer suffix` automatically appends the specified suffix after all prompts. **Use the command without a value to reset.**

Command example: `/prefer suffix` `--uplight --video`

Only [Parameters](https://docs.midjourney.com/parameter-list) can be used with `/prefer suffix`,  
`prefer suffix --no orange` is accepted  
`prefer suffix orange::-1` is not accepted

Subscribers can work one-on-one with the Midjourney Bot in Discord's Direct Messages instead of a public channel. Images made within your direct messages are still subject to content and moderation rules and will be visible on your Midjourney website gallery.

Was this article helpful?