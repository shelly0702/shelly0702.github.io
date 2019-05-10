---
title: 用hexo搭建自己的博客并免费发布至github空间
---

### 具备以下环境
1. git已安装
2. node已安装

### 具体步骤
1. 电脑上创建放置博客的文件夹

2. 打开git bash终端，全局安装hexo-cli依赖

```
npm install hexo-cli -g
```

3. 在放置博客的文件夹的位置执行如下命令，此命令的执行会从github上克隆下来博客模板项目并安装上相应的依赖包。

```
hexo init
``` 

4. 本地查看博客效果，执行以下命令

```
hexo serve
```

5. 在github官网上[https://github.com](https://github.com)注册自己的账号，注册的时候需要注意留自己可以登录的邮箱注册，通常很多信息会发送到这个邮箱里。注册账号给自己设定一个用户名，如：shelly0702

6. 注册完成后登录，进入主页，点击右上角new repository，输入与自己用户名一致的 Repository name，如：shelly0702.github.io。请注意这里的命名一定需要时username.github.io形式。

7. 创建完成后，克隆项目下来致本机，此时里面的内容可能是空的。在前面自己用hexo创建的项目目录中执行如下命令。

```
hexo g
```

8. 命令执行完成后，将public文件夹下的所有文件拷贝至空项目中。然后git提交计推送至github，过一会儿访问https://username.github.io 例如：[https://shelly0702.github.io](https://shelly0702.github.io/)搞定！

9. 如果觉得第7、8两个步骤比较麻烦啰嗦，你也可以继续往下看步骤。

10. 直接将hexo初始化的项目放置于 https://github.com/username/username.github.io.git的master分支下 例如 https://github.com/shelly0702/shelly0702.github.io.git的master分支

11. 接下来需要配置项目中的_config.yml文件里的deploy配置项。具体配置如下，格式须严格按照如下配置示例进行
```
deploy:
  type: git
  repo: https://github.com/username/username.github.io.git
  branch: pages
```

12. 在项目中安装插件，命令如下
```
npm install hexo-deployer-git -save
```

13. 在项目中跑如下两行命令，hexo g代表在本地生成静态文件，hexo d代表将生成的静态文件提交推送至pages分支中。等待deploy完成，再去github上查看源码发现pages分支里自动生成了静态页面文件。访问https://username.github.io 例如：[https://shelly0702.github.io](https://shelly0702.github.io/)搞定！
```
hexo g
hexo d
``` 
