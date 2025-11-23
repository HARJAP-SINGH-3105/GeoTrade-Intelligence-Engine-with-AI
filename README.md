AI-Powered Geo-Trade Intelligence System Using Neo4j & LLMs

This project explores how AI, graph databases, and macro-economic reasoning can be combined to understand global trade relations among countries. By modeling world trade as an interconnected graph and pairing it with LLM-based analysis, this system enables users to ask natural-language questions and receive data-backed insights on international trade and economic dynamics.

🌍 Project Overview

Global trade is complex — countries influence each other through exports, imports, investments, and macro-economic shifts. This project aims to simplify that complexity by:

Building a graph database of country-to-country trade relationships using Neo4j

Connecting the graph to a multi-agent LLM framework (CrewAI)

Allowing users to query the system through a simple user interface

Producing intelligent, contextual answers that blend factual trade data with economic reasoning

Think of it as:

“If countries were nodes and AI could tell their story.”

📦 Features
1. Graph-Based Trade Model

Countries represented as nodes

Trade relationships modeled as edges

Attributes include:

Export value

Import value

Number of traded products

Trade balance, etc.

2. Multi-Agent AI System

Two agents work together:

Trade Analyst Agent
Fetches factual data from the graph (via Cypher queries), and can call multiple tools/functions.

LLM Advisor
Acts as a macro-economics & geo-trade specialist that interprets the data and forms insights.

Together, they deliver accurate and well-reasoned responses.

3. LlamaIndex Graph Integration

An alternative approach using LlamaIndex graph components (graph store, LLM, embeddings) to provide a more streamlined and efficient pipeline.

4. Natural-Language Querying

Users can ask questions like:

“How does India’s export dependency on China change under rising interest rates?”

“Which countries benefit the most if the US reduces semiconductor imports?”

“What happens to UAE’s trade network if oil prices drop sharply?”

5. Simple User Interface

A text box for asking questions

A results/answer panel

A left-side info panel showing data source, frameworks, and database setup

📊 Data Source

Data is taken from the World Integrated Trade Solution (WITS), maintained by the World Bank.

For the prototype:

Trade summary data of India, China, UAE, and the US

Each country’s top 50 trading partners

Detailed product-level export/import data for India’s top 5 exported products

🗄️ Tech Stack
Backend

Python

Neo4j (Graph Database)

Cypher Query Language

CrewAI (Multi-agent orchestration)

LlamaIndex Graphs (optional alternative pipeline)

Models Used

llama-3.2-vision (Ollama test)

sentence-transformers/all-MiniLM-L6-v2 (embeddings)

Gemini free-tier models (tested but limited by TPM)
