# AI-Powered News Article Generator

This project leverages cutting-edge AI technologies to automate the creation of well-researched, high-quality news articles. By combining specialized AI agents in a sequential workflow, we ensure thorough research followed by engaging writing.

## Technologies Used

### 1. Serper Dev Tool

- **Purpose:** Web scraping and search engine querying
- **Usage:** Our `news_researcher` agent uses Serper to gather the latest and most relevant information on the chosen topic from across the web.
- **Benefits:** Ensures our articles are based on current, authoritative sources.

### 2. Crew AI

- **Purpose:** Orchestrating AI agents for complex tasks
- **Usage:** We use Crew AI to manage our two specialized agents:

1.  `news_researcher`: Gathers and analyzes information
2.  `news_writer`: Crafts engaging news articles

- **Benefits:**
- Modular design for easy expansion
- Sequential processing (`Process.sequential`) for logical flow:
  1.  Research phase
  2.  Writing phase

### 3. Google GEMINI

- **Purpose:** Advanced language model for text generation
- **Usage:** Powers our `news_writer` agent, enabling it to:
- Structure articles effectively
- Write in a journalistic style
- Adapt tone to the topic
- **Benefits:** Produces human-like, engaging news articles

## Workflow: Sequential Process

Our system uses a sequential workflow to ensure each phase is completed before the next begins:

Getting Started

### Install dependencies:

```bash
pip install -r requirements.txt


### Enter your API keys in a .env file:
SERPER_API_KEY=your_key_here
GEMINI_API_KEY=your_key_here
```
