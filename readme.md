git init

git add

git add .

git add glb

git commit -m "first commit"

git branch -M main

git remote add origin https://github.com/huangarron/pub\_source.git

git push -u origin main





git branch -M main

背景/目的: 早期 Git 仓库的默认主分支通常是 master。现在，许多平台（包括 GitHub）出于包容性考虑，鼓励使用 main 作为新的默认主分支名称。这个命令的作用就是将你本地仓库的当前分支（很可能就是 master）重命名为 main



git remote add origin https://github.com/huangarron/pub\_source.git

这个命令用于添加一个远程仓库地址，并给它起一个易于引用的名称。



git remote: 这是 Git 中用来管理远程仓库连接的命令。



add: 表示你要添加一个新的远程连接。



origin: 这是你给这个远程仓库地址起的一个别名（或简称）。origin 是一个约定俗成的名称，通常用来指代你代码的主要远程仓库。



https://github.com/huangarron/pub\_source.git: 这是远程 Git 仓库（即你在 GitHub 上创建的那个仓库）的实际 URL 地址。



目的: 通过这个命令，你告诉本地 Git 仓库：“这个 URL 地址是我要推送和拉取代码的地方，从现在起，我可以用 origin 来代表这个长长的 URL。”





git push -u origin main

这个命令用于将你的本地提交推送到远程仓库。



git push: 这是将本地分支的提交上传到远程仓库的命令。



origin: 指定要推送到的远程仓库的别名（在上一步中设置）。



main: 指定要推送的本地分支名称。



-u: 这是 --set-upstream 的缩写。



-u 的作用 (重点):



它告诉 Git 将本地的 main 分支与远程的 origin/main 分支关联起来（建立跟踪关系）。



一旦建立了跟踪关系，之后你再执行 git push 或 git pull 时，就不需要再指定 origin main 了，直接输入 git push 或 git pull，Git 就会自动知道要对 origin 上的 main 分支进行操作。



目的: 将本地 main 分支上的所有提交发送到 GitHub 远程仓库，并在第一次推送时建立跟踪关系，以便后续操作的简化。

