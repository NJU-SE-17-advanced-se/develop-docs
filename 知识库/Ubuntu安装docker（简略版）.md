# Ubuntu安装docker（简略版）

1. 看一下芯片架构：`uname -a`

   1. x86
   2. amd
   3. arm（aarch）

2. 看一下系统版本：`lsb_release -a`

3. 根据不同的芯片架构和系统版本，配置国内Ubuntu源

   1. 如果不介意网速慢，可以跳过这一步
   2. 建议选择中科大源、清华源或者163源，因为华为云可能会对阿里源限速

4. 按照docker官方文档进行安装，记得选择正确的芯片架构

   1. 参考链接：https://docs.docker.com/engine/install/ubuntu/
   2. 如果出现类似于 Unable to locate package docker-ce 的问题，可能是配置镜像时选择了错误的架构。参考链接：https://blog.csdn.net/HermitSun/article/details/108542163

5. 测试安装结果：`docker run hello-world`，应当输出：

   ```shell
   Hello from Docker!
   This message shows that your installation appears to be working correctly.
   ...
   ```