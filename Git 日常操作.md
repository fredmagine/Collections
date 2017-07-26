- # Git 日常操作

  - checkout
  - merge
  - update
  - commit
  - git 注册到 github
  - 推送本地仓库到远程
  - 获取 Github 上的项目

  ## checkout

  - 撤销本地修改 git checkout -- file 

  ## merge

  - `git mergin origin master`

  ## update

  - `git pull origin master`

    ​

  ## commit

  - refusing to merge unrelated histories  

    ```
    git pull origin master --allow-unrelated-histories
    ```

  - Changes not staged for commit

    ```
    git add .
    git commit -m 'something to describe'
    ```

    ​

    ​

  ## git 注册到 github

  - 本地初始化仓库

    ```
    git config --global user.name=''
    git config --global user.email=''

    cd /d/Helloworld
    git init
    git add readme.md
    git commit -m "my first commit"
    ```


  - 注册到 Github

    ```
    ssh-keygen rsa -t -C 'xxx@email'
    复制 id_rsa.pub 内的秘钥， 到Github的Setting中添加key
    ssh -T git@github.com
    yes
    ```

  - 在本地提交到GIthub

    ```
    git push origin master
    ```

  ​

  ## 推送本地仓库到远程

  1. 在项目路径, git bash here, 输入`git init` ，初始化git

  2. 然后添加所有文件到本地仓库 `git add .`

  3. 提交到本地仓库 `git commit -m ""`

  4. 在 Github 上新建 repository，复制 repository.git 地址

  5. 关联本地仓库到远程仓库

     `git remote add origin https://github/xxx/myvue1.git`

  6. 最后一步，将代码由本地仓库上传到 Github

     `git push -u origin master`

     ​

  ## 获取 Github 上的项目

  1. git bash 到项目空间

     ```
     cd /workplace
     ```

  2. clone 项目到本地

     ```
     git clone https://github.com/fredmagine/photoShare.git
     ```