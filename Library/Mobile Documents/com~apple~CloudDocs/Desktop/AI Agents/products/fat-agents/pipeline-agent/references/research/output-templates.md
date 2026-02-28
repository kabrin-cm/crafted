
---

## 10. OUTPUT TEMPLATES

### 10A. Knowledge Base Template
Use this structure when producing a full research brief:

# Client Knowledge File

> This file contains all client-specific context for the Research Agent. Fill this during the onboarding process using Tally form data, call transcript, and any provided materials. Every field includes its source in parentheses so builders know where to find the data.

---

## Business Overview

- **Company name:** [from Tally Q3: "What is your business name? Do you have a website?"]
- **Website:** [from Tally Q3, extract URL]
- **Industry:** [from Tally Q4: "What industry are you in?"]
- **What they sell:** [from Tally Q5: "What do you sell?"]
- **Revenue range:** [from Tally Q12: monthly revenue]
- **Team size:** [from Tally Q13: "How many people work in your business?"]
- **Business model:** [inferred from industry + what they sell, e.g., "B2B service agency", "DTC e-commerce", "coaching/consulting"]

## Offer Details

- **Core offer:** [synthesized from Tally + call transcript. What specifically they sell, to whom, at what price]
- **Price point:** [from call transcript or website]
- **Guarantee:** [from call transcript or website. If none, note "no guarantee offered"]
- **Delivery method:** [from call transcript. How they deliver the service/product, e.g., "1-on-1 coaching via Zoom", "self-paced course in Kajabi", "done-for-you service"]
- **Unique mechanism:** [from call transcript. What makes their approach different from competitors. If not articulated, leave blank and flag as "STRATEGIC OPPORTUNITY: client has not defined a unique mechanism yet"]

## Target Audience

- **Primary audience:** [synthesized from industry + offer + call transcript. Be specific: "Marketing agency owners doing $20K-$100K/mo who want to scale past $250K" not just "business owners"]
- **Secondary audience:** [if applicable. Often a sub-segment or adjacent audience]
- **Geographic focus:** [from call transcript or inferred. "US only", "English-speaking markets", "Global"]
- **Audience size estimate:** [from market research during build. Fill this after running the agent, not before]

## Current Operations

- **Top time-consuming tasks:** [from Tally Q8: "List 3-5 tasks that take you the most time"]
  1. [Task 1]
  2. [Task 2]
  3. [Task 3]
  4. [Task 4, if provided]
  5. [Task 5, if provided]
- **Current tools:** [from Tally Q9: "What tools or platforms do you currently use?" List all tools mentioned]
- **AI experience level:** [from Tally Q10. Map to one of: beginner (never used AI tools), intermediate (uses ChatGPT/Claude occasionally), advanced (has built prompts or workflows)]
- **Current workflow bottlenecks:** [from call transcript. Where manual work creates friction, slows delivery, or limits capacity]
- **Client acquisition method:** [from call transcript. How they get customers now: referrals, organic content, paid ads, cold outreach, partnerships, etc.]

## Goals and Priorities

- **90-day goals:** [from Tally Q11: "Top 3 business goals for the next 90 days"]
  1. [Goal 1]
  2. [Goal 2]
  3. [Goal 3]
- **Number one automation priority:** [from Tally Q12: "If you could wave a magic wand and automate one thing in your business, what would it be?"]
- **Why they chose you:** [What made them decide to work with you?]
- **Agreed-upon agent priorities:** [from onboarding call. What agents they want built and in what order. Example: "1. Research agent, 2. Content writer, 3. Ad strategist"]

## Competitors

- **Competitor 1:** [name, URL, brief description of what they offer and who they target]
- **Competitor 2:** [name, URL, brief description]
- **Competitor 3:** [name, URL, brief description]
- **How client differentiates:** [from call transcript. How they describe being different. Capture their exact words where possible]
- **Additional competitors identified during research:** [leave blank. The agent will fill this during the research process]

## Voice and Brand Notes

- **How they describe their business:** [capture their exact words from call transcript. These phrases reveal how they think about their positioning]
- **Key phrases they use:** [words or phrases they repeated during the call. These become inputs for the Voice DNA deliverable]
- **Formality level:** [from their website and social content. Rate as: formal, professional-casual, casual, informal]
- **Content they've shared:** [list any reference materials, examples, or samples they provided during onboarding]
- **Website copy tone:** [brief analysis of how their website sounds. Example: "Professional but approachable. Uses second person. Short paragraphs. Minimal jargon."]

---

## Research Configuration

### Module Selection

- **research focus areas:** [list of active research modules, auto-selected based on client tasks and goals]
  - Example: `["audience-research", "paid-ads", "content-strategy"]`
  - Module selection logic:
    - Tasks or goals mention "outreach", "dream 100", "leads", or "prospecting" --> add `outreach-intel`
    - Tasks or goals mention "copy", "scripts", "writing", "content", or "social media" --> add `content-strategy`
    - Tasks or goals mention "ads", "campaigns", "creative", or "media buying" --> add `paid-ads`
    - Tasks or goals mention "research", "data", "analysis", or "market" --> add `audience-research`
    - Default: always include `audience-research` (core module)

### Research Depth

- **research_depth:** [tier 1 / tier 2 / tier 3]
  - Tier 1 (Onboarding Sprint): Standard depth for all new clients during the 5-day build
  - Tier 2 (Standard): For clients requesting deeper research or operating in competitive niches
  - Tier 3 (Deep): For premium engagements, large markets, or high-stakes positioning decisions

### Research Focus

- **priority_research_areas:** [what to focus on first, from call transcript. Example: "competitor pricing models", "audience objections to coaching programs", "content gaps in the DTC supplement space"]
- **known_competitors:** [pre-identified competitors to start with. Include any the client mentioned by name]
- **specific_research_questions:** [any specific questions the client asked during onboarding. Example: "Why are my ads converting at half the industry benchmark?", "What are people saying about my competitors on Reddit?"]

---

## Data Sources

| Source | Status | Notes |
|--------|--------|-------|
| Tally form | [complete/partial/missing] | Submission ID: [TALLY_SUBMISSION_ID] |
| Onboarding call transcript | [available/not available] | Call date: [DATE] |
| Client website | [URL] | [analyzed/pending analysis] |
| Social media profiles | [list all profile URLs] | [analyzed/pending analysis] |
| Provided materials | [list any docs, examples, references shared] | [reviewed/pending review] |

---

## Agent Build Notes

- **Agent name:** [the client-facing name for this agent, e.g., "Market Scout", "Intel Engine", "Research HQ". Not generic "Research Agent"]
- **Build date:** [YYYY-MM-DD]
- **Builder:** [name of the person who built and configured this agent]
- **Last updated:** [YYYY-MM-DD]
- **Quality score:** [Leave blank until first review. Target: 4.0+]
- **Calibration notes:** [any adjustments made after initial test run. Document what was changed and why]

### 10B. Blueprint Template
Use this structure when producing a strategic blueprint:

# [YOUR BUSINESS NAME] Agent Blueprint

> Your personalized AI agent system, designed from your onboarding call on [ONBOARDING_DATE].

---

## Your Business at a Glance

| | |
|---|---|
| **Business** | [COMPANY_NAME] |
| **Industry** | [INDUSTRY] |
| **Revenue** | [REVENUE_RANGE] |
| **Core Offer** | [WHAT_THEY_SELL] |
| **Growth Goal** | [PRIMARY_90_DAY_GOAL] |

---

## Your Agent Stack

These are the AI agents we are building for your business, in priority order.

### Agent 1: [AGENT_NAME] (Research and Intelligence)

**What it does:** Conducts deep market research, competitor analysis, and audience intelligence for [SPECIFIC_USE_CASE]. Produces a complete market dossier, audience avatars, competitor matrix, voice-of-customer database, and strategic recommendations.

**Replaces:** [MANUAL_TASK_IT_REPLACES, e.g., "8-10 hours of manual competitor research per client onboarding"]

**Time saved:** [HOURS_PER_WEEK] hours/week

**Research modules active:** [LIST_OF_ACTIVE_MODULES, e.g., "audience-research, paid-ads, content-strategy"]

### Agent 2: [AGENT_NAME] ([AGENT_TYPE])

**What it does:** [SPECIFIC_DESCRIPTION_OF_WHAT_THIS_AGENT_PRODUCES]

**Replaces:** [MANUAL_TASK_IT_REPLACES]

**Time saved:** [HOURS_PER_WEEK] hours/week

### Agent 3: [AGENT_NAME] ([AGENT_TYPE])

**What it does:** [SPECIFIC_DESCRIPTION_OF_WHAT_THIS_AGENT_PRODUCES]

**Replaces:** [MANUAL_TASK_IT_REPLACES]

**Time saved:** [HOURS_PER_WEEK] hours/week

---

## Build Timeline

| Day | What Happens | Your Role |
|-----|-------------|-----------|
| Day 1 | Research agent built and tested with your real business data | None. We handle it. |
| Day 2 | Agent calibrated based on initial output review | Review the first output in your project channel |
| Day 3 | Research agent deployed. Agent 2 build begins. | Give feedback on research quality |
| Day 4 | Agent 2 built and tested | Review Agent 2 output |
| Day 5 | All agents deployed, tested, and packaged | Final review and go live |

---

## What You Will Receive

1. **Custom AI agents** configured for your business, your voice, and your workflows
2. **Research dossier** with market intelligence, competitor analysis, and audience insights you can act on immediately
3. **Voice profile** extracted from your existing content, so every agent sounds like you wrote the output yourself
4. **Agent exports** for multiple platforms (Claude, ChatGPT, Cursor) so you can use them wherever you work
5. **Training walkthrough** so you can operate, adjust, and refine your agents independently after the build

---

## What We Need From You

Before your build starts, please complete these items:

- [ ] Claude Pro subscription active ($20/mo at claude.ai)
- [ ] Reference materials posted in your project channel. This includes: examples of your work, content you like, client testimonials, and anything that shows how your business sounds.
- [ ] Respond to any questions we post in your project channel within 24 hours

Quick responses keep us on schedule. The 5-day build timeline depends on same-day feedback during review checkpoints on Days 2 and 4.

---

## What Success Looks Like

By Day 30, you should see measurable improvements in these areas:

- [METRIC_1, e.g., "Research tasks that used to take 8 hours now complete in 30 minutes"]
- [METRIC_2, e.g., "Consistent content output across all platforms, using your actual voice"]
- [METRIC_3, e.g., "Competitor intelligence updated weekly instead of quarterly"]

We will check in at Day 14 and Day 30 to measure progress against these benchmarks. If any agent is underperforming, we recalibrate.

---


*Questions? Message us in your project channel.*
*Build starts: [START_DATE]*
