访问[Build | Google AI Studio](https://aistudio.google.com/app/apps/bundled/blank?showPreview=true&showCode=true)

下载dark-server.js和dark-browser.js，楼层里有。

在左侧代码栏内粘贴dark-browser.js内容，复制完后一开始右侧是报错的，不用在意。 
![image](https://github.com/user-attachments/assets/9c900058-aecd-404e-977a-e3a2235ee258)

在本地任意文件夹内，存放dark-server.js，点击地址栏一行行输入cmd打开命令提示符。

```
npm init -y

npm install express   

npm install ws

node dark-server.js
```

如果报错

```
[ERROR] 2025-06-07T02:35:22.418Z [ProxyServer] - 启动失败: Missing parameter name at 1: https://git.new/pathToRegexpError
服务器启动失败: Missing parameter name at 1: https://git.new/pathToRegexpError
```

 原因：dark-server.js下错了，这个文档外部有可用的dark-server.js文件

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

![1749269760747](https://github.com/user-attachments/assets/bedb6369-30be-4f8c-8d1c-acc75a82f2d2)
![image](https://github.com/user-attachments/assets/7523673f-9c7f-432c-bd13-1dea2fd08121)

但是报错了那个网站

```
[11:11:53.044] [RequestProcessor] 请求执行失败: HTTP 500: UNKNOWN
[11:11:53.045] [ProxySystem] 错误响应已发送
```

原因：不知道，楼里重新找dark-browser.js覆盖就好了。

