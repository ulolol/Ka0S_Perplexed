# 🌀 Ka0S_Perplexed

**Ka0S_Perplexed** is a lightweight, single-file AI search engine inspired by Perplexica. It combines the power of **Google Gemini** for reasoning and **Tavily** for real-time web search to provide comprehensive, cited answers to your questions.

Everything runs locally in your browser—no backend server required.

## ✨ Features

- **🚀 Single File**: The entire app is contained in one `perplexed.html` file.
- **🔍 Smart Search**: Uses Tavily to fetch up to 7 relevant sources from the web.
- **🤖 AI Powered**: Uses Google Gemini (v2.5 Flash) to synthesize answers.
- **🎯 Focus Modes**:
    - **All**: General web search.
    - **Academic**: Prioritizes scholarly papers and articles.
    - **YouTube**: Finds relevant videos.
    - **Reddit**: Searches discussions and threads.
    - **Writing Assistant**: Chat directly with Gemini (no search).
    - **Wolfram Alpha**: Computational knowledge search.
- **💾 Local Storage**: Your chat history and API keys are stored securely in your browser.
- **🌗 Dark Mode**: Built-in dark and light themes.
- **📱 Responsive**: Works great on desktop and mobile.

## 🛠️ Setup

1.  **Download**: Save the `perplexed.html` file to your computer.
2.  **Get API Keys**:
    - **Tavily API Key**: Get one from [tavily.com](https://tavily.com/).
    - **Gemini API Key**: Get one from [aistudio.google.com](https://aistudio.google.com/).
3.  **Run**: Double-click `perplexed.html` to open it in your browser.
4.  **Configure**:
    - Click the **Settings** (gear icon) in the sidebar.
    - Enter your keys manually OR load them from a JSON file (see below).

### 🔑 API Keys JSON (Optional)

You can create a file named `api-keys-example.json` to quickly load your keys:

```json
{
  "tavily": "tvly-YOUR_KEY_HERE",
  "gemini": "AIzaSy-YOUR_KEY_HERE"
}
```

## 🏗️ Tech Stack

- **HTML5**: Structure.
- **Tailwind CSS**: Styling (via CDN).
- **Alpine.js**: Reactivity and state management.
- **Marked.js**: Markdown rendering.
- **DOMPurify**: Security and sanitization.

## ⚠️ Note

Since this is a client-side application using CDNs, it requires an internet connection to load libraries and make API calls. API keys are stored in your browser's `localStorage` and are never sent to any server other than the respective API providers (Google and Tavily).

---
*Inspired by [Perplexica](https://github.com/ItzCrazyKns/Perplexica).*
