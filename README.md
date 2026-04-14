# QA AI Agents for Langflow

Open-source Langflow agents built for QA workflows.

This repository contains ready-to-import JSON flows designed to help QA engineers, testers, and SDETs speed up repetitive work such as bug triage and test case generation using LLM-powered agents.

## What’s inside

This repo currently includes two Langflow agents:

- **AI_Agent_Bug_classifier.json**  
  Classifies bug reports into meaningful QA categories such as severity, issue type, and impact.
  <img width="1512" height="833" alt="Screenshot 2026-04-14 at 11 42 20 AM" src="https://github.com/user-attachments/assets/38d54bc9-53dd-4a0d-a83d-32fdea61bf8b" />


- **AI_Agent_Testcase_Generator.json**  
  Generates structured test cases from PRDs, feature descriptions, or requirement summaries.
 <img width="1512" height="833" alt="Screenshot 2026-04-14 at 1 47 15 PM" src="https://github.com/user-attachments/assets/1b06092f-7bc1-4b2f-b1a1-29aaf04c581f" />



## Who this is for

This project is useful for:

- QA Engineers
- SDETs
- Manual Testers exploring AI-assisted workflows
- Teams experimenting with Langflow for QA use cases
- Engineers building internal QA copilots or workflow accelerators

## Why this repo exists

QA teams still spend a lot of time on repeated documentation and triage work:

- reviewing bug descriptions
- assigning severity
- converting requirements into test cases
- maintaining structure across outputs

These tasks are important, but often repetitive.

The goal of this repo is to provide reusable AI agent flows that help make QA work:

- faster
- more structured
- easier to standardize
- easier to extend into larger workflows

This is not about replacing QA judgment.  
It is about reducing repetitive effort so testers can focus more on risk, quality, and product behavior.

---

## Features

### 1) Bug Classifier Agent
This flow helps analyze a bug description and classify it in a more structured way.

**Typical outputs may include:**
- severity suggestion
- issue category
- impact summary
- clarity improvement suggestions
- triage-friendly summary

**Good for:**
- bug triage support
- defect review workflows
- improving raw bug report quality
- faster issue categorization

---

### 2) Test Case Generator Agent
This flow converts requirement-style inputs into structured test cases.

**Typical outputs may include:**
- positive test cases
- negative test cases
- boundary scenarios
- validation checks
- edge cases
- functional coverage ideas

**Good for:**
- PRD to test-case conversion
- requirement analysis support
- faster QA documentation
- reusable test-design workflows

---

## Tech stack

- **Langflow**
- **Groq**
- **LLM-powered structured QA prompts**
- **Importable JSON flow files**

---

## Repository structure

```text
AI_Agents_Langflow_json_file/
│
├── AI_Agent_Bug_classifier.json
├── AI_Agent_Testcase_Generator.json
└── README.md
```
