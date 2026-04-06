# 🚀 GitHub 发布指南

## 前置准备

1. 确保你有 GitHub 账号
2. 确保已安装 Git（如未安装，访问 https://git-scm.com/）

---

## 步骤 1：创建 GitHub 仓库

1. 访问 https://github.com/new
2. **仓库名称**：`humanize-writing-skill`
3. **描述**：`去 AI 味，注入人味。A powerful skill to remove robotic tone and add human touch to your writing.`
4. **可见性**：Public（公开）
5. **不要**初始化 README（我们已经有完整的文件结构）
6. 点击 "Create repository"

---

## 步骤 2：初始化本地 Git 仓库

打开命令行（CMD 或 PowerShell），执行：

```bash
# 进入项目目录
cd D:\humanize-writing-skill

# 初始化 Git 仓库
git init

# 添加所有文件
git add .

# 提交
git commit -m "feat: initial commit - humanize-writing skill v1.0.0"

# 添加远程仓库（替换为你的 GitHub 用户名）
git remote add origin https://github.com/YOUR_USERNAME/humanize-writing-skill.git

# 推送到 GitHub
git push -u origin main
```

如果提示分支名称问题，使用：

```bash
# 重命名分支为 main
git branch -M main

# 再次推送
git push -u origin main
```

---

## 步骤 3：完善 GitHub 仓库信息

### 3.1 添加主题标签（Topics）

在 GitHub 仓库页面，点击 "Manage topics"，添加：
- `ai-writing`
- `humanize`
- `prompt-engineering`
- `openclaw`
- `writing-tools`
- `chinese-writing`
- `ai-skill`

### 3.2 设置仓库类别

- **Category**: `Writing` 或 `Productivity`

### 3.3 添加 GitHub Actions（可选）

如果需要自动化测试，可以添加 CI/CD 流程。

---

## 步骤 4：推广你的技能

### 4.1 分享到社区

- **Open Claw 社区**：在技能市场提交你的技能
- **知乎**：写一篇"如何去除 AI 味"的文章，附上仓库链接
- **Twitter/X**：发布 Before/After 对比图
- **微信公众号**：分享实战案例

### 4.2 示例推文

```
刚发布了我的第一个开源技能：humanize-writing-skill 🚀

专门用来去除 AI 生成文字的"机械味"，注入人类的场景感、情绪和瑕疵。

基于 Grammarly AI Humanizer 原理 + 中文实战案例提炼
包含 7 步手术法、3 大维度、N 个实战案例

GitHub: https://github.com/YOUR_USERNAME/humanize-writing-skill

#AI #写作 #开源 #去 AI 味
```

---

## 步骤 5：持续维护

### 5.1 收集反馈

- 在 README 中添加 Issue 模板
- 鼓励用户提交 Before/After 案例
- 定期更新案例库

### 5.2 版本迭代

```bash
# 更新 SKILL.md 中的版本号
# 更新 README.md 中的版本历史
# 更新 CHANGELOG.md（如需要）

git add .
git commit -m "chore: version bump to v1.1.0"
git push
```

### 5.3 添加新 Skill

当你开发新技能时，遵循相同模式：
1. 创建独立仓库：`new-skill-name`
2. 保持相同结构：README.md + SKILL.md + examples/ + LICENSE
3. 在个人主页添加 Topic 关联

---

## 常见问题

### Q1: 推送时提示权限错误？

**解决方案**：使用 Personal Access Token

1. 访问 https://github.com/settings/tokens
2. 创建新 Token，勾选 `repo` 权限
3. 推送时使用 Token 替代密码

```bash
git push https://YOUR_USERNAME:YOUR_TOKEN@github.com/YOUR_USERNAME/humanize-writing-skill.git main
```

### Q2: 如何更新已有的 Skill？

```bash
# 修改文件后
git add .
git commit -m "feat: 添加新的商业文案案例"
git push
```

### Q3: 如何添加协作者？

1. 访问仓库 Settings → Manage access
2. 点击 "Invite a collaborator"
3. 输入对方 GitHub 用户名

---

## 成功标志

✅ 仓库创建成功，文件完整
✅ 有 Star、Fork、Watch
✅ 有用户提交 Issue 或 PR
✅ 被其他项目引用
✅ 收到用户感谢或案例分享

---

## 下一步

发布后，考虑：
1. 写一篇技术博客介绍创作过程
2. 录制一个使用视频教程
3. 开发配套 VS Code 插件
4. 创建在线演示页面

**祝发布顺利！🎉**
