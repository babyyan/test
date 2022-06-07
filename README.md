## git常用场景命令
### 1. 查看commit提交了什么内容
    git show
#### 或者
    git log -n1 -p
### 2. 提交信息(commit message)写错了并且还未push,如何修改
    git commit --amend --only //打开编辑器修改
    或者
    git commit --amend --only -m 'xxxxxxx' //直接修改
> ### 3. 撤销
>> + 将暂存区(add后)中的文件覆盖工作目录中的文件
    git checkout filename
>> + 将文件从暂存区删除
    git rm --cached filename
>> + 从本地仓库（commit)里移除一个文件
    git checkout HEAD^ filename
>> + 将git仓库中指定的更新记录恢复出来，并且覆盖暂存区和工作目录
    git reset --hard commitId


