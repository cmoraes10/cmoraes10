# Cauã Moraes

Backend developer from Salvador, Brazil. I run **MoWave**, the software studio behind **[Lima](https://getlima.app)**, an AI agent that acts on your calendar, tasks, habits and money instead of answering questions about them. Launching October 2026.

Day to day I live in Java and Spring Boot, with Python for data work and Flutter on the mobile side. Most of my time goes into agent design: how a model picks the right tool, what it should remember about you, and when it should just do the thing instead of asking.

### Tech I work with

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

### Agent memory, open source

**[loci](https://github.com/cmoraes10/loci)** · `pip install mowave-loci` · An agent that forgets you every session is a search box with manners. Loci is the layer that fixes that: durable facts about a person, typed and ranked, extracted from the conversation rather than typed into a settings page, consolidated daily so the list does not rot.

- Eight categories, four importance tiers, a status lifecycle
- Extraction on two paths — a model reads for meaning, regex catches what it misses, merged with model precedence
- A write filter that drops passing mood, and a cap so twelve facts reach the model instead of four hundred
- Stored text is neutralised before injection, because a memory layer is a prompt-injection surface
- One core with no dependencies, an MCP server for any client, and a Hermes plugin for automatic extraction

**[loci-decisions-agent](https://github.com/cmoraes10/loci-decisions-agent)** · The agent that proves it. Once a day it asks loci what is due for review, texts you one question per fact, reads your answer in plain Portuguese and updates the store. Without memory it does nothing at all, which is the point.

### What I'm building

**[Lima](https://getlima.app)** keeps your calendar, tasks, habits, focus and money in one place, with an agent on top that can actually act on all of it. Ask about a flight and it checks whether the date is clear and whether the money is really there before answering.

A few pieces I enjoyed building:

- **65 tools** behind native function calling, with a bounded loop and parallel execution inside a single iteration
- **Specialized subagents** behind a keyword classifier that routes in under 5ms with no model cost, falling back silently to the generalist
- **Open Finance** through Pluggy across 200+ banks, so the agent reasons over real balances instead of numbers you typed in
- Voice, image and document input on one engine, with no separate transcription or OCR service

Java 21 and Spring Boot on the backend, Flutter on mobile. WhatsApp is built and waiting on platform approval.

### Other things I have built

- **[Cassandra](https://github.com/cmoraes10/cassandra)** · Monte Carlo and Markov chain simulations that map where a stock price can go, with backtesting and risk controls. `Python`
- **[Penumbra](https://github.com/cmoraes10/penumbra)** · Open-data index of the most overlooked municipalities in Bahia, plotted on an interactive map of the cocoa region. `Python`
- **[reconhecimento_sono](https://github.com/cmoraes10/reconhecimento_sono)** · Computer vision that notices when someone starts falling asleep and fires an alarm. `Python`
- **[tomorrowUFBA](https://github.com/cmoraes10/tomorrowUFBA)** · Led a team of 8 and won UFBA's programming competition with this one. `HTML`

Most of Lima lives in a private repo, so what is public here is only part of the picture.

### Where to find me

[![Lima](https://img.shields.io/badge/Lima-getlima.app-e8a838?style=flat-square&logo=googlechrome&logoColor=white)](https://getlima.app)
[![PyPI](https://img.shields.io/badge/PyPI-mowave--loci-3775A9?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/mowave-loci/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/cauamoraesaraujo)
