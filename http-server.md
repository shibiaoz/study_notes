## http-server

它是一个简单的服务部署，与Express相比，这货更轻了，它只是一个服务搭建工具，完全可以不安装到项目的目录中。安装使用：

npm install -g http-server
成功安装后，使用：

http-server -a hostip -p port
即可拉起当前目录的web应用。

当然，如果少年你比较倔强，非得安装到本地项目中也是可以的。启动时，就要在web应用的根目录运行：

node ../node_modules/http-server/bin/http-serve
