# LearnGithub
[@happypeter](https://github.com/happypeter) 老师是慕课网著名的声优，他的讲课思路清晰，准备充足，由浅入深，通俗易懂。<br />
学习一门新知识，自己动手做下总是好的。<br />
现在重新(:shipit:是的，第三遍看此视频了)跟随peter老师把《搬进Github》这门课程再学习一遍。
以下为课程摘要：
## 浏览器中使用Github
* 创建一个仓库
* commit的意思是做一个版本
## 客户端中使用Github
* 创建仓库
* 提交版本（添加文件／修改文件）
* Undo只适合于未同步的版本
* 发布项目
## 简单分支操作
* 创建分支（有新想法，但不想污染成熟代码）
![](http://gitbeijing.com/images/simple_branching/new_branch.png)
* 编辑分支
![](http://gitbeijing.com/images/simple_branching/new_branch_commit.png)
* 发布分支
## 合并分支
* 合并分支（Merge)<br />
idea 合并到 matser
![](http://gitbeijing.com/images/merge/after_merge.png)
* 删除分支（Delete)
* 并行开发 <br />
一般可以直接Merge（合并） 
![](http://gitbeijing.com/images/merge/p_merge.png)
* 变基(rebase)合并<br />
大概意思是把别人的分支拉下来，再合并，但从结果而言，这个概念并不重要。
* 代码冲突<br />
定义：两个分支改了同一个地方，并且改得不一样。<br />
例子：同一个地方既被改为AAA，也被改为了BBB
![](http://gitbeijing.com/images/merge/conflicts_view.png)
```html
<<<<<<< HEAD
BBB
=======
AAA
>>>>>>> idea
```
商量后把冲突表识符删除并仅保留需要的代码，然后提交版本，发布即可。
## 团队协作流程
- 给队友添加权限<br />
在这里我给Peter老师添加权限
- 创建新分支<br />
- 添加新版本
- 发Comment(评论)<br />
网页版，从Commit进去，点击版本号，拉到最下面可以对该版本进行评论。
  - 小技巧：<br />
支持[MarkDown语法](https://guides.github.com/features/mastering-markdown/),输入“:”符号，可以添加emoji表情。
- 开启一个Pull Request<br />
这是整个GithubFlow的核心
  - 选择恰当的需要对比的版本
  - 添加Request标题，摘要，或上传截图。
- 讨论和代码审核<br />
在原来的分支进行修改／同步即可推送到同一Request。
- 合并分支并部署(Merge Pull Request)
## 开源项目贡献流程
* Fork(拷贝/建立分叉)
![](http://gitbeijing.com/images/fork_flow/flow.png)
* clone(把仓库拉下来)并进行修改
* 发布版本，同步分支并Pull Request
* 完成贡献后删除仓库（可选）<br />
*从Settings中删除*
* 仓库主人查看项目的Fork情况<br />
*谁Fork了／进行了什么修改*<br />
Graphs➡️Network
* 其他技巧：Quick Pull Request<br />
*直接在网页编辑器编辑后提交并Pull Request*
## Github Issues
- 项目主页(Github pages)
- Wiki <br />
创作自己的知识库
- Issues(事务卡片)<br />
很多比较复杂的项目管理软件会把“报 Bug”，“提新需求”，“其他讨论”，这些项目相关的内容分成不同的板块来进行，在 Github 这里，所有的内容就都作为事务卡片来统一管理了。
  - Assignee(委派完成)<br />
  默认是自己
  - 拖队友参与讨论<br />
  直接@他
  - 引用之前的评论∏<br />
  点击某个评论的时间 ➡️ 在地址栏复制该链接 ➡️ 直接在新评论里粘贴使用
  - 插入代码<br />
  修改代码并在提交版本的时候，在版本描述里加上Issue号，例如：add README #2
  - 关闭某次事务<br />
  1. 方法一、直接在网页端关闭
  2. 方法二、提交版本时，添加fix标识符，例如：add desc fix #2
## Github Pages 搭建网站
* Github Pages是可以绑定自己的域名的
* 在项目文件夹新建index.html,提交版本并同步
* 域名为(https://username.github.io/repositoryname)
