# 芯宠工场 AI玩具伙伴 - 部署指南

## 项目简介
这是一个可爱儿童版治愈系AI陪伴应用的高保真原型展示，包含8个精美的移动端界面。

## 部署方式

### 方式1: GitHub Pages (推荐)
1. 将项目上传到GitHub仓库
2. 在仓库设置中启用GitHub Pages
3. 选择部署分支（通常是main或gh-pages）
4. 访问 `https://yourusername.github.io/repository-name`

### 方式2: Vercel
1. 访问 [vercel.com](https://vercel.com)
2. 连接GitHub账号
3. 导入项目仓库
4. 自动部署完成

### 方式3: 本地服务器
```bash
# 使用Python启动本地服务器
python -m http.server 8000

# 或使用Node.js
npx serve .

# 访问 http://localhost:8000
```

### 方式4: Firebase Hosting
```bash
# 安装Firebase CLI
npm install -g firebase-tools

# 登录Firebase
firebase login

# 初始化项目
firebase init hosting

# 部署
firebase deploy
```

### 方式5: Surge.sh
```bash
# 安装Surge
npm install -g surge

# 部署
surge .
```

## 项目结构
```
/
├── index.html              # 主页面 - 所有界面展示
├── home.html              # 连接设备页
├── device-scan.html       # 设备扫描页
├── network.html           # 连接网络页
├── wifi-password.html     # 网络密码输入页
├── character-selection.html # 角色选择页
├── character.html         # 角色配置页
├── chat.html             # 角色聊天界面
├── settings.html         # 设备设置页
└── share.html            # 分享设备页
```

## 特性
- 📱 完美的iPhone界面模拟
- 🎨 精美的渐变色彩设计
- ✨ 流畅的动画效果
- 🌈 可爱的儿童友好界面
- 📐 响应式设计适配
- 🔄 可滑动的角色选择栏

## 角色介绍
- 🌸 **爱瑞丝** - 温柔的AI伙伴，擅长讲故事和情感陪伴
- 🎊 **四喜财神** - 传统文化知识丰富，带来好运和快乐
- 🥚 **蛋仔派对** - 活泼好动，喜欢游戏和冒险

## 技术栈
- HTML5
- CSS3 (Flexbox, Grid, Animations)
- JavaScript (ES6+)
- Font Awesome Icons
- Google Fonts

## 浏览器支持
- Chrome 60+
- Firefox 60+
- Safari 12+
- Edge 79+

## 开发说明
所有页面都是独立的HTML文件，可以直接在浏览器中打开预览。主页面(index.html)通过iframe展示所有子页面。