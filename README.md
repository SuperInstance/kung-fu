# Kung-Fu

> *"I know Kung-Fu."*
>
> *"Show me."*
>
> — Neo & Morpheus, The Matrix (1999)

When your agent encounters an unfamiliar API or tool, it typically struggles. You find yourself pasting documentation and correcting the same mistakes. Kung-Fu addresses this by enabling agents to learn new capabilities on demand.

This is a meta-skill for the Cocapn Fleet—a skill that allows your agent to learn other skills autonomously. When your agent identifies a knowledge gap, it can discover, validate, and temporarily install the required expertise, then unload it when done.

## How It Works

Kung-Fu operates in two stages:

1. **Local Search**: Your agent first checks a curated set of 675+ verified skills from 15 repositories, including sources like Anthropic, Microsoft, and Trail of Bits, covering areas from API development to security audits.

2. **Remote Search**: If the local repository doesn't have the needed skill, it queries a public index of over 71,000 skills. Each skill is validated against the fleet trust index before being loaded.

Skills are ephemeral—loaded for a specific task and then removed to prevent bloat.

## Usage

Once installed, the process is automatic. When your agent encounters an unfamiliar domain:
1. It recognizes the knowledge gap.
2. It searches locally, then remotely if necessary.
3. It presents the skill it intends to load for your approval.
4. It installs the skill, uses it, and then unloads it.

No special prompts or commands are required.

## Installation

Install the Kung-Fu skill into your agent runtime:

```bash
npx -y add-skill johnhenry/kung-fu -y -a claude-code --skill kung-fu
```

To preview available verified skills first:
```bash
npx -y add-skill johnhenry/kung-fu --list
```

## Limitations

Kung-Fu relies on the availability and quality of skills in the public index. While skills are validated, performance can vary based on the specific skill's documentation and the agent's ability to interpret it correctly for complex tasks.

## Attribution

Kung-Fu is maintained by Superinstance & Lucineer (DiGennaro et al.). It is part of the Cocapn Fleet, an open-source agent runtime and fleet protocol.

---

<div>
  <a href="https://the-fleet.casey-digennaro.workers.dev">The Fleet</a> • 
  <a href="https://cocapn.ai">Cocapn</a>
</div>