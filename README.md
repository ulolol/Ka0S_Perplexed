# 🌀 Ka0S_Perplexed

![Ka0S Perplexed Logo](perplexed_lowQ_logo.gif)

**Ka0S_Perplexed** is a fully self-contained, single-file AI search engine inspired by Perplexica. Powered by **Google Gemini 2.5 Flash** for intelligent reasoning and **Tavily** for real-time web search, it delivers cited answers with **AI-selected images** and **current date/time grounding**.

🌐 Everything runs in your browser—no server needed.

## ✨ Features

- **🚀 Single HTML File** • Just `perplexed.html` • Instant deploy
- **🔍 Gemini-First Reasoning Loop**:
  - **Plans** optimal searches via AI assessment
  - **Executes** adaptive Tavily searches (up to 3 refinement rounds)
  - **Evaluates** result quality & auto-refines
  - Live status: `Planning... → Searching... → Selecting images...`
- **🖼️ Relevant Images** • AI curates 1-3 top thumbnails with hover previews
- **📅 Temporal Grounding** • Real-time UTC time in prompts for current events
- **🤖 32k Token Context** • Deep analysis, JSON parsing, multimodal files
- **🎯 Focus Modes**:
  | Mode | Description |
  |------|-------------|
  | **All** | General web |
  | **Academic** | Papers & research |
  | **Reddit** | Discussions |
  | **Writing Assistant** | Pure chat |
  | **Wolfram Alpha** | Math/compute |
- **📁 Multimodal Files** • Images/PDFs/text → AI-generated search queries
- **💾 Local History** • Persistent chats & keys in browser storage
- **🌗 Themes** • Auto dark/light + responsive mobile UI
- **🔍 Search Deeper** • 4-query deep dive for complex topics

> **~250 deep searches/mo** on Tavily free tier (1000 queries)

## 🧠 How It Works

1. **Query** → Gemini plans: needs search? → Generates queries
2. **Search Loop**:
   ```
   Search → Fetch sources + images → Evaluate → Refine? → Repeat (max 3)
   ```
3. **Select Images** → Gemini picks visuals
4. **Ground & Answer** → Synthesizes with date context + citations

![Flow](./Perplexed_Chat.png)

## 📸 Screenshots

| Chat | New Session | Settings | Light Mode |
|------|-------------|----------|------------|
| ![Chat](./Perplexed_Chat.png) | ![New](./Perplexed_newChat.png) | ![Settings](./Perplexed_settings.png) | ![Light](./Perplexed_lightMode.png) |

## 🚀 Quick Start

1. 💾 Save `perplexed.html`
2. 🔑 Get keys:
   - [Tavily](https://tavily.com) (search)
   - [Gemini AI Studio](https://aistudio.google.com) (reasoning)
3. ⚡ Open in browser
4. ⚙️ Settings → Paste keys **or** load `api-keys.json`:
   ```json
   {
     "tavily": "tvly-xxx",
     "gemini": "AIzaSy-xxx"
   }
   ```

## 🏗️ Stack

- **Alpine.js** (state)
- **Tailwind CSS** (CDN)
- **Marked.js** (MD)
- **Lucide** (icons)
- **DOMPurify** (secure)

## ⚠️ Notes

- Internet required (CDNs + APIs)
- Keys stored locally (localStorage)
- Console Tailwind warning? Normal for CDN.

---

*Inspired by [Perplexica](https://github.com/ItzCrazyKns/Perplexica)*  
✨ [Live Demo? Host yourself!]