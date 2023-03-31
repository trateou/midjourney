---
title: 订阅计划
weight: 1
---
Midjourney有三种订阅等级。按月付款或整年付款可享受20%的折扣。每个订阅计划包括访问Midjourney会员画廊、官方Discord、一般商业使用条款等等。如何订阅使用"/subscribe"命令生成个人链接到订阅页面。或者，访问[Midjourney.com/account](https://www.midjourney.com/account/) 或者在登录Midjourney网站后选择侧栏中的"Manage Sub"。

## 计划比较

|   | 免费试用  | 基础计划  | 标准计划  | 专业计划  |
|---|---|---|---|---|
|每月订阅费用 | -  | $10 | $30 | $60 |
|年度订阅费用 | - | $96（$8 /月）| $288（$24 /月） | $576（$48/月）|
|快速GPU时间|0.4小时/终身 |3.3小时/月 |15小时/月 |30小时/月 |
|每月松弛GPU时间 | - | - | 无限制 | 无限制 |
|购买额外GPU时间 | - | $4/小时 | $4/小时 | $4/小时 |
|在你的直接消息中独立工作 | - | ✓ | ✓ | ✓ |
|隐形模式 | - | - | - | ✓ |
|最大队列 | 3个并发作业和10个等待队列 | 3个并发作业和10个等待队列 | 3个并发作业和10个等待队列 | 12个并发快速作业，3个并发松弛作业和10个等待队列 |
|评定图片以赚取免费GPU时间  | - | ✓ | ✓ | ✓ |
|使用权 | [CC BY-NC 4.0](http://creativecommons.org/licenses/by-nc/4.0/) | 通用商业条款* | 通用商业条款* | 通用商业条款* |

- 如果您曾经订阅过，则可以在几乎任何方式中使用您的图片。如果您的公司每年的总收入超过1,000,000美元，则必须购买专业版。有关完整详情，请参阅[条款](https://docs.midjourney.com/terms-of-service)。

## 订阅计划

访问[https://www.midjourney.com/account/](https://www.midjourney.com/account/)或使用"/subscribe"命令生成链接到订阅页面。不要分享您的链接，每个账户的链接是唯一的，不应与其他人分享！

### 付款方式

目前仅接受[Stripe支持的付款方式](https://stripe.com/docs/payments/cards/supported-card-brands)：例如Mastercard ，VISA或美国运通所发行的信用或借记卡 。Stripe是PCI服务提供商等级1，在支付行业中可获得最严格的认证。在某些地区，谷歌支付和Apple Pay可用。不支持PayPal，电汇和类似方法。

## 管理您的计划

在[https://www.midjourney.com/account/](https://www.midjourney.com/account/)上管理您的订阅计划。

![显示Midjourney订阅者管理订阅页面的图像](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_AccountPage.png)

### 月度续订

未使用的月度快速GPU时间不会滚动。订阅续订时，快速模式会自动重新激活。

### 切换计划

可随时升级或降级计划。在升级时，您可以选择升级是否立即生效，或在当前计费周期结束时生效。如果您选择立即升级，将根据您从升级的计划中使用情况提供按比例计算的价格。降级总是在当前计费周期结束时生效。

![显示Midjourney订阅者升级和降级计划的Midjourney账户页面的图像](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Plan_Upgrade.png)

### 取消订阅

在任何时候访问[https://www.midjourney.com/account/](https://www.midjourney.com/account/)以取消订阅。取消订阅在当前计费周期结束时生效。订阅优惠，如访问社区画廊，在当前计费周期结束前仍可使用。

![显示Midjourney订阅用户管理和取消计划的弹出窗口的图像](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_CancelPlan.png)

取消订阅时不会删除已生成的图像。随时通过访问[https://www.midjourney.com/account/](https://www.midjourney.com/account/)重新订阅计划。

### 退款

对于使用的月度GPU分钟少于1％的订阅者，包括松弛模式中使用的时间，可以获得退款。如果您有资格进行退款，则当您单击取消帐户时，对话框将自动弹出。

![显示Midjourney账户页面退款对话框的图像](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_PlanRefund.png)

## 购买更多快速GPU时间

在每月订阅续订之前用完了快速GPU并想购买更多？您可以购买额外的快速GPU时间，每小时4美元。该成本按增量计费，并在月底或达到计费阈值时（基本计划的每月价格）收费。小时价格是试验性的，可能会更改。

在您的[Midjourney账户页面](http://www.midjourney.com/account)上购买更多的快速GPU时间。购买的快速GPU时间不会过期，但您必须有一个活动订阅才能使用它们。

## 帐户信息

使用“/info”命令查看有关您的帐户的信息，包括订阅期剩余的快速时间，生命周期使用统计数据，排队或运行作业的数量以及订阅续订日期。

![用户信息面板](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_Command_Info_Result.png)

图像生成有两种模式，快速模式和松弛模式。快速模式尝试即时提供GPU。它是最高优先级的处理层，并使用您订阅的每月GPU时间。松弛模式将您的生成排队在其他人之后，根据您使用系统的情况。等待时间有所变化，通常为1-10分钟。默认情况下，使用快速模式生成图像。如果您有标准或专业的订阅，可以切换到松弛模式。

这篇文章对您有帮助吗？