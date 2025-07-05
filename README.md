# MagicSea Photography Portfolio

一个极简优雅的摄影作品集网站，专注于展示摄影作品的纯净之美。

## 🌟 特色功能

- **极简设计**：米白色主题，优雅简洁
- **响应式布局**：完美适配桌面、平板、手机
- **瀑布流展示**：自适应的照片网格布局
- **灯箱查看**：优雅的大图浏览体验
- **快速加载**：优化的图片加载和显示

## 🎯 网站结构

- `index.html` - 公开展示页面
- `admin.html` - 后台管理页面（本地使用）

## 🚀 快速开始

### 在线访问
直接访问 GitHub Pages 部署的网站：
```
https://yourusername.github.io/photography-portfolio/
```

### 本地开发
1. 克隆仓库：
```bash
git clone https://github.com/yourusername/photography-portfolio.git
cd photography-portfolio
```

2. 启动本地服务器：
```bash
python3 -m http.server 8000
```

3. 访问网站：
- 主页：`http://localhost:8000`
- 管理后台：`http://localhost:8000/admin.html`

## 📝 使用说明

### 展示页面 (index.html)
- 纯净的作品展示界面
- 支持灯箱查看
- 响应式设计
- 适合公开访问

### 管理后台 (admin.html)
- 上传新照片
- 管理现有照片
- 数据导出/导入
- 存储统计信息

> **注意**: 管理后台仅供本地使用，不会部署到线上

## 🔧 技术栈

- **前端**: HTML5, CSS3, JavaScript
- **样式**: Tailwind CSS
- **字体**: Inter + Playfair Display
- **存储**: localStorage
- **部署**: GitHub Pages

## 📱 兼容性

- ✅ Chrome 70+
- ✅ Firefox 70+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ 移动端浏览器

## 🎨 定制化

### 修改主题色
在 `index.html` 中找到 CSS 变量：
```css
body {
  background-color: #faf9f7; /* 主背景色 */
  color: #2d3748;            /* 文字颜色 */
}
```

### 修改布局
调整瀑布流列数：
```css
.masonry {
  column-count: 4; /* 桌面端列数 */
}
```

### 添加照片
在管理后台 (`admin.html`) 中：
1. 点击"上传新照片"
2. 选择图片文件
3. 填写照片信息
4. 保存即可

## 📄 许可证

MIT License

## 🔗 链接

- [在线预览](https://yourusername.github.io/photography-portfolio/)
- [GitHub仓库](https://github.com/yourusername/photography-portfolio)

---

**让您的摄影作品以最优雅的方式呈现** ✨ 