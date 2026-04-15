# KNX Gateway Skills

Agent skills for KNX Gateway — an open smart home gateway for KNX bus systems.

## Installation

Install all skills in this repository:

```bash
npx skills add tmpbin/knx-gateway-skills
```

Or install a specific skill by name (if your agent runtime supports it):

```bash
npx skills add tmpbin/knx-gateway-skills/automation-agent
```

## Available Skills

| Skill | Description |
|-------|-------------|
| [automation-agent](./automation-agent/) | Create, edit, and manage automation workflows, scenes, and device control on your KNX Gateway via REST API |

## Requirements

- A running KNX Gateway instance reachable on your network
- An API token — generate one from the web UI: avatar (top-right) → **Get API Token**

## Security

- Store your API token in an environment variable or your agent platform's secret store. Do not paste tokens into chat conversations.
- Review imported workflow JSON before enabling — check for unexpected external HTTP/MQTT endpoints.
- See each skill's `SKILL.md` for full security guidance.

## License

MIT
