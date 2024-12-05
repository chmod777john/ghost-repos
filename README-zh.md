# ghost-repos

我本来是在做 GitHub 的仓库分析，想找到那些最近两天 star 增速最快的仓库，没曾想发现了大量“幽灵仓库”

以下这些仓库是由不同账号创建的。但是创建时间、获得的 star 总数都非常相近。内容也基本一致。

都是伪装成某些工具包，诱导用户去下载某个 exe ，实际一行代码都没有。

![image](https://github.com/user-attachments/assets/2ea400d8-e6d8-42ad-b5bb-0cc3bb4acde6)

![image](https://github.com/user-attachments/assets/8cba0af3-2fdb-4cf9-8e77-ee3c39eada3e)

这样的仓库，创建十几小时内就有接近 200 star，明显不正常。

按照之前的经验，它们存活一段时间之后就会被删掉。

为此，我已经把这些页面存档到了 GhostArvhice 上，这样即使攻击者删库跑路，还是能看到这些仓库的原貌。

![image](https://github.com/user-attachments/assets/a14cdfaa-8de8-4c15-a683-6e04e869402d)

复现代码也是开源的，大家可以自行验证

https://github.com/chmod777john/github-hunter/blob/main/index.ipynb

## 题外话：

其实项目本意是用来寻找那些创建时间短，但是短时间内 star 增长很多的项目。这些项目可以认为是典型的早期优秀项目，日后必然大火的。

挖到这些项目之后，我会写到一段文字里，传到区块链上，作为“预言”。日后我预言到的项目大火了，大家都能知道“这小伙儿眼光不错”

没想到还能挖出这些幽灵仓库来。果然是黑暗森林，第一次真切感受到有人在 Github 上从事这些社会工程学活动。

不过现在情况还算好的，这些仓库基本都是同一个风格，说明干这事儿的基本上就只有一个组织。

## 合理推测
要达成以上的攻击行为，攻击者首先要有多个 GitHub 账号来创建仓库。其次，还要有更多的假账号来给仓库点赞。

GitHub 的账号管理还是相对严格的，新注册的账号立马去别人仓库点赞，是会被封掉的。所以可以认为点赞账号基本都是一次性的僵尸号。

注册一个 GitHub 账号至少需要一个邮箱，而且注册过程中有相当严格的人机验证码，就是类似 OpenAI 那种，给一幅图片和一个手指，要求把手指转到图片中的指向。

这样的条件下，注册账号应该是避免不了手动的了。如前面所说，账号基本都是一次性的，意味着每天都要新注册大量账号。这个手工成本是很高的，至少都应该是一个团队。

这种机械性的工作基本都不会让程序员自己去完成，所以注册账号的，应该只是团队里的小兵。

团队里的首脑位置应该主要是负责病毒的编写，以及用 Github API 取批量控制账号。

不过这样看来范围还是太大了，很多组织都可以做到这一点。那会是谁呢？ 最大概率是情报机构和诈骗集团。

克格勃？ CIA？ 东南亚的汇旺集团？ 哥伦比亚的毒贩？ 不会是我们的人干的吧

## 蛛丝马迹

以下所有页面都在 GhostArchive 有备份。

我决定查找真凶。首先去查看谁 star 了这个仓库。

访问 https://github.com/ezzy-aja/Valorant-H4ck/stargazers?page=1    (backup  https://ghostarchive.org/archive/aqOPS )

和

https://github.com/Thang2k7/Xbox-Game-Pass-Activator-Free-2024/stargazers   (backup   https://ghostarchive.org/archive/28kJL)

可以看到有很多重复的。其中大部分账号没有任何痕迹，没有 commit 历史。但经过寻找，我终于找到一个像真人的账号

https://github.com/G4tito?tab=stars    (backup   https://ghostarchive.org/archive/UESF2)

可以看到他 star 了很多这种欺诈仓库。

https://github.com/G4tito/Simple-WaBot    (backup   https://ghostarchive.org/archive/ozlFg)

而且他自己也有一个真实的仓库。说明这并非僵尸账号，而是欺诈者（或者其同伙）的主账号。

但是仅此还不能够在现实世界中找出他来。他还有一个 follower ，这个关注者是个大牛，现实世界中也有 youtube 账号。

https://github.com/G4tito?tab=followers   (backup     https://ghostarchive.org/archive/J4ckv )

https://github.com/elrebelde21      (backup    https://ghostarchive.org/archive/tiCSv )


