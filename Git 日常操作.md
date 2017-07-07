# Git 日常操作

## checkout



## update



## commit

- refusing to merge unrelated histories  

  ```
  git pull origin master --allow-unrelated-histories
  ```

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