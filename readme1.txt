git 命令 
具体步骤参考https://blog.csdn.net/ZYXKN/article/details/154536541



第一步：空文件夹git 初始化git init
第二步：关联远程仓库 git remote add origin https://github.com/你的用户名/仓库名.git
第三步：验证关联是否成功：git remote -v（输出 origin 对应的地址即成功）
第四步：上传文件前要将文件暂存，这个暂存就是标记你要上传的文件。
                  git add 文件名1 文件名2  # 上传指定文件
                  # 或上传所有文件（推荐，忽略 .gitignore 中指定的内容）
                   git add .
第五步：git commit -m "提交说明：如「上传项目源码、配置文件」"
第六步：拉取远程仓库最新内容（避免冲突，首次上传必做）： 
git pull origin main --allow-unrelated-histories
说明：main 是 GitHub 默认分支名，若你的分支名是 master，替换为 git pull origin master --allow-unrelated-histories；
git push -u origin master 

