# 飞行模拟器网站 ✈️

一个现代化的飞行模拟器网站界面，具有交互式控制面板和仪表盘。

## 🚀 功能特点

- 🎮 交互式飞行控制面板
- 📊 实时飞行仪表显示
- 🔄 动态数据更新
- 📱 响应式设计
- 🎨 现代化UI界面

## 🛠️ 部署设置

### Netlify 自动部署配置

1. **设置 GitHub Secrets**
   在你的 GitHub 仓库中，进入 Settings > Secrets and variables > Actions，添加以下secrets：
   
   - `GGS`: 你的 Netlify 认证令牌
   - `FREEPROJECTID`: 你的 Netlify 站点 ID

2. **获取 Netlify 令牌和站点 ID**
   
   **获取认证令牌 (GGS):**
   - 登录 [Netlify](https://netlify.com)
   - 进入 User settings > Applications > Personal access tokens
   - 点击 "New access token"
   - 复制生成的令牌
   
   **获取站点 ID (FREEPROJECTID):**
   - 在 Netlify 控制台中打开你的站点
   - 进入 Site settings > General
   - 在 "Site details" 部分找到 "Site ID"
   - 复制站点 ID

3. **自动部署**
   - 每次推送到 `main` 或 `master` 分支时自动部署
   - Pull Request 时创建预览部署
   - 部署状态会在 GitHub 中显示

### 手动部署

如果你想手动部署到 Netlify：

1. 将项目文件夹拖拽到 Netlify 控制台
2. 或者连接 GitHub 仓库进行持续部署

## 📁 项目结构

```
jay/
├── index.html          # 主页面文件
├── netlify.toml        # Netlify 配置文件
├── .github/
│   └── workflows/
│       └── deploy.yml  # GitHub Actions 工作流
└── README.md          # 项目说明
```

## 🎯 使用说明

1. 打开 `index.html` 在浏览器中查看
2. 使用左侧控制面板调整飞行参数
3. 观察中央仪表盘的数据变化
4. 右侧状态面板显示系统信息

## 🔧 开发

这是一个纯静态网站，不需要构建步骤：
- HTML/CSS/JavaScript 都在单个文件中
- 可以直接在浏览器中打开运行
- 支持实时编辑和刷新

## 📝 许可证

MIT License
