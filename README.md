

# ◈ Nexus AI Chatbot

A sleek, modern AI chatbot web app powered by **Groq API** with a dark cyber-themed UI. Built as a single HTML file — no frameworks, no build tools, no dependencies.

---

## 🚀 Features

- **Groq-powered responses** using `llama-3.3-70b-versatile`
- **Voice input** via Web Speech API
- **Markdown rendering** — bold, italic, inline code, code blocks
- **Chat history persistence** via localStorage
- **Typing indicator** with animated dots
- **Responsive design** — works on mobile and desktop
- **Single file** — just open in a browser, no setup needed

---

## 🛠 Setup

1. Get a free API key from [groq.com](https://console.groq.com)
2. Open `nexus-chatbot.html` in a text editor
3. Replace the API key on line 240:
   ```js
   const API_KEY = 'your_groq_api_key_here';
   ```
4. Open the file in any modern browser — done!

---

## 📡 API Details

| Property | Value |
|---|---|
| Provider | [Groq](https://groq.com) |
| Endpoint | `https://api.groq.com/openai/v1/chat/completions` |
| Model | `llama-3.3-70b-versatile` |
| Max Tokens | 1024 |
| Temperature | 0.7 |

---

## 🗂 File Structure

```
nexus-chatbot.html   ← entire app in one file
```

Internally organized as:
```
├── <style>       CSS variables, layout, animations
├── <body>        Header, chat window, input footer
└── <script>      API calls, state, rendering, voice, storage
```

---

## 💬 Usage

| Action | How |
|---|---|
| Send message | Type and press **Enter** |
| New line | **Shift + Enter** |
| Voice input | Click the 🎙 mic button |
| Clear chat | Click **⟳ Clear** in the header |

---

## ⚙️ Customization

**Change the model** — edit line 293:
```js
model: 'llama-3.3-70b-versatile'  // or gemma2-9b-it, mixtral-8x7b-32768
```

**Change the system prompt** — edit line 241:
```js
const SYSTEM_PROMPT = 'You are a helpful, friendly AI assistant...';
```

**Change the accent color** — edit line 15 in the CSS:
```css
--accent: #00e5ff;
```

---

## 🌐 Browser Support

| Browser | Support |
|---|---|
| Chrome | ✅ Full (including voice) |
| Firefox | ✅ Full (no voice) |
| Safari | ✅ Full (no voice) |
| Edge | ✅ Full (including voice) |

---

## ⚠️ Note

The API key is embedded in the HTML file. **Do not share or publish this file publicly** with your real API key inside it. For production use, route API calls through a backend server.

---

## 📄 License

MIT — free to use, modify, and distribute.
