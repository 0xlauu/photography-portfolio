<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->

<a name="readme-top"></a>

<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/JoaoFranco03/photography-portfolio">
    <img src="dist/assets/Logo.jpg" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Photography Portfolio</h3>

  <p align="center">
    A Website created using Tailwind CSS, HTML, CSS <br /> and JavaScript that can be used as a Photography Portfolio.
    <br />
    <br />
    <a href="https://photography-portfolio-joaofranco03.netlify.app/">View Demo</a>
    <br />
    <br />
    
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li>
      <a href="#built-with">Built With</a>
      <ul>
        <li><a href="#html-badge">HTML</a></li>
        <li><a href="#css-badge">CSS</a></li>
        <li><a href="#js-badge">JavaScript</a></li>
        <li><a href="#tailwind-badge">Tailwind CSS</a></li>
      </ul>
    </li>
    <li><a href="#quick-start">Quick Start</a></li>
    <li><a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

# 📋 About The Project <a name="about-the-project"></a>

[![Product Name Screen Shot][product-screenshot]](https://github.com/JoaoFranco03/photography-portfolio)

This project is a web-based portfolio that beautifully showcases the photography work of Sophia Williams, a fictional photographer. The portfolio was skillfully built using a combination of powerful front-end technologies, including Tailwind CSS, CSS, HTML, and JavaScript.

# MagicSea 摄影作品集

一个优雅的响应式摄影作品集网站，专为摄影师和摄影爱好者打造。

## ✨ 功能特色

### 🖼️ 照片展示
- **瀑布流布局** - 自动适应不同尺寸的照片
- **响应式设计** - 完美适配桌面端和移动端
- **优雅灯箱** - 左右分区设计，文字与图片完美结合
- **键盘导航** - 支持方向键切换和ESC关闭

### 📸 照片管理
- **拖拽上传** - 支持拖拽文件或点击选择
- **智能压缩** - 自动压缩图片，节省存储空间
- **信息编辑** - 可添加标题、地点和描述信息
- **本地存储** - 使用localStorage保存用户照片

### 🎨 用户体验
- **现代UI** - 采用Inter和Playfair字体的优雅设计
- **微动画** - 照片渐入效果和悬停动画
- **管理模式** - 便捷的照片删除和管理功能
- **存储监控** - 实时显示存储使用情况

## 🚀 快速开始

1. **克隆项目**
   ```bash
   git clone https://github.com/yourusername/photography-portfolio.git
   cd photography-portfolio
   ```

2. **启动本地服务器**
   ```bash
   # 使用Python
   python3 -m http.server 8000
   
   # 或使用Node.js
   npx serve .
   ```

3. **访问网站**
   打开浏览器访问 `http://localhost:8000`

## 📱 使用说明

### 上传照片
1. 点击左侧边栏的"+ 上传照片"按钮
2. 拖拽照片到上传区域或点击选择文件
3. 填写照片标题和拍摄地点（必填）
4. 可选填写照片描述
5. 点击"上传照片"完成

### 查看照片
- 点击任意照片进入灯箱模式
- 使用左右区域或方向键切换照片
- 按ESC键退出灯箱

### 管理照片
1. 点击左侧边栏的"管理照片"按钮
2. 悬停在照片上会显示删除按钮
3. 点击"清理存储"可删除所有用户照片

## 🛠️ 技术栈

- **前端框架**: 原生HTML5 + CSS3 + JavaScript
- **样式框架**: Tailwind CSS
- **字体**: Inter + Playfair Display
- **存储**: localStorage
- **图片处理**: Canvas API压缩

## 📐 项目结构

```
photography-portfolio/
├── index.html          # 主页面
├── src/
│   └── input.css      # 源样式文件
├── dist/              # 构建文件
├── photos/            # 照片目录（可选）
├── README.md          # 项目说明
└── .gitignore        # Git忽略文件
```

## 🎯 特性详解

### 响应式瀑布流
- 桌面端：4列自适应布局
- 平板端：3列布局
- 移动端：2列布局
- 自动计算照片间距和尺寸

### 智能图片压缩
- 自动将图片压缩到1200px宽度
- 保持80%的图片质量
- 大幅减少存储空间占用
- 支持JPEG、PNG、GIF格式

### 优雅的灯箱设计
- 左侧文字信息，右对齐设计
- 右侧照片展示，自适应尺寸
- 全区域导航，左右50%区域切换
- 微妙的毛玻璃效果和动画

## 🔧 自定义配置

### 修改压缩设置
在`index.html`中找到`compressImage`函数：
```javascript
const compressedDataUrl = await compressImage(file, 1200, 0.8);
// 参数说明：文件、最大宽度、质量(0-1)
```

### 修改瀑布流列数
在CSS中修改`masonry`类的`column-count`属性

### 更改字体
在HTML头部的Google Fonts链接中替换字体URL

## 📄 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 🤝 贡献

欢迎提交Issue和Pull Request来改进这个项目！

## 📧 联系

- 项目链接: [https://github.com/yourusername/photography-portfolio](https://github.com/yourusername/photography-portfolio)
- 作者网站: [0xlau.com](https://0xlau.com)

---

⭐ 如果这个项目对您有帮助，请给它一个星标！

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🛠️ Built With <a name="built-with"></a>

- [![HTML][html-badge]][html-url]
- [![CSS][css-badge]][css-url]
- [![JavaScript][js-badge]][js-url]
- [![Tailwind][tailwind-badge]][tailwind-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🚀 Quick Start <a name="quick-start"></a>

Create your own page with one click on [Netlify](https://app.netlify.com/signup):

[<img src="https://www.netlify.com/img/deploy/button.svg" alt="Deploy to Netlify" />](https://app.netlify.com/start/deploy?repository=https://github.com/JoaoFranco03/photography-portfolio)
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🎯 Getting Started <a name="getting-started"></a>

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### 🏗️ Installation <a name="installation"></a>

1. Clone the repo

```sh
 git clone https://github.com/JoaoFranco03/photography-portfolio/.git
```

2.  Run the following command:

```sh
 npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```
3.  Run the Project in a Server

4.  Change it with your own photos, about me and contact info.

5.  Publish it using your preferred hosting platform.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- Ko-fi -->

## ☕ Support Me on Ko-fi

If you find this project useful, consider supporting me on Ko-fi. Thanks for checking it out!  

<a href="https://ko-fi.com/joaofranco03" target="_blank">
    <img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="Support me on Ko-fi" style="height:40px;">
</a>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->

## 📜 License <a name="license"></a>

Distributed under the GPL-3.0 License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->

## 📧 Contact <a name="contact"></a>

João Franco - https://www.linkedin.com/in/joão-franco-452161195/

Project Link: [https://github.com/JoaoFranco03/photography-portfolio/](https://github.com/JoaoFranco03/photography-portfolio/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->

## 🌟 Acknowledgments <a name="acknowledgments"></a>

- [FancyBox](https://fancyapps.com/fancybox/)
- [Unsplash](https://unsplash.com/)
- [Tailwind Documentation](https://tailwindcss.com/docs/installation)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[tailwind-badge]: https://img.shields.io/badge/Tailwind_CSS-62BAF3?style=for-the-badge&logo=tailwind-css&logoColor=white
[tailwind-url]: https://tailwindcss.com
[html-badge]: https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=white
[html-url]: https://developer.mozilla.org/en-US/docs/Web/HTML
[css-badge]: https://img.shields.io/badge/CSS-239120?&style=for-the-badge&logo=css3&logoColor=white
[css-url]: https://developer.mozilla.org/en-US/docs/Web/CSS
[js-badge]: https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black
[js-url]: https://developer.mozilla.org/en-US/docs/Web/JavaScript
[license-url]: https://github.com/JoaoFranco03/photography-portfolio/blob/main/LICENSE.md
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/joão-franco-452161195/
[product-screenshot]: dist/assets/mockup.png
