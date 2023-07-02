1.git第一次登入需要全局配置
sudo git config --global user.name "example"
sudo git config --global user.email "xxxxx@xxxx.com"
>本地配置不需要sudo，服务器需要。

2.SSH密钥配置
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
查看密钥
cat ~/.ssh/id_rsa.pub

3.Git指令
mkdir d:/project
cd project
rm -rf project
cd ~/priject
git clone git@codeserver.youkeda.com:xxxxxx.git
提交库
git add .
git commit -am "XXX"
git pull
git push

4.在push之后，系统会进行项目'构建'build。
复制对应部分，在终端进行项目'部署'，在预览查看效果

移除部署：
先停止sudo docker stop tank
再删除sudo docker rm tank
