# Movie Navigator

一个 Netflix 风格的影视导航网站，采用纯静态设计，可轻松部署到 Cloudflare Pages 或 GitHub Pages。



## 特点

- 💫 Netflix 风格设计
  - 深色主题
  - 响应式布局
  - 平滑过渡动画
  - 精心设计的卡片交互

- 🎯 核心功能
  - 影视资源导航
  - 优雅的视觉体验
  - 流畅的动画效果
  - 完全响应式设计

- 🚀 技术特点
  - 纯静态实现
  - 无需后端支持
  - 零依赖
  - 快速加载

## 部署方式

### Cloudflare Pages 部署

1. Fork 本仓库
2. 登录 Cloudflare Dashboard
3. 进入 Pages 板块
4. 点击 "Create a project"
5. 选择 "Connect to Git"
6. 选择你 fork 的仓库
7. 部署配置：
   - Build command: 留空
   - Build output directory: /
   - Root directory: /
8. 点击 "Save and Deploy"

### GitHub Pages 部署

1. Fork 本仓库
2. 进入仓库设置
3. 找到 "Pages" 设置项
4. Source 选择 "main" 分支
5. 选择根目录 "/(root)"
6. 点击 "Save"
7. 等待部署完成

## 本地开发

```bash
# 克隆仓库
git clone https://github.com/yourusername/movie-navigator.git

# 进入项目目录
cd movie-navigator

# 使用任意 HTTP 服务器运行
# 例如 Python 的 HTTP 服务器
python -m http.server 3000
```

## 自定义

### 修改网站

编辑 `index.html` 文件：

- 修改网站标题
- 更新导航链接
- 添加/删除卡片

### 样式定制

所有样式都在 `<style>` 标签中：

- 修改颜色变量
- 调整间距
- 自定义动画效果

## 贡献

欢迎提交 Pull Request 或创建 Issue。

## 许可

MIT License
