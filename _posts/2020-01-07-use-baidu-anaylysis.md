---
layout: post
title:  "集成百度统计"
date:   2020-01-07 23:56:52
categories: blog
---

由于防火墙问题，google-analytics 在国内无法正常使用，因此选择了“百度统计”。  
现在，我能知道你来过，但仍然不知道你是谁 :)

Jekyll 集成“百度统计”方式：
1. 注册“[百度统计](https://tongji.baidu.com/){:target="_blank"}”帐号；
2. 新增网站（网站列表功能模块）；
3. 获取代码（统计代码）；
4. 将统计代码添加到 Jekyll 的 _includes/footer.html 最后，完成。

附：  
如果你是用命令 Jekyll new 建立的博客， minima 将会是默认主题，由于 minima 是基于 gem，所以在你的博客系统文件路径下不会出现 _includes 以及 _layouts 等目录。  
这时，你可以执行命令 bundle info --path minima ，得到 minima 主题的安装路径，将 _includes/footer.html 拷贝到你的博客系统根路径下的 _includes/footer.html 位置，并将“百度统计”的统计代码添加到文件最后，Jekyll 会优先使用博客系统里的 footer.html 文件。