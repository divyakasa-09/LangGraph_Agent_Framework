# LangGraph Agent Framework

A modern AI agent framework built with LangGraph, featuring a FastAPI backend and Streamlit frontend for creating and interacting with intelligent AI agents.

## 🚀 Project Overview

This project demonstrates how to build a scalable AI agent system using LangGraph, a framework for building stateful, multi-actor applications with LLMs. The system supports multiple AI providers (Groq and OpenAI) and includes web search capabilities for enhanced responses.

## ✨ Features

- **Multi-Provider Support**: Choose between Groq (Llama models) and OpenAI (GPT models)
- **Web Search Integration**: Enable real-time web search using Tavily API for up-to-date information
- **Customizable Agents**: Define custom system prompts to create specialized AI agents
- **Modern UI**: Clean Streamlit interface for easy interaction
- **RESTful API**: FastAPI backend with automatic API documentation
- **Stateful Conversations**: LangGraph-powered agent with conversation memory

## 🏗️ Architecture

The project consists of three main components:

1. **AI Agent (`ai_agent.py`)**: Core LangGraph agent implementation with support for multiple LLM providers
2. **Backend (`backend.py`)**: FastAPI server providing REST endpoints for agent interactions
3. **Frontend (`frontend.py`)**: Streamlit web interface for user interactions

## 🔧 Supported Models

### Groq Models
- `llama-3.3-70b-versatile` - Versatile Llama 3.3 70B model
- `mixtral-8x7b-32768` - Mixtral 8x7B model with large context

### OpenAI Models
- `gpt-4o-mini` - GPT-4 Omni mini model

## 📋 Prerequisites

Before setting up the project, you'll need API keys for the following services:

- **Groq API Key**: For using Groq's Llama models
- **OpenAI API Key**: For using OpenAI's GPT models  
- **Tavily API Key**: For web search functionality

Set these as environment variables:
```bash
export GROQ_API_KEY="your_groq_api_key"
export TAVILY_API_KEY="your_tavily_api_key"
export OPENAI_API_KEY="your_openai_api_key"
```

## 🛠️ Technology Stack

- **LangGraph**: Agent framework for building stateful LLM applications
- **LangChain**: Framework for developing applications with LLMs
- **FastAPI**: Modern, fast web framework for building APIs
- **Streamlit**: Rapid web app development for data science
- **Pydantic**: Data validation using Python type annotations
- **Uvicorn**: ASGI server for running FastAPI applications

---

# Project Setup Guide

This guide provides step-by-step instructions to set up your project environment, including setting up a Python virtual environment using Pipenv, pip, or conda.

## Table of Contents

1. [Setting Up a Python Virtual Environment](#setting-up-a-python-virtual-environment)
   - [Using Pipenv](#using-pipenv)
   - [Using pip and venv](#using-pip-and-venv)
   - [Using Conda](#using-conda)
2. [Running the application](#project-phases-and-python-commands)


## Setting Up a Python Virtual Environment

### Using Pipenv
1. **Install Pipenv (if not already installed):**  
```
pip install pipenv
```

2. **Install Dependencies with Pipenv:** 

```
pipenv install
```

3. **Activate the Virtual Environment:** 

```
pipenv shell
```

---

### Using `pip` and `venv`
#### Create a Virtual Environment:
```
python -m venv venv
```

#### Activate the Virtual Environment:
**macOS/Linux:**
```
source venv/bin/activate
```

**Windows:**
```
venv\Scripts\activate
```

#### Install Dependencies:
```
pip install -r requirements.txt
```

---

### Using Conda
#### Create a Conda Environment:
```
conda create --name myenv python=3.11
```

#### Activate the Conda Environment:
```
conda activate myenv
```

#### Install Dependencies:
```
pip install -r requirements.txt
```


# Project Phases and Python Commands

## Phase 1: Create AI Agent
```
python ai_agent.py
```

## Phase 2: Setup Backend with FastAPI
```
python backend.py
```

## Phase 3: Setup Frontend with Streamlit
```
python frontend.py
```

## IMPORTANT
### Make sure backend python script is running in a separate terminal



