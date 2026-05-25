# AI Chat Studio · 多模型中枢

> 多模型 AI 对话平台 — 统一调度、Key 轮转、Token 仪表盘、技能库

一个功能完整的单页 AI 聊天应用，支持多种大模型 API 的统一调度与管理。无需后端服务，纯前端运行，开箱即用。

---

## 特性

### 多模型支持
统一接入多个大模型 API，在一个界面中切换使用：

- 兼容 OpenAI 协议的所有模型
- 多 Key 自动轮转，提高可用性
- 各模型用量独立统计

### API Key 轮转池
- 为每个模型添加多个 API Key
- 自动按顺序轮转，单 Key 耗尽自动切换下一个
- 实时显示各 Key 的剩余配额和状态

### Token 仪表盘
- 各模型用量实时监控
- 配额消耗进度可视化
- 自动估算剩余可用量

### 智能体技能库
- 自定义智能体名称、头像、系统提示词
- 保存多个预设技能模板
- 快速切换不同角色设定

### 多主题
- **深空黑** — 默认暗色主题
- **星辰大海** — 蓝色海洋风格
- **暖阳橙光** — 暖色调主题
- **翡翠森林** — 绿色自然风格

### 其他功能
- 多会话管理，自由切换对话
- 消息撤回与重新生成
- 支持上传 .docx 文件并解析内容
- 对话历史自动保存（localStorage）
- 全屏模式
- 完全离线可用（无后端依赖）

---

## 快速开始

### 方式一：直接使用

打开 [GitHub Pages](https://shanguier.github.io/ai-chat-studio/) 即可使用。

### 方式二：本地运行

```bash
git clone https://github.com/Shanguier/ai-chat-studio.git
cd ai-chat-studio
# 直接用浏览器打开 index.html
# 或者用任意 HTTP 服务器托管
python3 -m http.server 8080
# 访问 http://localhost:8080
```

### 配置 API Key

1. 点击侧边栏底部的「API Key 池」
2. 选择模型提供商
3. 输入你的 API Key
4. 点击添加即可开始对话

---

## 技术栈

- **纯 HTML/CSS/JS** — 无框架依赖，单页应用
- **localStorage** — 数据持久化，无需后端
- **Mammoth.js** — .docx 文件解析
- **CSS 变量** — 多主题切换
- **响应式设计** — 适配桌面端与移动端

---

## 项目结构

```
ai-chat-studio/
├── index.html          # 完整应用（约 4000 行）
├── .gitignore
└── README.md
```

整个应用封装在单个 HTML 文件中，无需构建、无需安装依赖。

---

## License

MIT
