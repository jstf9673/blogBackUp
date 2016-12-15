##learn how to build a hexo blog
================

准备环境工具
nodejs,git bash,github

—————————————————————

###**install hexo**

``` bash
$ mkdir blog     
$ cd blog     

$ npm install hexo -g --save      
$ hexo init      
```
###**start hexo**

``` bash
$ hexo server     //hexo s
```

###**常用命令**

``` bash
$ hexo init       //初始化
$ hexo clean / hexo c       //清除本地public文件
$ hexo generate / hexo g      //生成静态文件
$ hexo server / hexo s      //启动服务
$ hexo deploy / hexo d      //部署到github(执行后会要求输入git账号信息)
$ hexo new 'postName'      //新建文章
$ hexo new page 'pageName'      //新建页面
$ hexo public       //发布文章
```  

####**更换主题**

##### 安装主题

``` bash
$ git clone https://github.com/litten/hexo-theme-yilia.git
```
``` bash
cd themes/yilia
git pull
```
然后在根目录编辑_config.yml

``` bash
$ vim blog/_config.yml
theme: yilia
```

#### 配置

主题配置文件在主目录下的`_config.yml`，请根据自己需要修改使用。
完整配置例子，可以参考[我的博客备份](https://github.com/jstf9673/BlogBackup)

```
# Header

menu:
  主页: /
  随笔: /tags/随笔/

# SubNav
subnav:
  github: "#"
  weibo: "#"
  rss: "#"
  zhihu: "#"
  #qq: "#"
  #weixin: "#"
  #jianshu: "#"
  #douban: "#"
  #mail: "#"
  #facebook: "#"
  #google: "#"
  #twitter: "#"
  #linkedin: "#"

rss: /atom.xml

# 是否需要修改 root 路径
# 如果您的网站存放在子目录中，例如 http://yoursite.com/blog，
# 请将您的 url 设为 http://yoursite.com/blog 并把 root 设为 /blog/。
root:

# Content

# 文章太长，截断按钮文字，然后在文章合适的位置加<!--more-->
excerpt_link: more
# 文章卡片右下角常驻链接，不需要请设置为false
show_all_link: '展开全文'
# 数学公式
mathjax: false
# 是否在新窗口打开链接
open_in_new: false

# 打赏
# 请在需要打赏的文章的md文件头部，设置属性reward: true

# 打赏基础设定：0-关闭打赏； 1-文章对应的md文件里有reward:true属性，才有打赏； 2-所有文章均有打赏
reward_type: 2
# 打赏wording
reward_wording: '谢谢你请我吃糖果'
# 支付宝二维码图片地址，跟你设置头像的方式一样。比如：/assets/img/alipay.jpg
alipay:
# 微信二维码图片地址
weixin:

# Miscellaneous
baidu_analytics: ''
google_analytics: ''
favicon: /favicon.png

#你的头像url
avatar:

#是否开启分享
share_jia: true

#是否开启多说评论，填写你在多说申请的项目名称 duoshuo: duoshuo-key
#若使用disqus，请在博客config文件中填写disqus_shortname，并关闭多说评论
duoshuo: false

# 智能菜单
# 如不需要，将该对应项置为false
# 比如
#smart_menu:
#  friends: false
smart_menu:
  innerArchive: '所有文章'
  friends: '友链'
  aboutme: '关于我'

friends:
  友情链接1: http://localhost:4000/
  友情链接2: http://localhost:4000/
  友情链接3: http://localhost:4000/
  友情链接4: http://localhost:4000/
  友情链接5: http://localhost:4000/
  友情链接6: http://localhost:4000/

```
