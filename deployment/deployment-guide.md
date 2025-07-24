# 🚀 Vertex AI Bot Deployment Guide

This guide explains how to deploy the **InsuraBot** using **Google Cloud's Vertex AI Studio**.

---

## 🧠 Objective

Deploy a prompt-based conversational assistant that answers user questions about insurance policies using grounded context (PDF document).

---

## 🔧 Step-by-Step Instructions

### ✅ 1. Open Vertex AI Studio

- Go to: [Vertex AI Studio](https://console.cloud.google.com/vertex-ai/prompt-library)
- Select your Google Cloud project
- Click **"Create New Prompt"**

---

### ✅ 2. Paste the Prompt

- Copy content from `prompts/main-prompt.txt`
- Paste into the **Prompt** section of Vertex AI Studio

---

### ✅ 3. Configure Model Settings

- **Model**: `Gemini 1.5 Pro` (or the latest available)
- **Temperature**: `0.4` (for consistent outputs)
- **Top-P**: `0.9`
- **Top-K**: `40`
- **Max Tokens**: `1024`
- **Response Type**: `Text`

---

### ✅ 4. Add Grounding Context

- Upload the document: `insurance-policy.pdf`
- Make sure **Context Grounding** is enabled

---

### ✅ 5. Test the Prompt

Use sample questions like:
- "How to file a claim?"
- "Is maternity covered under this plan?"
- "What documents are needed for hospitalization claims?"

---

### ✅ 6. Save and Share

- Save the prompt with name: `InsuraBot Prompt`
- Optionally deploy as an API endpoint if needed
- You can export configuration to JSON for tracking (`vertex-ai-config.json`)

---

## 📌 Tips

- Use the **History** tab to monitor user conversations
- Add **Follow-up prompts** from `prompts/follow-up-prompts.md` to test different user flows
- You can further improve with function calling or UI integration later

---

> 🛡️ This bot was built for educational purposes using Vertex AI Studio under Google Cloud Skills Boost lab exercises.

