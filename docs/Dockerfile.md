### 	Dockerfile构建wordpress

在本地主机新建一个目录（本文为mydocker）存放Dockerfile文件，新建Dockerfile文件：

`mkdir /mydocker`

`cd /mydocker`

> `vim Dockerfile`

向Dockerfile文件中添加如下内容：



![](/docs/img/x3/图片99.jpg)



> vim setup.sql
>

在文件中添加如下内容：

![](/docs/img/x3/图片98.jpg)



> vim setup.sh
>

在文件中添加如下内容：

![](/docs/img/x3/图片97.jpg)



在mydocker下键入：docker build -t centos10 .



![](/docs/img/x3/图片95.jpg)

完成后键入：docker run -it --privileged=true -p 4005:80 -d centos:dockerfile /usr/sbin/init



![](/docs/img/x3/图片94.jpg)







[](/docs/img/x3/图片93.jpg)



在主机浏览器键入：106.54.3.52:4005



[](/docs/img/x3/图片96.jpg)