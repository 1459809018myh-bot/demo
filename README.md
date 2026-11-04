# 📚 学习目标管理系统

> 一个现代化的全栈学习目标管理应用，帮助你高效规划和追踪学习进度

[![React](https://img.shields.io/badge/React-18.x-blue.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue.svg)](https://www.typescriptlang.org/)
[![Fastify](https://img.shields.io/badge/Fastify-5.x-green.svg)](https://www.fastify.io/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## ✨ 功能特性

- 🎯 **目标管理** - 创建、编辑和追踪学习目标，支持目标分类和进度追踪
- ✅ **任务管理** - 每日任务计划和完成追踪，支持优先级设置
- ⏰ **番茄钟学习** - 内置番茄钟计时器，记录学习时长和效率
- 📊 **数据分析** - 可视化统计图表，展示学习趋势和成果
- 🌙 **主题切换** - 支持深色/浅色主题，保护视力
- 💾 **数据持久化** - 基于 SQLite 的本地数据存储，安全可靠
- 🤖 **AI 辅助** - 智能学习建议和知识测验（可选功能）

## 🛠️ 技术栈

### 前端
- **框架**: React 18 + TypeScript
- **构建工具**: Vite
- **样式**: TailwindCSS
- **状态管理**: Zustand + TanStack Query
- **路由**: React Router
- **图标**: Lucide React
- **图表**: Recharts
- **日期处理**: Day.js

### 后端
- **框架**: Fastify + TypeScript
- **数据库**: Better-SQLite3
- **验证**: Zod
- **日志**: Pino

## 🚀 快速开始

### 环境要求

- Node.js >= 18.0.0
- npm >= 9.0.0

### 安装步骤

1. **克隆项目**
```bash
git clone <repository-url>
cd one
```

2. **安装依赖**
```bash
npm install
```

3. **配置环境变量**
```bash
cp .env.example .env
```

编辑 `.env` 文件，配置必要的环境变量（如 API 密钥等）

4. **初始化数据库**
```bash
npm run db:migrate
npm run db:seed
```

5. **启动开发服务器**

使用快速启动脚本：
```bash
# Windows
quick-start.bat

# Linux/Mac
./quick-start.sh
```

或者手动启动：
```bash
# 启动后端服务（端口 3000）
npm run dev:server

# 启动前端开发服务器（端口 5173）
npm run dev:client
```

6. **访问应用**

打开浏览器访问 [http://localhost:5173](http://localhost:5173)

## 📁 项目结构

```
one/
├── client-new/           # 前端应用
│   ├── src/
│   │   ├── components/  # React 组件
│   │   ├── pages/       # 页面组件
│   │   ├── lib/         # 工具库和 API 客户端
│   │   └── store/       # 状态管理
│   └── index.html
├── server-new/           # 后端应用
│   ├── db/              # 数据库相关
│   ├── routes/          # API 路由
│   └── services/        # 业务服务
├── shared-new/           # 共享类型定义
├── data/                 # 数据库文件
└── dist/                 # 构建输出
```

## 📖 使用说明

### 创建学习目标

1. 点击侧边栏的「目标」菜单
2. 点击「新建目标」按钮
3. 填写目标标题、描述、分类和目标日期
4. 保存后可在目标列表中查看和管理

### 添加每日任务

1. 进入「任务」页面
2. 点击「添加任务」
3. 设置任务标题、优先级、预计时长等
4. 完成后勾选任务即可标记完成

### 使用番茄钟学习

1. 进入「学习」页面
2. 选择要学习的内容
3. 点击「开始」按钮开启番茄钟
4. 专注学习 25 分钟后休息 5 分钟
5. 系统自动记录学习时长

### 查看数据分析

1. 进入「分析」页面
2. 查看学习时长趋势图
3. 查看任务完成统计
4. 查看目标进度分析

## 🔧 开发指南

### 可用脚本

```bash
# 开发
npm run dev:client      # 启动前端开发服务器
npm run dev:server      # 启动后端开发服务器

# 构建
npm run build          # 构建生产版本
npm run preview        # 预览生产构建

# 数据库
npm run db:migrate     # 运行数据库迁移
npm run db:seed        # 填充示例数据

# 代码质量
npm run type-check     # TypeScript 类型检查
```

### 环境变量说明

在 `.env` 文件中配置以下变量：

```env
# 服务器配置
PORT=3000
HOST=0.0.0.0

# AI 服务（可选）
ANTHROPIC_API_KEY=your_api_key_here

# 数据库
DB_PATH=./data/study-tracker.db
```

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本项目
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 🙏 致谢

- [React](https://reactjs.org/) - 用户界面框架
- [Fastify](https://www.fastify.io/) - 高性能 Web 框架
- [TailwindCSS](https://tailwindcss.com/) - CSS 框架
- [Lucide](https://lucide.dev/) - 图标库

## 📮 联系方式

如有问题或建议，欢迎通过 Issue 联系我们。

---

⭐ 如果这个项目对你有帮助，欢迎给个 Star！
