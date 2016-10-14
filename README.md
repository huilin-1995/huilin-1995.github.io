# 我的博客

标签（空格分隔）： hexo

---

最近搭建了一个博客，感觉很有意思，分享给大家
## 配置环境

 1. 安装Node（必须）
 2. 安装Git（必须）
 3. 安装Git（必须）

### 正式安装HEXO　
``` brash
$ sudo npm install -g hexo
```
``` brash
hexo init
```
``` brash
hexo generate （hexo g  也可以） 
```
``` brash
hexo server
```
浏览器输入http://localhost:4000
## 配置Github
### 建立Repository
``` brash
Blog 
　｜ 
　｜－－ _config.yml 
　｜－－ node_modules 
　｜－－ public 
　｜－－ source 　　　 　 　｜－－ db.json	
　｜－－ package.json 
　｜－－ scaffolds 
　｜－－ themes 　
```
现在我们需要_config.yml文件，来建立关联，命令：
``` brach
vim _config.yml
```
翻到最下面，改成我这样子的，注意： : 后面要有空格
``` brach
deploy:
  type: git
  repository: https://github.com/huilin-1995/huilin-1995.github.io.git
  branch: master
```
执行如下命令才能使用git部署
``` 
npm install hexo-deployer-git --save
```
```
hexo deploy
```
然后再浏览器中输入http://huilin-1995.github.io/就行了
部署的步骤
```
hexo clean
hexo generate
hexo deploy
```
一些常用命令：
```
hexo new "postName" #新建文章
hexo new page "pageName" #新建页面
hexo generate #生成静态页面至public目录
hexo server #开启预览访问端口（默认端口4000，'ctrl + c'关闭server）
hexo deploy #将.deploy目录部署到GitHub
hexo help  # 查看帮助
hexo version  #查看Hexo的版本
```
好看的主题
　[Cover](https://github.com/daisygao/hexo-themes-cover) - A chic theme with facebook-like cover photo  个人感觉挺好看的
　[Oishi](https://github.com/henryhuang/oishi) - A white theme based on Landscape plus and Writing. 
　[TKL](https://github.com/SuperKieran/TKL) - A responsive design theme for Hexo. 一个设计优雅的响应式主题 
　[Tinnypp](https://github.com/levonlin/Tinnypp) - A clean, simple theme based on Tinny 
　[Writing](https://github.com/yunlzheng/hexo-themes-writing) - A small and simple hexo theme based on Light 
[　Yilia](https://github.com/litten/hexo-theme-yilia) - Responsive and simple style 优雅简洁响应式主题，我用得就是这个。 




