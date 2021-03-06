---
category: Tools
layout: post
title: Github深入应用——贡献代码
---

用了一个多星期的github，只是会git clone别人的项目，然后本地修修改改，最后git push到自己的github上。如果你git clone别人的项目，本地修改后，在不知道别人github帐号密码的提前下，想git push到别人的github上，需要怎么办？可以通过一下方式解决你的难题：

##1 添加合作者

github可以给项目添加合作者，假如你想参与我的项目，你跟我说一声，我就把你添加到我的项目里作为合作者，这个选项在项目的Settings里面有Collaborators，github需要你输入自己帐号密码确认你真的准备添加合作者，然后通过输入合作者github帐号，点击add就成功了。只要我添加你为合作者后，你就可以git clone我的代码，然后修修改改，直接push到我的github上来。--添加项目合作者要谨慎！

##2 通过github上fork

先通过github上的fork，fork下别人的项目，于是你的github上就出现了同名的项目，这个项目就属于你自己。你把这个自己的项目git clone到本地，修修改改，然后push到你自己的项目里。这里又引发一个问题，那么你如何把你对自己项目的改动，发给之前fork的那个原项目呢？在github上你的项目页面有个叫Pull Requests的按钮，点击就会把你改动代码发到对方的项目里，对方还会收到邮件，由原项目主人决定是否接受你的修改。如果是在你fork别人的项目后，原项目代码发生了改动，你要想同步到本地，就直接git fetch origin 从原项目地址同步最新的项目代码，然后再merge就好了。

以上内容也都是我的理论，还未进行实践。如果大家在实践过程中，遇到问题欢迎随时跟我讨论。