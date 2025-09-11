# Resume Police 🕵️‍♂️

A professional resume review tool that helps job seekers optimize their resume content and enhance their job competitiveness.

[中文版本 (README.md)](./README.md)

---

# Effect Display

[Effect Display of DJJ's Resume Review](./examples/backend_EN.md)

---

## ✨ Features

- 🔍 **Professional Resume Review** - Rigorously examine every detail in resumes like code review
- 💡 **Personalized Advice** - Provide specific and actionable modification suggestions and career guidance
- 🎯 **Job Matching Analysis** - Targeted evaluation based on target job descriptions
- 🚀 **Multi-language Support** - Support for both Chinese and English resume reviews

---

## 📋 Prompts

We offer several versions of prompts to suit different scenarios.

| Type | Language | Description / Difference | File Link |
| :--- | :--- | :--- | :--- |
| Resume Review | 🇺🇸 English | **Resume Police**: The core prompt for comprehensively reviewing and revising resumes, using the "Critique-Analysis-Suggestion" model. | [`resume_police_EN.md`](./prompt/resume_police_EN.md) |
| Interview Question Generation | 🇺🇸 English | **Interviewer's Perspective V1**: Legendary CTO persona, uses a 4-step reconnaissance and P.O.S.E.R. model to generate systematic, in-depth interview questions with traps. | [`qeustion_v1_EN.md`](./prompt/qeustion_v1_EN.md) |
| Interview Question Generation | 🇺🇸 English | **Interviewer's Perspective V2**: Legendary CTO persona, uses a 3-step reconnaissance for a more direct style, producing a more concise list of interview questions. | [`qeustion_v2_EN.md`](./prompt/qeustion_v2_EN.md) |

---

## 🔧 Dify Workflows & Usage

To facilitate use on the Dify platform, we provide the following workflow files.

| Version | Key Features | File Link |
| :--- | :--- | :--- |
| Resume Police | Early version, basic workflow. | [`简历警察.yml`](./workflow/简历警察.yml) |
| Resume Police V2 | Version with optimized prompts and flow. | [`简历警察V2.yml`](./workflow/简历警察V2.yml) |
| Resume Police V3 | **(Recommended)** The most stable text generation workflow, with the latest Resume Police prompt built-in. | [`简历警察V3.yml`](./workflow/简历警察V3.yml) |
| Resume Police Chat | **(Recommended)** Conversational workflow, supports multi-turn dialogue for follow-up questions and revisions. | [`简历警察Chat.yml`](./workflow/简历警察Chat.yml) |
| Resume Police (Transcript Ver) V1 | Corresponds to **Interviewer's Perspective V1** prompt for generating in-depth interview questions. | [`简历警察(笔录版)V1.yml`](./workflow/简历警察(笔录版)V1.yml) |
| Resume Police (Transcript Ver) V2 | Corresponds to **Interviewer's Perspective V2** prompt for generating a concise list of interview questions. | [`简历警察(笔录版)V2.yml`](./workflow/简历警察(笔录版)V2.yml) |
|大厂产研简历优化教练-C-Level|The original prompt words are broken down into 4 steps, each of which is completed independently by a model to output the review results.|[`大厂产研简历优化教练-C-Level.yml`](./workflow/大厂产研简历优化教练-C-Level.yml)|

### Usage

#### Method 1: Import Workflow File
1. Download the workflow file you need (e.g., [`简历警察V3.yml`](./workflow/简历警察V3.yml) / [`简历警察Chat`](./workflow/简历警察Chat.yml))
2. Go to your Dify application platform
3. Click to import the DSL file

![Click Load DSL](./assets/click_load_dsl.png)

#### Method 2: Drag & Drop Import
1. Go to the Dify application page
2. Directly drag and drop the workflow file onto the page

![App Page](./assets/dify_app_page.png)
![Drop File](./assets/drop_file.png)

---
## Model Selection and API Key Configuration
### Model Selection
<img width="2560" height="1229" alt="image" src="https://github.com/user-attachments/assets/9111bd38-3614-485e-8087-5b3bf065a49b" />

### API Key Configuration
Example with Gemini
<img width="2560" height="1230" alt="image" src="https://github.com/user-attachments/assets/21b84f11-0797-4fc4-bb26-5319373b6f3b" />
<img width="2560" height="1229" alt="image" src="https://github.com/user-attachments/assets/f2f3f9cd-1016-43cc-9342-3b3cbc36182d" />
<img width="2560" height="1229" alt="image" src="https://github.com/user-attachments/assets/eeb97cd3-79b5-4589-9f34-870e81e92980" />
<img width="2560" height="1230" alt="image" src="https://github.com/user-attachments/assets/6ebc1538-e485-4ff2-940f-5a0ebe88c6e4" />
[Get Google API Key](https://aistudio.google.com/apikey)
<img width="2560" height="1229" alt="image" src="https://github.com/user-attachments/assets/99d906dd-ab8f-41a2-98e9-8625ddbc4a79" />
<img width="2560" height="1230" alt="image" src="https://github.com/user-attachments/assets/5eb31ed8-2344-44f9-9a99-b069da3e41c1" />
After configuration, it will look like this:
<img width="2560" height="1230" alt="image" src="https://github.com/user-attachments/assets/151b088e-9968-4618-99ef-91133d8cd4d3" />

---

## 🎯 Core Philosophy

The Resume Police uses the "Critique-Analysis-Suggestion" Trinity Model:

- ❓ **Critique** - Directly identify issues
- 🤔 **Analysis** - Explain negative impacts
- 💡 **Suggestion** - Provide specific solutions
