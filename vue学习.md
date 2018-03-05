由于其他项目占用了8080端口,所以,安装live-server 后, 

执行live-server 报错 Error: listen EACCES 0.0.0.0:8080

解决办法:
1. 释放端口
2. 修改默认端口

我才用的是方法2 修改默认端口,找到live-server 的配置文件 index.js,

D:\soft\nodejs\node_global\node_modules\live-server 下的index.js: var port = options.port !== undefined ? options.port : 7999;

然后再次运行: live-server

Serving "F:\project\vuedemo" at http://127.0.0.1:7999


Ready for changes

完成
