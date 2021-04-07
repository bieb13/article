# 拖稿的Nobelium使用体验  
之所以没敢写'教程'二字，是因为其实我也是在摸索中。自己都是半桶水，哪里敢教人。  
不过为了📝记录，里面也会有简单的部署教程，也是为了自我备忘。 
## 仓库介绍  
[仓库地址](https://github.com/craigary/nobelium/)  
该项目非常适合notion用户，当然如果你没有用过notion，同样简单!  
只要去注册一个notion账号，你同样可以10分钟完成✅网站的部署。  
且因为它是部署在vercel上的，所以非常适合国内访问！
在此感谢@craigary  
## 前期准备  
- Github账号 
- Notion账号  
- Vercel账号
- 一个域名(非必需，但是当然是自己指定域名更漂亮啦）   
### 开始
- 将 [这个 Notion 模板](https://www.notion.so/68be9021bca34b8e89f0246f27e608df) 制作副本，设置share状态让所有人都能看到它！
- [Fork](https://github.com/craigary/nobelium/fork) 这个项目
- 在GitHub仓库里的 `blog.config.js` 配置相关选项
- _(可选)_ 用自己的图片替换 `/public` 文件夹里的 `avatar.svg`、`favicon.svg` 和 `favicon.ico`
- 登录vercel在 [Vercel](https://vercel.com) ，新建一个项目
  - 选择nobelium仓库点击import,  ![](https://bieb13.github.io/post-images/1617788264181.png)
  - 选择个人账户，设定一个环境变量`NOTION_PAGE_ID`：
  ![](https://bieb13.github.io/post-images/1617788826399.png)
    - `NOTION_PAGE_ID`: 你刚刚分享的 Notion 页面网址中的页面 ID，通常是网址中工作区地址后的 32 位字符串，如图，千万别弄错哦！
  ![](https://bieb13.github.io/post-images/1617787577269.png)  
  - 点击Deploy![](https://bieb13.github.io/post-images/1617788485474.png)
- **成功部署！** vercel会出现撒花并且成功展示的页面哦！部署成功后返回，可以看到项目的ready状态![](https://bieb13.github.io/post-images/1617789312508.png)
-  vercel支持绑定域名，点击这个项目的setting里的Domain，前去绑定域名即可。![](https://bieb13.github.io/post-images/1617789266209.png)
-  后期更新文章，只需要去刚刚分享的notion页面里添加即可，属性里的published标签即是发布的意思。![](https://bieb13.github.io/post-images/1617788608330.png)
***
展示一下我利用nobelium搭建的页面效果![](https://bieb13.github.io/post-images/1617789399729.png)  
简洁，美观，且后期更新文章，只要在notion页面添加即可，其他的vercel会自动更新部署！超方便。

*转载请附带原文链接，谢谢！* https://bieb13.com/nobelium
