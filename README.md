# 简单 AI 聊天

一个基于原生 JavaScript 和 HTML/CSS 构建的轻量级网页 AI 聊天界面。

## 功能特性

- **实时流式传输**: 带有输入指示器的实时流式响应
- **Markdown 支持**: 为丰富文本对话提供完整的 markdown 渲染
- **队列管理**: 处理多条消息并提供可视化队列指示器
- **响应式设计**: 针对桌面和移动设备进行优化
- **性能优化**: 节流更新和平滑滚动
- **会话管理**: 自动会话处理和恢复

## 技术栈

- **前端**: 原生 HTML, CSS, JavaScript
- **AI 服务**: LiteAgent SDK
- **Markdown**: Marked.js 用于内容渲染
- **样式**: CSS3 渐变主题和动画

## 快速开始

1. 克隆仓库
2. 在浏览器中打开 `index.html`
3. 在 JavaScript 部分配置您的 API 密钥
4. 开始聊天！

## 配置

在脚本部分更新 API 配置：

```javascript
const client = new LiteAgent.LiteAgentClient({
    apiKey: 'your-api-key-here',
    baseUrl: 'https://www.liteagent.cn/liteAgent/v1'
});
```

## 文件结构

```
├── chat_app.html          # 主应用程序文件
└── README.md             # 项目文档
```

## 功能详情

### 消息队列系统
- 处理多条快速消息
- 可视化队列指示器
- 带延迟的顺序处理

### 性能优化
- 节流 DOM 更新（约60fps）
- 防抖滚动事件
- GPU 加速动画
- 移动端触摸事件优化

### UI/UX
- 渐变主题界面
- 平滑动画和过渡效果
- 自动调整大小的输入框
- 智能滚动行为

## 浏览器支持

- 支持 ES6+ 的现代浏览器
- 移动浏览器（iOS Safari, Chrome Mobile）
- 桌面浏览器（Chrome, Firefox, Safari, Edge）

## 许可证

MIT 许可证