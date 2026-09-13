# 🚀 **healthnest-ai**

<div align="center">

**AI Health Assistant | Powered by Your Data**

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Web-blue?style=for-the-badge" alt="Platform">
  <img src="https://img.shields.io/badge/Language-TypeScript-blue?style=for-the-badge" alt="Language">
  <img src="https://img.shields.io/badge/Framework-Next.js-black?style=for-the-badge" alt="Framework">
</p>

> **Upstream web demos:** The original OpenHealth project provides two options:  
> **[Clinic](https://qna.open-health.me/)** — Quick health consultations  
> **[Full Platform](https://www.open-health.me/)** — Comprehensive health management tools

### 🌍 Choose Your Language

[English](README.md) | [Français](i18n/readme/README.fr.md) | [Deutsch](i18n/readme/README.de.md) | [Español](i18n/readme/README.es.md) | [한국어](i18n/readme/README.ko.md) | [中文](i18n/readme/README.zh.md) | [日本語](i18n/readme/README.ja.md) | [Українська](i18n/readme/README.uk.md) | [Русский](i18n/readme/README.ru.md) | [اردو](i18n/readme/README.ur.md)

</div>

> **Naming note:** This README presents the project as **healthnest-ai**. The repository URL, `open-health` directory, original project demos, star history, and community contacts below still belong to OpenHealth; they are not healthnest-ai releases or accounts.

---

<p align="center">
  <img src="/intro/openhealth.avif" alt="healthnest-ai demo">
</p>

## 🌟 Overview

> healthnest-ai helps you **take charge of your health data**. By using AI and your personal health information, it provides a private assistant to help you better understand and manage your health. You can run it locally for greater privacy.

## ✨ Project Features

<details open>
<summary><b>Core Features</b></summary>

- 📊 **Centralized Health Data Input:** Consolidate your health data in one place.
- 🛠️ **Smart Parsing:** Parse health data and generate structured data files.
- 🤝 **Contextual Conversations:** Use structured data as context for personalized interactions with GPT-powered AI.

</details>

## 📥 Supporting Data Sources & Language Models

<table>
  <tr>
    <th>Data Sources You Can Add</th>
    <th>Supported Language Models</th>
  </tr>
  <tr>
    <td>
      • Blood Test Results<br>
      • Health Checkup Data<br>
      • Personal Physical Information<br>
      • Family History<br>
      • Symptoms
    </td>
    <td>
      • LLaMA<br>
      • DeepSeek-V3<br>
      • GPT<br>
      • Claude<br>
      • Gemini
    </td>
  </tr>
</table>

## 🤔 Why We Built healthnest-ai

> - 💡 **Your health is your responsibility.**
> - ✅ Health management combines **your data** + **intelligence** to turn insights into actionable plans.
> - 🧠 AI can support long-term health management.

## 🗺️ Project Diagram

```mermaid
graph LR
    subgraph Health Data Sources
        A1[Clinical Records<br>Blood Tests/Diagnoses/<br>Prescriptions/Imaging]
        A2[Health Platforms<br>Apple Health/Google Fit]
        A3[Wearable Devices<br>Oura/Whoop/Garmin]
        A4[Personal Records<br>Diet/Symptoms/<br>Family History]
    end

    subgraph Data Processing
        B1[Data Parser & Standardization]
        B2[Unified Health Data Format]
    end

    subgraph AI Integration
        C1[LLM Processing<br>Commercial & Local Models]
        C2[Interaction Methods<br>RAG/Cache/Agents]
    end

    A1 & A2 & A3 & A4 --> B1
    B1 --> B2
    B2 --> C1
    C1 --> C2

    style A1 fill:#e6b3cc,stroke:#cc6699,stroke-width:2px,color:#000
    style A2 fill:#b3d9ff,stroke:#3399ff,stroke-width:2px,color:#000
    style A3 fill:#c2d6d6,stroke:#669999,stroke-width:2px,color:#000
    style A4 fill:#d9c3e6,stroke:#9966cc,stroke-width:2px,color:#000
    style B1 fill:#c6ecd9,stroke:#66b399,stroke-width:2px,color:#000
    style B2 fill:#c6ecd9,stroke:#66b399,stroke-width:2px,color:#000
    style C1 fill:#ffe6cc,stroke:#ff9933,stroke-width:2px,color:#000
    style C2 fill:#ffe6cc,stroke:#ff9933,stroke-width:2px,color:#000
    classDef default color:#000
```

> **Note:** Data parsing currently runs in a separate Python server; a future TypeScript migration is planned.

## Getting Started

## ⚙️ How to Run healthnest-ai

<details open>
<summary><b>Installation Instructions</b></summary>

1. **Clone the upstream repository:**
   ```bash
   git clone https://github.com/OpenHealthForAll/open-health.git
   cd open-health
   ```

2. **Set up and run:**
   ```bash
   # Copy environment file
   cp .env.example .env

   # Start the application using Docker or Podman Compose
   docker compose --env-file .env up
   ```

   With Podman, use `podman compose --env-file .env up` instead. For existing users:
   ```bash
   # Generate an ENCRYPTION_KEY and add it to .env
   head -c 32 /dev/urandom | base64

   # Rebuild and start the application
   docker compose --env-file .env up --build
   ```
   Rebuild after changes to `.env`.

3. **Access healthnest-ai:** Open `http://localhost:3000` in your browser.

> **Note:** The system has parsing and LLM components. Parsing can use docling for local execution; the LLM can run locally with Ollama.

> **Note:** With Ollama and Docker, use `http://docker.for.mac.localhost:11434` on macOS or `http://host.docker.internal:11434` on Windows.

</details>

---

## Upstream Star History

[![Star History Chart](https://api.star-history.com/svg?repos=OpenHealthForAll/open-health&type=Date)](https://star-history.com/#OpenHealthForAll/open-health&Date)

---

## 🌐 Original Project Community and Support

<div align="center">

### 💫 Share Your Story & Give Feedback
[![AIDoctor Subreddit](https://img.shields.io/badge/r/AIDoctor-FF4500?style=for-the-badge&logo=reddit&logoColor=white)](https://www.reddit.com/r/AIDoctor/)
[![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/B9K654g4wf)

### 🤝 Talk with the Original Team
[![Calendly](https://img.shields.io/badge/Schedule_Meeting-00A2FF?style=for-the-badge&logo=calendar&logoColor=white)](https://calendly.com/open-health/30min)
[![Email](https://img.shields.io/badge/Send_Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sj@open-health.me)

</div>
