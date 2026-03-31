🎨 花拾-妙笔 (Huashi - Miaobi)

网页版本和手机iOS版本都在里面

智能 AI 绘画鉴赏与教学辅助平台 —— 你的专属“AI 美院教授”

花拾-妙笔 是一款专为美术生和绘画爱好者打造的智能画作测评应用。通过上传大师原画与个人临摹作品，应用将调用先进的视觉大模型（Vision LLM）进行双图对比分析，从构图、色彩、光影等多个专业维度输出结构化的鉴赏报告，提供专业、客观且具有鼓励性的修改建议。

✨ 核心功能 (Core Features)
⚖️ 双图对比测评： 支持同时上传“大师参考图”与“学生临摹图”，进行像素级与语义级的双重比对。

🧑‍🏫 教授级专业点评： 内置精心调优的 Prompt，AI 化身资深美院评委，提供包含综合打分、闪光点表扬、核心问题剖析及针对性修改建议的深度报告。

📊 多维度专业评分： 深度解析构图、色彩与色温、光影过渡、透视与形体、线条等绘画核心要素。

Markdown 流式输出： 沉浸式的流式生成体验（Streaming），报告排版清晰，一目了然。

🗂️ 鉴赏历史记录： 自动在本地保存历史测评数据，随时回顾自己的成长轨迹。

🖥️ 页面架构与用户体验 (Pages & UX)
本项目采用了极简、现代且带有艺术气息的 UI 设计风格：

/ 首页 (Marketing 落地页)

Hero Section: 带有双图对比动态演示的视觉冲击区域。

Features: 多维度分析、一键出报告的卖点展示。

Bento Grids: 现代化的网格化特性展示。

FAQ & CTA: 完善的落地页转化路径，指引用户开启鉴赏之旅。

/evaluate 核心工作台

左右分栏的大面积拖拽上传区，交互直观流畅。

条件触发机制：双图准备就绪后方可发起鉴赏。

优雅的报告渲染区（带阴影与虚线边框设计），完美呈现 Markdown 内容。

/history 鉴赏记录页

网格卡片（Grid）形式展示过往鉴赏历史。

直观展示缩略图拼接、鉴赏时间与综合评分。

🛠️ 技术栈 (Tech Stack)
本项目采用现代化的前端与 AI 技术栈构建：

框架: Next.js (App Router)

样式: TailwindCSS

组件库: Shadcn/UI

AI 赋能: Vercel AI SDK (ai & @ai-sdk/openai)

大模型: 阿里云通义千问视觉大模型 qwen-vl-max (兼容 OpenAI 接口规范)

数据存储: 本地数据库 (Local DB)

🚀 快速开始 (Getting Started)
1. 克隆项目
Bash
git clone https://github.com/你的用户名/huashi-miaobi.git
cd huashi-miaobi
2. 安装依赖
Bash
npm install
# 或者使用 yarn / pnpm
3. 配置环境变量
在项目根目录创建一个 .env 或 .env.local 文件，并填入你的通义千问 API Key。本项目使用兼容 OpenAI 规范的调用方式：

代码段
# 阿里云百炼平台获取的通义千问 API Key
QWEN_API_KEY=your_qwen_api_key_here
4. 运行本地开发环境
Bash
npm run dev
打开浏览器访问 http://localhost:3000 即可体验应用。

🧠 AI 系统提示词设计 (System Prompt Engineering)
本项目的核心竞争力之一在于其背后的业务逻辑与 Prompt 设计。系统被设定为**“资深的美院教授和严格的绘画评委”**，强制大模型以结构化的 Markdown 格式输出：

🏆 综合评分 (百分制及一句话总结)

✨ 闪光点 (至少两点具体表扬)

🔍 核心问题分析 (从具体专业维度拆解3个主要问题)

🛠️ 教授的修改建议 (具体可操作的下一步练习方向)

这种设计既保证了专业深度，又兼顾了教育产品应有的温度与鼓励性。

🤝 贡献与反馈
欢迎提交 Issue 或 Pull Request 来完善这个项目！如果你对 AI 在艺术教育领域的落地有更多想法，也欢迎在 Discussions 中交流。