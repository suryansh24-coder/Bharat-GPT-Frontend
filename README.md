# Bharat GPT – Frontend

![Version](https://img.shields.io/badge/version-1.0.0-peach)
![Status](https://img.shields.io/badge/status-production--ready-success)
![Deployment](https://img.shields.io/badge/deployment-static--ready-brightgreen)

A lightweight, blazing-fast, single-page AI chat interface built using **pure modern web technologies — without heavy frameworks.**

Designed for performance, portability, and zero build complexity.

---

# 🚀 Overview

**Bharat GPT Frontend** is a fully static, framework-free Single Page Application (SPA) engineered for:

- ⚡ Maximum speed  
- 📦 Zero build tools  
- 🌐 CDN-based libraries  
- 📱 Full responsiveness  
- 🧠 AI-powered backend integration  
- 💾 Local persistence  
- 🎤 Voice interaction  
- 📄 PDF export support  

No React.  
No Angular.  
No Vue.  

Just clean **HTML5**, modern **ES6+ JavaScript**, and **Tailwind CSS**.

---

# 🛠 Tech Stack

## Core Technologies

| Technology | Purpose |
|------------|----------|
| **HTML5** | Semantic SPA structure (`index.html`) |
| **Vanilla JavaScript (ES6+)** | State management, API calls, DOM manipulation |
| **Tailwind CSS (CDN)** | Utility-first styling |
| **Custom CSS** | Scrollbars, animations, Markdown overrides |

---

# 📦 CDN Libraries Used

All libraries are imported directly inside `<head>` for zero-build deployment.

| Library | Purpose |
|----------|----------|
| **Lucide Icons** | Modern SVG icon system |
| **Marked.js** | Markdown → HTML parser |
| **Highlight.js** | Syntax highlighting (atom-one-dark theme) |
| **Emoji Picker Element** | Native emoji selector |
| **html2pdf.js** | Export chat to PDF |

---

# 🎨 Design System

## 🎨 Color Palette

| Element | Color |
|----------|--------|
| Primary Accent | `#F4B38A` (Peach) |
| Secondary Accent | `#327382` (Teal Blue) |
| Light Theme Background | `#F7F5F2` |
| Dark Theme Base | `#0f172a` |

---

## 🖋 Typography

- **Font:** Inter (Google Fonts)  
- **Weights:** 300 – 700  
- Clean, readable, professional design  

---

# 📐 Layout Architecture

- Flexbox-based layout  
- Collapsible sidebar  
- Dynamic chat expansion  
- Mobile hamburger menu  
- Tailwind responsive breakpoints (`sm:`, `md:`)  

---

# 🧠 Core JavaScript Architecture

All logic is handled inside a monolithic script within `index.html`.

---

## 1️⃣ Unified State Management

Global variables emulate lightweight React-like behavior:

    ```javascript
      let currentChatId;
      let chats = {}; 
      let chatHistory = [];
      Tracks:







## Active conversation

Message arrays

Metadata (titles, timestamps)

### 2️⃣ Local Storage Persistence

##### Automatically saves:

Chat history

Theme preference

Language preference

User settings

On reload:

Re-hydrates from localStorage

Restores UI state instantly

No database required.

### 3️⃣ Backend API Integration
Core Functions
generateAIResponse(prompt);
performWebSearch(query);
Communication Method

Native fetch()

HTTP POST

JSON payload

Error handling

Timeout protection

Safe fallback messaging

Example Backend Endpoint
https://your-render-url.com/api/search
### 4️⃣ Advanced Features
🎤 Voice-to-Text

Web Speech API

webkitSpeechRecognition

Real-time speech → text

📝 Markdown Rendering

Parsed using Marked.js

Code blocks auto-highlighted

Sanitized output pipeline

📄 Export System

Export Chat → PDF

Export Chat → Markdown

DOM parsing → formatted output

🌍 Multi-Language Support (i18n)

Supported Languages:

English

Hindi

Spanish

French

Mandarin

Core function:

changeLanguage(langKey);

Instant UI transformation without reload.

### 5️⃣ Responsiveness & Mobile Optimization
Screen Size	Behavior
> 768px	Sidebar fixed
< 768px	Sidebar hidden (-translate-x-full)
Mobile	Hamburger toggle with overlay

Function:

toggleMobileSidebar();

Smooth animations and overlay transitions included.

#### 🗂 Project Structure
/ (root)
 ├── index.html
 ├── logo.png
 └── README.md

No:

package.json

node_modules

build directory

Fully static architecture.

#### 🚀 Deployment

Since the frontend is 100% static, deploy instantly on:

✅ Vercel

✅ GitHub Pages

Deployment Steps (Vercel Example)

Push repository to GitHub

Import project into Vercel

Select:

Framework → Other

Build Command → None

Output Directory → /

Click Deploy

Done.

🔥 Performance Philosophy

No React re-renders

No heavy bundle sizes

No build tools

No runtime overhead

CDN-first architecture

Minimal DOM repainting

Result

⚡ Extremely fast load time
📱 Mobile-first performance
🌐 Global CDN compatibility

## 📌 Key Highlights

Framework-free SPA

Full LocalStorage persistence

AI Markdown rendering pipeline

Syntax highlighting

Voice recognition

Export to PDF

Internationalization support

Fully responsive

Zero backend dependency for UI state

### 🎯 Why This Architecture?

Most AI applications rely on bulky frontend stacks.

Bharat GPT proves:

Clean architecture + Vanilla JS = Production-level performance

Ideal for:

Hackathons

Lightweight AI products

Static SaaS interfaces

Portfolio projects

Edge deployments

#### 📜 License

Open for innovation and contribution.

#### 👨‍💻 Author

Suryansh Tiwari
Engineering Student | AI Builder | Bharat GPT Creator
