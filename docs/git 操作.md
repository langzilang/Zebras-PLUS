# git 一些操作
### 删除远程分支文件
```git rm -r --cached dirname    // 删除远程文件夹，但保留本地文件夹

git status  // 查看下状态

git commit -m 'delete a file or dir'   // 提交操作，并添加描述

git push origin dev    // 推送
```

### 回退 git add
```javascript
git reset HEAD
```
但是这个命令使用的时候，提示了这么个信息
![img_1.png](img_1.png)
#### 解决办法
```
// 第一种
git add .

git reset --hard

// 第二种
git stash

git stash drop
```

出现这种现象的原因好像是因为在新分支上，repos感知不到这个阶段的改变，你要用 add 或 stash, 让其知晓，才能做想要的回滚。


## 修改当前项目用户名和密码
```javascript
// 查看当前项目配置
git config --local --list

// 修改
git config --local user.name "XXX"
git config --local user.email "XXX"

// 删除配置项
git config --local -–unset site.name  // 删除项目中的 site.name 配置值
```
