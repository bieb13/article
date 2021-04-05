# 利用notion免费搭建自定义域名主页
该方案来自[Frution](https://fruitionsite.com/771ef38657244c27b9389734a9cbff44/)

### 10分钟即可获取拥有自己域名的主页！

👉需求：在不会代码的前提下免费搭建一个自定义域名的主页

✔️实现  
<details><summary>准备（点击左边展开）</summary>  
1. 将自己的notion主页设置为share状态  

2. 一个自己的域名，如果你还没有，并且想免费注册一个，[请点击👉](https://www.notion.so/6317a1b6e622478185a2cb9dff7aada7/)    
</details>  
    
### 开始配置CloudFlare账户（点击左边三角展开）：  
1. 注册账户 [https://dash.cloudflare.com/sign-up](https://dash.cloudflare.com/sign-up)  
2. 输入你的自定义域名  
![01.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fd7561a5f-d8df-4303-97ba-3ff0bd913f8d%2FUntitled.png?table=block&id=4b688cb7-cf4a-4260-9f69-81dd1adbc90f&cache=v2)  
3. 选择免费计划  
![02.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fc732e996-769a-4362-be92-f8815c761dc3%2FUntitled.png?table=block&id=6b972bcd-798d-40e3-9c61-2b5fd99e9a86&cache=v2)    
4. 如果你没有导入任何A记录，请为域名添加一个A记录，地址可填8.8.8.8  
![04.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F4ce6072e-d4e7-43d8-8088-1d0330e458f0%2FUntitled.png?table=block&id=b0caaaeb-43ba-4947-bc90-e64254b3ab2c&cache=v2)  
5. 复制以下两个DNS名称服务器  
![05.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F72f6b1c5-0226-4d47-bb9c-30d817a5d421%2FUntitled.png?table=block&id=e9a28abc-3e7b-4def-baf8-44d9c766ea15&cache=v2)  
6. 去你的域名提供商的后台，在域名设置中的nameservers处添加这两个名称服务器，保存。
7. 等待一分钟，返回Cloudflare页面检查名称服务器
8. 选择灵活的加密模式（这样访问你的网站就会拥有一把小锁了！） 
![08.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F2e9b3a65-60a5-4536-8370-aef0818cb955%2FUntitled.png?table=block&id=77d25d17-5335-4606-a9b7-a262f86a1354&cache=v2)

9. 始终使用 HTTPS，自动 HTTPS 重写

    ![09.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F5a1027d6-e4bf-4a23-9fe4-e0a5cec61db1%2FUntitled.png?table=block&id=0830b8f9-a53b-4206-a6e8-5149868f6819&cache=v2)

10. 完成以上设置后，cloudflare成功接管你的dns  
    ![10.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F0062a94e-1056-43e7-a179-ed5573ffe099%2FUntitled.png?table=block&id=77c45d6e-1338-4be1-9923-a127d8ac6311&cache=v2)

11. 点击Workers，单击管理Workers，为你的workers选择一个任意的子域名（点击创建），直接用系统默认的就行。单机设置并确认。 
    ![11.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F34dec507-387a-4ab8-ba05-b6995510e740%2FUntitled.png?table=block&id=2821a58f-faa9-4d89-9c09-169950c76931&cache=v2)

12. 选择免费计划

    ![12.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Ff8bf34b7-63d4-4069-bfcd-0a5685907de7%2FUntitled.png?table=block&id=ffe094fc-01a7-4dc4-b4f1-ba066f24b87c&cache=v2)

13. 验证邮箱。返回workers页面，点击蓝色的创建Worker按钮

    ![13.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F295e133a-2cf5-4ddf-80a2-b94a04abfdb4%2FUntitled.png?table=block&id=cb891703-47c2-4fae-8676-f57d6a302431&cache=v2)

14. 好了，将左边的脚本区域清空。

    ![14.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F98f3b0a1-8f1e-456e-b523-bb8febf5e0ff%2FUntitled.png?table=block&id=5bc0f525-98cc-425a-a470-6eed1ee6438d&cache=v2)

15. 准备好代码（这里有方便你一键输出代码的小程序）

    [https://fruition.stephenou.vercel.app](https://fruition.stephenou.vercel.app)

    - 将你的域名填入上方Your Domain处
    - 将你的notion主页链接填入Notion URL中
    - 代码自动生成，点击蓝色的COPY THE CODE。代码复制成功！
16. 将代码填入第14步中的脚本框。点击保存并部署。
17. 保存后单击页面顶部的站点名称，转到Worker界面添加路由  
![17.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F61292ae4-5c83-4e32-97ee-355ed0c8f64c%2FUntitled.png?table=block&id=6564c38a-92fb-4980-a876-a4597d9abc70&cache=v2)  
18. 路由输入`yourdomain.com/*` ，worker选择你刚刚创建的那个  
![18.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fd6554895-673e-4d9f-aad4-93547dd45957%2FUntitled.png?table=block&id=b3908509-43c6-4459-a37b-2a4254f40e55&cache=v2)  

19. 点击保存。**完成了！**
20. 你现在可以访问你的域名了！


>💻  
>其实作为网站，最重要的还是内容，如果框架再美，没有实际的内容去填充，  
>也只不过是徒有其表，你自己可能都忘到天边，别人又怎么会点击进去看呢？  
>工具始终是工具，最重要的还是使用的人如何输出内容。  

>⚠️  
>值得注意的一点：  
>有时有些新手朋友们，常会出现，点击域名后跳到notion的登录界面的情况。  
>1.通常是主页share状态未开  
>2.主页的标题修改，导致主页链接已经发生变化，所以访问域名会跳转到notion登录界面而不显示你想要展示的主页。  

**转载请注明出处并附带此文链接，谢谢！**
