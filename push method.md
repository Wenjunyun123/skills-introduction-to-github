


          
# 📋 项目完成后的Git推送操作指南

基于您的TODOLIST项目经验，为您总结完整的Git工作流程：

## 🚀 标准推送流程

### 1. 项目初始化（首次）
```bash
# 初始化Git仓库
git init

# 配置用户信息（首次使用）
git config --global user.name "您的用户名"
git config --global user.email "您的邮箱"

# 添加远程仓库
git remote add origin https://github.com/Wenjunyun123/仓库名.git
```

### 2. 日常提交流程
```bash
# 查看文件状态
git status

# 添加文件到暂存区
git add .                    # 添加所有文件
git add 文件名               # 添加特定文件
git add *.js                # 添加特定类型文件

# 提交更改
git commit -m "提交信息"     # 简短描述
git commit -m "feat: 添加新功能" -m "详细描述功能实现"  # 详细提交

# 推送到远程仓库
git push origin main         # 推送到main分支
git push -u origin main      # 首次推送（设置上游分支）
```

## 🔧 常用Git操作

### 分支管理
```bash
# 查看分支
git branch                   # 本地分支
git branch -r               # 远程分支
git branch -a               # 所有分支

# 创建和切换分支
git checkout -b feature/新功能  # 创建并切换到新分支
git checkout main           # 切换到main分支
git merge feature/新功能     # 合并分支
```

### 远程仓库操作
```bash
# 查看远程仓库
git remote -v

# 拉取最新代码
git pull origin main
git fetch origin            # 仅获取不合并

# 推送到不同分支
git push origin feature/新功能
```

### 版本管理
```bash
# 查看提交历史
git log --oneline           # 简洁格式
git log --graph --oneline   # 图形化显示

# 版本回退
git reset --soft HEAD~1     # 软回退（保留更改）
git reset --hard HEAD~1     # 硬回退（丢弃更改）

# 创建标签
git tag v1.0.0
git push origin v1.0.0
```

## 📝 提交信息规范

### 常用提交类型
- `feat:` 新功能
- `fix:` 修复bug
- `docs:` 文档更新
- `style:` 代码格式调整
- `refactor:` 代码重构
- `test:` 测试相关
- `chore:` 构建过程或辅助工具的变动

### 示例
```bash
git commit -m "feat: 添加用户登录功能"
git commit -m "fix: 修复TODO删除按钮无响应问题"
git commit -m "docs: 更新README安装说明"
```

## 🛠️ 实用技巧

### 文件管理
```bash
# 忽略文件（.gitignore）
node_modules/
.env
*.log
dist/

# 删除已跟踪的文件
git rm --cached 文件名
git rm -r --cached node_modules/
```

### 问题解决
```bash
# 撤销暂存
git reset HEAD 文件名

# 修改最后一次提交
git commit --amend -m "新的提交信息"

# 强制推送（谨慎使用）
git push --force-with-lease origin main
```

## 🎯 您的项目特色操作

基于TODOLIST项目：
```bash
# 完整的项目推送流程
git add .
git commit -m "feat: 完成全栈TODO应用开发"
git push -u origin main

# 添加许可证后
git add LICENSE
git commit -m "docs: 添加MIT许可证"
git push origin main
```

这套流程适用于您未来所有的前后端项目开发！
        
