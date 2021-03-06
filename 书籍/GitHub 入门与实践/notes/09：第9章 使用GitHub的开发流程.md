---
title: 第9章 使用GitHub的开发流程
hidden: true
---

# 第9章 使用GitHub的开发流程

- [ ] 9.1 团队使用GitHub时的注意事项
  - 一切从简
    - 项目管理工具与GitHub的区别
    - 项目管理工具与GitHub相异的原因
  - 不Fork仓库的方法
- [ ] 9.2 GitHub Flow——以部署为中心的开发模式
- [ ] 9.3 GitHub Flow的流程
  - 随时部署，没有发布的概念
  - 进行新的作业时要从master分支创建新分支
  - 在新创建的分支中进行提交
  - 定期push
  - 使用Pull Request
  - 务必让其他开发者进行审查
  - 合并后立刻部署
- [ ] 9.4 实践GitHub Flow的前提条件
  - 部署作业完全自动化
    - 使用部署工具
    - 通过Web界面进行部署的工具
    - 导入开发时的注意事项
  - 重视测试
    - 让测试自动化
    - 编写测试代码，通过全部测试
    - 维护测试代码
- [ ] 9.5 模拟体验GitHub Flow
  - Fizzbuzz的说明
  - 添加新功能
  - 创建新的分支
    - 如果尚未clone仓库
    - 如果之前clone过仓库
    - 创建特性分支
  - 实现新功能
  - 创建Pull Request
  - 接收反馈
  - 修正缩进
  - 添加测试
  - 培育Pull Request
  - Pull Request被合并
- [ ] 9.6 团队实践GitHub Flow时的几点建议
  - 减小Pull Request的体积
  - 准备可供试运行的环境
  - 不要让Pull Request中有太多反馈
  - 不要积攒Pull Request
- [ ] 9.7 GitHub Flow的小结
- [ ] 9.8 Git Flow——以发布为中心的开发模式
  - 便于理解的标准流程
  - 有时显得过于复杂
- [ ] 9.9 导入Git Flow前的准备
  - 安装git-flow
    - Mac下的安装
    - Linux下的安装
    - 确认运行状况
  - 仓库的初始设置
    - 创建仓库
    - 进行git flow的初始设置
    - 在远程仓库中也创建develop分支
- [ ] 9.10 模拟体验Git Flow
  - master分支与develop分支的区别
    - master分支
    - develop分支
  - 在feature中进行的工作
    - 创建分支
    - 在分支中进行作业
  - 发送Pull Request
  - 通过代码审查提高代码质量
  - 更新本地的develop分支
  - 在release分支中进行的工作
    - 专栏：设置默认分支
    - 创建分支
    - 分支内的工作
    - 进行发布与合并
    - 查看版本标签
  - 更新到远程仓库
  - 在hotfix分支中进行的工作
    - 创建分支
    - 创建标签和进行发布
    - 从hotfix分支合并至develop分支
- [ ] 9.11 Git Flow 的小结
  - 专栏：版本号的分配规则
