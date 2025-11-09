# 🌍 AI Trip Planner - Agentic Workflow System
> An intelligent trip planning system powered by LLM agents, real-time APIs, and MLOps best practices.

## 🎯 Overview

**AI Trip Planner** is an advanced MLOps project that demonstrates the implementation of an **Agentic AI Workflow System**. The application uses Large Language Models (LLMs) combined with real-time API integrations to automatically generate personalized travel itineraries based on user preferences.

### What Makes This Special?

- 🤖 **Agentic AI**: Uses LangGraph to orchestrate multiple AI tools autonomously
- 🔄 **Real-time Data**: Integrates 7+ external APIs for live weather, places, and currency data
- 🏗️ **MLOps Ready**: Modular architecture following production-grade best practices
- ⚡ **Fast & Efficient**: Powered by `uv` package manager and optimized workflows
- 📊 **Observable**: Built-in logging and LangSmith integration for monitoring

## ✨ Features

### Core Capabilities

- ✅ **Intelligent Trip Planning**: Generate day-by-day itineraries for any destination
- ✅ **Real-time Weather**: Get current and forecasted weather conditions
- ✅ **Smart Recommendations**: Discover attractions, hotels, and restaurants
- ✅ **Currency Conversion**: Automatic budget calculations in local currency
- ✅ **Expense Calculator**: Detailed cost breakdown for your entire trip
- ✅ **Multiple Output Formats**: Export to TXT, MD, PDF, or DOCX

### Technical Features

- 🔧 **5 Custom LangChain Tools**: Weather, Places, Currency, Calculator, Arithmetic
- 🌐 **RESTful API**: FastAPI backend with async support
- 💻 **Interactive UI**: Beautiful Streamlit frontend
- 📝 **Comprehensive Logging**: Track every step of the workflow
- 🛡️ **Error Handling**: Robust exception management and validation
- 🔌 **Modular Design**: Easy to extend with new tools and APIs

## 🏗️ Architecture

```
┌─────────────────────────────┐
│      Streamlit Frontend     │
│   (User Input & Display)    │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│      FastAPI Backend        │
│  (REST API & Validation)    │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│    Agentic Workflow Layer   │
│  (LangGraph + LangChain)    │
└──────────────┬──────────────┘
               │
    ┌──────────┴──────────┐
    ▼                     ▼
┌─────────┐         ┌─────────┐
│  Tools  │         │  APIs   │
│  Layer  │◄───────►│  Layer  │
└─────────┘         └─────────┘
```

### Workflow Pipeline

1. **User Input** → Query submitted via Streamlit UI
2. **API Gateway** → FastAPI receives and validates request
3. **Agent Processing** → LangGraph orchestrates tool execution
4. **Tool Execution** → Sequential calls to Weather, Places, Currency, Calculator tools
5. **Data Synthesis** → LLM combines results into coherent itinerary
6. **Output Generation** → Formatted response returned to user

## 🔧 Prerequisites

- **Python**: 3.10 or higher
- **Package Manager**: `uv` (recommended) or `pip`
- **API Keys**: Required for external services (see Configuration)


   **

Made with ❤️ by the AI Trip Planner Team
