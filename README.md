# Chatbot with Tools

A conversational AI assistant built with LangGraph and Claude 3.5 Sonnet, capable of accessing external tools like web search.

## Overview

This project implements a chatbot that:
- Uses Anthropic's Claude 3.5 Sonnet model
- Integrates with the Tavily search API for retrieving real-time information
- Utilizes LangGraph for orchestrating the conversation flow
- Provides a simple CLI interface for interacting with the chatbot

## Architecture

The system is built using the following components:

- **LangGraph**: Manages the conversation flow and tool execution
- **Claude 3.5 Sonnet**: Powers the core conversational capabilities
- **Tavily Search API**: Enables the chatbot to search the web for up-to-date information
- **Tool Node**: Handles the execution of external tools

## Prerequisites

- Python 3.8+
- An Anthropic API key
- A Tavily API key

## Installation

1. Clone the repository
2. Install dependencies:
```
pip install -r requirements.txt
```
3. Create a `.env` file with your API keys:
```
ANTHROPIC_API_KEY=your_anthropic_api_key
TAVILY_API_KEY=your_tavily_api_key
```

## Usage

Run the chatbot with:
```
python main.py
```

Interact with the chatbot through the CLI interface. Type your questions or commands, and the chatbot will respond. The chatbot can search the web for information using the Tavily search integration.

Type 'quit', 'exit', or 'q' to end the conversation.

## Project Structure

- `main.py`: Entry point of the application, handles user input and output
- `graph.py`: Defines the LangGraph conversation flow
- `tools/tavily.py`: Implementation of the Tavily search tool
- `requirements.txt`: Lists project dependencies