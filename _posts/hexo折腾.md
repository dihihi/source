title: hexo折腾
date: 2015-10-09 21:09:58
tags:
---
瞎折腾,在github上用hexo管理博客,简单记录一下。
<!--more-->
需要安装nodejs git以及

	npm install -g hexo
在目录里

    hexo init
	npm install
	hexo generate
	hexo server

创建github工厂"username.github.io"

编辑_config.yml
    # Site
    title: MarkDown使用
    subtitle: 学习
    description: 学习 笔记 管理
    author: Dihihi
    language: zh_CN
    timezone: Asia/Shanghai

    # Extensions
    theme: jacman
    stylus: 
        compress: true

    # Deployment
    deploy:
    type: git
    repository: git@github.com:dihihi/dihihi.github.io.git
    branch: master


没有部署器的话，安装
	npm install hexo-deployer-git --save

    hexo generate == hexo g
    hexo deploy == hexo d

    hexo server == hexo s
    hexo new == hexo n
    hexo d -g #生成部署

更换主题时，修改_config.yml,以及

    rm -rf public
    hexo clean
    
# 其他电脑上使用
主题的话可以fork一个然后自定义修改

	git remote add mine xxx
	git push -u mine master
    git clone git@github.com:dihihi/jacman.git themes/jacman
备份_config.xml
source目录可以创建一个仓库保存在github上
    
# 引用链接
* [如何使用 Jacman 主题](http://wuchong.me/jacman/2014/11/20/how-to-use-jacman/#more "打开")
* [Markdown 语法说明 (简体中文版)](http://wowubuntu.com/markdown/ "打开")
* [在github上用hexo搭建博客](http://pleasureswx123.github.io/2014/08/29/%E5%9C%A8github%E4%B8%8A%E7%94%A8hexo%E6%90%AD%E5%BB%BA%E5%8D%9A%E5%AE%A2/)
* [hexo Documentation](https://hexo.io/docs/index.html)
* [hexo你的博客](http://ibruce.info/2013/11/22/hexo-your-blog/)