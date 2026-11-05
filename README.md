# unslop-business

**A design skill for coding agents that build premium, clean business websites.**

`unslop-business` helps AI coding agents work like a thoughtful brand designer, UX strategist, and frontend engineer—not a template generator. Its mandatory uniqueness protocol requires a business-specific design fingerprint and a logo-swap test so unrelated businesses do not receive the same layout with superficial changes.

It is designed for business websites including:
- Cafes, restaurants, hospitality, and food brands
- Fashion, retail, and product storefronts
- Premium service businesses
- Brand and company websites
- Local businesses and experience-led businesses

The skill uses reference websites as design research. It extracts useful principles—such as editorial storytelling, image direction, product discovery, typography, navigation, and conversion patterns—and translates them into an original design for the user's business.

## Reference inspiration

The initial reference set supplied for this project:

| Website | Useful design lessons to investigate |
|---|---|
| [Roastery Coffee House](https://roasterycoffee.co.in/) | Specialty brand storytelling, café discovery, retail and hospitality working together |
| [Boojee Cafe](https://boojeecafe.com/) | Product-led discovery, café locations, subscriptions, commerce navigation |
| [Blackberrys](https://blackberrys.com/) | Large retail taxonomy, collection navigation, merchandising and product grids |
| [Cravin' by Andy](https://www.cravinbyandy.com/) | Hospitality storytelling, menu and location discovery, experience-led content |
| [Beta Coffee](https://betacoffee.com.au/) | Concise editorial copy, strong information hierarchy, distinctive business positioning |

These are inspiration and research examples, not layouts to copy. The skill is dynamic: users can supply completely different reference URLs for each project.

## Installation

This repository follows the open Agent Skills convention: a skill directory contains a `SKILL.md` file with YAML frontmatter and instructions.

### Claude Code

Place the skill directory in your project's `.claude/skills/` folder:

```text
your-project/
└── .claude/
    └── skills/
        └── unslop-business/
            ├── SKILL.md
            └── references/
```

You can also install it in your personal skills directory if preferred by your Claude Code setup.

### Codex

Place the skill directory in `.agents/skills/` in the repository:

```text
your-project/
└── .agents/
    └── skills/
        └── unslop-business/
            ├── SKILL.md
            └── references/
```

Codex can discover project skills from `.agents/skills/`.

### Google Antigravity

Add the skill folder to the skills directory supported by your Antigravity installation/workspace, or follow the current Antigravity documentation for importing Agent Skills. Availability and discovery paths can vary by release.

### Other agents

Any coding agent that supports the Agent Skills format can use the `SKILL.md` instructions. Copy the complete `unslop-business/` folder into that agent's configured skills directory.

## How to use

After installation, ask your coding agent something like:

> Use the unslop-business skill to build a premium website for my specialty bakery. Study these reference websites first: [URLs]. The site should focus on online orders and store visits. Use the existing project stack.

Or:

> Redesign this business website using unslop-business. Keep the current framework, inspect the existing code, and make the design feel editorial, premium, and distinctive. Prioritize mobile usability and booking enquiries.

Give the agent:
1. Business name and what it does.
2. Target audience and location/market.
3. Main action visitors should take.
4. Pages or sections required.
5. Reference URLs (optional).
6. Existing brand assets, copy, and technical constraints.

The agent should inspect references, synthesize a design direction, establish design tokens, implement, and visually review the result.

## What's included

```text
unslop-business/
├── SKILL.md
├── README.md
├── LICENSE
├── references/
│   ├── reference-analysis.md
│   ├── design-system.md
│   ├── business-patterns.md
│   ├── visual-quality-checklist.md
│   └── reference-sites.md
└── workflows/
    ├── inspect-references.md
    ├── plan-and-design.md
    └── implement-and-review.md
```

## Important notes

- The skill does not bundle or redistribute assets from the reference websites.
- The skill cannot guarantee browser access or visual inspection; the agent must report limitations honestly.
- The quality of the output depends on the agent's browser, coding, and screenshot capabilities.
- SEO is intentionally out of scope for this initial version and can be added later.

## License

MIT. See [LICENSE](LICENSE).


## Uniqueness is mandatory

Every project must create a Design Identity Record before coding. The agent must reconsider the composition, information architecture, typography, image direction, and section sequence for each business. Merely swapping a logo, colors, photos, and copy is not acceptable.

The skill also includes a logo-swap test: if the same design could serve an unrelated business with only superficial changes, the agent must rethink it.

**Honest limitation:** a standalone skill cannot know what every agent has built for every other user. It cannot mathematically guarantee global uniqueness across separate users or sessions unless the agent has access to a shared project history or design registry. It does, however, enforce project-specific design decisions and comparison against any prior work available in the current workspace/context.
