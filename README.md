# 🎯 AI Pitch Deck Debater
**Multi-Agent AI System for Comprehensive Pitch Deck Analysis**

AI Pitch Deck Debater revolutionizes how entrepreneurs and startups refine their pitch decks by leveraging multiple specialized AI agents that debate, critique, and provide expert-level feedback—just like presenting to a real panel of investors, CTOs, and industry experts.

---

## 🚀 Overview

Get instant, comprehensive feedback on your AI/ML pitch deck from 8 specialized AI personas working together through structured debates. Each agent brings unique expertise, challenges perspectives, and provides actionable recommendations to help you perfect your pitch before presenting to real investors.

**Key Features:**
- 🤖 **Multi-Agent Debate System** - 8 AI experts analyze and debate your deck
- 🎨 **Beautiful UI** - Modern glassmorphism design with Next.js 14
- 🔊 **Audio Feedback** - Text-to-speech synthesis for critique summaries
- 📊 **Comprehensive Analysis** - Individual critiques + unified consensus
- ⚡ **Real-time Processing** - Powered by Claude Haiku for fast analysis
- 📄 **Multiple Formats** - Supports PDF and PowerPoint uploads

---

## 🎯 Problem

Traditional pitch deck feedback requires:
- **Time-consuming meetings** with multiple stakeholders
- **Limited perspectives** from a small review circle
- **Delayed feedback** cycles that slow down iteration
- **Incomplete coverage** missing critical blind spots
- **Expensive consultants** for expert-level analysis

Entrepreneurs need fast, comprehensive, multi-perspective feedback to identify critical issues before presenting to real investors.

---

## 💡 Our Solution

AI Pitch Deck Debater provides instant access to a virtual panel of 8 specialized AI experts who:

1. **Analyze Each Slide** - From technical depth to market positioning
2. **Debate Perspectives** - Challenge each other to uncover blind spots
3. **Generate Consensus** - Synthesize unified recommendations with priority actions
4. **Provide Audio Summaries** - Listen to critiques while reviewing slides
5. **Identify Deal Breakers** - Surface critical issues that could kill your pitch

### ✨ Value Proposition:

| Benefit | Description |
|---------|-------------|
| **Save Time** | Get instant expert-level feedback instead of scheduling multiple meetings |
| **Multiple Perspectives** | See your deck through the eyes of VCs, CTOs, Data Scientists, and more |
| **Actionable Insights** | Receive prioritized recommendations you can implement immediately |
| **Improve Quality** | Identify and fix critical issues before presenting to real investors |
| **Cost-Effective** | Access expert analysis without expensive consultants |

> From **"hoping for the best"** to **"pitch-perfect confidence."**

---

## 🤖 Meet the AI Expert Personas

Our system features 8 specialized AI agents, each bringing unique expertise:

| Persona | Focus Area | Voice Characteristics |
|---------|-----------|----------------------|
| 💼 **VC Partner** | Investment potential, market size, ROI | Strategic, numbers-focused |
| 🔬 **AI Architect** | Technical feasibility, architecture depth | Detail-oriented, technical |
| 📊 **Data Scientist** | ML methodology, data strategy | Analytical, evidence-based |
| 💰 **CFO** | Financial projections, unit economics | Conservative, risk-aware |
| 🎨 **Product Manager** | UX, product-market fit, user journey | User-centric, pragmatic |
| 🔒 **Security Expert** | Data privacy, compliance, risk assessment | Cautious, regulatory-focused |
| 📈 **Growth Lead** | Scalability, go-to-market, traction | Aggressive, growth-minded |
| ⚖️ **Legal Advisor** | Compliance, IP, regulatory landscape | Cautious, detail-oriented |

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|-----------|---------|
| **Next.js 14** | React framework with App Router |
| **TypeScript** | Type-safe development |
| **Tailwind CSS** | Utility-first styling with glassmorphism theme |


### Backend
| Technology | Purpose |
|-----------|---------|
| **FastAPI** | High-performance Python web framework |
| **Anthropic Claude Haiku** | AI model for multi-agent analysis |
| **Edge TTS** | Microsoft Text-to-Speech synthesis |
| **python-pptx** | PowerPoint file parsing |
| **PyPDF2** | PDF document parsing |
| **Uvicorn** | ASGI server |

### Architecture
```
┌─────────────────────────────────────────────────┐
│            Next.js Frontend (Port 3000)         │
│  ┌─────────────┐  ┌──────────────┐              │
│  │  HomePage   │  │  Main App    │              │
│  │  Component  │  │  Components  │              │
│  └─────────────┘  └──────────────┘              │
└─────────────┬───────────────────────────────────┘
              │ API Routes Proxy
              ▼
┌─────────────────────────────────────────────────┐
│         FastAPI Backend (Port 8000)             │
│  ┌──────────────┐  ┌─────────────────┐          │ 
│  │ API Endpoints│  │  Multi-Agent    │          │
│  │   /upload    │  │  Debate Engine  │          │
│  │   /analyze   │  │  (8 AI Agents)  │          │
│  │   /tts       │  └─────────────────┘          │
│  └──────────────┘                               │
└─────────────┬───────────────────────────────────┘
              │
              ▼
     ┌────────────────────┐
     │  Anthropic Claude  │
     │   API              │
     └────────────────────┘
```

---

## 📦 Installation & Setup

### Prerequisites
- **Node.js** 18+ and npm
- **Python** 3.10+
- **Anthropic API Key** ([Get one here](https://console.anthropic.com/))

### 1. Clone the Repository
```bash
git clone https://github.com/sathishsravanakumar/Pitch-deck-debator.git
```

## 🎮 Usage Guide

### Step 1: Upload Your Pitch Deck
1. Visit **http://localhost:3000**
2. Click **"Get Started"** from the home page
3. Upload your pitch deck (PDF or PPTX format)
4. Wait for slides to be extracted and displayed

### Step 2: Select AI Expert Agents
1. Choose which AI personas should review your deck
2. Recommended: Select at least 3-4 agents for comprehensive feedback
3. Click **"Apply"** to confirm selection

### Step 3: Analyze Slides
1. Select a slide from the dropdown
2. Click **"Analyze This Slide"**
3. Wait for multi-agent analysis to complete (1-2 minutes per slide)

### Step 4: Review Feedback

**🎯 Unified Feedback Tab:**
- View consensus from all agents
- See overall slide score (1-10)
- Review priority actions and deal breakers
- Read the debate transcript

**👥 Individual Critiques Tab:**
- Detailed feedback from each AI persona
- Key strengths identified
- Critical issues highlighted
- Specific recommendations
- Generate audio summaries

**📊 Results Tab:**
- Export analysis to JSON
- Download improved pitch deck (coming soon)
- View aggregate scores

---

## 🎨 Features Deep Dive

### 1. Multi-Agent Debate System
- Each agent independently analyzes the slide
- Agents engage in structured debate to challenge perspectives
- Consensus is generated from collaborative discussion
- Transcripts show the full debate conversation

### 2. Text-to-Speech Audio
- Generate audio summaries for each persona's critique
- Uses Microsoft Edge TTS with persona-specific voices
- Play audio while reviewing written feedback
- Useful for multitasking or accessibility

### 3. Glassmorphism UI
- Modern, professional design aesthetic
- Blue gradient theme with frosted glass effects
- Responsive layout for all screen sizes
- Smooth transitions and hover effects

### 4. Comprehensive Analysis
- **Slide Scores**: 1-10 rating from each expert
- **Key Strengths**: What's working well
- **Critical Issues**: Problems that must be fixed
- **Recommendations**: Specific, actionable improvements
- **Deal Breakers**: Issues that could kill funding
- **Priority Actions**: Top 3 things to fix first

---

## 🔑 Environment Variables

### Backend (.env)
```bash
ANTHROPIC_API_KEY=sk-ant-...your-key-here
```

### Frontend (.env.local)
```bash
NEXT_PUBLIC_API_URL=http://localhost:8000
PYTHON_API_URL=http://localhost:8000
```

---

## ⭐ Show Your Support

If you find this project helpful, please consider giving it a star on GitHub!

**Built with ❤️**  
