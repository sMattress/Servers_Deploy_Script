- **webhook.rb**
  Webhook服务器，用于接收`Docker阿里云镜像`的构建事件，然后调用自动部署脚步更新服务器。
  `Docker阿里云镜像`hook到`GitHub`，所以只要在对于`GitHub`的release分支提交**编译以后**的代码，就可以实现自动部署。
- **auto-deploy-netty.sh**
  Netty服务器更新脚本，使用时需要将其拷贝至对于目录。
- **auto-deploy-tomcat.sh**
  Tomcat服务器更新脚本，使用时需要将其拷贝至对于目录。