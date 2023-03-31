---
title: Setting命令
weight: 3
---
设置命令提供切换按钮，包括模型版本、样式值、质量值和升频器版本等常见选项。设置还有`/stealth`和`/public`命令的切换按钮。

![显示Midjourney设置命令界面的图像](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_settings.jpg)

___

`1️⃣ MJ Version 1` `2️⃣ MJ Version 2` `3️⃣ MJ Version 3` `4️⃣ MJ Version 4` `5️⃣ MJ Version 5`

`🌈 Niji Mode` `🤖MJ Test` `📷 MJ Test Photo`

`🔥 Half Quality` `🔥 Base Quality` `🔥 High Quality (2x cost)`

设置用于作业的[质量参数](https://docs.midjourney.com/quality)。
Half Quality = `--q .5`，Base Quality = `--q 1`，High Quality = `--q 2`。

`🖌️ Style Low` `🖌️ Style Med` `🖌️ Style High` `🖌️ Style Very High`

设置用于作业的[Stylize Parameter](https://docs.midjourney.com/stylize)。
Style Low = `--s 50`，Style Med = `--s 100`，Style High = `--s 250`，Style Very High = `--s 750`。

`🧍♂️Public` `🕵️ Stealth`

`🎛️ Remix`

`🐇 Fast` `🐢 Relax`

设置说明

在提示的末尾添加的参数将覆盖使用`/settings`进行的选择。

___

## 自定义首选项

使用首选命令创建自定义选项，以便自动向提示的末尾添加常用参数。
`/prefer auto_dm`：完成的作业将自动发送到直接消息。
`/prefer option`：创建或管理自定义选项。
`/prefer option list`：查看当前自定义选项。
`/prefer suffix`：指定要添加到每个提示末尾的后缀。

___

### 首选项

`/prefer option set <name> <value>`：创建自定义参数，可以快速将多个参数添加到提示的末尾。

![PreferOptionSet.png](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/PreferOptionSet.png)

`/prefer option set` `mine` `--hd --ar 7:4`：创建一个名为“mine”的选项，它转换为`--hd --ar 7:4`。

![PreferOptionSet_Used.jpg](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/PreferOptionSet_Used.jpg)

使用`/imagine prompt` `vibrant California poppies --mine`，被解释成`/imagine prompt` `vibrant California poppies --hd --ar 7:4`。

将“value”字段留空以删除选项。

`/prefer option list`：列出由`prefer option set`创建的所有选项。用户最多可以拥有20个自定义选项。

![PreferOptionList.png](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/PreferOptionList.png)

要删除自定义选项，请使用`/prefer option set` `<name to delete>`并将值字段留空。

___

### 后缀

`/prefer suffix`：将指定的后缀自动附加在所有提示后面。 **使用命令不带值进行重置。**

命令示例：`/prefer suffix` `--uplight --video`

仅可以使用[参数](https://docs.midjourney.com/parameter-list)与`/prefer suffix`一起使用，
`prefer suffix --no orange`可接受
`prefer suffix orange::-1`不被接受

订阅者可以与Midjourney Bot在Discord的直接消息中进行一对一的交流，而不是通过公共频道。在您的直接消息中创建的图像仍受内容和管制规则的约束，并将在Midjourney网站的画廊中可见。

本文是否有帮助？