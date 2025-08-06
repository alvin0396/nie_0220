# 只给小frennie的游戏☆☆

一个特别为小frennie制作的互动游戏网站。

## 功能特色

### 第一部分 - 开场
- 淡粉红色渐变背景配白色波纹
- 闪烁的黄金星星效果
- 浮动泡泡动画
- 优雅的开始按钮

### 第二部分 - 问答游戏
- 12个精心设计的问题
- 3种日系动漫风景背景（天空、日出、乡村）
- 简洁的选择界面（"嗯" / "不是"）
- 进度显示

### 第三部分 - 结尾信息
- 滚动式文字展示
- 个人照片背景（需要替换）
- 月亮和星星动画效果
- 最终祝福信息

## 使用说明

### 1. 音乐文件准备
由于浏览器无法直接播放YouTube链接，你需要：

1. 下载以下YouTube视频的音频：
   - 开场音乐：https://www.youtube.com/watch?v=aqGhPk73tkU
   - 游戏音乐：https://www.youtube.com/watch?v=H5ohDQ-umHM  
   - 结尾音乐：https://www.youtube.com/watch?v=9IP2S9aSWfI

2. 将音频转换为MP3格式，重命名为：
   - `intro-music.mp3`
   - `quiz-music.mp3`
   - `ending-music.mp3`

3. 在index.html中找到这些行并替换：
```html
<source src="https://www.youtube.com/watch?v=aqGhPk73tkU" type="audio/mpeg">
```
替换为：
```html
<source src="intro-music.mp3" type="audio/mpeg">
```

对其他两个音频文件做同样的操作。

### 2. 背景照片设置
在index.html中找到这一行：
```javascript
document.getElementById('endingBg').style.backgroundImage = 'url("data:image/svg+xml,<svg xmlns=\\"http://www.w3.org/2000/svg\\" viewBox=\\"0 0 800 600\\"><rect width=\\"800\\" height=\\"600\\" fill=\\"%23FFB6C1\\"/><text x=\\"400\\" y=\\"300\\" text-anchor=\\"middle\\" font-size=\\"24\\" fill=\\"white\\">Your Photo Here</text></svg>")';
```

替换为：
```javascript
document.getElementById('endingBg').style.backgroundImage = 'url("your-photo.jpg")';
```

将你的照片命名为`your-photo.jpg`并放在与index.html同一文件夹中。

### 3. 上传到网站
你需要以下文件：
- `index.html` (主文件)
- `intro-music.mp3` (开场音乐)
- `quiz-music.mp3` (游戏音乐)  
- `ending-music.mp3` (结尾音乐)
- `your-photo.jpg` (背景照片)

将这些文件上传到你的网站主机，然后通过 Alv_Nie.com 访问。

### 4. 测试
确保所有功能正常工作：
- 开场动画和音乐
- 问题导航
- 背景图片切换
- 结尾滚动文字
- 最终星星和月亮动画

## 技术特性
- 响应式设计，支持手机和桌面
- 平滑的场景切换动画
- 优雅的视觉效果
- 中文字体优化
- 无需额外框架，纯HTML/CSS/JavaScript

## 自定义选项
你可以轻松修改：
- 问题内容（在JavaScript的questions数组中）
- 结尾信息（在endingMessage变量中）
- 颜色主题（在CSS中）
- 动画时间（在CSS动画中）

享受这个特别的游戏！💕