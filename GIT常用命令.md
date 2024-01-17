# GIT常用命令



## git项目搭建命令

1. add：从workspace上传到index暂存区
2. commit：从index上传到Repository本地仓库
3. push：从Repository上传到Remote远程仓库
4. fetch/clone：从Repository传回Repository本地仓库
5. checkout：从Repository传回workspace
6. pull：从Remote传回workspace

![image-20240116173423969](https://gitee.com/anan0428/PicGo/raw/master/202401161734705.png)



## 本地仓库搭建

1. git init：在该目录创建仓库
2. git clone +远程库的url：克隆远程目录到本地目录



## GIT文件操作

1. 文件的4中状态

   * Untracked：未跟踪，文件在文件夹中，没有加入git库
   * Unmodify：文件已经入库，未修改
   * Modified：文件已修改
   * Staged：暂存状态

2. 查看文件状态

   * git status：查看所有文件状态
   * git status [filename]：查看指定文件的状态
   * git diff 文件名：查看修改内容

3. 文件提交操作

   * git add .：添加所有文件到暂存区
   * git commit -m "消息内容"：提交暂存区中的内容到本地仓库  -m 提交信息

4. 忽略文件

   在主目录建立"gitignore"文件，该文件有一下规则：

   * #为注释

   * *表示任意多个字符
   * ？表示一个字符
   * ！表示例外规则，不被忽略
   * 名称前是一个/，表示要忽略的文件在此名称文件所在目录下，而子目录中文件不被忽略
   * 名称后是一份/，表示要忽略的是此名称文件的子目录