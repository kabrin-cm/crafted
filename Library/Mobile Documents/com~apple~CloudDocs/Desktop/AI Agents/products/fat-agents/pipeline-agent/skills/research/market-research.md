
---

## 6. MARKET RESEARCH (Master Skill)

---
name: market-research
description: "Deep market research across every discoverable source — competitor funnels, Meta Ad Library, YouTube, Reddit, X/Twitter, Amazon reviews, Google SERP, forums, review sites, podcasts, LinkedIn, TikTok. Produces a complete research dossier that feeds every downstream skill. This is the FIRST skill triggered for every client engagement. Triggers on: market research, research this niche, analyze competitors, who is the audience, understand the market, new client research, competitive analysis, ad library, social listening. Outputs: Market Research Dossier, Avatar Profile, Competitor Matrix, Ad Intelligence Report, Voice-of-Customer Database, Objection Map, Opportunity Gap Analysis."
---

# Market Research (Complete Tactical Manual)

> The quality of everything downstream — offer, copy, ads, funnels, emails — is capped by the quality of your research. Bad research = generic output. Deep research = surgical output. This skill is the foundation of the entire system.

## Trigger Keywords

`market research`, `research this niche`, `analyze competitors`, `who is the audience`, `understand the market`, `new client research`, `competitive analysis`, `ad library`, `social listening`, `avatar research`, `voice of customer`, `competitor teardown`, `audience research`, `niche research`, `market intelligence`

---

## Core Job

Produce a comprehensive research dossier for a client (or your own business) that makes every downstream skill dramatically more effective. The dossier covers:

1. **Who the audience actually is** — demographics, psychographics, awareness level, language they use
2. **What competitors are doing** — their funnels, offers, ads, positioning, strengths, weaknesses
3. **What the market is saying** — real conversations on Reddit, X, YouTube, forums, reviews
4. **What ads are running** — Meta Ad Library analysis, creative patterns, scaling signals
5. **Where the opportunities are** — gaps competitors miss, messaging angles nobody's using, objections nobody's addressing

> **Note:** This skill replaces and supersedes the market research prompts previously embedded in vsl-scripting. Those prompts are now here where they belong — at the foundation layer.

---

## Inputs Required

| Input | Required? | Source |
|-------|-----------|--------|
| Client's offer (what they sell, to whom, at what price) | Yes | the business details you provide |
| Industry/niche | Yes | the business details you provide |
| Client website URL | Yes | User |
| 3-5 competitor URLs | Strongly recommended | User or discovered during research |
| Social media profiles | Helpful | User |
| Sales call transcripts (if available) | Highly valuable | User uploads |
| Existing ad accounts / current metrics | Helpful | User |
| Onboarding call recording/transcript | Helpful | User |

---

## The 7-Phase Research Protocol

```
Phase 1: Client Briefing & Existing Intel → Understand what we're working with
Phase 2: Competitor Funnel Teardowns     → Dissect what competitors are doing
Phase 3: Ad Intelligence                 → What's running, what's scaling, what creative patterns exist
Phase 4: Social Listening                → What the market is ACTUALLY saying (Reddit, X, YouTube, forums)
Phase 5: Audience Voice Mining           → Extract exact language, pain points, desires from reviews/comments
Phase 6: Search & Content Intelligence   → What Google says, what content ranks, what questions people ask
Phase 7: Synthesis & Deliverables        → Compile everything into actionable documents
```

---

# PHASE 1: CLIENT BRIEFING & EXISTING INTEL

## Goal
Collect everything the client already knows and everything we can extract from their existing assets before going to external sources.

## Step 1.1: Intake Data Collection

Gather from client or the business details you provide:
- Company name, industry, business model
- Core offer: what, for whom, at what price, with what guarantee
- Delivery method (DFY, coaching, course, software, hybrid)
- Current funnel type (VSL, webinar, challenge, lead form, none)
- Current metrics (CPL, CPA, show rate, close rate, ROAS — whatever exists)
- Revenue range, team size, how long in business
- What's worked before (angles, hooks, campaigns that performed)
- What's failed (and why they think it failed)

## Step 1.2: Scrape Client's Own Assets

**Execution scripts:**
- `directives/execution/scrape_website.py` — scrape client website for messaging, offers, testimonials, funnel pages
- `directives/execution/youtube_transcripts.py` — pull transcripts from client's YouTube content
- `directives/execution/transcribe.py` — transcribe onboarding call recordings

**What to extract:**
- Current homepage headline, subheadline, CTA
- Current offer structure visible on their site
- Testimonials and case studies (with specific numbers)
- Blog/content topics (what do they write about)
- YouTube video titles and themes
- Social media bio, posting patterns, engagement levels

## Step 1.3: Process Sales Call Transcripts (If Available)

If the client provides sales call recordings or transcripts, this is the single most valuable research input. Run the full transcript analysis prompt (see AI Research Prompts section below).

**What transcripts reveal that no other source can:**
- The exact words prospects use to describe their problem
- Objections that come up in real buying conversations
- Questions that reveal what they don't understand
- The emotional state of buyers vs. non-buyers
- What competing solutions they've tried and why they failed
- How they describe the "dream outcome" in their own words

---

# PHASE 2: COMPETITOR FUNNEL TEARDOWNS

## Goal
Understand what competitors are doing — their positioning, offers, funnels, pricing, and messaging — so we can find gaps and differentiate.

## Step 2.1: Identify Competitors

**Start with:**
- Competitors the client names
- Google search: "[niche] + [offer type]" (e.g., "real estate investing course," "B2B lead generation agency")
- Meta Ad Library search for the niche
- YouTube search for the niche
- Reddit mentions of competitors

**Target:** 3-5 direct competitors + 2-3 adjacent/aspirational competitors

## Step 2.2: Funnel Teardown Per Competitor

For each competitor, go through their entire funnel as if you were a prospect:

**Tool:** `directives/execution/scrape_website.py` for each competitor URL, plus manual WebFetch/WebSearch

**Capture:**

```markdown
## [Competitor Name]
**URL:** [website]
**Social:** [IG, YT, X, LinkedIn handles]

### Positioning
- Headline: [exact text]
- Subheadline: [exact text]
- Unique mechanism: [what's their "how"?]
- Primary promise: [what do they promise?]
- Who they target: [who is this for?]

### Offer
- Core product/service: [what]
- Price: [how much]
- Guarantee: [what guarantee, if any]
- Bonuses: [what extras]
- Delivery: [DFY, coaching, course, etc.]

### Funnel Structure
- Traffic sources: [paid ads, organic, D100, etc.]
- Entry point: [lead magnet, VSL, webinar, application]
- Pages in funnel: [list each page and its purpose]
- Call booking: [yes/no, what platform]
- Follow-up visible: [email sequences, retargeting, etc.]

### Social Proof
- Testimonial count: [approximate]
- Case study quality: [specific numbers? vague claims?]
- Trust signals: [logos, media mentions, Trustpilot, etc.]
- Community size: [followers, group members, etc.]

### Content Strategy
- Blog: [active/inactive, topics, posting frequency]
- YouTube: [subscriber count, video frequency, themes]
- Podcast: [yes/no, name]
- Social: [which platforms, posting frequency]

### Strengths
- [What they do well]

### Weaknesses / Gaps
- [What's missing, weak, or exploitable]

### Active Ads (Meta Ad Library)
- Running ads: [yes/no]
- Estimated spend level: [low/medium/high based on # of active ads]
- Creative style: [talking head, UGC, static, B-roll, etc.]
- Primary hooks: [what do their ads lead with]
- Landing page from ads: [what page do ads point to]
```

## Step 2.3: Competitive Positioning Map

After teardowns, synthesize:
- What ALL competitors are saying (the market consensus)
- What NO competitor is saying (messaging gaps)
- Where the client's offer is uniquely positioned
- Claims the client can make that competitors can't
- Proof/evidence the client has that competitors don't

---

# PHASE 3: AD INTELLIGENCE

## Goal
Understand what ads are running in the market, what creative patterns work, what's scaling, and what angles are being used.

## Source 3.1: Meta Ad Library

**How to access:** https://www.facebook.com/ads/library/ — Search by keyword, advertiser name, or topic

**What to capture per competitor:**
- Number of active ads (proxy for spend level)
- Ad creative types (video, static, carousel)
- Hook patterns (what do the first 3 seconds / first line say)
- Body copy patterns (what frameworks — PAS, story, listicle)
- CTA patterns (book a call, learn more, apply now)
- Landing page destinations
- How long ads have been running (longevity = working)
- A/B test variations visible (same ad with different hooks = testing)

**What to look for:**
- **Ads running 90+ days** = proven winners, study these deeply
- **Multiple variations of the same ad** = they're actively testing, the concept works
- **New ads from a big spender** = they're diversifying, market may be saturating on old angles
- **Video vs. static mix** = tells you what format the audience responds to

**Capture at least:**
- Top 3 longest-running ads per competitor (screenshot + transcript of copy)
- Top 3 newest ads per competitor (what are they testing now)
- Common hooks across ALL competitors (pattern = market-validated)
- Hooks NO competitor is using (gap = opportunity)

## Source 3.2: TikTok Creative Center

**How to access:** https://ads.tiktok.com/business/creativecenter/

**What to capture:**
- Top-performing ads in the niche category
- Creative patterns (format, length, style)
- Hook patterns specific to TikTok's audience
- Trending sounds/formats being used in ads

## Source 3.3: YouTube Ads (Pre-Roll)

**How to find:** Watch YouTube content in the niche — note the pre-roll ads that appear. Or search "[competitor name] ad" on YouTube.

**What to capture:**
- Who's advertising on YouTube in this niche
- Ad format (skippable, non-skippable, bumper)
- Hook (first 5 seconds before skip)
- CTA and landing page

## Source 3.4: Google Ads (Search)

**How to find:** Search the primary keywords a prospect would use. Note the sponsored results.

**What to capture:**
- Who's bidding on these keywords
- Their ad copy (headlines, descriptions)
- Landing pages from search ads
- Estimated competitive density (how many advertisers)

---

# PHASE 4: SOCIAL LISTENING

## Goal
Understand what the market is ACTUALLY saying — unfiltered, raw conversations about the problem, the niche, the competitors, and the desired outcomes.

## Source 4.1: Reddit

**Why Reddit is #1 for research:** People on Reddit are brutally honest. They don't perform for an audience. They ask real questions, share real frustrations, and give unfiltered reviews.

**How to search:**
- Google: `site:reddit.com [niche keyword]`
- Google: `site:reddit.com "[competitor name]" review`
- Google: `site:reddit.com "[problem keyword]" help`
- Reddit search within specific subreddits

**Subreddits to find:**
- Search for subreddits related to the niche (e.g., r/realestateinvesting, r/Entrepreneur, r/personalfinance)
- Check the sidebar of relevant subs for related subreddits
- Look at where the target audience posts (not just the niche sub)

**What to capture:**
- **Pain point language:** Exact phrases people use to describe their problems (copy these verbatim — this IS your ad copy)
- **Desired outcomes:** How they describe what they want (in their words, not marketing language)
- **Objections to solutions:** Why they're skeptical of products/courses/services in the niche
- **Competitor mentions:** What people say about specific competitors (positive AND negative)
- **Failed attempts:** What they've tried before and why it didn't work
- **Questions they ask:** These become ad hooks, email subjects, and FAQ content
- **Emotional intensity:** Which topics get the most upvotes, most comments, most heated debate (= highest emotional charge = best ad angles)

**Capture template per thread:**

```markdown
**Thread:** [title]
**Subreddit:** r/[name]
**Upvotes/Comments:** [count]
**Key quotes:**
- "[exact quote]" (pain point)
- "[exact quote]" (desired outcome)
- "[exact quote]" (objection)
**Insight:** [what this tells us]
```

**Minimum:** 15-20 threads, across 3-5 subreddits

## Source 4.2: X (Twitter)

**How to search:**
- X advanced search: https://twitter.com/search-advanced
- Search by keyword, filter by engagement (min likes/retweets)
- Search competitor handles to see what their audience says TO them
- Search niche hashtags

**What to capture:**
- Viral threads about the topic (high engagement = resonant angles)
- Complaints and frustrations expressed in tweets
- What influencers in the space are saying (their angles, positioning)
- Quote tweets of competitor content (reveals audience sentiment)
- Threads where people share results/transformations (social proof language)

**Specific searches to run:**
- `[niche keyword] advice` — what people recommend
- `[niche keyword] scam OR overrated OR waste` — objections and skepticism
- `[niche keyword] changed my life OR best decision` — positive transformation language
- `[competitor name] review OR honest OR truth` — competitor sentiment
- `[problem keyword] frustrated OR tired OR sick of` — pain language

**Minimum:** 10-15 high-engagement tweets/threads

## Source 4.3: YouTube

**Tool:** `directives/execution/youtube_transcripts.py` for transcripts

**What to research:**
1. **Competitor channels** — What content do they produce? What gets the most views? What are their most-commented videos?
2. **Comment sections** — The comment section of popular videos in the niche is a goldmine of audience language, questions, and objections
3. **"Honest review" videos** — Search "[product/niche] honest review" — these contain unfiltered customer experiences
4. **Tutorial/educational content** — What questions is the audience trying to answer themselves?

**Specific searches to run:**
- `[niche keyword] for beginners` — reveals what newcomers struggle with
- `[competitor name] review` — reveals competitor perception
- `[niche keyword] mistakes` — reveals fears and pain points
- `[niche keyword] results` — reveals desired outcomes and proof expectations

**What to capture:**
- Video titles that get high views (these ARE validated hooks)
- Top comments (sort by Top, not Newest)
- Questions in comments (these become content/ad angles)
- Sentiment in comment sections (positive, negative, skeptical)
- Thumbnail patterns (what visual approach works in this niche)

**Minimum:** 5-10 competitor/niche videos analyzed (titles, view counts, top 20 comments each)

## Source 4.4: Facebook Groups

**How to find:** Search Facebook for groups related to the niche. Look for groups with 10K+ members and active recent posts.

**What to capture:**
- Most popular post types (questions, wins, complaints)
- Common questions asked repeatedly
- What members recommend to each other
- How members describe their struggles and goals
- Admin/moderator recommendations (often the influencers)

## Source 4.5: Quora

**How to search:** Google `site:quora.com [niche keyword]`

**What to capture:**
- Most-upvoted answers (validated advice = what the audience trusts)
- Questions with high follower counts (= high interest topics)
- Long, detailed personal experience answers (voice-of-customer gold)

## Source 4.6: TikTok

**How to search:** Search the niche keyword directly in TikTok

**What to capture:**
- Viral videos in the niche (what hooks/formats work)
- Comment sections (audience language, questions, objections)
- Creator content patterns (talking head, text overlay, duets)
- Trending sounds used in the niche

## Source 4.7: Niche Forums & Communities

**Where to look:** Skool groups, Discord servers, Slack communities, niche-specific forums

**What to capture:**
- Same as Reddit — pain language, desired outcomes, objections, competitor mentions

---

# PHASE 5: AUDIENCE VOICE MINING

## Goal
Extract the EXACT language your audience uses to describe their problems, desires, and experiences. This language goes directly into ad copy, VSL scripts, email subjects, and landing pages.

## Source 5.1: Amazon Book Reviews

**Why this works:** People who buy books on a topic are invested in solving the problem. Their reviews reveal exactly what they hoped to learn, what disappointed them, and what language they use.

**How to find:** Search Amazon for the top 3-5 books in the niche

**What to mine:**
- **5-star reviews:** What did they love? What outcome did the book help them achieve? What phrases do they use to describe the transformation?
- **1-star reviews:** What did they hate? What were they hoping for but didn't get? What objections do they have? What alternative did they wish existed?
- **3-star reviews:** These are the most nuanced — they reveal what partially worked and what was missing

**Capture template:**

```markdown
**Book:** [title]
**Rating:** [1/3/5 star]
**Key quote:** "[exact words]"
**What this reveals:** [pain point / desire / objection / gap]
```

**Minimum:** 30-50 reviews across 3-5 books (mix of 1, 3, and 5 star)

## Source 5.2: Review Sites

**Platforms:** Trustpilot, G2, BBB, Google Reviews, Yelp (if local), Capterra (if software)

**What to search:** Competitor names, product names, brand names

**What to capture:**
- Positive reviews: transformation language, specific results mentioned, what they value most
- Negative reviews: what went wrong, unmet expectations, refund reasons
- Response patterns: how the company handles complaints (reveals their weaknesses)

## Source 5.3: Podcast Appearances

**How to find:** Search "[founder name] podcast" or "[brand name] interview" on YouTube, Spotify, or Apple Podcasts

**What to capture:**
- How the founder describes their own offer (their pitch in their words)
- Origin story they tell
- Specific claims/numbers they share publicly
- How they position against competitors
- What advice they give (reveals their methodology)

**Tool:** `directives/execution/youtube_transcripts.py` for YouTube-hosted podcast episodes, `directives/execution/transcribe.py` for audio files

## Source 5.4: LinkedIn

**Best for:** B2B offers, wealth management, professional services

**What to search:**
- Posts by industry thought leaders
- Company pages of competitors
- Comments on popular industry posts
- Job postings (reveal what skills/outcomes companies pay for)

---

# PHASE 6: SEARCH & CONTENT INTELLIGENCE

## Goal
Understand what Google says about the market — what questions people ask, what content ranks, what the search landscape looks like.

## Step 6.1: Google SERP Analysis

**Searches to run:**
- `[primary niche keyword]` — see who ranks, what types of content
- `[niche keyword] + course/program/coaching` — see what offers exist
- `[niche keyword] + review/scam/worth it` — see what skeptics say
- `best [niche keyword] [current year]` — see what's recommended
- `[competitor name] + review/alternative/vs` — see competitor perception

**What to capture:**
- Who ranks on page 1 (authority indicators)
- Content types that rank (listicles, guides, reviews, videos)
- Featured snippets (what does Google consider the best answer)
- Related searches at the bottom of results

## Step 6.2: People Also Ask (PAA)

**Why this matters:** Google's PAA boxes show the EXACT questions the market is asking. These become:
- Ad hooks ("Are you wondering [PAA question]?")
- Email subject lines
- Breakout video topics
- FAQ content for landing pages

**How to extract:**
- Search the primary keyword
- Click on PAA questions to expand more
- Each click reveals 2-3 more questions
- Keep clicking until you've exhausted the thread (usually 15-30 questions)

**Capture all questions verbatim.**

## Step 6.3: Google Trends

**Why this matters:** Shows whether the niche is growing, stable, or declining. Also shows seasonal patterns and related queries.

**How to use:** https://trends.google.com — search the primary keyword, set timeframe to 5 years

**What to capture:**
- Trend direction (growing/stable/declining)
- Seasonal patterns (when is interest highest)
- Related topics and queries (new angles)
- Geographic concentration (if relevant)

---

# PHASE 7: SYNTHESIS & DELIVERABLES

## Goal
Compile all research into actionable documents that feed every downstream skill.

## Deliverable 1: Market Research Dossier

The master document. Contains:

```markdown
# Market Research Dossier: [Client Name]
**Date:** [date]
**Researcher:** AI Market Research Skill
**Sources consulted:** [list all sources checked]

## 1. Executive Summary
- [3-5 key findings that will drive strategy]
- [The single biggest opportunity identified]
- [The single biggest risk/challenge identified]

## 2. Market Overview
- Market size and trajectory (growing/stable/declining)
- Key players and their positioning
- Market sophistication level (Schwartz scale: Unaware → Most Aware)
- Demand type: In-Market (3-4%) vs. Needs-Convinced (30%) vs. Mass (33%)

## 3. Target Audience Profile
[See Avatar Profile deliverable below — summary here]

## 4. Competitor Landscape
[See Competitor Matrix deliverable — summary here]

## 5. Ad Intelligence Summary
[See Ad Intelligence Report — summary here]

## 6. Voice-of-Customer Findings
[See Voice-of-Customer Database — summary here]

## 7. Objection Map
[See Objection Map deliverable — full list here]

## 8. Opportunity Gaps
- Messaging angles no competitor is using
- Audience needs no competitor is addressing
- Creative formats no competitor is testing
- Positioning spaces that are unclaimed

## 9. Recommended Strategy Direction
- Primary positioning angle: [recommendation]
- Primary audience segment: [who to target first]
- Primary funnel type: [VSL/webinar/challenge/lead form]
- Primary ad approach: [strategy recommendation]
- Key messaging themes: [3-5 themes from research]

## 10. Confidence Assessment
- Data quality: [high/medium/low] — based on volume and recency of sources
- Competitive intelligence depth: [high/medium/low]
- Audience understanding depth: [high/medium/low]
- Areas needing more research: [list]
```

## Deliverable 2: Avatar Profile

```markdown
# Avatar Profile: [Client Name]

## Demographics
- Age: [range]
- Gender: [if relevant]
- Income: [range]
- Job title / Industry: [specifics]
- Location: [if relevant]
- Education: [level]
- Family status: [if relevant]

## Psychographics
### Top 3 Fears (what keeps them up at night)
1. [fear + exact language from research]
2. [fear + exact language from research]
3. [fear + exact language from research]

### Top 3 Desires (what they dream about)
1. [desire + exact language from research]
2. [desire + exact language from research]
3. [desire + exact language from research]

### Top 3 Frustrations (what makes them angry)
1. [frustration + exact language from research]
2. [frustration + exact language from research]
3. [frustration + exact language from research]

### Failed Solutions (what they've tried that didn't work)
1. [solution + why it failed + their words]
2. [solution + why it failed + their words]
3. [solution + why it failed + their words]

## Awareness Level (Schwartz Scale)
- Level: [Unaware / Problem-Aware / Solution-Aware / Product-Aware / Most Aware]
- Evidence: [what from research supports this]
- Implication: [what this means for copy approach]

## Where They Hang Out
- Social platforms: [ranked by concentration]
- Communities: [specific groups, forums, subreddits]
- Content they consume: [podcasts, YouTube channels, blogs]
- Influencers they follow: [names]

## Language Bank
### How they describe the problem:
- "[exact phrase from research]"
- "[exact phrase from research]"
- "[exact phrase from research]"
[minimum 10 phrases]

### How they describe the desired outcome:
- "[exact phrase from research]"
- "[exact phrase from research]"
- "[exact phrase from research]"
[minimum 10 phrases]

### Words/phrases they use frequently:
- [word] — used in context of [what]
[minimum 10 words]

### Words/phrases that turn them off:
- [word] — because [why]
[minimum 5 words]
```

## Deliverable 3: Competitor Matrix

```markdown
# Competitor Matrix: [Client Name]

| Factor | [Competitor 1] | [Competitor 2] | [Competitor 3] | [Client] |
|--------|----------------|----------------|----------------|----------|
| Positioning | | | | |
| Core Offer | | | | |
| Price | | | | |
| Guarantee | | | | |
| Funnel Type | | | | |
| Primary Traffic | | | | |
| Content Strategy | | | | |
| Social Proof Strength | | | | |
| Active Ad Count | | | | |
| Unique Mechanism | | | | |
| Biggest Strength | | | | |
| Biggest Weakness | | | | |

## Positioning Map
[Where each competitor sits on key dimensions — e.g., price vs. done-for-you level, or beginner vs. advanced focus]

## Gaps We Can Exploit
1. [Gap + how to exploit it]
2. [Gap + how to exploit it]
3. [Gap + how to exploit it]
```

## Deliverable 4: Ad Intelligence Report

```markdown
# Ad Intelligence Report: [Client Name]

## Market Ad Landscape
- Total competitors running ads: [count]
- Dominant creative format: [video/static/carousel]
- Average ad longevity of winners: [days]
- Common hook patterns: [list top 5]
- Common CTA patterns: [list top 3]

## Top Performing Ads (Longest Running)
### Ad 1: [Competitor Name]
- Running since: [date/estimate]
- Format: [video/static]
- Hook: "[first line or first 3 seconds]"
- Angle: [what positioning angle]
- CTA: [what action]
- Landing page: [where it goes]
- Why it works: [analysis]

[Repeat for top 5-10 ads]

## Creative Patterns
- Hooks that appear across multiple competitors: [list]
- Hooks that NO competitor is using: [list — these are opportunities]
- Body copy frameworks in use: [PAS, story, listicle, etc.]
- Video styles in use: [talking head, UGC, B-roll, demo, etc.]

## Recommendations
- Ad formats to test first: [based on what's working in market]
- Hook angles to test: [based on gaps identified]
- Creative differentiation opportunity: [what would stand out]
```

## Deliverable 5: Voice-of-Customer Database

```markdown
# Voice-of-Customer Database: [Client Name]

## Pain Points (sorted by frequency/intensity)
| # | Pain Point | Exact Language | Source | Frequency |
|---|-----------|----------------|--------|-----------|
| 1 | [pain] | "[verbatim quote]" | Reddit r/[sub] | High |
| 2 | [pain] | "[verbatim quote]" | Amazon review | High |
[minimum 15 pain points]

## Desired Outcomes (sorted by frequency/intensity)
| # | Desire | Exact Language | Source | Frequency |
|---|--------|----------------|--------|-----------|
| 1 | [desire] | "[verbatim quote]" | YouTube comment | High |
[minimum 10 desired outcomes]

## Objections & Skepticism
| # | Objection | Exact Language | Source | Reframe |
|---|----------|----------------|--------|---------|
| 1 | [objection] | "[verbatim quote]" | Reddit | [how to address] |
[minimum 10 objections]

## Transformation Stories (proof language)
| # | Story Summary | Exact Language | Source |
|---|--------------|----------------|--------|
| 1 | [what happened] | "[verbatim quote]" | Trustpilot |
[as many as found]

## Competitor Mentions
| Competitor | Sentiment | Quote | Source |
|-----------|-----------|-------|--------|
| [name] | Positive/Negative/Mixed | "[quote]" | Reddit |
[all mentions found]
```

## Deliverable 6: Objection Map

```markdown
# Objection Map: [Client Name]

| # | Objection | Category | Evidence | Reframe | Use In |
|---|----------|----------|----------|---------|--------|
| 1 | "It's too expensive" | Price | [source] | [reframe] | VSL, ads, emails |
| 2 | "I've tried this before" | Skepticism | [source] | [reframe] | VSL, confirmation page |
| 3 | "I don't have time" | Logistics | [source] | [reframe] | Ads, emails |
[minimum 10 objections with full handling]

Categories: Price, Skepticism, Logistics, Trust, Timing, Competence, Risk
```

---

# AI RESEARCH PROMPTS

## Prompt A: Full Analysis With Sales Call Transcripts

Use this when the client has provided sales call recordings or transcripts. This is the highest-quality research input available.

**Prerequisite:** Upload all transcripts to the conversation first. Tell the AI to read every single one before proceeding.

```
You've been provided sales call transcripts for our offer. Your job is to read every single file that has been provided so that you fully understand the conversations that are occurring back and forth with actual real prospects. When reading these files, recognize who the sales person is vs. who the prospect is. Recognize in your knowledge whether something was said by the salesperson or if it was said by the prospect.

Your job is to use that data in order to assist me with creating the four following items. If, when generating the items, you don't believe the contents of the sales call transcripts provides a sufficient amount of information in order to accurately deliver the highest quality response for each item, your job is to use reasoning, research, and experience in order to deliver the best possible answer of what you believe it should be in order to maximize the probability of creating the highest possible converting marketing material. If you are using your own knowledge to assist with the creation of each item, please explicitly state exactly which parts you have, and detail your reasoning as to why you did that.

Here are the items:

1. The pain points, questions, concerns, and categorization of the types of people that are on the calls. Basically just an understanding of who the target market actually is and what they really want. Attempt to use reasoning to infer if there is something they actually want, but did not explicitly say. If you do not believe there are inferred desires from the transcripts, then do not make one up. Provide a confidence score for each.

2. Given this information, what you believe the value proposition of the offer is, even if it isn't explicitly stated. You may need to derive the value proposition from the information you gather inside of the sales calls. A value proposition is a clear, concise statement of the unique benefits a product or service offers a target customer, explaining how it solves their problems or improves their lives better than competitors. If you cannot derive it directly from the information inside of the calls, assist me with the creation of it. Provide a confidence score as to whether you believe this would be the highest converting value proposition if we went to market with it that would generate the maximum possible sales.

3. The unique benefits of the offer. If they're not stated, then please, using the provided transcripts of sales calls, help me come up with some unique benefits that could potentially be part of the offer that would maximize the probability of future prospects closing and being interested in purchasing. Given your understanding of the offer and market, if you believe it's necessary, suggest unique benefits that you believe would maximize the probability of prospects purchasing.

4. A full description of a full sales argument for the offer. I want a persuasive reasoning designed to demonstrate to a potential client or customer why my specific product or service is the best solution for their needs, ultimately convincing them to purchase. You should derive this information based on what you've gathered from the sales call transcripts, and what you've created from all of the previously created items.

When you create all of these items, I want you to act as a direct response copywriter who is a professional at human psychology, marketing, and sales, and has generated billions of dollars of sales through advertising. You are intricately aware of the active market dynamics in today's digital landscape, and know what competitors for specific offers exist, and are acutely aware of what makes a great offer vs. a bad offer. You know that the strength of the offer dictates the performance of the marketing, and understand how to design a great offer, and then convey it's value accurately inside of a sales argument. Your job is to provide the best possible information in order to maximize the probability we make the most amount of sales and convert the highest quantity and quality of customers with our offer.

Additional rules:
- No hallucinated internal facts. Separate SUPPORTED vs INFERRED. Provide confidence scores.
- If competitors are not given and web access is unavailable, do a category-level competitor snapshot from the transcripts and your general knowledge; label as INFERRED.
- Style: concise, punchy, direct-response ready. No fluff. Be explanative with minimal fluff.
- Do not lie or make up data.

Now, please begin, and ensure to read EVERY SINGLE SALES CALL. Do not proceed until you have read every single sales call transcript.
```

## Prompt B: Full Analysis Without Transcripts

Use this for new offers or clients without sales call recordings. Fill in the bracketed fields first.

**Input template:**

```
Offer: [DESCRIBE THE OFFER - what you sell, how it works, what makes it unique]

Target Market: [DESCRIBE THE TARGET MARKET - who they are, what stage they're at, what they ideally already believe/know]

Alternatives: [DESCRIBE CURRENT ALTERNATIVES - how else do people solve this problem today, what are the downsides of those alternatives]

Other Info: [ANY ADDITIONAL CONTEXT - successful angles used before, known pain points, market dynamics]
```

**Full prompt (paste after filling input template):**

```
Your job is to help research, formulate, and use advanced reasoning and research in order to help me develop the four action items listed below for our offer we are selling. Unfortunately, I currently lack transcripts of sales calls, as this is going to be a new offer. Therefore, I need you to conduct independent research and execute your own reasoning based off of the data I can provide to you. Your job is to use reasoning, research, and experience in order to deliver the best possible answer of what you believe it should be in order to maximize the probability of creating the highest possible converting marketing material. If you are using your own knowledge to assist with the creation of each item, please explicitly state exactly which parts you have, and detail your reasoning as to why you did that.

Here is the data I can provide to you in absence of sales call transcripts:

[PASTE FILLED INPUT TEMPLATE HERE]

Notes: What I have provided you in the above information is not exhaustive, it's simply what I was able to formulate by sitting and thinking about it for a bit. Therefore, your job is to independently figure out more information about the alternatives, current market state, potentially other relevant target markets and angles of offer positioning to use against them, and other potentially useful information about the offer that will assist you in the creation of your action items below. I would like you to access your base of knowledge, and perhaps conduct research online, in order to understand everything you possible can about the target market, and therefore be able to produce the highest quality inferences on them when creating the action items below.

Here are the items:

1. The pain points, questions, concerns, and categorization of the types of people that are on the calls. Basically just an understanding of who the target market actually is and what they really want. Attempt to use reasoning to infer if there is something they actually want, but I did not explicitly say. If you do not believe there are inferred desires that you can find from your research or knowledge, then do not make one up. Provide a confidence score for each.

2. Given this information, what you believe the value proposition of the offer is, even if it isn't explicitly stated. You may need to derive the value proposition from the information you gather inside your research. A value proposition is a clear, concise statement of the unique benefits a product or service offers a target customer, explaining how it solves their problems or improves their lives better than competitors. If you cannot derive it directly from the information I provided you, assist me with the creation of it. If you believe there is a better value proposition that would convert more customers that I did not explicitly state, then recommend me that one and provide your reasoning for it. Provide a confidence score as to whether you believe this would be the highest converting value proposition if we went to market with it that would generate the maximum possible sales.

3. The unique benefits of the offer. If they're not stated, then please, using your knowledge or research and what you can infer about the market, help me come up with some unique benefits that could potentially be part of the offer that would maximize the probability of future prospects closing and being interested in purchasing. Given your understanding of the offer and market, if you believe it's necessary, suggest unique benefits that you believe would maximize the probability of prospects purchasing.

4. A full description of a full sales argument for the offer. I want a persuasive reasoning designed to demonstrate to a potential client or customer why my specific product or service is the best solution for their needs, ultimately convincing them to purchase. You should derive this information based on what you've gathered from your knowledge, research, and inferences, and what you've created from all of the previously created items.

When you create all of these items, I want you to act as a direct response copywriter who is a professional at human psychology, marketing, and sales, and has generated billions of dollars of sales through advertising. You are intricately aware of the active market dynamics in today's digital landscape, and know what competitors for specific offers exist, and are acutely aware of what makes a great offer vs. a bad offer. You know that the strength of the offer dictates the performance of the marketing, and understand how to design a great offer, and then convey it's value accurately inside of a sales argument. Your job is to provide the best possible information in order to maximize the probability we make the most amount of sales and convert the highest quantity and quality of customers with our offer.

Additional rules:
- No hallucinated internal facts. Separate SUPPORTED vs INFERRED. Provide confidence scores.
- If competitors are not given and web access is unavailable, do a category-level competitor snapshot from your general knowledge; label as INFERRED.
- Style: concise, punchy, direct-response ready. No fluff. Be explanative with minimal fluff.
- Do not lie or make up data.

Now, please begin.
```

## Prompt C: Social Listening Synthesis

Run this AFTER completing Phase 4 (social listening). Feed it all captured quotes.

```
I've collected voice-of-customer data from Reddit, X, YouTube comments, Amazon reviews, forums, and other sources for [CLIENT/NICHE]. Here is the raw data:

[PASTE ALL CAPTURED QUOTES AND THREADS]

Synthesize this into:

1. TOP 10 PAIN POINTS ranked by frequency and emotional intensity. For each: the pain point, 3 verbatim quotes that express it, and a "copy-ready" version I can use directly in ads/VSLs/emails.

2. TOP 10 DESIRED OUTCOMES ranked by frequency. For each: the desire, 3 verbatim quotes, and a "copy-ready" version.

3. TOP 10 OBJECTIONS ranked by how deal-killing they are. For each: the objection, 3 verbatim quotes, a suggested reframe, and where to deploy the reframe (ads, VSL, confirmation page, sales call).

4. LANGUAGE BANK: The 20 most powerful words and phrases this audience uses that we should incorporate into all marketing copy. Include context for each.

5. EMOTIONAL TRIGGERS: The 5 strongest emotional triggers identified, with evidence and recommended deployment.

6. OPPORTUNITY SIGNALS: Any unmet needs, underserved segments, or messaging gaps that no competitor appears to be addressing.

Rules:
- Prioritize REAL language over marketing language
- Flag which source each insight came from
- Note confidence level for each finding
- Do not fabricate quotes — only use what was provided
```

## Prompt D: Competitive Intel Synthesis

Run this AFTER completing Phase 2 (competitor teardowns) and Phase 3 (ad intelligence).

```
Here are the complete competitor funnel teardowns and ad intelligence findings for [CLIENT/NICHE]:

[PASTE COMPETITOR TEARDOWNS AND AD INTELLIGENCE DATA]

Synthesize into:

1. COMPETITIVE LANDSCAPE MAP: Where each competitor sits, what they claim, where they're strong, where they're weak.

2. POSITIONING GAPS: 3-5 positioning angles that are NOT being used by any competitor but are supported by audience demand (from our social listening data).

3. CREATIVE GAPS: Ad formats, hooks, or creative approaches that no competitor is testing but would likely work based on market patterns.

4. PRICING INTELLIGENCE: How competitors price, what guarantees they offer, and where our client can differentiate on offer structure.

5. FUNNEL INTELLIGENCE: What funnel types competitors use, conversion bottlenecks visible from outside, and what funnel approach would best differentiate our client.

6. THREAT ASSESSMENT: Which competitor is the biggest threat and why. What would happen if they copied our client's approach.

Rules:
- Be specific — name competitors, cite evidence
- Separate facts from inferences
- Rank opportunities by impact potential
```

---

# EXECUTION SCRIPTS

## Available Scripts

| Script | Location | What It Does | When to Use |
|--------|----------|-------------|-------------|
| `scrape_website.py` | `directives/execution/` | Scrapes a URL for content | Competitor websites, client site, landing pages |
| `youtube_transcripts.py` | `directives/execution/` | Pulls YouTube video transcripts | Competitor YouTube content, client content, podcast interviews |
| `transcribe.py` | `directives/execution/` | Transcribes audio/video files | Sales call recordings, onboarding calls, podcast episodes |
| `extract_docx.py` | `execution/` | Converts .docx to markdown | Client documents, SOPs, briefs |

## Manual Research (No Script Needed)

These sources are researched using WebSearch and WebFetch tools directly:
- Meta Ad Library (facebook.com/ads/library)
- Reddit (site:reddit.com searches via Google)
- X/Twitter (search.twitter.com or via Google)
- Amazon reviews (direct URL)
- Google SERP / People Also Ask
- Google Trends
- Review sites (Trustpilot, G2, BBB)
- TikTok Creative Center

---

# RESEARCH DEPTH TIERS

Not every client engagement requires the same depth. Match research depth to the engagement:

## Tier 1: Quick Research (2-3 hours)
**When:** Small project, single deliverable, tight timeline
- Phase 1 (briefing) — abbreviated
- Phase 2 (competitors) — top 2-3 competitors, surface-level teardown
- Phase 4 (social listening) — 5-10 Reddit threads, quick X search
- Phase 7 (synthesis) — abbreviated dossier

## Tier 2: Standard Research (4-8 hours)
**When:** New client onboarding, full funnel build
- All 7 phases at standard depth
- 3-5 competitor teardowns
- 15-20 Reddit threads + X + YouTube
- Ad library analysis
- Full deliverable set

## Tier 3: Deep Research (8-16 hours)
**When:** High-ticket client ($10K+/month), competitive niche, complex offer
- All 7 phases at maximum depth
- 5-8 competitor teardowns with full funnel walkthroughs
- 30+ social listening threads across all platforms
- Complete ad library analysis with creative transcription
- Amazon review mining (50+ reviews)
- Podcast transcript analysis
- Full deliverable set with extended voice-of-customer database

---

# QUALITY CHECKS

## Research Quality
- [ ] Minimum 3 competitors analyzed with full teardown format
- [ ] Minimum 15 voice-of-customer quotes captured verbatim (not paraphrased)
- [ ] Reddit, X, and YouTube all checked (not just one platform)
- [ ] Ad library checked for all identified competitors
- [ ] Pain points sourced from AUDIENCE language (not marketing assumptions)
- [ ] Awareness level assessed with evidence (not guessed)
- [ ] At least one non-obvious opportunity gap identified
- [ ] All SUPPORTED vs INFERRED content labeled

## Deliverable Quality
- [ ] All 6 deliverables produced (dossier, avatar, competitor matrix, ad intel, VoC database, objection map)
- [ ] Verbatim quotes included (not just summaries)
- [ ] Confidence scores provided where applicable
- [ ] Actionable recommendations in every section (not just data dumps)
- [ ] Language bank has minimum 10 pain phrases + 10 desire phrases
- [ ] Objection map has minimum 10 objections with reframes
- [ ] Competitor matrix is comparative (not just individual profiles)

## Integration Quality
- [ ] Research is saved to `clients/[client-name]/research/` directory
- [ ] Findings can be directly consumed by positioning-angles, offer-creation, vsl-scripting, meta-ad-strategy
- [ ] Executive summary is concise enough to pass as context to downstream skills
- [ ] Language bank is formatted for direct use in copy

---

# CONNECTIONS

- **Requires:** Client profile (minimum: offer, niche, website, competitors)
- **Feeds into:** EVERY downstream skill — this is the foundation
  - positioning-angles (uses opportunity gaps + audience language)
  - offer-creation (uses pain points + competitor pricing + objection map)
  - vsl-scripting (uses sales argument + avatar + voice-of-customer)
  - webinar-scripting (uses avatar + pain points + transformation language)
  - meta-ad-strategy (uses ad intelligence + competitor creative + audience segments)
  - email-flows (uses objection map + voice-of-customer + pain/desire language)
  - landing-page (uses competitor teardowns + positioning gaps)
  - direct-response-copy (uses language bank + pain points + proof stack)
  - brand-voice (uses audience language patterns + competitor voice analysis)
- **Part of:** Phase I of the client pipeline (see `directives/client_onboarding.md`)
- **Supersedes:** The market research prompts previously in vsl-scripting, and the research.md directive (which was a lighter version of this skill)
