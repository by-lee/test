# ATOM与GitHub的协同工作
## 将本地文件链接到GitHub

1. 在GitHub上，create New Repository

2. 填写Repository name ，点击Creative Repository

3. 创建后会有串命令行提示，如下图

  ![](http://91jean.oss-cn-hangzhou.aliyuncs.com/18-7-26/95965344.jpg)

4. 在本地电脑上创建一个项目文件夹

5. 右键单击文件夹，选择Git Bash Here

6. 输入第三步的命令（根据自己的输入）

  ```git
  echo "# test" >> README.md
  git init
  git add README.md
  git commit -m "first commit"
  git remote add origin https://github.com/by-lee/test.git
  git push -u origin master
  ```

  7. 有时候会需要你输入`Username for 'https://github.com':` 后面填写自己的github账户名即可，然后会有一个弹窗要求输入github的账户密码，按要求输入即可。
  8. 输入完成后，等待上传，上传完成后看到`Branch 'master' set up to track remote branch 'master' from 'origin'.`代表你已经成功了。
  ## 利用Atom随时提交本地文件到GitHub
  1. 用Atom打开刚刚创建好的项目文件（注意此时的文件夹的图标是与普通的图标是不一样的）
  ![][1]
  2. 在此项目文件夹内即可创建修改文件了（例如，我们此时创建一个文件-`index.html`)
  3. 保存创建的文件，打开git面板（``拓展-GitHub-切换Git面板``，或者鼠标移动到面板右边，点击>）
  4. 点击`Stage ALL`
![][2]
5. 填写`commit message`，此处填写你作出的改动例如本次我填写的是`create index.html`然后点击`Commit to master`
![][3]
6. 点击`Push`上传
![][4]
等待上传完成，刷新github的仓库就可以看到你改动的代码啦！









[1]:http://91jean.oss-cn-hangzhou.aliyuncs.com/18-7-26/60809809.jpg
[2]:http://91jean.oss-cn-hangzhou.aliyuncs.com/18-7-26/35718017.jpg
[3]:http://91jean.oss-cn-hangzhou.aliyuncs.com/18-7-26/16159490.jpg
[4]:http://91jean.oss-cn-hangzhou.aliyuncs.com/18-7-26/76558608.jpg
