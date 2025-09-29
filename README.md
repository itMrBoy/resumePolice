# 写在前面

## 我们正在尝试打造一个 **求职者** 与 **招聘方** 之间精准高效的连接通道。
## 基于Github Issue打造的完全透明的求职和招聘平台, 完全透明, 完全公开

- 求职者：如果你认为自己足够优秀，不妨带着你的简历/博客/开源贡献来这里寻找优秀的工作机会。
- 招聘方：如果你认为你的产品/工作岗位拥有动人的产品力，不妨带上你的jd来这里会一会各路英豪。

[**代码, 是最好的简历**](https://github.com/TokenRollAI/talent-hub-cn)

# 简历警察 🕵️‍♂️
**已帮助修改超过500份简历**

[English Version (README_EN.md)](./README_EN.md)

---

# 效果展示

[DJJ的简历审查结果](./examples/backend_ZH.md)

---

## 特别感谢

> AiHubMix为本项目提供了慷慨的调用额度
>
> ![AihubMix](https://www.resource.nestsound.cn/one-api-web/logo.png?v=1)

---

## ChangeLog

2025-08-04 在以之的强迫下, 添加了Chat的Dify workflow: [`简历警察Chat`](./workflow/简历警察Chat.yml)

---

## 📋 提示词 (Prompts)

我们提供了多个版本的提示词，以适应不同场景的需求。

| 类型 | 语言 | 描述 / 区别 | 文件链接 |
| :--- | :--- | :--- | :--- |
| 简历评估 | 🇨🇳 中文 | **简历警察**：核心提示词，用于全面审查和修改简历，采用“批判-解析-建议”模型。 | [`resume_police_Zh.md`](./prompt/resume_police_Zh.md) |
| 面试问题生成 | 🇨🇳 中文 | **面试官视角 V1**: 传奇CTO人设，采用四步勘探法和P.O.S.E.R.模型，生成体系化、带陷阱的深度面试问题。 | [`question_v1_Zh.md`](./prompt/question_v1_Zh.md) |
| 面试问题生成 | 🇨🇳 中文 | **面试官视角 V2**: 传奇CTO人设，采用三步勘探法，风格更直接，产出更精简的面试问题清单。 | [`question_v2_Zh.md`](./prompt/question_v2_Zh.md) |

---

## 🔧 Dify 工作流 (Workflows) 与使用方法

为了方便在 Dify 平台使用，我们提供了以下工作流文件。

| 版本 | 主要特点 | 文件链接 |
| :--- | :--- | :--- |
| 简历警察 | 早期版本，基础工作流。 | [`简历警察.yml`](./workflow/简历警察.yml) |
| 简历警察 V2 | 优化了提示词和流程的版本。 | [`简历警察V2.yml`](./workflow/简历警察V2.yml) |
| 简历警察 V3 | **（推荐）** 当前最稳定的文本生成工作流，内置了最新的简历警察提示词。 | [`简历警察V3.yml`](./workflow/简历警察V3.yml) |
| 简历警察 Chat | **（推荐）** 对话式工作流，支持与简历警察进行多轮对话，进行追问和修改。 | [`简历警察Chat.yml`](./workflow/简历警察Chat.yml) |
| 简历警察(笔录版)V1 | 对应 **面试官视角 V1** 提示词，用于生成深度面试问题的文本生成工作流。 | [`简历警察(笔录版)V1.yml`](./workflow/简历警察(笔录版)V1.yml) |
| 简历警察(笔录版)V2 | 对应 **面试官视角 V2** 提示词，用于生成精简面试问题清单的文本生成工作流。 | [`简历警察(笔录版)V2.yml`](./workflow/简历警察(笔录版)V2.yml) |
|大厂产研简历优化教练-C-Level|将原有提示词拆解成 4 个步骤，每一步由一个模型独立完成，输出审查结果。|[`大厂产研简历优化教练-C-Level.yml`](./workflow/大厂产研简历优化教练-C-Level.yml)|

### 使用方法

#### 方法一：导入工作流文件
1. 下载您需要的工作流文件 (例如 [`简历警察V3.yml`](./workflow/简历警察V3.yml) / [`简历警察Chat`](./workflow/简历警察Chat.yml))
2. 进入您的Dify应用平台
3. 点击导入DSL文件

![点击加载DSL](./assets/click_load_dsl.png)

#### 方法二：拖拽文件导入
1. 进入Dify应用页面
2. 直接拖拽工作流文件到页面中

![应用页面](./assets/dify_app_page.png)
![拖拽文件](./assets/drop_file.png)

---
## 模型的选择及Api key 的配置
### 模型选择
<img width="2560" height="1229" alt="image" src="https://github.com/user-attachments/assets/9111bd38-3614-485e-8087-5b3bf065a49b" />

### Api key 配置
以Gemini为例
<img width="2560" height="1230" alt="image" src="https://github.com/user-attachments/assets/21b84f11-0797-4fc4-bb26-5319373b6f3b" />
<img width="2560" height="1229" alt="image" src="https://github.com/user-attachments/assets/f2f3f9cd-1016-43cc-9342-3b3cbc36182d" />
<img width="2560" height="1229" alt="image" src="https://github.com/user-attachments/assets/eeb97cd3-79b5-4589-9f34-870e81e92980" />
<img width="2560" height="1230" alt="image" src="https://github.com/user-attachments/assets/6ebc1538-e485-4ff2-940f-5a0ebe88c6e4" />
[Google API Key 获取链接](https://aistudio.google.com/apikey)
<img width="2560" height="1229" alt="image" src="https://github.com/user-attachments/assets/99d906dd-ab8f-41a2-98e9-8625ddbc4a79" />
<img width="2560" height="1230" alt="image" src="https://github.com/user-attachments/assets/5eb31ed8-2344-44f9-9a99-b069da3e41c1" />
配置完成后，显示如下
<img width="2560" height="1230" alt="image" src="https://github.com/user-attachments/assets/151b088e-9968-4618-99ef-91133d8cd4d3" />

---

## 🎯 核心理念

简历警察采用"批判-解析-建议"三位一体模型：

- ❓ **批判** - 直接指出问题
- 🤔 **解析** - 解释负面影响
- 💡 **建议** - 提供具体方案

## 联系我们
<img width="1376" height="1933" alt="03e4c20ca40a485a8f315d1e344f0be" src="https://github.com/user-attachments/assets/05afa584-ace4-49ea-94b9-91d682fa2f82" />






