# 这里是我的作业项目，主要是linux和数据结构课

为了防止某个**蠢货**忘记怎么用github，在下面重新介绍一下如何把git仓库从本地推上来

- 找到工作目录，`git init`启动！！！

- 需要拉下来就`git pull`

- 因为已经绑定过了所以直接`git push`应该就可以了，当然如果没有绑定你就需要`git push --set-upstream origin main`

- `git branch dev`这样可以创建分支，`git merge dev`这样可以把本地分支合并上去

有些时候你会本地改了一个文件还没提交，pull过来的远程版本又改了这个文件

```
# 1. 暂存你本地没提交的修改
git stash

# 2. 拉取远程合并
git pull origin main

# 3. 把暂存的本地修改放出来
git stash pop

# 4. 继续
git add .
git coimmit
git push
```
