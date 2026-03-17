# Haystack Agentic RAG Pipelines

A collection of modular AI applications built using the Haystack framework, showcasing advanced patterns like Retrieval-Augmented Generation (RAG), branching pipelines, self-reflecting agents, and function-calling chat systems.

This repository demonstrates how to design scalable, extensible, and production-ready LLM applications using structured pipelines and reusable components.

---

## Features

- Modular RAG pipelines with document stores and retrievers
- Custom components for extending pipeline capabilities
- Conditional branching with fallback to external search
- Self-reflecting agents with iterative loops and validation
- Function-calling chat agents with tool integration
- Clean orchestration using Haystack pipelines

---

## Architecture Overview

This project leverages Haystack’s core abstractions:

- **Components** → Individual processing units (retrievers, generators, validators)
- **Pipelines** → Directed graphs connecting components
- **Document Stores** → Backend for storing and retrieving context
- **Agents** → LLM-driven decision-makers using tools and loops

The system is designed to be:
- Modular
- Extensible
- Easy to debug and scale

---

## Project Structure

### 1. Build Customized RAG
Implements a retrieval-augmented generation pipeline with document ingestion, retrieval, and LLM-based answer generation.

### 2. Custom Components – News Summarizer
Builds a custom Haystack component that fetches and summarizes external data (Hacker News API).

### 3. Fallbacks with Branching Pipelines
Implements conditional routing with fallback to web search when retrieval confidence is low.

### 4. Self-Reflecting Agents with Loops
Creates an agent that evaluates and iteratively improves its outputs using validation feedback.

### 5. Chat Agent with Function Calling
Builds a tool-augmented chat agent using function calling to invoke pipelines dynamically.

---

## Setup

```bash
git clone https://github.com/your-username/Haystack-Agentic-RAG-Pipelines.git
cd Haystack-Agentic-RAG-Pipelines
pip install -r requirements.txt
export OPENAI_API_KEY=your_key_here
```
Running the Notebooks

Launch Jupyter:

jupyter notebook

Run notebooks in sequence to explore:

1 → RAG
2 → Custom Components
3 → Branching Pipelines
4 → Self-Reflecting Agents
5 → Chat Agent

## Key Learnings

Designing composable LLM systems using pipeline abstractions

Extending retrieval systems with custom components

Handling uncertainty via fallback and routing strategies

Building agentic workflows with loops and validation

Integrating tool use via function calling

## Use Cases

Knowledge assistants with RAG

News aggregation and summarization

Intelligent chatbots with tool usage

Autonomous agents with self-correction

Multi-step reasoning systems

## Future Improvements

Add evaluation pipelines (LLM-as-judge)

Integrate vector DBs (FAISS, Weaviate)

Add async execution for latency optimization

Deploy as API using FastAPI + Docker

## Tech Stack

- Python
- Haystack
- OpenAI APIs
- Jupyter Notebooks
