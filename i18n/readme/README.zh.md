# 🚀 **OpenHealth**

**AI健康助手 | 由您的数据驱动，本地运行**

---

<p align="center">
  <img src="/intro/openhealth.gif" alt="OpenHealth 演示">
</p>

## 🌟 概述

OpenHealth帮助您**掌控健康数据**。通过利用AI和您的个人健康信息，
OpenHealth提供私密且本地运行的助手，帮助您更好地理解和管理健康。

---

## ✨ 项目特点

- 📊 **集中化健康数据输入：** 轻松整合所有健康数据于一处
- 🛠️ **智能解析：** 自动解析您的健康数据并生成结构化数据文件
- 🤝 **上下文对话：** 使用结构化数据作为上下文，与GPT驱动的AI进行个性化交互

---

## 📥 支持的数据源和语言模型

| **可添加的数据源** | **支持的语言模型** |
|-------------------|-------------------|
| 血液检测结果      | LLaMA,DeepSeek-V3  |
| 体检数据          | GPT,Claude,Gemini  |
| 个人体格信息      |                   |
| 家族病史          |                   |
| 症状              |                   |

---

## 🤔 为什么我们建立OpenHealth

- 💡 **您的健康由您负责。**
- ✅ 真正的健康管理结合**您的数据** + **智能**，将洞察转化为可行计划。
- 🧠 AI作为无偏见的工具，有效指导和支持您管理长期健康。

---

## 🗺️ 项目图示

```plaintext
健康数据输入 --> 数据解析模块 --> 结构化数据文件 --> GPT集成
```

> **注意：** 数据解析功能目前在独立的Python服务器中实现，计划未来迁移到TypeScript。

## 开始使用

## ⚙️ 如何运行 OpenHealth

1. **克隆仓库：**
   ```bash
   git clone https://github.com/OpenHealthForAll/open-health.git
   cd open-health
   ```

2. **设置和运行：**
   ```bash
   # 复制环境配置文件
   cp .env.example .env

   # 使用 Docker Compose 启动应用
   docker compose --env-file .env up
   ```

3. **访问 OpenHealth：**
   打开浏览器并访问 `http://localhost:3000` 开始使用 OpenHealth。

> **注意：** 如果您在 Docker 中使用 Ollama，请确保将 Ollama API 端点设置为：`http://docker.for.mac.localhost:11434/`

---

## 🌐 社区与支持

在Reddit上联系我：[我的主页](https://www.reddit.com/user/Dry_Steak30/) 