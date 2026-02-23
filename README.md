# 🤖 Gemini Clone

A pixel-perfect, feature-rich clone of Google's **Gemini AI** web interface — built with **React + Vite** and powered by the **Google Generative AI SDK** (`gemini-2.5-flash`).

---

## ✨ Features

- 💬 **Real-time AI Chat** — Send text prompts and receive AI-generated responses powered by Google Gemini
- 🖼️ **Image Upload Support** — Attach images alongside prompts for multimodal conversations
- 🕘 **Chat History** — Sidebar keeps a list of your recent prompts for quick re-access
- 🌗 **Light / Dark Theme Toggle** — Switch themes from the sidebar; preference is persisted in `localStorage`
- ✨ **Typing Animation** — Responses appear word-by-word with a smooth typewriter effect
- ➕ **New Chat** — Instantly reset the conversation and start fresh
- 📱 **Responsive Layout** — Collapsible sidebar with a clean, minimal design

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| [React 19](https://react.dev/) | UI framework |
| [Vite 7](https://vitejs.dev/) | Build tool & dev server |
| [@google/generative-ai](https://www.npmjs.com/package/@google/generative-ai) | Gemini API SDK |
| React Context API | Global state management |
| Vanilla CSS | Styling with light/dark theme support |

---

## 📁 Project Structure

```
gemini-clone/
├── public/
├── src/
│   ├── assets/          # Icons and images
│   ├── components/
│   │   ├── Main/        # Chat area (prompt input, results, cards)
│   │   └── Sidebar/     # Navigation, history, theme toggle
│   ├── config/
│   │   └── gemini.js    # Gemini API configuration & runChat function
│   ├── context/
│   │   └── Context.jsx  # Global state (input, history, theme, loading)
│   ├── App.jsx
│   └── main.jsx
├── .env                 # API key (not committed)
├── index.html
└── package.json
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** v18 or higher
- A **Google Gemini API key** — get one at [Google AI Studio](https://aistudio.google.com/app/apikey)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/gemini-clone.git
   cd gemini-clone
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up your API key**

   Create a `.env` file in the root of the project:
   ```env
   VITE_GEMINI_API_KEY=your_google_gemini_api_key_here
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. Open your browser at **[http://localhost:5173](http://localhost:5173)**

---

## 📜 Available Scripts

| Script | Description |
|---|---|
| `npm run dev` | Start the local development server |
| `npm run build` | Build the project for production |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run ESLint for code quality |

---

## 🔑 Environment Variables

| Variable | Description |
|---|---|
| `VITE_GEMINI_API_KEY` | Your Google Gemini API key |

> ⚠️ **Never commit your `.env` file.** It is already listed in `.gitignore`.

---

## 🤝 Contributing

Contributions, issues and feature requests are welcome!

1. Fork the project
2. Create your feature branch: `git checkout -b feature/awesome-feature`
3. Commit your changes: `git commit -m 'Add awesome feature'`
4. Push to the branch: `git push origin feature/awesome-feature`
5. Open a Pull Request

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

> Built with ❤️ as a learning project to explore Google Gemini API and modern React development.
