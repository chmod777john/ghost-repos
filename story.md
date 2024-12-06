# 危机13小时：记录一场 GitHub 投毒犯罪

## 事件概要
自北京时间 2024.12.4 晚间6点起， GitHub 上不断出现“幽灵仓库”，仓库中没有任何代码，只有诱导性的病毒文件。当天，他们成为了 GitHub 上 star 增速最快的仓库。超过 180 个虚假僵尸账户正在传播病毒，等待不幸者上钩。

而这一切被一位中国开发者--我收在眼底。经过几天的探测寻找，找到了攻击者的真身。


## 事件经过

起初，我在编写一套开源程序，用于寻找当下最早期的潜力种子项目。
源码 https://github.com/chmod777john/github-hunter

在 12.4 的搜寻过程中，我发现了一批不太一样的仓库。
![image](https://github.com/user-attachments/assets/122926b9-02ee-447e-bc6c-c0955b11e2b8)

这里面的 is None 代表仓库有大量 star 记录，后来却被删库。为何有如此大量的高赞仓库会被删除呢？

期初我没在意，而在一天后，这些仓库再次出现。

![image](https://github.com/user-attachments/assets/3c6d956b-a77e-440b-9288-0a4fb57254c7)

就好像幽灵一样，建仓->取得高赞->删库->再次创建。

## 罪证

这些仓库点进去一看，都是同一种风格： 声称自己是某个游戏的外挂或者 PhotoShop 破解版之类的，引导用户下载并且打开他的 exe 文件。

![image](https://github.com/user-attachments/assets/82e1d920-14c1-4d99-aa0a-11a909fe2296)

基本可以确定是钓鱼仓库了。所有这些仓库创建时间都非常相近，大约就是十多小时之前，而且短时间内积累到几百 star ，其背后必有高人。

## 追凶

这些攻击者是谁？ 我决定一探究竟。


### 历时4年的攻击

首先查看是谁给这些仓库点了赞，

![image](https://github.com/user-attachments/assets/3362c28e-bf9b-446d-975d-ed89ee0cbfad)

我本以为大多是最新创建的机器人账号。

出乎意料的是，这些账号的加入时间并不短。有些账号甚至是 2020 年就加入 Github 了。

4年的老号可不是说弄就弄的，如果这号是他自己的，那可真是下了血本，一个号养4年就为了这一天？ 

如果这号是他在黑市上买的，那说明4年前就有人开始批量养小号，也是一条很可观的产业链了。（创业都不一定能创4年呢）

无论这些号是攻击者自己养的还是在黑市上买的，成本都不低。

### 一片空白

我开始逐个账户打开查看，坐实了一件事：这些仓库都是一伙儿的！

![image](https://github.com/user-attachments/assets/e585b9f0-cb45-4848-8bd0-7c7d548d3fca)

这个人点赞过的所有仓库，都是刚刚说的幽灵仓库！

不过个人资料卡上完全没有任何痕迹。 没有粉丝，也没有关注的人，这让我们无从下手，简直一片空白。

### 漫漫长路

180 多个账号，我真的逐个点开来看了。其中大部分的都是纯粹的空白账户，只用来点赞。但仍然有一些是附带个人资料的。

![image](https://github.com/user-attachments/assets/bc2e601b-92b7-4370-be55-17a0ed55c0c9)

这个账号甚至附带了个人网页和 Instagram 。

不过凡事讲究双向证明。万一这个账号是冒用小哥的信息呢？ 只能将其列为怀疑对象。

### 峰回路转

攻击者账户 follow 了谁，并不重要，因为攻击者可以冒用他人信息。真正有用的线索，应该看谁 follow 了攻击者。

踏破铁鞋无觅处，我找到了一个活人账号。

![image](https://github.com/user-attachments/assets/722cc2b6-5608-472a-9837-9e9332baa3b8)

有 5 个人 follow 了这个账号！而且看他的 star 历史，可以明确他是攻击者之一。

而且该账号有真实的 Github 代码提交记录，说明它曾经是个活人！

![image](https://github.com/user-attachments/assets/babc1c60-4654-4ac7-8f78-f847c785e345)

我们来看看是谁 follow 了这个 G4tito

![image](https://github.com/user-attachments/assets/8526e5bf-7515-4796-94ee-640b65c57e34)

这位 elrebelde21 可是个大人物！ 看看他的 Github 主页

![image](https://github.com/user-attachments/assets/fa1cc85b-c8ce-43d0-a5bd-c9e4fc40228d)

他也同样参与过一个叫 SimpleBot 的项目。前面提到的明确攻击者 G4tito 也有同名的仓库。

![image](https://github.com/user-attachments/assets/a4bd6e18-e2b5-4304-9d60-39c24be7e8fe)

这位大V 在 youtube 上面还有账号呢


