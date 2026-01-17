# 🧭 Fortune Compass Agent

An AI-powered fortune telling divination Agent (ChatGPT App/MCP) that integrates traditional **Tarot**, **Zhouyi (I Ching)**, and **Guangong Oracle** into a unified digital experience. The agent performs real-world drawing logic (shuffling and orientation) and uses LLM intelligence to interpret the results. 

Deploy at [DeepNLP Agent Workspalce](https://deepnlp.org/workspace/deploy) and Live URL [https://derekzz.aiagenta2z.com/fortune-compass-agent/mcp](https://derekzz.aiagenta2z.com/fortune-compass-agent/mcp)

---

## 🔮 Divination Methods

### 🃏 Tarot
* **Complete Deck:** Randomly draws from all 78 cards.
* **Orientation Logic:** 1. Simulates a physical draw with a 50/50 chance.
    2. If `0`: Display the **Upright** meaning.
    3. If `1`: Display the **Reversed** meaning.
* **Example Prompt:** *"What should I focus on to succeed in my career right now?"*


### ☯️ Zhouyi (I Ching)
* **Hexagram Generation:** Generates a 6-line hexagram using randomized binary logic ($2^6 = 64$ combinations).
* **Binary Mapping:** Maps results to specific assets based on binary strings (e.g., `000000.jpg`).

### 🏮 Guangong Oracle
* **Divine Lots:** Traditional temple-style randomized draws for spiritual guidance.

---

## 🚀 Getting Started

### 1. Installation & Build
Install dependencies and compile the TypeScript source code into executable JavaScript:

```bash
pnpm install
pnpm build
```


```bash
# Start the static file server (Port 4444)
pnpm run serve &
# Start the main agent server
pnpm start
```

Change port
```bash
PORT=7104 pnpm start
```


### 2. Tool
The agent exposes the following primary tool to the LLM:

`tell_fortune`: Tell Your Fortune by Divination via Tarot, ZhouYi, or Guangong Drawing and Asking
prompt: The question you want to ask
method: all,tarot,zhouyi,guangong


### 3. Deployment

Deploy to [DeepNLP Workspalce](https://deepnlp.org/workspace/deploy) and Live URL(https://derekzz.aiagenta2z.fortune-compass-agent/mcp)


