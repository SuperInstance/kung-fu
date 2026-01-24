# Kung-Fu

> *"I know Kung-Fu."*
>
> *"Show me."*
>
> — Neo & Morpheus, The Matrix (1999)

## What if you could download knowledge directly into your brain?

In The Matrix, Neo sits in a chair, cables jack into his skull, and seconds later he opens his eyes with complete mastery of martial arts. No years of training. No endless practice. Just... **knowledge transfer**.

This skill brings that concept to AI coding agents.

## The Construct

Kung-fu is a **meta-skill** — a skill that teaches your agent how to learn other skills. Once installed, your agent can discover, evaluate, and install any skill it needs on demand.

Need to build a Flask API? *Upload Flask knowledge.* Deploying to Azure? *Upload Azure skills.* Writing smart contracts? *Upload security audit expertise.*

```
Tank, I need a pilot program for a React application.

Loading...

I know React.
```

## How It Works

### The Local Dojo (Known Skills)

Your agent first searches through **675+ validated skills** across 15 curated repositories:

| Source | Skills | Specialty |
|--------|--------|-----------|
| Anthropic | 30 | Documents, MCP, creative |
| Microsoft | 13 | Azure AI, FastAPI |
| Trail of Bits | 45 | Security audits |
| Scientific | 142 | Bioinformatics, astronomy |
| Community | 445+ | Everything else |

### The Matrix (Remote Search)

If the local dojo doesn't have what you need, jack into the Matrix — a global index of **71,000+ skills** at [skills.sh](https://skills.sh):

```bash
curl -s "https://skills.sh/api/search?q=kung-fu&limit=10"
```

## Usage

Once installed, your agent automatically gains the ability to learn. When it encounters an unfamiliar domain:

1. **Agent recognizes the gap** — "I need to work with Terraform but lack expertise"
2. **Agent searches for skills** — First local repositories, then remote if needed
3. **Skills are uploaded** — Relevant knowledge is installed via `add-skill` CLI
4. **Agent opens its eyes** — "I know Terraform."

The skill activates whenever your agent needs capabilities it doesn't have. No slash command required — it's always watching, always ready to learn.

## The Red Pill

```bash
# Install the kung-fu skill
npx -y add-skill johnhenry/kung-fu -y -a claude-code --skill kung-fu
```

Or preview what you're about to download:

```bash
# List available skills
npx -y add-skill johnhenry/kung-fu --list
```

Once installed, your agent gains the ability to teach itself anything it needs to know.

## Philosophy

> *"I'm trying to free your mind, Neo. But I can only show you the door. You're the one that has to walk through it."*

This skill doesn't make your agent omniscient. It gives your agent the **awareness** that knowledge exists and the **ability** to acquire it on demand. The agent still decides what to learn and when.

The difference between a good agent and a great one isn't what it knows — it's knowing that it *can* know more.

## There Is No Spoon

Traditional development: Learn a framework over months, practice for years, become an expert.

Kung-fu development: Need expertise? Download it. Move on. Ship.

The skills aren't real in the sense that they're not permanent parts of your agent's training. They're loaded on demand, used for the task, then cleaned up. Like programs in the Matrix — real enough to be useful, ephemeral enough to be replaceable.

---

*"What are you trying to tell me? That I can write production code in any framework?"*

*"No, Neo. I'm trying to tell you that when you're ready... you won't have to."*

---

## License

MIT

Free your mind.
