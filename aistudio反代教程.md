访问[Build | Google AI Studio](https://aistudio.google.com/app/apps/bundled/blank?showPreview=true&showCode=true)

下载dark-server.js和dark-browser.js，楼层里有。

在左侧代码栏内粘贴dark-browser.js内容     

在本地任意文件夹内，存放dark-server.js，点击地址栏输入cmd打开命令提示符。

```
npm init -y

npm install express   

npm install ws

node dark-server.js
```

报错

```
[ERROR] 2025-06-07T02:35:22.418Z [ProxyServer] - 启动失败: Missing parameter name at 1: https://git.new/pathToRegexpError
服务器启动失败: Missing parameter name at 1: https://git.new/pathToRegexpError
```

 原因：dark-server.js下错了。

安装插件，我开了梯子。

```
https://github.com/LenAnderson/SillyTavern-CustomModels
```

```
聊天补全来源选择为GoogleAIStudio
将kingfall-ab-test复制进去保存，模型旁边那个笔的图形，这个在装了上面的插件就有了
```

```
反向代理地址写http://127.0.0.1:8889/ ，模型名称写kingfall-ab-test 。
```

![image-20250607111128528](C:\Users\杨 佳雪\AppData\Roaming\Typora\typora-user-images\image-20250607111128528.png)

![image-20250607112615621](C:\Users\杨 佳雪\AppData\Roaming\Typora\typora-user-images\image-20250607112615621.png)

但是报错了那个网站

```
[11:11:53.044] [RequestProcessor] 请求执行失败: HTTP 500: UNKNOWN
[11:11:53.045] [ProxySystem] 错误响应已发送
```

原因：不知道，楼里重新找dark-browser.js覆盖就好了。

