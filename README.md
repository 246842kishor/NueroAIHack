# Hackathon Idea Finder

This project is a simple agent-based example built around the Neuro-San framework. It demonstrates how a main orchestrator agent can delegate requests to specialist agents for different domains such as Market, Healthcare, Finance, and Travel.

## What this project does

The application helps users generate hackathon ideas by routing their request through a small agent network. Each specialist agent contributes domain-specific suggestions, and the orchestrator combines them into a final response.

## Requirements

- Python 3.10 or newer
- pip
- A working internet connection if you want to use the default LLM providers

## Setup instructions

1. Create and activate a virtual environment

   On Windows:

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\activate
   ```

   On macOS/Linux:

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

2. Install the required dependencies

   ```bash
   pip install -r requirements.txt
   ```

3. Configure environment variables

   If needed, create a `.env` file from the example values in the repository and set your API keys for the LLM providers you plan to use.

4. Run the application

   From the project root, start the local server:

   ```bash
   python -m neuro_san_studio run
   ```

5. Open the UI

   Open your browser and go to:

   ```text
   http://localhost:4173/
   ```

## Project structure

- `registries/basic/hackathon_idea_finder.hocon` — the main agent network definition
- `docs/examples/basic/hackathon_idea_finder.md` — example documentation
- `architecture.md` — architecture overview
- `summary.md` — project summary

## Notes

This project is intended as a lightweight example of an agentic workflow. You can extend it by adding more specialist agents or by introducing additional tools and integrations.
