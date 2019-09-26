git相关操作
---

* Git global setup
```
git config --global user.name "bebee"
git config --global user.email "grsong.cn@gmail.com"
```

* Create a new repository
```
git clone https://gitlab.com/bebee4java/streamingetl.git
cd streamingetl
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master
```

* Push an existing folder
```
cd existing_folder
git init
git remote add origin https://gitlab.com/bebee4java/streamingetl.git
git add .
git commit -m "Initial commit"
git push -u origin master
```

* Push an existing Git repository
```
cd existing_repo
git remote rename origin old-origin
git remote add origin https://gitlab.com/bebee4java/streamingetl.git
git push -u origin --all
git push -u origin --tags
```

## 基本命令

1. 查看本地分支信息

    git branch

2. 查看远程分支信息

    git branch -r

3. 创建并切换songgr分支
   git checkout -b songgr

4. 获取commit id
   > 获取完整commit id

   git rev-parse HEAD
   > 获取short commit id

   git rev-parse --short HEAD
