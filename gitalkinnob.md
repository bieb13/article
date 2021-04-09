# 超简单在Nobelium添加Gitalk评论系统
## 超简单！超简单！超简单！
因为作者已经提前在博客系统里帮我们安装好了Gitalk，所以我们需要做的就是  
**补充`blog.config.js`文件里这些数据就可以了！**
![](https://bieb13.github.io//post-images/1617937851381.jpg)
![](https://bieb13.github.io//post-images/1617943064786.png)

### 上图的数据如何获得呢？  
- 创建一个公共github仓库,记住这个仓库名，我的是 `nob`
  ![](https://bieb13.github.io//post-images/1617941453567.png)
- 创建一个GitHub Application，[请点击这里](https://github.com/settings/applications/new)，生成`client id`和`client secret`
  ![](https://bieb13.github.io//post-images/1617949445676.png)
  ![](https://bieb13.github.io//post-images/1617942344470.png)
  ![](https://bieb13.github.io//post-images/1617942583213.png)
- 返回你的nobelium的仓库将`blog.config.js`补充好
  ![](https://bieb13.github.io//post-images/1617943064786.png)  
  一定记得`repo`那里不要多写，不要傻乎乎把整个仓库地址都填进去

### 配置完毕  
刷新你的主页，查看评论是否配置成功。有时会出现下图  
![](https://bieb13.github.io//post-images/1617943305806.png)  
我也不知道这是啥bug，我是登录了一下自己的GitHub后就变正常了。   
对了你的网页地址不要设置过长，不然也会出现bug.  

现在咱也是博客有评论系统的人了~撒花💐🌺  
*转载请附带原文链接，谢谢！*<https://bieb13.com/gitalkinnob>
