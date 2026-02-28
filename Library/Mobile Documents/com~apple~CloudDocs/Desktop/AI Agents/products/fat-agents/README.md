# AI Agents - Self-Contained Marketing Intelligence Suite

4 plug-and-play AI agents with all proprietary skills, frameworks, and SOPs baked in. Each agent comes in two formats: a **project folder** for AI IDEs and a **single file** for chat platforms.

## The 4 Agents

| Agent | What It Does | Folder | Single File |
|-------|-------------|--------|-------------|
| **Pipeline Agent** | Autonomous orchestrator that chains Research → Fulfillment and/or Outreach automatically. Contains ALL skills from all 3 agents. No manual copy-paste between agents. | `pipeline-agent/` | N/A (folder only) |
| **Research Agent** | Deep market intelligence: avatars, voice analysis, competitive landscape, positioning strategy, keyword intel, SEO audit, AI SEO | `research-agent/` | `RESEARCH-AGENT.md` (297 KB) |
| **Fulfillment Agent** | Production-ready marketing assets: VSL scripts, ad copy, email sequences, landing pages, challenge/webinar funnels, marketing psychology, copy editing, launch strategy | `fulfillment-agent/` | `FULFILLMENT-AGENT.md` (1,030 KB) |
| **Outreach Agent** | Dream 100 deliverable builder: bespoke landing pages, deliverable hubs, Gamma decks, Loom scripts, 10-touch email sequences, sales enablement | `outreach-agent/` | `OUTREACH-AGENT.md` (190 KB) |

## Quick Start

### For AI IDEs (Claude Code, Cursor, OpenClaw, Gemini Antigravity) -- RECOMMENDED

1. **Copy the agent folder** (e.g., `pipeline-agent/` or `research-agent/`) to wherever you want to work
2. **Open it as a project** in your AI IDE
3. The instruction file loads automatically (`CLAUDE.md` for Claude Code, `AGENTS.md` for OpenClaw, `GEMINI.md` for Gemini Antigravity)
4. Start a new conversation and use one of the "Getting Started" prompts

The agent will automatically load skill files from `skills/` as needed, save deliverables to `deliverables/`, and use web search for live research.

**Standalone agent folder structure:**
```
research-agent/          (or fulfillment-agent/ or outreach-agent/)
├── CLAUDE.md            # Agent instructions (Claude Code)
├── AGENTS.md            # Agent instructions (OpenClaw)
├── GEMINI.md            # Agent instructions (Gemini Antigravity)
├── skills/              # Skill files (agent loads on demand)
├── references/          # Reference materials (agent loads on demand)
├── deliverables/        # Agent saves output here
└── memory/              # Persistent context between sessions
```

**Pipeline agent folder structure:**
```
pipeline-agent/
├── CLAUDE.md            # Orchestration instructions (Claude Code)
├── AGENTS.md            # Orchestration instructions (OpenClaw)
├── GEMINI.md            # Orchestration instructions (Gemini Antigravity)
├── skills/
│   ├── research/        # 8 research skills
│   ├── fulfillment/     # 14 fulfillment skills
│   └── outreach/        # 7 outreach skills
├── references/
│   ├── research/        # Research reference packs
│   ├── fulfillment/     # Fulfillment reference packs
│   └── outreach/        # Outreach reference packs
├── deliverables/
│   ├── research/        # Research outputs
│   ├── fulfillment/     # Fulfillment outputs
│   └── outreach/        # Outreach outputs
└── memory/              # Persistent context between sessions
```

### For Chat Platforms (Claude.ai, ChatGPT, etc.)

1. Open the single-file version (e.g., `RESEARCH-AGENT.md`)
2. Copy the entire contents
3. Paste into your AI tool:
   - **Claude** (claude.ai): Create a new Project, paste into Project Instructions
   - **ChatGPT**: Create a custom GPT, paste into Instructions
4. Start a new conversation

> **Note:** The Fulfillment single file (1,030 KB) exceeds some platforms' context limits. If your platform struggles with it, use the folder version instead.

### Step 3: Use the Getting Started Prompts
Each agent has a "Getting Started" section with copy-paste prompt templates. Pick the mode you need, fill in your business details, and let the agent work.

## Recommended Workflow

### Option A: Pipeline Agent (Autonomous -- RECOMMENDED)

Use the Pipeline Agent to run the entire workflow automatically. No copy-pasting between agents.

```
Pipeline Agent
    |
    Phase 1: Research (runs automatically)
    |
    Phase 2: Auto-Route (analyzes your request)
    |
    Phase 3: Execute
    ├── Fulfillment (marketing assets)
    ├── Outreach (D100 deliverables)
    └── Both (full pipeline)
```

Just tell the Pipeline Agent what you need and it handles the rest.

### Option B: Standalone Agents (Manual)

Run agents individually with manual copy-paste between them.

```
Research Agent (run first)
    |
    |-- Copy the Research Brief output
    |
    v
Fulfillment Agent              Outreach Agent
(paste Research Brief here)    (paste Outreach Intel here)
    |                              |
    v                              v
Marketing Assets               D100 Deliverable Packages
(VSL, ads, emails,             (landing pages, hubs,
 landing pages, funnels)        Loom scripts, email sequences)
```

1. **Run Research first** to get your avatar, voice analysis, positioning, and competitive intel
2. **Copy the output** from the Research Agent
3. **Paste it into Fulfillment** to create marketing assets informed by deep research
4. **Paste it into Outreach** to create hyper-personalized D100 deliverables for prospects

You can also use each agent standalone -- just provide your business details in the first prompt.

## What's Inside Each Agent

**Pipeline Agent** (29 skills, 15 reference packs -- all 3 agents combined)
- Everything from Research + Fulfillment + Outreach in one autonomous package
- 3-phase orchestration protocol with auto-routing
- Phase-based skill loading (stays within context limits by only loading skills for the current phase)

**Research Agent** (8 skills, 2 reference packs, 16 sections total)
- Market research frameworks, keyword research, positioning strategy (Dunford, Schwartz, Hormozi), audience research modules, output templates, competitor/alternatives analysis, SEO audit, 139 marketing ideas, AI SEO (answer engine optimization), brand voice analysis

**Fulfillment Agent** (14 skills, 6 reference packs, 23 sections total)
- 10 master copywriter profiles (Ogilvy, Schwartz, Halbert, Hopkins, Kennedy, Collier, Carlton, Abraham, Bencivenga, Sugarman), NLP patterns, VSL scripting, Meta ad strategy, email flows, sales closing, offer creation, landing pages, challenge funnels, webinar scripting, 70+ marketing psychology models, 7-sweep copy editing system, launch strategy, confirmation pages, web3 design system, 50+ quality gates

**Outreach Agent** (7 skills, 7 reference packs, 14 sections total)
- Dream 100 methodology, 8-step deliverable workflow, cold email craft, spam protection, prospect research, 18 SOPs from D100 and Sell More Online training, Gamma templates, Cinematic Loom scripting, sales enablement collateral, landing pages with web3 design, confirmation pages, direct response copy, 50+ quality gates

## Agent Mode Features (Folder Versions)

When using the folder versions in an AI IDE, the agents automatically:

- **Load skills on demand** -- only reads the skill files needed for your specific task
- **Save deliverables to files** -- outputs go to `deliverables/` as organized markdown files
- **Use web search** -- researches your website, competitors, and market in real-time
- **Maintain memory** -- saves business context to `memory/` for continuity across sessions
- **Stay within context limits** -- CLAUDE.md is lightweight (~7-37K tokens), leaving maximum room for conversation

## Rebuilding the Agents

If source files are updated, rebuild with:

```bash
# Build both single-file and folder versions (default)
python3 execution/build_fat_agent.py all

# Build only single-file versions
python3 execution/build_fat_agent.py all --single-file

# Build only folder versions
python3 execution/build_fat_agent.py all --folder

# Rebuild a single agent
python3 execution/build_fat_agent.py research
python3 execution/build_fat_agent.py fulfillment
python3 execution/build_fat_agent.py outreach
python3 execution/build_fat_agent.py pipeline --folder
```
