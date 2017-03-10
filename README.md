WARDLL的前端之路
=======================

2017年3月5日 启程

***

> 学会拥抱失败，期待失败，接受失败，并准备直面失败。————by《Soft Skills》

> 如果你想成功，你必须要学会收起自己脆弱的自尊心，勇敢走出去，别害怕让自己出丑。每一个著名演员、音乐家、专业运动员和公共演说家都曾有过表现不佳的时候，他们自觉地选择了走出困境，尽力而为。成功终将会来。你不可能专注做某件事而毫无长进，你只要坚持足够长的时间就会有收益。你的生存之道就是不必太在意。别害怕被人看作傻瓜。 ————by《Soft Skills》

> 准备好面对批评，但不要惧怕。总会有人不喜欢你的言论，或者不赞同你的观点。你永远不可能取悦每一个人。 ————by《Soft Skills》

***


Git的使用
————————————————————————

###基本指令

将文件添加到暂存区
```git
git add 文件名
```

将文件提交到仓库
```git
git commit -m "文件名"
```

推送到Github
```git
git push origin master
```

**

###Git使用中的错误

执行“Git add” 
```注释
Another git process seems to be running in this repository, e.g.
an editor opened by 'git commit'. Please make sure all processes
are terminated then try again. If it still fails, a git process
may have crashed in this repository earlier:
remove the file manually to continue.
```

解决方法：
```注释
rm -f ./.git/index.lock
```

Git中创建密匙 ssh-keygen -t rsa -C "lhwardll@gmail.com"
```注释
too many arguments.
```

解决方法：
```注释
手动输入，从左到右，在句子末尾处敲回车。
```

使用git remote add origin添加远程主机
```注释
fatal: Not a git repository (or any of the parent directories): .git
```

解决方法：
```注释
git inti
```

输入上传指令 git push -u origin master
```注释
error: src refspec master does not match any.
error: failed to push some refs to https://github.com/WARDLL/QianDuan.git' ​​​​
```

解决方法：
如果在github的remote上已经有了文件，会出现错误。此时应当先pull一下：
```注释
git pull origin master
```
然后再进行：
```注释
git push origin master】
```
正确输入会弹出Github登录窗口
![github](http://odxwjay9m.bkt.clouddn.com/Github/README/QQ%E6%88%AA%E5%9B%BE20170310074052.png “github”)；

**