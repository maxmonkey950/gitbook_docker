# gitbook docker 镜像
为gitbook docker镜像
# 效果图
效果如下图所示
![](https://melovemingming-1253878077.cos.ap-chengdu.myqcloud.com/blog-image/2019/02/13/%E9%80%89%E5%8C%BA_075.png)
# 使用说明
## 环境准备
需要docker环境。
## 使用步骤 
### 第一种
1. 请先frok本项目
2. frok完成以后，登录主机，输入如下命令，项目拉取下来
```
git clone [您的frok项目地址];
```
3. 进行本地构建，输入如下代码
```
sudo docker build ./ -t gitbook:vo
```
4. 运行该镜像 
```
sudo docker run -p 4000:4000 gitbook:vo
```
5. 访问地址
```
http://[服务器ip]:4000/
```

### 使用自动化工具进行构建（推荐）
推荐使用自动化构建工具，在本地自动化构建
