# CQ-updateFile
使用GitHub上传文件
--------------------------------------------
#1-下载并安装git 
下载官网 https://git-scm.com/

#2-git绑定用户
打开git-bash.exe（直接在桌面上点击右键，或者点击开始按钮找到Git Bash）

在打开的GIt Bash中输入以下命令（用户和邮箱为你github注册的账号和邮箱）
  $ git config --global user.name "CQ001"
  $ git config --global user.email "643061480@qq.com"

#3-生成秘钥（没有默认通过）

#4-找到要上传的文件夹 进入 （创建本地仓库）
  git init (生成一个.git结尾的文件夹)
  git add . (将所有文件添加到仓库)
  git commit -m "备注"
 
#5-关联github仓库
 到github text仓库复制仓库地址
 git remote add origin https://github.com/hanyuntao/text.git
 上传本地代码
 git push -u origin master （或git push -f origin master）(master为分支名)
 
 
## 拉取仓库文件
1、将远程仓库克隆到本地：

git clone https://github.com/Aaron0525/Vue-juejin-App.git(项目克隆地址)

2、生成分支gh-pages并切换到此分支

cd flexSupplement （进入到你克隆仓库的本地文件夹）
git checkout --orphan gh-pages (创建分支并切换)

3、将本地克隆文件(文件名为github仓库名)里面除.git文件以外的其他文件全部删除，再将根目录下dist文件夹里面的内容复制到克隆文件中。

依次执行以下命令：
git add . （将本地所有文件加到仓库里）
git commit -m "message" （设置提交信息）
git remote add origin https://github.com/Aaron0525/　Vue-juejin-App.git（本地仓库链接远程仓库）
git push -u origin gh-pages （push文件到仓库中）

######项目打包后制作GitHub在线预览效果###########
参考链接： http://www.imooc.com/article/19464?block_id=tuijian_wz
