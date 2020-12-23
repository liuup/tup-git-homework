# tup-git-homework
TUP computer vision git homework for new learners

## 作业要求
1. star this repo
2. fork this repo
3. pull request(every file is ok) to this main branch
4. talk something in Issues

# Git使用教程(无原理讲解)

## 1. 常用命令
以linux下为例,使用git前需要```sudo apt-get install git```  
 - ```git init``` 仓库初始化(也就是说运行这条命令后git就会自动记录所有更改)
 - ```git status .``` 查看当前路径下的状态
 - ```git commit -m "更改信息"``` 向git提交更改,并记录更改log
 - ```git push``` 把版本库的所有更新内容,向远端服务器(github,gitee...)推送
 - ```git pull``` 将远端服务器的内容拉取到本地(拉代码)
 - ```git log``` 查看此仓库的所有更改记录
 - ```git diff``` 比较自己都做了什么修改
 - ```git clone [url]``` 将远端服务器的所有代码复制到本地(clone只在第一次使用,后来的拉代码使用pull)

****
**当我们修改了本地代码,向远端服务器推送时,操作步骤如下:**
1. ```git add .``` //添所有修改
2. ```git commit -m "updtae main.cpp"``` //提交更改信息
3. ```git push``` //推送代码到远端服务器


## 2.Github操作实例
1. 首先,我在Github创建一个空的repo  
![empty_repo](https://akaliuup.gitee.io/pics/Screenshot%20from%202020-05-03%2019-03-58.png)  
url为[liuup/git_sample](https://github.com/liuup/git_sample)

2. 随便写几行代码,对本地文件夹执行```git init```
![init](https://akaliuup.gitee.io/pics/Screenshot%20from%202020-05-03%2019-24-02.png)

3. 对代码随便修改几处  
![change](https://akaliuup.gitee.io/pics/Screenshot%20from%202020-05-03%2019-28-45.png)

4. 在本地记录修改内容  
```git add .```  
```git commit -m "add hello,github"```  
![add](https://akaliuup.gitee.io/pics/Screenshot%20from%202020-05-03%2019-30-43.png)

5. 可以查看log  
```git log```  
![log](https://akaliuup.gitee.io/pics/Screenshot%20from%202020-05-03%2019-33-10.png)

6. 配置一下远端服务器
- 记录 url ```https://github.com/liuup/git_sample```
- 执行```git remote add sample https://github.com/liuup/git_sample``` 其中的sample是随便起的一个名字

7. 向远端服务器推送代码,会提示输入账号名和密码  
```git push -u sample master```  
![push](https://akaliuup.gitee.io/pics/Screenshot%20from%202020-05-03%2019-39-31.png)  
可以使用↓记住账号和密码  
```git config --global credential.helper store```

8. 从远端服务器拉取代码并查看log  
> 假设此时有别人更改了代码,那么我本人就需要更改我本地的代码和log  

```git pull```  
![pull](https://akaliuup.gitee.io/pics/Screenshot%20from%202020-05-03%2019-47-21.png)

9. 查看本地的仓库  
```git remote```  
![remote](https://akaliuup.gitee.io/pics/Screenshot%20from%202020-05-03%2019-57-16.png)

10. 远程仓库的重命名  
```git remote rename <old> <new>```  
![rename](https://akaliuup.gitee.io/pics/Screenshot%20from%202020-05-03%2019-57-31.png)

11. 远仓库的删除  
```git remote remove example```


## Reference
1. [适合小白/外行的git与github最基础最浅显教程](https://www.cnblogs.com/yaoxiaowen/p/8227873.html)
2. [Git 基础 - 远程仓库的使用](https://git-scm.com/book/zh/v2/Git-%E5%9F%BA%E7%A1%80-%E8%BF%9C%E7%A8%8B%E4%BB%93%E5%BA%93%E7%9A%84%E4%BD%BF%E7%94%A8)


