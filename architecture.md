# Architecture of Hackathon Idea Finder

## Purpose

Hackathon Idea Finder is a focused agent-based application designed to help users discover relevant hackathon project ideas quickly. The system is built around a small network of specialized agents that collaborate to generate ideas in different domains such as Market, Healthcare, Finance, and Travel.

## What the project is trying to do

The goal of this project is to make idea generation more structured and domain-aware. Instead of returning one generic answer, the application helps users by:

- understanding the request
- selecting relevant domains
- delegating work to specialist agents
- combining their outputs into a useful final response

## Main files and components

### Registry definition

The core behavior of the project lives in [registries/basic/hackathon_idea_finder.hocon](registries/basic/hackathon_idea_finder.hocon).

This file defines the complete agent network, including:

- the main orchestrator agent named HackathonIdeaFinder
- domain-focused agents such as MarketArea, HealthCareArea, FinanceArea, and TravelArea
- instructions for each agent
- the flow of control between the orchestrator and specialist agents

### Documentation files

The project also includes supporting documentation files:

- [docs/examples/basic/hackathon_idea_finder.md](docs/examples/basic/hackathon_idea_finder.md)
- [summary.md](summary.md)

These files help explain how the example works and what the project is intended to demonstrate.

## Flow of the system

The workflow is intentionally simple and modular:

1. A user submits a request for hackathon ideas.
2. The main orchestrator agent receives the request.
3. The orchestrator decides which domain-specific agents should handle the request.
4. Each specialist agent generates ideas within its own area.
5. The orchestrator combines those outputs into a final answer for the user.

## Agentic system design

This project is a clear example of an agentic system because it uses multiple cooperating agents rather than a single static response model.

### Why this is agentic

The design highlights several important agentic characteristics:

- specialization: each agent has a clear role
- delegation: the main agent sends work to the most relevant specialist
- coordination: results from different agents are merged into one response
- instruction-driven behavior: each agent follows defined rules and prompts
- extensibility: new domains can be added by adding new agents

## How the project achieves its goal

The project achieves its goal by combining orchestration with domain-specific expertise. The orchestrator provides the entry point and coordination layer, while the specialist agents contribute focused suggestions. This creates a more thoughtful and structured brainstorming experience for the user.

## Summary

Hackathon Idea Finder demonstrates how a small multi-agent system can be used to solve a creative task such as generating hackathon ideas. By routing the request through specialized agents and combining their responses, the project shows the practical value of an agentic workflow in a simple and understandable way.
