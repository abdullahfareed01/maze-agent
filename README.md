# Autonomous Maze Exploration Agent

## Project Overview

This project implements an autonomous maze-exploring agent using an LLM and Python tool calling.

The agent explores a maze hosted at:
https://maze.edwarddonner.com/

Its objective is to discover room connections, handle dead ends, find the exit, and retrieve the secret message.

## How It Works

1. Python provides a webpage-opening function.
2. The function is exposed to the language model through a JSON tool schema.
3. The language model decides which room to explore next.
4. Python executes the requested webpage calls.
5. The webpage results are returned to the model.
6. The process continues until the exit is found.
7. The agent generates a final exploration report.

## Technologies Used

- Python
- OpenAI-compatible API
- OpenRouter
- NVIDIA Nemotron model
- Requests
- python-dotenv
- import-ipynb
- NetworkX
- Matplotlib
- Jupyter Notebook

## Project Structure

```text
maze_agent/
├── agent_tools.ipynb
├── maze_agent.ipynb
├── maze_map.ipynb
├── requirements.txt
├── README.md
├── .gitignore
└── .env (local only, not committed)