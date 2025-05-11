# 高中题库管理系统

一个完整的高中题库管理平台，帮助学生有效学习和复习高中知识点。

## 功能特点

- **多种题型支持**：单选题、多选题、填空题和简答题
- **个性化推荐**：基于学习情况智能推荐题目
- **错题本管理**：自动记录错题，支持间隔复习
- **学习进度跟踪**：可视化展示学习进度和薄弱环节
- **讨论社区**：学生可以对题目进行讨论和交流

## 技术栈

### 前端
- React 18
- TypeScript
- Material UI
- Redux Toolkit
- React Router
- Axios
- Chart.js

### 后端
- Node.js
- Express
- TypeScript
- MongoDB
- JWT认证
- RESTful API

## 快速开始

### 后端设置
```bash
cd backend
npm install
# 创建.env文件并配置
npm run dev
```

### 前端设置
```bash
cd frontend
npm install
npm start
```

## 环境变量配置

在`backend`目录下创建`.env`文件，参考`.env.example`配置：

```
NODE_ENV=development
PORT=5000
MONGO_URI=mongodb://localhost:27017/high-school-question-bank
JWT_SECRET=your_jwt_secret
JWT_EXPIRE=30d
JWT_COOKIE_EXPIRE=30
```

## 项目结构

```
high-school-question-bank/
├── backend/              # 后端代码
│   ├── src/
│   │   ├── config/       # 配置文件
│   │   ├── controllers/  # 控制器
│   │   ├── middleware/   # 中间件
│   │   ├── models/       # 数据模型
│   │   ├── routes/       # 路由
│   │   ├── services/     # 服务
│   │   ├── types/        # 类型定义
│   │   ├── utils/        # 工具函数
│   │   └── index.ts      # 入口文件
│   └── package.json
│
├── frontend/             # 前端代码
│   ├── public/
│   ├── src/
│   │   ├── app/          # Redux配置
│   │   ├── components/   # 可复用组件
│   │   ├── features/     # 功能模块
│   │   ├── hooks/        # 自定义钩子
│   │   ├── pages/        # 页面组件
│   │   ├── services/     # API服务
│   │   ├── types/        # 类型定义
│   │   └── App.tsx       # 主应用组件
│   └── package.json
│
└── README.md
```