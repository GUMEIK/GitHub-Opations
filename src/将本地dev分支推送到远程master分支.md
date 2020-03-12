## 默认情况下，git是不允许合并两个不相干的分支的。
如在主分支下：
```git merge dev```
会出现以下出错:
```fatal: refusing to merge unrelated histories```
我们可以这样做:
- 执行命令使git允许不相干分支的合并
```git pull origin master --allow-unrelated-histories```
- 合并
```git merge dev```
## 直接从dev分支推送到master分支也是不可以的