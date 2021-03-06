---
layout: article
title: "我是如何拿到Facebook Offer的"
modified:
categories: mysql
#excerpt:
tags: [facebook, interview, 面试]
image:
    feature: /teaser/facebook_feature.jpg
    teaser: /teaser/facebook.jpg
#  thumb:
date: 2015-04-15T21:23:55+08:00
---


> 本系列文章将总结和分享我顺利通过Facebook面试并获得Offer的经历和经验

> 申明：本文为[本人](http://cenalulu.github.io/about/)亲身经历，原创作品。如需转载，请在转载文章的最开头部分包含原文地址：<http://cenalulu.github.io/mysql/how-i-become-a-facebook-dba/>


## 写在前面

> 2014年10月，我有幸通过了Facebook的电面，参加了在Palo Alto的on-site面试，并最终成功拿到了offer。期间有很多经历的东西想要记录下来，以做备忘。同时在当时准备的时候，发现国内对于Facebook面试经历的资料和分享时少之又少。因此，也想以记录的方式和大家分享经验，让更多的华人成为Facebook的一员！整个记录会分为三个大部分：面试流程，面试题集锦，入职流程和生活准备。前两部分为了避免误人子弟，我尽可能的客观描述，如非特别需要减少主观的理解在其中。

> 由于我申请的职位是MySQL Database Administrator，相对比较冷门。为了使得读者受众面更广，我尽可能的挑选面试中对于程序员和其他IT岗位能普遍试用的经验来作重点描述。如果你受不了博主的流水账叙述形式，可以直接跳到最后一节，获取简要通关秘籍。:)


## 基础要求

我们来看看要成为一个Facebook的潜在员工候选人，需要有哪些硬条件。要求的远比你想到的要简单很多：

- *学历* 由于拿到offer后，办理工作签证时出示本科成绩单。所以本科学历是最低要求的。
- *英语* 英语没有硬性要求，不需要雅思托福成绩。个人觉得能无障碍的听懂youtube上的技术分享，会一些基本日常语法加上相关专业词汇，就能比较顺利的完成电面和人肉面。
- *专业经验* 没有硬性的相关领域证书要求，当然如果你没有内推渠道，有个把证可以增加通过简历过滤器脱引而出的机会。
- *技术经验* 是否有能力维护设计Facebook服务器量级的系统是一个重要考察点。当然不要求你一定要经历过这么大的量级经验（毕竟这样的公司不多）。
- *家庭* “一人Offer，全家受益”是我对Facebook Relocation的总结。拿到Offer后的所有环节，Facebook都会把你的家庭（配偶和子女）作为一个整体考虑进去。所以只要家人支持，家庭不会成为入职的羁绊。
- *国外生活经历* 博主在去Facebook前，除了一次自助蜜月游，从来没有出过国。也证明这方面没有硬性要求。个人觉得生活就像学游泳，扔进水里了，扑腾几下怎么样都会了。
- *会翻墙* 呵呵。。。

看了那么多，是不是觉得自己也是个合格的FB准候选人呢？ :) 火速进入网申阶段。

## 第0阶段：网申

其实因为我[cenalulu](http://cenalulu.github.io/about/)本来就安排在2014年9月底的时候去一次旧金山。所以一开始是报着试试看想法，并带着`万一要on-site面试，我还可以省个机票钱`的心态，通过Linkedin找了几家正在招募MySQL DBA职位的硅谷公司。从中挑选了几个巨头投了简历，包括：`Google`,`EA`,`Apple`,`Linkedin`,`Twitter`,`Facebook`(后简称：FB）。悲剧的是，只有FB通过了简历筛选，并得到了邮件回复。之后从已经在这些公司工作过的朋友那边了解到，海投简历确实是一个效率比较低下的方式。很有可能因为简历关键字匹配不成功就直接失去了后续面试机会。所以，如此悲催的首轮通过率也不足为奇了。他们强烈建议如果想从硅谷公司的简历筛选中脱颖而出，还是尽可能找公司员工做内推。{: style="color: red"} 
不过，相较于国内公司，硅谷巨头做的比较好的一点就是无论你简历通过与否，都会在两天内给到邮件结果。所以，网投时留得邮箱建议是能够每天查收一次的。下面是我众多悲剧（被拒）信中的一封：

> Thank you for your interest in a role at Twitter. We have reviewed your experience in regards to this open position, and unfortunately do not see a strong match for you at this time. We will also keep your resume on file should a future match become available. We realize it is a time commitment to engage any company in the application process and we sincerely appreciate your efforts. 

关于职位的具体信息，各个巨头都有自己的招聘主页。也可以通过Linkedin搜索。FB家的职位具体信息可以通过：<https://www.facebook.com/careers?_rdr>查找。什么？博主！这个链接打不开啊！好吧，翻墙对于大陆应聘者是一道“面试题”。
此外，走整个申请面试流程前，确保自己已经准备好了。因为，FB的效率非常高，从网申到第一次电面最短会只有两三天的时间。一旦闯关失败，距离下一次申请需要有至少半年的冷却时间。


## 第1阶段：电面

在和HR互通几封邮件后我们商定了电话面试时间。由于时差问题，面试定在了北京时间凌晨1点。Facebook的工作时间是当地时间早上9点到晚上6点，对应的北京时间是凌晨1点到第二天早上10点，如果是美国夏令时的话，那么时差从16个小时减少到15个小时。所以对于大陆应聘者来说面试时间有两个选择：一个是熬夜到凌晨，一个是早起面试。博主由于当时还是在前公司任职，早上10点在公司面试并不是一个很稳妥的选择。因此几次电面时间都是定的凌晨在家面试。
如果进行顺利的话总共会有3-4次电面（我进行了3次，具体数量按照岗位要求和面试质量决定）。电面采用直接淘汰制。电面结果直接决定了你能够进入下一轮（不是多次面试成绩取平均）。所以，对于每一轮电面都要格外的重视。每次电面时间都控制在45钟内，技术电面无论题目是否完成，都会用足45分钟。电面方式可选电话（由面试官座机打过来）或者skype。博主建议使用手机，Skype通话质量不太稳定。我的电面过程中，两种都用过。相比之下电话的体验更好些，因为可以把电话内容录下来之后做回顾。每次电面前，我都会提前半小时呆在一个安静的房间，做一些简单的面经操练进行热身。然后确保电话畅通，耳机音量OK，Skype在线。一般来说面试官的来电时间非常准时，我的三次电面来电时间都和约定时间误差不超过5分钟！这也是FB严谨的招聘风格的一部分。电面全程使用英语。每次电面的一开始，面试官会有简短的自我介绍，并对本次电话面试的时间和内容安排做一个约有5分钟的详细介绍。这部分是你适应面试官口音的一个绝佳环节。我的运气较好所有电面都是英语的native speaker。如果你对于印度口音承受力较差的话建议先在youtube上搜一些印度哥们的技术分享视频研究下。
以上就是每次电面共性的内容，下面按照电面轮次，逐一详细介绍：

> 注：本文只介绍流程，所有技术面的题目会在后续文章中分享

#### 1.1 第一次电面

第一次电面全程是Recruiter（即国内常说的HR）。整个招聘流程中从电面到入职，除了技术考官外，他是你唯一的联系接口人。所以给他留下一个好印象当然是成功的第一步。简单的流程介绍后，就要求我进行一个自我介绍。然后会根据几个和应聘职位相关的工作经历提几个具体的非技术问题。之后会进行客观基础题的问答。所谓客观基础题就是有唯一标准答案的问答题。例如：Linux上HTTP上的端口是多少? MySQL和Linux基础题各20题。答题期间，recruiter不会告诉你正确与否。因此，在答题结束前是可以修正之前的答案的。我就这么修正过一次。所有40题答完之后，面试官会告知答错了几题。我当时是错了一题，面试官暗示成绩应该足以让我进入下一轮面试（具体的及格线我不清楚）。答完题以后就是，Q&A环节。问了两个事先准备的套路问题，一个关于职位本身，一个关于公司文化。最后，互相感谢，等待面试官先挂断电话。

#### 1.2 第二次电面

第二次电面是coding技术面，由将来的team内部的员工全程主持。coding技术面的形式是，45分钟内，面试官会给出4道技术题，让面试者在 [Stypi](https://code.stypi.com/)上进行答题。Stypi是一个在线协同代码编辑网站，即你的实时代码编写和修改都会在面试官那边展现出来（可以理解是网页版的远程桌面）。每道题都会通过Stypi贴在编辑区域内，然后答题者在编辑区域内当场进行coding。每次出完题后，如果觉得题目表述不清楚或者觉得模棱两可的地方可以及时询问面试官。每一题答完后，面试官如果决定有明显的bug或者效率比较低的地方会提出，让答题者进行修改，或者口述改进方案（具体根据时间进度而定）。
下面是一个Stypi界面的截图：
![stypi](/images/mysql/fb/stypi.png)

#### 1.3 第三次电面

由于应聘的是MySQL Database Administrator，电面也必然免不了进行MySQL技术面试。第三面就是另一个来自将来同事的面试。该轮面试是问答形式，因此也就没有用到电脑。题目由浅入深，考察的都是MySQL的一些基础知识。同时也会根据简历上的自我介绍和项目经验进行深入的提问。

#### 1.4 第四次电面

本来在第一次电面中Recruiter提到会有一共会有四轮电面，且第四轮电面是故障排查演练。也许是进度原因（因为离我出发去旧金山只有一周了），又也许是之前的考察已经达到了目的。Recruiter邮件告知我，接下来就直接去Palo Alto总部面试了。Bravo！


---


![facebook_site](/images/mysql/fb/facebook_site.jpg)

## 第2阶段 On-site面试

#### 2.0 面试前夕

确认有on-site面试资格后，面试官会确认具体面试时间。同时，让候选人办理入境签证。由于我因为之前的出国计划，已经有了B1/B2的visa所以就略过了这一步。一般来说美国签证的周期在两周以上，包括材料准备，提交，大使馆面签，护照快递等。按照之后的经验，所有这些流程都会有FB指定的代理商BAL跟踪协助。所以，整个流程会非常的省心，非常的人性化！
由于我的个人安排，机票和住宿是自己搞定的。实际上根据FB的政策，所有面试的来回机票费用和住宿费用都是全包的。按照之后的经验，机票会由FB的指定代理CWT代为下单，商务舱标准。酒店是五星级，时间一般最长三天，即：面试前夜，面试当天和面试后的调整日。这两部分的钱都是FB支付。此外，FB允许报销面试期间发生的生活费用，每天150美元。包括：来回酒店机场的出租票，伙食费和基本生活用品。这部分的费用在面试结束后一个月内，通过系统上传发票（Receipt），最后通过银行转账的方式打给面试者。所以最好能提前拥有一张支持国际汇款(有SWIFT CODE)的银行的银行卡。


#### 2.1 面试当天

面试约定在Hacker Way Site早上9：45进行。搭乘宾馆提供的直达车，早早的到了FB总部。在前台进行访客登记，等了约10分钟我的接口Recruiter就来接我了。由于来的较早，他先带我大致参观了下园区，当然免不了show一下 [FB引以为傲的十几个餐厅](http://news.ittime.com.cn/news/news_3820.shtml?utm_source=tuicool)。随后，在某个休息室匆匆的抓了杯咖啡就到了面试室。所谓的面试室就是预先book了一天的会议室，候选人整个一天的面试都会在这里进行。
on-site面试总共是5轮，每轮严格控制在45分钟（答不完就结束，有空余则继续聊），每轮一位面试官。按照我当时的情况和之前的面经来看5轮的分工都比较明确，分别是：coding、实战经验、未来的manager、未来的teamate、未来的兄弟team组员。由于今天我们主要讲流程，在这里我就大致过一下每个人的面试题倾向。具体的面试题内容会在后续博文中分享。

- coding部分：和之前的电面题类型大致一致，只是形式变成了FB著名的white-board coding，即在一块大白板上写代码。也就是说：没有高亮！没有自动补全！重度依赖IDE的童鞋在没有准备的情况可能会有些吃紧。
- 实战经验部分：由于我是面试MYSQL DBA方向，因此内容和MySQL内部原理密切相关。按照Recruiter的说法是：问到你不会为止（找到知识的边界）。一般来说这一面都会是技术专家出面进行。形式为问答+白板的伪代码。
- 未来manager部分：0.5人文+0.5技术。主要考察团队合作能力，以及过去的一些项目中遇到的困难和如何解决的。如果简历上没有撒谎，并且实战经验丰富的话，这一关会是非常轻松的。
- 未来的teamate：全技术，这部分的深度会没有技术专家面的那么深。个人猜测这一关除了做技术能力的double check外，也是为了确保候选人能够很好的与将来的同事交流。
- 未来的兄弟team成员：这部分主要考察周围知识面的触及程度。例如：作为MySQL DBA了解Linux相关知识就是必要的；对于programmer来说，了解一些产品设计原理，或者前端知识也是必要的，等等。此外，也考察部分跨团队交流的能力。

由于是从上午开始的面试，在前两面结束后就是一个一小时的午休时间。当然，这段时间就是好好享受FB奢华的饭菜调整状态的时候啦。Recruiter当时和我说，每天最烦恼的时候就是午饭时刻，因为“去哪个食堂吃，吃什么”是最困难的问题。为此，他们内部还有一个APP，用于展示每个食堂当天提供伙食菜单，ORZ。。。
全天面试完成后，没有特殊安排的话，Recruiter会询问你是否想继续逛下。否则就陪同离开园区，完成一天的面试执行。

#### 2.2 面试后的结果

大约在面试当周的周五都会有个候选人PK会，每位面试官会表明自己的看法。在这个会上就会有一个候选人是否通过的结论。我当时在面试后5天左右就收到了录用结果。之后Recruiter就会起草offer，谈工资（具体工资我就不说啦，如果想知道一个大概的业界标准可以上[Glassdoor](http://www.glassdoor.com/Salaries/index.htm)），邮件确认，走流程。Offer搞定后，就开始启动relocation项目了。所有的relocation相关你能够想到的问题，FB都有指定的代理回来帮助你，实在是非常的周到！例如：签证，搬家海运，临时落脚点，机票等。关于华人relocation和国外生活的部分，我也会在日后的博文中陆续更新。


## Tips

如果你将要或准备参加FB电面/面试的话，下面是一些我个人感觉比较需要注意的点

- 没有做过的或者不清楚的知识千万不要写在简历中，任何信息都有可能在电面中被考察到
- 申请时留的邮箱，保持畅通可用，建议每天查收新邮件。
- 电面环境建议安静，温度合适，电话信号良好。
- 电面准备一条有麦克的耳机（普通手机的通话耳机就行）。
- 注意保证手机电量充足
- *王淮的《打造Facebook》一定要看，我的大部分面试流程的疑问都在书里得到了解答*（PS：我真的不是出版社的托！觉得我是托的可以看PDF。PPS：出版社别打我）
- coding电面之前，建议先通过stypi练习一些简单的算法题
- 关于白板题目去哪里找：[Leetcode](https://leetcode.com/problemset/database/) [TopCoder](https://www.topcoder.com/), [Codeforces](http://codeforces.com/), [Project Euler](https://projecteuler.net) 都是不错的选择
- 关于薪资范围, 可以参考[Glassdoor](http://www.glassdoor.com/Salaries/index.htm)上给出的标准基本上很准
- 关于家庭
    - 收入：以Facebook的待遇，一个人养活一家三口基本不是问题，会有少许结余。
    - 签证：Facebook的指定代理会帮一家三口搞定一切（但是不包括申请人的家长）



## Q&A

这部分我将会持续更新大家感兴趣的问题。如果你对于来FB面试，工作有什么样的疑问，都可以来我的博客原文下留言
 
>  <http://cenalulu.github.io/mysql/2015-03-02-how-i-become-a-facebook-dba/> 

或者给我发Email: cenalulu@gmail.com 所有共性的问题我都会在文章下面作答或者邮件回复。
当然，如果你在看了本文以后有了来FB工作的念头的话，也可以把英语简历和想要应聘的职位及应聘所在地发到我的Email，我会筛选后在平时空闲的时间帮忙走内推流程。
具体职位见：<https://www.facebook.com/careers?_rdr>



