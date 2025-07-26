# Resume Police 🕵️‍♂️

A professional resume review tool that helps job seekers optimize their resume content and enhance their job competitiveness.

---

## ✨ Features

- 🔍 **Professional Resume Review** - Rigorously examine every detail in resumes like code review
- 💡 **Personalized Advice** - Provide specific and actionable modification suggestions and career guidance
- 🎯 **Job Matching Analysis** - Targeted evaluation based on target job descriptions
- 🚀 **Multi-language Support** - Support for both Chinese and English resume reviews

---

## 📋 Prompts

We provide carefully designed prompts that you can use directly:

### 🇨🇳 Chinese Version
**[Resume Police Chinese Prompt](./prompt/resume_police_Zh.md)**
- For Chinese resume review
- Complete role definition and evaluation criteria
- Detailed Critique-Analysis-Suggestion model

### 🇺🇸 English Version
**[Resume Police English Prompt](./prompt/resume_police_EN.md)**
- For English resume review
- Complete role definition and evaluation criteria
- Detailed Critique-Analysis-Suggestion Trinity Model

---

## 🔧 Usage

### Method 1: Import Workflow File
1. Download the [`简历警察V3.yml`](./workflow/简历警察V3.yml) workflow file
2. Enter your Dify application platform
3. Click to import DSL file

![Click Load DSL](./assets/click_load_dsl.png)

### Method 2: Drag & Drop Import
1. Enter Dify application page
2. Directly drag and drop the workflow file to the page

![App Page](./assets/dify_app_page.png)
![Drop File](./assets/drop_file.png)

---

## 📁 Project Structure

```
resumePolice/
├── prompt/                    # Prompt files
│   ├── resume_police_Zh.md   # Chinese prompt
│   └── resume_police_EN.md   # English prompt
├── workflow/                  # Workflow files
│   └── 简历警察V3.yml        # Dify workflow config
├── assets/                    # Operation images
│   ├── dify_app_page.png     # App page screenshot
│   ├── click_load_dsl.png    # Click load DSL screenshot
│   └── drop_file.png         # Drop file screenshot
├── README.md                  # Project documentation (Chinese)
└── README_EN.md              # Project documentation (English)
```

---

## 🎯 Core Philosophy

The Resume Police uses the "Critique-Analysis-Suggestion" Trinity Model:

- ❓ **Critique** - Directly identify issues
- 🤔 **Analysis** - Explain negative impacts
- 💡 **Suggestion** - Provide specific solutions