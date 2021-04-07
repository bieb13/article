# Freenom域名自动续期
>注册了很多Freenom的免费域名，但是担心自己的域名没有及时续期而丢失？  
>有个大佬在GitHub上分享了一个项目，可以帮助你实现freenom域名的自动续期。  
>这样理论上可以实现域名无限期免费使用。  

## 项目地址：
[luolongfei/freenom](https://github.com/luolongfei/freenom)

如果你和我一样，没有vps，且不会这样那样的部署，可以直接跳到🤣 项目最简单的使用方法  
详细说明请看作者原文。  
## - 准备：
    1.一个Github账号  
    2.一个telegram账号  


- **开始**

    1. 点击[该仓库地址](https://github.com/luolongfei/freenom) ，fork该仓库
    2. 在你 Fork 的本仓库下的 Settings -> Secrets 页面追加以下几个secret秘密环境变量

        ![1.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fd534e0d2-bed1-407c-b587-4688240c53d7%2FUntitled.png?table=block&id=0601aa74-9eb1-49ae-93e0-bd4400c7a1b8&cache=v2)

        ![2.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F9a49625a-30d7-4b6e-8f6a-71d7cf68bb82%2FUntitled.png?table=block&id=58d6507b-199a-4d65-861a-7bec52532576&cache=v2)

    3. 需要添加的变量如下：

        [变量设置](https://www.notion.so/b17c0acc54e54a90afa8ac5da5dbd052)

        - FREENOM_USERNAME
        - FREENOM_PASSWORD
        - MULTIPLE_ACCOUNTS（多账户支持,若没有多个freenom账户，可不用添加）
        - MAIL_ENABLE
        - TELEGRAM_CHAT_ID
        - TELEGRAM_BOT_TOKEN
        - TELEGRAM_BOT_ENABLE
        - NOTICE_FREQ
        - 详细介绍看下图

            ![3.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F2349f823-291b-40ff-be2f-abac9d1cab33%2FUntitled.png?table=block&id=b8484431-93ce-4f38-bbc2-9658c032025c&cache=v2)

        ![4.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F6bcdd80f-51fa-466f-962d-c9f97da82e6e%2FUntitled.png?table=block&id=5443c1fc-dd23-4b26-904e-bbb1f7dc268e&cache=v2)

    4. 上述变量添加好了以后，点击仓库上方的Action，同意启用 Actions

        ![05](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F1aad18e6-7316-404f-81c2-17a1edb9c5a2%2FUntitled.png?table=block&id=9d7fc372-e743-4022-85cd-24bacd52d8a6&cache=v2)

        ![06.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F17d7b4e3-833f-4844-8f51-997e2e5b88b4%2FUntitled.png?table=block&id=43742bdc-822e-4d3b-8c55-f3cd28add109&cache=v2)

    5. 解除禁用

        ![07.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F272b87ca-6c50-415d-831e-e9561f51d792%2FUntitled.png?table=block&id=5329f923-98dc-440a-8472-f2817942bf1f&cache=v2)

    6. 任意发起一次 commit，可以参考下面点击这个yml文件进行修改

        – 打开 点击编辑按钮

        ![08.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F381dadfb-08a8-4fc1-a6fb-912f3d87ff8b%2FUntitled.png?table=block&id=78dccc77-77ab-4261-ba61-4fb221acb8e8&cache=v2)

        ![09.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F86454548-36e4-46fd-a97c-09537292dfbc%2FUntitled.png?table=block&id=236a0806-12f7-43eb-803d-684fce2e1fb1&cache=v2)

        – 修改任意内容，比如在在最后加个空格。将页面滑动到最下面，点击Commit changes

        ![10.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F3eb5a699-ac3c-4565-bf24-23044ef9bd43%2FUntitled.png?table=block&id=ae07901b-6b8d-44c2-9b7d-afb426a88468&cache=v2)

    7. 返回Actions查看执行情况。也可以选择手动触发项目执行。成功收到电报信息就代表你成功啦！

        ![11.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fa65f5020-f456-400e-8732-57e1fe3993bd%2FUntitled.png?table=block&id=d0fe19a9-b3bf-4cdf-abac-687c0f937fd0&cache=v2)

        ![12.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Ffd297a2a-8c39-4541-a315-09b613c028da%2FUntitled.png?table=block&id=656d20a6-38e1-419b-90f5-285b199e76f5&cache=v2)

    8. 以上步骤完成后无需其他操作。现在每天上午十点左右Github Actions会自动触发执行本项目，注意查收电报推送信息。
### 上述是我的个人简化版教程，同时补充了一些些内容。一切以项目作者的文档为准。  
### 好了，愉快地完成第一次自动续期！为自己鼓掌👏
*转载文章请附带原文出处，谢谢*<https://bieb13.com/freenomrenew>
