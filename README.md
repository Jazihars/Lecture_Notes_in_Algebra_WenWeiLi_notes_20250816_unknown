# Lecture_Notes_in_Algebra_WenWeiLi_notes_20250816_unknown
李文威《代数学讲义》学习笔记（3.3多项式环-待定）（20250816开始从3.3多项式环开始学，开始在本仓库中更新）（活跃更新仓库）（之后笔记数量过多时，本仓库会转入封存）

## 在两台电脑上向本仓库提交的安全流程
因为需要在两台不同的电脑上向本仓库提交文件，面临着：

* 不确定上次在哪台电脑push
* 不确定当前本地是否有修改
* 不确定是否存在本地提交
* 不确定远程是否领先

的问题。因此，在提交之前，在本地`Git`终端上（通常是在`VSCode`的终端中操作`Git`）运行以下的安全流程（以后仍然有可能会完善此安全流程）：

``` bash
# 往本地clone下来的本地GitHub仓库中放入新文件之前，按顺序运行以下命令：

git fetch
git pull --rebase

# 如有报错：
# git stash
# git pull --rebase
# git stash pop

git status
git diff
git diff --cached

# 如果以上命令都没有报错，也没有需要处理的状况，现在开始往本地clone下来的GitHub仓库中放入新文件

git add .
git commit -m "XXX"
git push

```

目前（2026.1.22）暂定执行此安全流程，以后仍有可能继续修改完善