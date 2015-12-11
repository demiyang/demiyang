title: Evernote iOS版 登录页设计
tags: []
date: 2014-10-25 12:18:00
---

Evernote iOS版一度把登录和注册页设计成这样：

一般这一页会有两个选项——1注册 2登录（当然Evernote 这个版本多了一个转到international版的选项，虽说肯定是有不得已的原因，但区分两个不能共用账号的版本把记忆和区分任务交给用户真不太好。）

Evernote替用户省掉了选择，直接输入邮箱或者用户名。这是一个挺不错的设计，因为用户再也不用做选择，不管是否注册过，都可以直接输入自己的邮箱或者用户名。然后点next，下一步。
<figure data-orig-width="500" data-orig-height="750">![image](http://41.media.tumblr.com/71f9a9d4c603e52588fa295c1c907394/tumblr_inline_nloaurbmAS1rze6u9_500.png)</figure>

这个时候会有两个情况：

1 输入的 Email 或 Username 如果已经存在，那么进入输入密码的页面。这个页面的过度是很平缓的，本来提示语、输入框和 Sign In 和上图一样在下半部，输入框激活后，键盘推出，整体一起移动到上方。Forgot Password? 在键盘的正上方，这样就不会出现点不到或看不到“忘记密码”提示的情况。提示语会告诉你，现在正以某某账户的身份登录印象笔记。
<figure data-orig-width="500" data-orig-height="750">![image](http://40.media.tumblr.com/40563b10d07ca44a791ced80e20ce7ba/tumblr_inline_nloav1o9qa1rze6u9_500.jpg)</figure>

2 上一步输入账户信息后如果是未注册的账号，会变成注册页。

输入密码之后完成注册。开始使用。

这样设计的好处是用户不需要做“已有账号”还是“初次使用”的选择，输入邮箱加密码就可以使用。但是这个设计跟以往的登录设计比，要多访问一次服务器。输入邮箱－访问服务器看是不是存在账号－输入密码－看密码是不是正确。如果用户的网速不够快的话，比如在信号不太好的郊区，这个体验并不是太好。我后来就遇到了这样的问题，只好选择更稳妥的设计。

后来Evernote改变了设计。

变成下图这样同时输入用户名／邮箱和密码登录，如果要注册新用户点下方的创建账户。
<figure data-orig-width="422" data-orig-height="750">![image](http://41.media.tumblr.com/ee970d9e2eb3424b555005b667086999/tumblr_inline_nloavp7ZIP1rze6u9_500.png)</figure>

很好奇为什么Evernote把登录改回来了。是因为前一种页面上“next”等文字按钮看齐来太不像按钮，给部分用户造成了困惑吗？但是由于有键盘上“Go”的配合，这应该不是问题。还是说他们觉得两次服务器请求没必要？嗯，也许是因为对于Evernote这样一个已经有着广泛用户基础的工具型应用，登录是大多数用户安装app之后的选择，所以设计成默认打开就可以登录了。如果是一个新推出的社交app，是需要更突出“注册”的。