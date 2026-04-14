# 🤖 QA AI Agents Collection

> A curated collection of powerful, open-source LangFlow agents designed to supercharge QA Engineers and Software Testers. Built with [LangFlow](https://www.langflow.org/) and powered by lightning-fast [Groq](https://groq.com/) LLMs.

---

## 🌟 Beginner's Guide: What is this?
If you're new to AI agents or LangFlow, don't worry! This repository contains pre-configured "brains" (JSON files) that you can drag and drop into LangFlow. 

Once imported, these agents act like virtual team members:
1. **The Bug Classifier**: You tell it about a bug, and it acts like a 15-year Senior QA Lead to categorize it and assign its severity.
2. **The Test Case Generator**: You give it a feature description (PRD), and it automatically writes a complete suite of test cases (including edge cases and negative scenarios!) and saves them to a Markdown file.

---

## 📦 What's Inside?

### 1️⃣ Agent 1: The Testcase Generator (`AI_Agent_Testcase_Generator.json`)
*(Newest Addition!)*

This agent acts as a Senior QA Automation Engineer. It reads your Product Requirements Document (PRD) and generates a comprehensive test plan containing happy paths, negative scenarios, boundary values, and edge cases.

**✨ Key Features:**
- **Chain of Thought Reasoning:** The AI is instructed to "think" about hidden constraints and edge cases *before* writing the test cases, drastically improving the quality of the tests.
- **Enterprise Formatting:** Outputs a clean, structured table format.
- **Auto-Save:** Automatically saves the generated test cases as a formatted `Test_Cases_Generated.markdown` file straight to your local drive!
- **Model:** Tuned for `llama-3.3-70b-versatile` ensuring deep reasoning capabilities.

**How to use:**
1. Import into LangFlow.
2. Open the Playground.
3. Paste your PRD/Feature description into the chat.
4. Watch it generate and automatically save a Markdown file of your test cases!

---

### 2️⃣ Agent 2: The Bug Classifier (`AI_Agent_Bug_classifier.json`)

The Bug Classifier analyzes raw bug reports submitted by users or testers and returns a structured, professionally triaged classification.

**✨ Key Outputs:**
- **Severity Level:** (CRITICAL / HIGH / MEDIUM / LOW)
- **Category:** (UI/UX, FUNCTIONAL, PERFORMANCE, SECURITY, etc.)
- **Reproduction Confidence:** Identifies if you provided clear steps or if information is missing.
- **Similar Known Issues:** Recognizes common software failure patterns.

---

## 🚀 How to Install & Use (Easy Setup)

Never used LangFlow before? Follow these easy steps:

### Step 1: Get the prerequisites
- Install **LangFlow** (v1.7.2 or higher). You can install it on your machine using Python: `pip install langflow` then run `langflow run`.
- Get a **Free Groq API Key** by signing up at [console.groq.com](https://console.groq.com/).

### Step 2: Import the Agents
1. Download this repository to your computer.
2. Open LangFlow in your web browser (usually at `http://127.0.0.1:7860`).
3. On the main dashboard, click **"Upload Flow"** ⬆️ (or simply drag and drop the `.json` files from this folder directly into the browser window).

### Step 3: Add your API Key
1. Open the imported flow.
2. Find the node labeled **"Groq"**.
3. Click on the `Groq API Key` field and paste your key.

*(Optional but recommended: Save your API key in LangFlow's global environment variables so you don't have to paste it every time!)*

### Step 4: Run the Agent!
1. Click the **Playground** button (usually a chat bubble icon) in the bottom right corner.
2. Type in your prompt (a bug report or a feature description) and hit send!

---

## 🛠️ Modifying the Agents

These agents are highly customizable! You can easily tweak them to fit your specific company needs:
- **Change the Output Format:** Click on the `Groq` node and edit the `System Message` field to change how the agent structures its responses.
- **Swap Models:** In the `Groq` node, you can open the Dropdown under `Model` and select different AI models depending on if you want speed vs. deep reasoning.

---

## 🤝 Contributing

Got an idea for a new QA Agent? Feel free to fork this repo and submit a Pull Request! Some ideas for future agents:
- 📊 Selenium/Cypress Code Generator
- 📎 Jira Issue Auto-creator
- 📉 Root Cause Analysis Agent

---

*Built with ❤️ to make QA engineering faster and smarter.*
