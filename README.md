# Simple AI Research Agent

This project is a hands-on exploration of building an AI research agent from scratch using **LangChain** and **Anthropic Claude** as the LLM. The agent can autonomously research user-provided topics using built-in LangChain tools and organize the information into a structured format.

## Features

- Accepts user queries on arbitrary topics
- Uses **DuckDuckGoSearch** and **Wikipedia** tools to gather information
- Parses results into structured data with **Pydantic**
- Saves the final response to a text file using a custom output tool
- Powered by **Anthropic Claude** via LangChain

## Tech Stack

- Python
- LangChain
- Anthropic Claude
- Pydantic

## Getting Started

### Installation

```bash
git clone https://github.com/farrelsp/agent-from-scratch.git
cd agent-from-scratch
pip install -r requirements.txt
```

> Make sure you have access to the Anthropic Claude API and set your API key in the .env file.

### Usage

Run the agent with:

```bash
python main.py
```

The agent will prompt:

```
What can I help you research?
```

Type your topic.
Example input:

```
Iran versus Israel. Save the result to a text file.
```

The agent will:

- Search the web and Wikipedia for relevant information
- Parse and structure the data using Pydantic
- Save the summary to `research`.txt
