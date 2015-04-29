欢迎来到 Mirantis OpenStack 文档中心
===============
# Mirantis OpenStack 是由三个组成部分构成: #


**Hardened packages in Mirantis OpenStack**. Hardened packages in Mirantis OpenStack 包含核心OpenStack项目， 随着OpenStack每个稳定版本更新，支持范围广泛的操作系统、虚拟机监控程序和部署拓扑。 
**Fuel**. Fuel是一种开放源码，通过一个单一的界面部署多个OpenStack环境的软件生命周期管理应用程序,并且使您能够管理这些环境部署。
**Support**. 30天免费基础试用支持。

此页面包含最新的Mirantis OpenStack的文档。从以下列表中选择你需要的标题，每个标题就是一个文档手册。

## Mirantis OpenStack 规划指南 ##


您在准备安装Fuel和部署Mirantis OpenStack之前应该考虑规划信息 

## 主要版本历史
* 0.1: 2015-04-29
    * 添加基本内容;
    * 修正错别字和表达不通顺的地方。


本书源码在 Github 上维护，欢迎参与：[https://github.com/boboke/Mirantis-OpenStack-Planning-Guide](https://github.com/boboke/Mirantis-OpenStack-Planning-Guide)。贡献者 [名单](https://github.com/orgs/boboke/people)。

## 参加步骤
* 在 GitHub 上 `fork` 到自己的仓库，如 `docker_user/docker_practice`，然后 `clone` 到本地，并设置用户信息。
```
$ git clone git@github.com:boboke/Mirantis-OpenStack-Planning-Guide.git
$ cd docker_practice
$ git config user.name "yourname"
$ git config user.email "your email"
```
* 修改代码后提交，并推送到自己的仓库。
```
$ #do some change on the content
$ git commit -am "Fix issue #1: change helo to hello"
$ git push
```
* 在 GitHub 网站上提交 pull request。
* 定期使用项目仓库内容更新自己仓库内容。
```
$ git remote add upstream https://github.com/boboke/Mirantis-OpenStack-Planning-Guide.git
$ git fetch upstream
$ git checkout master
$ git rebase upstream/master
$ git push -f origin master
```
