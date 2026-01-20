# AI工具集导航网站

一个基于 Vue.js 3 的 AI 工具导航网站，灵感来自 ai-bot.cn。

## 功能特性

- ✨ **分类导航**：左侧边栏展示不同类型的 AI 工具分类
- 🔍 **实时搜索**：支持按工具名称和描述快速搜索
- 📱 **响应式设计**：完美适配桌面、平板和手机
- 🎨 **现代界面**：采用渐变色主题，卡片式布局
- ⚡ **轻量快速**：使用 Vue 3 CDN，无需构建工具
- 🎯 **简单易用**：点击分类筛选，点击卡片跳转

## 项目结构

```
ToolWeb/
├── index.html      # 主页面
├── css/
│   └── style.css   # 样式文件
├── js/
│   └── data.json   # 工具数据
└── README.md       # 项目说明
```

## 如何使用

### 1. 直接打开

直接在浏览器中打开 `index.html` 文件即可使用。

### 2. 使用本地服务器（推荐）

由于浏览器的 CORS 策略，建议使用本地服务器运行：

**使用 Python：**
```bash
# Python 3
python -m http.server 8811

# Python 2
python -m SimpleHTTPServer 8000
```

**使用 Node.js：**
```bash
npx http-server
```

然后在浏览器访问 `http://localhost:8811`

## 如何添加新工具

编辑 `js/data.json` 文件，在 `tools` 数组中添加新的工具：

```json
{
  "id": 11,
  "name": "工具名称",
  "description": "工具描述",
  "url": "https://example.com",
  "categoryId": "chatgpt",
  "icon": "https://example.com/icon.png"
}
```

## 如何添加新分类

编辑 `js/data.json` 文件，在 `categories` 数组中添加新的分类：

```json
{
  "id": "new-category",
  "name": "新分类",
  "icon": "🆕"
}
```

## 技术栈

- **Vue.js 3**：渐进式 JavaScript 框架
- **CSS3**：使用 Flexbox 和 Grid 布局
- **原生 JavaScript**：ES6+ 语法

## 浏览器支持

- Chrome (推荐)
- Firefox
- Safari
- Edge

## 自定义样式

编辑 `css/style.css` 文件可以自定义网站样式：

- 修改颜色主题
- 调整布局和间距
- 更改字体和图标大小

## 许可证

MIT License

## 贡献

欢迎提交 Issue 和 Pull Request！
