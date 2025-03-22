# 沉浸式数字相框

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![ff4f990c7aeafa6967396dbe75300f1.png](https://bu.dusays.com/2025/03/22/67deb759b8438.png)<br>
基于现代 Web 技术实现的沉浸式图片展示方案，具有优雅的过渡动画和交互设计。
## 查看效果
Previvew in [https://love.xuanbo.top/](https://love.xuanbo.top/)
## 功能特性

✨ **核心亮点**
- 渐进式加载体验（带加载动画）
- 智能图片预加载机制
- 流畅的 CSS 过渡动画（淡入淡出 + 缩放效果）
- 响应式布局支持（移动端/桌面端自适应）
- 动态标题与说明文字联动
- 右键下载功能（支持触屏长按操作）
- 开发者友好型代码结构

🎨 **设计理念**
- 极简主义视觉风格
- 精确到毫秒级的动画时序控制
- 高性能渲染优化（使用 `will-change` 属性）
- 无障碍交互设计（禁用文本选择/点击高亮）

## 快速使用

### 基础部署
1. 替换 `images` 数组中的图片地址

```javascript
const images = [
  { url: 'your-image-1.jpg', caption: '这里是图片说明1' },
  { url: 'your-image-2.jpg', caption: '这里是图片说明2' }
];
```
备注:图片说明将显示在主标题下方


2. 自定义显示内容

```html
<div class="text">这里是主标题</div> <!-- 主标题 -->
<div class="tip-text">点击屏幕切换图片<br>长按或右键下载此图片</div>
```

### 高级定制
- 修改 `style.css` 中的动画参数：

```css
.transition {
  /* 调整 cubic-bezier 曲线改变动画节奏 */
  transition: opacity 0.6s cubic-bezier(0.4, 0, 0.2, 1);
}
```

- 扩展右键菜单功能：

```javascript
const newMenuItem = document.createElement('div');
newMenuItem.className = 'context-menu-item';
newMenuItem.textContent = '新功能';
contextMenu.appendChild(newMenuItem);
```

## 署名协议 (Attribution License)

本作品采用 **知识共享-署名协议**，您需要遵守以下条款：

### 您可以自由地：
- **共享**：在任何媒介以任何形式复制、发行本作品
- **演绎**：修改、转换或以本作品为基础进行创作

### 惟须遵守以下条件：
- **署名**：您必须给出适当的署名，提供指向本许可协议的链接，同时标明是否对原始作品作了修改。您可以用任何合理的方式来署名，但不得以任何方式暗示许可人为您或您的使用背书
- **无附加限制**：您不得增设法律条款或技术措施，来限制他人执行本许可允许的操作

## 技术栈
- 现代 CSS3 动画
- Vanilla JavaScript (ES6+)
- 渐进增强设计模式
- 模块化代码结构

## 浏览器支持

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24">](https://www.google.com/chrome/) | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24">](https://www.mozilla.org/firefox/) | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24">](https://www.apple.com/safari/) |
|:---:|:---:|:---:|
| 最新版 ✔ | 最新版 ✔ | 14.1+ ✔ |
