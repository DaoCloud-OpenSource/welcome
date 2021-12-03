## 手册介绍

本手册主要介绍 `开源&AD` 团队工作内容，旨在让刚加入的船员有一个初步的认识，可以更快的融入到团队中来。在此之前，需要有一定的`知识储备`：

* [SCRUM](https://www.scrumcn.com/agile/scrum-knowledge-library/%e4%bb%80%e4%b9%88%e6%98%afscrum.html)： 是用于开发、交付和持续支持复杂产品的一个框架，是一个增量的、迭代的开发过程。在这个框架中，整个开发过程由若干个短的迭代周期组成，一个短的迭代周期称为一个`Sprint`，每个 Sprint 的长度是2周。
阅读[Scrum-Guide-Chineses](./docs/Scrum-Guide-Chinese.pdf)了解更多详情。
下面将介绍团队<a href="#chapter1">使用</a> SCRUM 的细节。

* [OKR](https://wiki.mbalib.com/wiki/OKR)：(Objectives and Key Results)，简称 OKR，翻译成中文叫“目标与关键结果”，OKR 就是一种讲述如何执行目标的管理方法。请预览 [OKR培训脑图](https://dwiki.daocloud.io/pages/viewpage.action?pageId=87835516)和[部门 OKR 主页](https://dwiki.daocloud.io/display/NDC/NDX+OKR)，下面将介绍怎么<a href="#chapter2">制定</a> OKR。

* [k8s开发Handbook](https://github.com/DaoCloud-OpenSource/handbook/blob/main/KubernetesDeveloperHandbook.md)：介绍 `kubernetes` 社区和怎么在社区工作的开发手册，帮助想加入社区的船员快速入门，必须掌握的内容。

* 团队：浏览[团队介绍](https://dwiki.daocloud.io/pages/viewpage.action?pageId=76295507)和[开源/AD 空间主页](https://dwiki.daocloud.io/pages/viewpage.action?pageId=76295473)可以让你快速了解团队详情。

## 日常工作

 ### <a id="chapter1">Jira</a>

[Jira](https://www.atlassian.com/zh/software/jira/guides/getting-started/overview) 是一套敏捷的工作管理解决方案。每两个星期为一个周期划分 Sprint，在 Sprint 开始前，将预计这个 Sprint 要完成的工作，在 Jira 上以故事的形式创建，创建的时候自己评估指定故事点（工作量）。每个 Sprint 以8个故事点为平衡点。不能完成的任务可以纳入下一个 Sprint 中。在 Sprint 开始前会进行评估，结束时进行总结分析。任务分为4个阶段：
 
 1. `代办`：还没有开始的任务，刚创建的任务都是代办状态；
 2. `处理中`：正在处理的任务；
 3. `阻塞`：阻塞状态一般指提交的 PR 还没有被 Merge 的任务。注意，被阻塞状态的任务如果在下个 Sprint 中如果还没有被完成，不宜将故事点分配更高；
 4. `完成`：已经完成的任务。

> 及时更新任务状态，任务过程中的细节可以适当使用英文或者中文评论，方便站立会同步。

### <a id="chapter2">OKR</a>

每个季度前会制定部门，团队及个人的 OKR，个人与团队的 OKR 应该保持一致的方向。OKR 的核心:

* 聚焦目标；
* 结果可衡量；
* 给自己一些挑战（完成0.7就是很不错，和 scrum 类似）；
* 与公司部门战略对齐；
* 开源特殊性，按照自己的积累和职业规划，尤其是学习方面有自驱力非常重要。

制定好自己的 OKR 后，在 [wiki](https://dwiki.daocloud.io/display/NDC/NDX+OKR) 上编辑保存。部门、团队及个人的 OKR 都放在 [wiki](https://dwiki.daocloud.io/display/NDC/NDX+OKR) 目录下，可供参考。在 OKR 开始前确定团队及个人的 OKR，结束时根据`打分系统`（0-1分）打分和总结：

| 分值 | 目标 |
| --- | --- |
| 1分 | 远远超过预期，几乎不可能达成 |
| 0.7分 | 虽然很难但可以达成（希望达成的目标） |
| 0.3 分 | 肯定能达成，只需要很少的帮助或者不需要帮助 |
| 0分| 没有任何的进展 |

### 周报

每周结束后会在 wiki 简单总结，周报实行部门轮岗制，当值船员在周五下午在群里通知并附加 wiki [链接](https://dwiki.daocloud.io/pages/viewpage.action?pageId=95579048)，下周一整理上报。建议在周五的时候写周报，因为没有公司的网络环境，需要[配置 VPN](https://dwiki.daocloud.io/pages/viewpage.action?pageId=41582354)。

### <a id="chapter3">会议</a>

工作日常中的会议都是以远程的形式进行，会议时间一般是不会有太大的变动，如果有变动会在群里通知，会议请`准时`参加。下面将所有会议详情整理如下：

| 会议 | 时长 | 方式 | 描述 | 注意事项 |
| --- | --- | --- | --- | --- |
| 站立会 | 20～30分钟 | 企业微信 | 每个船员会轮流过下上个工作日的状态，将工作内容跟大家做一个同步，整个过程中使用英语（初衷：为了提高英语口语能力参加兴趣小组的周会），难以用英语陈述的部分，可以使用中文代替 | 每个 Sprint 的周一因为要开计划会，所以当天不开站立会 |
| 计划会 1个小时 | 腾讯会议 | 明确 Sprint 任务目标，确定的优先级并调整到一个合理的范围 | 提前先计划好这个 Sprint 的任务 |
| 评审会 | 1～1.5个小时 | 腾讯会议 | 对整个 Sprint 的工作做一个评估，并生成量化图 | 提前更新任务状态，方便统计 |
| 回顾会 | 1～1.5个小时 | 腾讯会议 | 对这个 Sprint 工作做出评价，好的和不好的方面，不好的点会创建跟踪任务，等下次回顾会确认 | 可以先想好的和不好的方面，会上也有15分钟思考 |
| OKR 计划会 | 1～2个小时 | 腾讯会议 | 明确团队及个人的 OKR，大家相互交流意见 | 会前在 wiki 上准备好自己的 OKR 计划 |
| OKR 总结会 | 1~2小时 | 腾讯会议 | OKR 完成情况及总结（团队和个人） | 会前先写好个人的 OKR完成情况及总结 |

### 分享

将自己的知识分享给别人，互相成长，分享分为对内和对外分享：

* 每个 Sprint 的回顾会轮流分享（两周分享一次），分享内容自拟，跟开源工作相关。
* 工作日每天 9.30 的公司组织的晨会。
* 文档输出，优质文章可以在微信公众号发布。
* 公司组织的外部活动

### OnCall

解决产品线上问题，团队会轮值 OnCall，一般会有几个人一起完成，刚刚开始接触 OnCall 任务的船员不用着急，会有人带着一起做。

## 团队资源库

下面是日常工作过程中`常用`的资源列表，包括了 `wiki`，`github`，`gitbook` 上的知识和文档库：

| 文档 | 链接 | 备注 |
| --- | --- | --- |
| Handbook | https://github.com/DaoCloud-OpenSource/handbook/blob/main/KubernetesDeveloperHandbook.md | k8s开源社区开发指南 |
| Jira | https://jira.daocloud.io/secure/RapidBoard.jspa?rapidView=79&projectKey=DOS&view=detail&selectedIssue=DOS-72 |Sprint 工作任务体系 |
| OKR | https://dwiki.daocloud.io/display/NDC/NDX+OKR | wiki 上 OKR 主页 |
| 开源/AD 空间主页 | https://dwiki.daocloud.io/pages/viewpage.action?pageId=76295473 | 团队介绍和知识库 |
| 团队介绍 | https://dwiki.daocloud.io/pages/viewpage.action?pageId=76295507 | 团队船员的简介 |
| Oncall |  https://dwiki.daocloud.io/pages/viewpage.action?pageId=13869769 | DCE OnCall 轮值队列 |
| gitbook 知识库 | https://ericwvi.gitbook.io/cloud-native-network/ | 团队gitbook知识库（团队自己维护，需要大家持续更新维护的知识库） |
| 周报链接 | https://dwiki.daocloud.io/pages/viewpage.action?pageId=95579048 | 默认链接 |
| vsphere 简单教程 | https://dwiki.daocloud.io/pages/viewpage.action?pageId=95105963 | vsphere创建虚拟机建议教程 |
| VPN 设置方法 | https://dwiki.daocloud.io/pages/viewpage.action?pageId=41582354 | 适应于手机 |
| k8s基础知识 | https://dwiki.daocloud.io/pages/viewpage.action?pageId=13869829 | wiki 上整理了大量的 k8s 基础知识 |
| k8s开发指南 | https://dwiki.daocloud.io/pages/viewpage.action?pageId=63773874 | 类似 Handbook，值得参考 |
| DaoCloud OpenSource | https://github.com/DaoCloud-OpenSource | github DaoCloud OpenSource 主页 |
| DaoCloud | https://github.com/DaoCloud | github DaoCloud 主页 |
| KLTS | https://github.com/klts-io | github klts 主页 |

## 关于远程协作

目前团队船员来自不同的城市，base 不在上海的船员需要以远程协作的方式办公。下面是一些远程协作的日常事项。

* 会议和分享：上面所述的<a href="#chapter3">会议</a>都以腾讯会议或者微信的方式（站立会）开展，每个分公司需要提前找到会议室，保证网络畅通和避免回音，有特殊情况及时在群里沟通。

* 沟通：工作中，我们可以在企业微信，sclak，邮件，github等多渠道进行工作上的交流。刚入职的船员遇到什么工作的问题，可以多在群里提出自己疑问，如果有技术难题需要多人讨论的情况，也可以随时约一个远程会议。如果有自己的想法和感兴趣文章也可以及时的分享出来。让大家更好的了解到自己工作状态，促进工作效率。

## 转正答辩

入职一般在3～6个月，HR 会通知参加转正答辩，提前准备好答辩 PPT，内容重在展示自己的成果和工作总结，开源贡献，技术分享，发布公众号文章都可以作为自己强有力的成果。在日常工作中可以多积累一些贡献，做好 OKR 的总结，转正答辩将是非常轻松的事情。

## 正式加入

在正式加入之前，[这里](https://github.com/DaoCloud-OpenSource/welcome/issues/1)准备了 `小试牛刀` 的任务，顺利完成任务即可正式加入开源团队。
