# 部署到 GitHub Pages

## 步骤（约 2 分钟）

### 1. 创建 GitHub Repo

1. 访问 https://github.com/new
2. Repository name: `quote-form`
3. Public
4. 不要勾选 "Initialize with README"
5. 点「Create repository」

### 2. Push 代码

回到 Terminal，在 `quote-form/` 目录下运行：

```bash
git remote add origin https://github.com/YOUR_USERNAME/quote-form.git
git branch -M main
git push -u origin main
```

### 3. 启用 GitHub Pages

1. 访问 repo 的 Settings → Pages
2. Source: 选「Deploy from a branch」
3. Branch: 选「main」，目录选「/ (root)」
4. 点「Save」

### 4. 获取链接

等待 1-2 分钟后，访问：
`https://YOUR_USERNAME.github.io/quote-form/`

---

## 更快的方式（如果有 GitHub CLI）

```bash
cd quote-form
gh repo create quote-form --public --source=. --remote=origin --push
gh repo view --web
# 然后在 Settings → Pages 启用
```

---

完成后，这个链接就是永久的，随时随地都能用！
