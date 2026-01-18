
# 🎬 Movie Studio Simulator
**Powered by CrewAI + OpenAI**

> **Transform movie concepts into complete productions. Enter a genre, setting, and logline, and watch a multi-agent AI film crew generate script outlines, character bios, budgets, and marketing materials—all in one seamless workspace.** ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-16-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB.svg)](https://react.dev/)
[![CrewAI](https://img.shields.io/badge/CrewAI-Multi_Agent-purple.svg)](https://www.crewai.com/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)
[![Vercel](https://img.shields.io/badge/Deploy-Vercel-black.svg)](https://vercel.com/)

---

## ✨ What It Does

Movie Studio Simulator is an intelligent film development platform that uses a **multi-agent CrewAI workflow** to:

1. **Process Your Concept** — Analyze genre, setting, logline, and tone using GPT-4o-mini
2. **Orchestrate Specialized Agents** — Coordinate 5 film industry experts working in parallel
3. **Generate Complete Outputs** — Produce script outlines, character bios, budgets, and marketing materials
4. **Enable Real-Time Refinement** — Chat with AI, get suggestions, and generate poster images

All in a beautiful, responsive interface with smooth animations and zero page reloads.

---

## 🎯 Core Features

### 🤖 **AI-Powered Film Crew**
- **Multi-Agent Orchestration** — CrewAI coordinates 5 specialized agents (Director, Screenwriter, Casting Agent, Producer, Marketing Exec)
- **Real OpenAI Integration** — GPT-4o-mini for intelligent, context-aware responses
- **Live Crew Status** — Real-time animations showing which agent is working
- **Structured Outputs** — JSON-parsed results with fallback handling

### 📊 **Rich Creative Workspace**
- **Script Outline** — Three-act structure with key beats and full script preview
- **Character Bios & Casting** — Detailed character descriptions with actor suggestions
- **Budget Breakdown** — Realistic estimates with category percentages
- **Poster & Tagline** — Compelling marketing materials with DALL-E image generation
- **Interactive Editor** — Edit scripts with AI-powered suggestions

### 🎨 **Modern UI/UX**
- **State-Driven Architecture** — Smooth component transitions, no page reloads
- **Dark/Light Mode** — Beautiful theme with system preference support
- **Mobile-First Design** — Responsive with 44px+ touch targets, bottom navigation
- **Micro-Animations** — Agent status animations with reduced-motion support
- **Hero Video Backgrounds** — Cinematic video backgrounds (disabled on mobile for performance)

### 📱 **Full Feature Set**
| Feature | Description |
|---------|-------------|
| 🎬 **Multi-Agent Crew** | 5 specialized AI agents working in parallel |
| 📝 **Script Editor** | Interactive editor with AI refinement suggestions |
| 💬 **Real-Time AI Chat** | Streaming chat assistant with project context |
| 🎨 **Image Generation** | DALL-E 3 integration for poster creation |
| 🎤 **Voice Input** | Speech-to-text for logline input |
| 📊 **Analytics Dashboard** | Project metrics and activity tracking |
| 🔄 **Project Comparison** | Side-by-side comparison of different concepts |
| 📤 **Export & Share** | Export projects in JSON/Markdown, generate share links |
| 🏥 **Health Monitoring** | Database connectivity status with RPC function checks |
| 📱 **Mobile Optimized** | Full feature parity on mobile devices |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 16** | React 19.2 with App Router, Turbopack |
| **TypeScript** | Type-safe development with strict mode |
| **Ant Design** | Enterprise-grade component library |
| **CSS Custom Properties** | Theme system with light/dark mode |
| **React Hooks** | Custom hooks for agent orchestration |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance async Python API |
| **CrewAI** | Multi-agent AI orchestration framework |
| **OpenAI GPT-4o-mini** | Intelligent content generation |
| **Pydantic v2** | Data validation and serialization |
| **SSE (Server-Sent Events)** | Real-time streaming for chat |

### **Data & Cache** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL with `moviestudio` schema |
| **RPC Functions** | Secure database access without schema exposure |
| **Upstash Redis** | Job queue & caching with `moviestudio` prefix |

### **External APIs** 🔌
| API | Purpose |
|-----|---------|
| **OpenAI** | GPT-4o-mini for chat, suggestions, and CrewAI |
| **DALL-E 3** | High-quality poster image generation |
| **TMDb** | Optional reference film integration |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting with edge functions |
| **Railway** | Backend API with Railpack builder |

---

## 📖 User Guide

### Getting Started

1. **Enter Your Concept** — Fill out the form with genre, setting, and logline
2. **Optional: Add Tone** — Specify the desired tone (Gritty, Whimsical, Epic, etc.)
3. **Run the Crew** — Watch as 5 specialized agents work in parallel
4. **Explore Results** — Navigate through tabs to see script, characters, budget, and marketing materials
5. **Refine & Iterate** — Use AI chat, suggestions, and image generation to enhance your concept

### Understanding Your Results

| Section | What It Shows |
|---------|---------------|
| **Script Outline** | Three-act structure with detailed summaries and key story beats |
| **Character Bios** | Main characters with descriptions and casting suggestions |
| **Budget Breakdown** | Realistic budget estimates with category percentages |
| **Poster & Tagline** | Marketing materials ready for DALL-E image generation |
| **Crew Status** | Real-time visualization of which agent is working |

### Pro Tips

- **Be specific** with your logline for better results
- **Use voice input** for quick logline entry on mobile
- **Explore AI chat** for follow-up questions and refinements
- **Generate images** to visualize your poster concept
- **Compare projects** to see how different concepts differ
- **Export projects** to save your work

---

## 🎨 Customization

### Theme Options
- ☀️ **Light Mode** — Clean, professional interface
- 🌙 **Dark Mode** — Cinematic dark theme
- 🖥️ **System** — Follows OS preference

### Crew Configuration
- **Agent Roles** — Customizable in `crewai_movie_adapter.py`
- **Task Prompts** — Enhanced prompts for better structured output
- **Model Selection** — Configurable via `OPENAI_MODEL` env var

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Crew Run Time | ~30-60 seconds |
| Frontend Bundle | Optimized with Next.js 16 |
| Mobile Performance | 90+ Lighthouse score |
| API Response Time | <200ms (non-AI endpoints) |
| Streaming Latency | <100ms first token |

---

## 🛡️ Security

- ✅ **RPC Functions** — Secure database access without schema exposure
- ✅ **API Rate Limiting** — Redis-based rate limiting
- ✅ **CORS Protection** — Configured for production origins
- ✅ **Environment Variables** — All secrets in env vars
- ✅ **Input Validation** — Pydantic models for all inputs
- ✅ **Error Sanitization** — No sensitive data in error messages

---


## 👨‍💻 Creator

**Derril Filemon**

This project demonstrates proficiency in:
- 🤖 **AI/ML Integration** — CrewAI multi-agent workflows, OpenAI GPT-4o-mini, DALL-E 3
- ⚛️ **Modern React** — Next.js 16, React 19.2, App Router, Server Components
- 🐍 **Python Backend** — FastAPI, async/await, Pydantic v2, SSE streaming
- 🎨 **UI/UX Design** — Ant Design, responsive design, animations, accessibility
- ☁️ **Cloud Architecture** — Supabase, Upstash Redis, Railway, Vercel
- 🔧 **DevOps** — CI/CD, environment management, health monitoring
- 📱 **Mobile Development** — Mobile-first design, touch targets, safe area insets
- 🔐 **Security** — RPC functions, input validation, error handling

---

## 🙏 Acknowledgments

- **[CrewAI](https://www.crewai.com/)** — Multi-agent orchestration framework
- **[OpenAI](https://openai.com/)** — GPT-4o-mini and DALL-E 3 APIs
- **[Supabase](https://supabase.com/)** — PostgreSQL database & RPC functions
- **[Upstash](https://upstash.com/)** — Redis caching and job queue
- **[Railway](https://railway.app/)** — Backend deployment platform
- **[Vercel](https://vercel.com/)** — Frontend hosting
- **[Ant Design](https://ant.design/)** — Enterprise UI component library

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
