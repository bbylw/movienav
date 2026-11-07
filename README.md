# Movie Navigator

一个 Netflix 风格的影视导航网站，纯静态实现，可轻松部署到 Cloudflare Pages 或 GitHub Pages。

## 特点

- **纯静态实现**
  - 只包含 HTML、CSS 和少量 JavaScript
  - 零依赖，无需构建工具
  - 快速加载

- **界面设计**
  - Netflix 风格的深色主题
  - 响应式布局，适配多种设备
  - 平滑过渡动画
  - 精心设计的卡片交互效果

- **数据驱动**
  - 使用 `<script type="application/json" id="sites-data">` 集中管理网站数据
  - 便于维护和扩展

## 技术栈

- HTML5
- CSS3
- JavaScript (原生)
- Font Awesome 7.3.1 (图标)

## 项目结构

```tree
.
├── README.md        # 项目说明文档
├── favicon.svg      # 网站矢量图标
├── index.html       # 主页面，包含所有 HTML、CSS 和 JavaScript
└── LICENSE          # MIT 许可证文件
```

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

## 自定义

### 修改网站数据

编辑 `index.html` 文件中的 `<script type="application/json" id="sites-data">` 标签内的 `sites` 数组：

```json
{
  "sites": [
    {
      "name": "网站名称",
      "url": "https://example.com",
      "icon": "fa-solid fa-play",
      "description": "网站描述",
      "tags": ["标签1", "标签2"]
    }
  ]
}
```

每个网站对象包含以下字段：

- `name`: 网站名称
- `url`: 网站链接地址
- `icon`: Font Awesome 图标类名（如 `fa-solid fa-play`）
- `description`: 网站简短描述
- `tags`: 网站标签数组

> 图标可以在 [Font Awesome 图标库](https://fontawesome.com/icons) 中选择，复制对应图标的类名即可

### 修改网站外观

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
