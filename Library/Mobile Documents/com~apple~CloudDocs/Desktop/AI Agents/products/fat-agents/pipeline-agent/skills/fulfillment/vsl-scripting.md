
---

## 6. VSL SCRIPTING

# Skill: VSL Scripting

> Write high-converting Video Sales Letter scripts, sales pages, video ad scripts, and static ad copy. This skill installs the COMPLETE tactical system from `Mastering_VSLs_SOP.md` + `AI_Copywriting_SOP.md` + `Direct_Response_Ad_Creation_Framework_SOP.md` -- every AI prompt verbatim, every framework, every named methodology.

## Trigger Keywords

`VSL`, `video sales letter`, `VSL script`, `write a VSL`, `sales video`, `explainer video script`, `funnel video`, `webinar replacement`, `sales page`, `landing page copy`, `video ad script`, `static ad`, `ad creative`, `talking head VSL`, `gamma doc VSL`

---

## Core Job

Write a complete VSL script that takes a cold or warm viewer from "who are you?" to "I need to book a call / buy this" in 2-45 minutes, following the 9-step direct response framework. Optionally produce companion deliverables: sales page copy (B2B or B2C), video ad scripts, static ad copy, opt-in email sequences, and breakout video scripts.

---

## Inputs Required

| Input | Required? | Source |
|-------|-----------|--------|
| Client's offer (what they sell, price, guarantee) | Yes | the business details you provide or offer-creation skill output |
| Target audience (avatar) | Yes | avatar-research.md |
| Campaign angle (which angle to lead with) | Yes | campaign-angles.md or user selection |
| Creative strategy (proof stack, objection map) | Yes | creative-strategy.md |
| Brand voice guidelines | Helpful | the business details you provide |
| Existing results/testimonials | Helpful | User |
| VSL length preference | Helpful | User (default: based on audience) |
| Sales call transcripts (if available) | Helpful | User uploads |

---

# PHASE 0: MARKET RESEARCH (Run Before Writing Anything)

The actual writing of copy is 90% of the fulfillment work. Before writing any VSL, sales page, or ad script, you MUST conduct market research to establish a base understanding of the offer. There are two scenarios:

## Scenario A: Sales Call Transcripts ARE Available

Use this prompt verbatim. Upload all sales call transcripts first.

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

## Scenario B: No Sales Call Transcripts Available

Use this prompt verbatim. Fill in the bracketed sections with client-specific information.

```
Your job is to help research, formulate, and use advanced reasoning and research in order to help me develop the four action items listed below for our offer we are selling. Unfortunately, I currently lack transcripts of sales calls, as this is going to be a new offer. Therefore, I need you to conduct independent research and execute your own reasoning based off of the data I can provide to you. Your job is to use reasoning, research, and experience in order to deliver the best possible answer of what you believe it should be in order to maximize the probability of creating the highest possible converting marketing material. If you are using your own knowledge to assist with the creation of each item, please explicitly state exactly which parts you have, and detail your reasoning as to why you did that.

Here is the data I can provide to you in absence of sales call transcripts:

Offer: [DESCRIBE THE OFFER - what you sell, how it works, what makes it unique]

Target Market: [DESCRIBE THE TARGET MARKET - who they are, what stage they're at, what they ideally already believe/know]

Alternatives: [DESCRIBE CURRENT ALTERNATIVES - how else do people solve this problem today, what are the downsides of those alternatives]

Other Info: [ANY ADDITIONAL CONTEXT - successful angles used before, known pain points, market dynamics]

Notes: What I have provided you in the above information is not exhaustive, it's simply what I was able to formulate by sitting and thinking about it for a bit. Therefore, your job is to independently figure out more information about the alternatives, current market state, potentially other relevant target markets and angles of offer positioning to use against them, and other potentially useful information about the offer that will assist you in the creation of your action items below. I would like you to access your base of knowledge, and perhaps conduct research online, in order to understand everything you possible can about the target market, and therefore be able to produce the highest quality inferences on them when creating the action items below.

Here are the items:

1. The pain points, questions, concerns, and categorization of the types of people that are on the calls. Basically just an understanding of who the target market actually is and what they really want. Attempt to use reasoning to infer if there is something they actually want, but I did not explicitly say. If you do not believe there are inferred desires that you can find from your research or knowledge, then do not make one up. Provide a confidence score for each.

2. Given this information, what you believe the value proposition of the offer is, even if it isn't explicitly stated. You may need to derive the value proposition from the information you gather inside your research. A value proposition is a clear, concise statement of the unique benefits a product or service offers a target customer, explaining how it solves their problems or improves their lives better than competitors. If you cannot derive it directly from the information I provided you, assist me with the creation of it. If you believe there is a better value proposition that would convert more customers that I did not explicitly state, then recommend me that one and provide your reasoning for it. Provide a confidence score as to whether you believe this would be the highest converting value proposition if we went to market with it that would generate the maximum possible sales.

3. The unique benefits of the offer. If they're not stated, then please, using your knowledge or research and what you can infer about the market, help me come up with some unique benefits that could potentially be part of the offer that would maximize the probability of future prospects closing and being interested in purchasing. Given your understanding of the offer and market, if you believe it's necessary, suggest unique benefits that you believe would maximize the probability of prospects purchasing.

4. A full description of a full sales argument for the offer. I want a persuasive reasoning designed to demonstrate to a potential client or customer why my specific product or service is the best solution for their needs, ultimately convincing them to purchase. You should derive this information based on what you've gathered from your knowledge, research, and inferences, and what you've created from all of the previously created items.

When you create all of these items, I want you to act as a direct response copywriter who is a professional at human psychology, marketing, and sales, and has generated billions of dollars of sales through advertising. You are intricately aware of the active market dynamics in today's digital landscape, and know what competitors for specific offers exist, and are acutely aware of what makes a great offer vs. a bad offer. You know that the strength of the offer dictates the performance of the marketing, and understand how to design a great offer, and then convey it's value accurately inside of a sales argument. Your job is to provide the best possible information in order to maximize the probability we make the most amount of sales and convert the highest quantity and quality of customers with our offer.

Additional rules:
- No hallucinated internal facts. Separate SUPPORTED vs INFERRED. Provide confidence scores.
- If competitors are not given and web access is unavailable, do a category-level competitor snapshot from the transcripts and your general knowledge; label as INFERRED.
- Style: concise, punchy, direct-response ready. No fluff. Be explanative with minimal fluff.
- Do not lie or make up data.

Now, please begin.
```

**Critical Rule:** The documents produced by market research ARE the foundation for ALL subsequent copy. Ideally, produce all assets (sales page, VSL, ads) in the same conversation window so the AI retains full context.

---

# PHASE 1: THE MANUS CONVERSATION WORKFLOW

This is the sequential workflow for producing all copy assets. Each prompt builds on the previous output. Run them in order within the same conversation window.

**Step 1:** Market Research (Phase 0 above) -- produces pain points, value proposition, unique benefits, sales argument

**Step 2:** Sales Page Copy (Phase 2 below) -- uses market research output to produce full landing page / sales page copy

**Step 3:** VSL Script (Phase 3 below) -- uses market research + sales page copy to produce the VSL script

**Step 4:** Video Ad Scripts (Phase 5 below) -- uses all prior context to produce ad creatives

**Step 5:** Static Ad Scripts (Phase 6 below) -- uses all prior context to produce static ad text

**Step 6:** Opt-In Emails (Phase 7 below) -- uses all prior context to produce email sequences

Each step references "documents provided in this conversation" because the AI should retain the market research output and sales page copy when writing the VSL, ads, etc.

---

# PHASE 2: SALES PAGE COPY GENERATION

## Pre-Work: Determine VSL Length

| Audience Type | Recommended Length | Why |
|---------------|-------------------|-----|
| Affluent, action-taking, already aware | 2-10 minutes | They don't need convincing, just clarity |
| Analytical, skeptical, less aware | 15-30 minutes | Need more proof, more objection handling |
| Cold traffic, problem-unaware | 30-45 minutes | Full education + persuasion required |

## B2B vs B2C Structure Decision

- **B2B Structure** -- for small-to-medium business buyers evaluating professional solutions
- **B2C Structure** -- for individual consumers making personal purchase decisions
- **Adaptive Structure** -- let the AI determine what's best for the particular offer

**Pricing disclosure rule:** If the funnel is a sales call funnel, do NOT reveal pricing on the page. If it's a low ticket product where checkout occurs on the page, reveal pricing.

---

### B2B Sales Page Generation Prompt (Verbatim)

```
You've been provided with comprehensive documentation containing the Benefits, Value Proposition, Pain Points, Questions, Concerns, and Sales Argument for our B2B offer. Your job is to read and fully internalize this information to create high-converting sales page copy specifically designed for small-to-medium B2B buyers of my target market for this particular offer. A description of the target market is inside the documentation (and, if you have been provided transcripts of sales calls previously in this conversation, also inside of those).

You will create copy for each of the following sections in the exact order presented. For each section, use the provided documentation as your primary source, but if critical persuasive elements are missing, use your expertise to enhance the copy while explicitly noting what you've added and why. Provide a conversion confidence score (1-10) for each section.

Required Sales Page Sections:

1. Pre-Headline - A small text above the main headline that provides context or credibility (10-15 words)

2. Main Headline - Focus on the primary business outcome or transformation, not features (10-20 words). Must speak to measurable business impact.

3. Subheadline - Expand on the mechanism or method that delivers the headline's promise (20-30 words)

4. Problem Agitation Section - 3-5 paragraphs that demonstrate deep understanding of their current situation. Start with their external problem (business metric), bridge to internal problem (daily frustration), end with philosophical problem (why this matters to their business identity).

5. Solution Introduction - 2-3 paragraphs introducing our solution as the bridge from their problem to their desired outcome. Focus on the unique mechanism, not features.

6. Authority/Credibility Block - Brief section establishing why our company can deliver this solution. Include relevant credentials, experience, or unique positioning.

7. Benefits Section - 3-5 major benefits, each with:
   - Benefit headline (business outcome focused)
   - 2-3 sentences explaining the benefit
   - Specific metric or outcome when possible
   - Connection to a pain point from the documentation

8. Social Proof Section - Structure as:
   - Case Studies with specific quantifiable return generated
   - If you have not been provided case studies previously inside this conversation, leave this section blank. Do not make up case studies or use fake data.

9. Process/Method Overview - 3-5 step breakdown of how the solution works. Each step should include:
   - Step name
   - What happens
   - Why it matters to their business

10. Objection Handling Section - Address the 3-4 biggest concerns from the documentation using "Even if..." or "Without..." frameworks

11. Offer Stack - Itemized list of everything included, with:
    - Core offer
    - Additional components/bonuses

12. Risk Reversal - Specific guarantee that addresses their biggest fear about moving forward

13. CTA:
    - Primary CTA: Book a strategy call/demo

14. FAQ Section - 5-7 questions addressing remaining concerns not covered above

15. Final Urgency/Scarcity Block - Legitimate reason to act now (capacity, bonus deadline, price change, etc.). Do not use fake urgency or fake scarcity. Attempt to reason the most logical, legitimate reason they need to act now, without using any cringey marketing language that makes us seem shady.

Execution Rules:
- Write from the business owner's perspective, understanding they care about: revenue, efficiency, team productivity, competitive advantage, and risk mitigation
- Use specific numbers and metrics wherever possible
- Every claim must tie back to business impact
- Avoid jargon unless it's industry-standard and adds credibility
- Write at an 8th-grade reading level for clarity
- Each section should flow logically to the next
- Include transition sentences between major sections if necessary
- Label each response section with [SUPPORTED] if derived from documentation or previous material in this chat history or [ENHANCED] if you've added based on expertise

Voice Guidelines:
Act as a B2B direct response copywriter who has generated over $500M in B2B sales. You understand that B2B buyers are simultaneously rational (need ROI justification) and emotional (want to look good to their team/boss/friends). You know that trust and risk mitigation are paramount. You write with authority but not arrogance, with data but not drowning in it, with benefits but always tied to business outcomes.

Output Format:
For each section, provide:
- The copy itself
- [SUPPORTED/ENHANCED] label
- Confidence score (1-10) for conversion potential
- Brief note on any strategic decisions made

Do not proceed until you have fully read and understood all provided documentation about the Benefits, Value Proposition, Pain Points, Questions, Concerns, and Sales Argument.
```

---

### B2C Sales Page Generation Prompt (Verbatim)

**Note:** If product is high ticket through a sales call, remove the part about pricing from this prompt. If it's a low ticket product, leave pricing in.

```
You've been provided with comprehensive documentation containing the Benefits, Value Proposition, Pain Points, Questions, Concerns, and Sales Argument for our B2C offer. You may have also been provided transcripts of sales calls inside of this chat window. Your job is to read and fully internalize this information to create high-converting sales page copy specifically designed for individual consumers making personal purchase decisions.

You will create copy for each of the following sections in the exact order presented. For each section, use the provided documentation as your primary source, but if critical persuasive elements are missing, use your expertise to enhance the copy while explicitly noting what you've added and why. Provide a conversion confidence score (1-10) for each section.

Required Sales Page Sections:

1. Pattern Interrupt Pre-Headline - A provocative statement or question that stops scrolling and creates curiosity

2. Main Headline - Focus on the primary emotional benefit or transformation, using power words that trigger desire and/or urgency. Must connect to a deep emotional want or pain.

3. Subheadline - Expand on how they'll achieve the headline's promise or what makes this solution unique.

4. Lead Section - 2-5 paragraphs that create an emotional connection by painting a picture of their current frustration versus their desired future state. Start with empathy, build desire, introduce the possibility of change.

5. Big Promise Statement - One powerful sentence or short paragraph that crystallizes exactly what transformation they'll experience

6. Social Proof Bar - Immediate credibility indicators such as number of customers, aggregate reviews, media mentions, or awards

7. Benefits Section - 3-5 transformational benefits, each with:
   - Emotionally-charged benefit headline
   - 1-2 sentences painting a picture of life with this benefit
   - Connection to eliminating a specific pain or achieving a specific desire

8. Features Bridge - 3-4 key features that support the benefits, explained in terms of what they mean for the customer's life, not technical specifications

9. Social Proof Deep Dive - Structure as:
   - 2-3 detailed customer transformation stories with before/after elements
   - 4-5 shorter testimonials addressing specific results or experiences
   - Visual proof elements (before/after photos, screenshots, results)

10. Authority Section - Brief section establishing credibility through founder story, media mentions, certifications, or unique expertise (keep concise and relevant to customer benefit)

11. Objection Handling Section - Address the 3-4 biggest hesitations using "What if..." or "But I..." frameworks, providing reassuring responses

12. Product Reveal/Offer Stack - Clear presentation of what they receive:
    - Main product/service
    - Bonuses that increase perceived value
    - Any additional resources or support

13. Price Anchoring Section - Present price in context of value, alternatives, or cost of not solving the problem

14. Risk Reversal - Strong guarantee that removes the fear of making a wrong decision

15. Urgency/Scarcity Element - Legitimate reason to act now (limited quantity, special pricing, bonus deadline, seasonal relevance)

16. CTA:
    - Primary CTA: Book a call

17. FAQ Section - 5-7 questions addressing logistics, usage, and remaining concerns

18. Final Emotional Close - Brief section reconnecting to the transformation and inviting them to take action

Execution Rules:
- Write from the customer's personal perspective, understanding they care about how they'll feel, look, save time, reduce stress, gain status, or improve their life
- Use sensory language and emotional triggers throughout
- Paint pictures of life before and after the purchase
- Keep sentences short and punchy for easy scanning
- Use power words that create urgency, excitement, and desire
- Every feature must be translated into a personal benefit
- Include specific details that make claims feel real and tangible
- Write at a 6th-grade reading level for maximum accessibility
- Create emotional peaks and valleys throughout the page
- Use conversational language that sounds like a friend giving advice

Voice Guidelines:
Act as a direct response copywriter specializing in consumer psychology who has generated over $1 billion in B2C sales. You understand that consumers buy emotionally and justify rationally. You know how to tap into deep desires, fears, and aspirations while maintaining authenticity. You write with enthusiasm and energy, creating a sense of excitement and possibility. Your copy feels like a conversation with a trusted friend who genuinely wants to improve their life.

Psychological Triggers to Incorporate:
- Fear of missing out (FOMO)
- Social proof and belonging
- Instant gratification promise
- Status and identity enhancement
- Loss aversion
- Curiosity gaps
- Pattern interrupts
- Future pacing (helping them visualize success)

Output Format:
For each section, provide:
- The copy itself
- [SUPPORTED/ENHANCED] label
- Confidence score (1-10) for conversion potential
- Brief note on psychological triggers or strategic decisions employed

Additional B2C-Specific Requirements:
- Include emotional power words throughout (discover, transform, breakthrough, revolutionary, secret, proven, instant)
- Create visual breaks with short paragraphs, single-sentence paragraphs for emphasis, and strategic use of ellipses or dashes
- Address the individual's personal identity and how the product aligns with who they want to be
- Focus on speed of results and ease of implementation
- Emphasize the experiential and emotional outcomes over technical details
- Create micro-commitments throughout the page that build toward the final purchase decision
- Use "you" and "your" frequently to maintain personal connection
- Include lifestyle imagery descriptions when relevant

Do not proceed until you have fully read and understood all provided documentation about the Benefits, Value Proposition, Pain Points, Questions, Concerns, and Sales Argument.
```

---

### Adaptive Sales Page Generation Prompt (Verbatim)

Use when the offer does not fit neatly into B2B or B2C categories.

```
You've been provided with comprehensive documentation containing the Benefits, Value Proposition, Pain Points, Questions, Concerns, and Sales Argument for our offer. You also may have been given sales calls transcripts. Your job is to read and fully internalize this information to create high-converting sales page copy that adapts to the specific nature of the product and target audience identified in the documentation.

Your first task is to analyze the provided materials to determine the optimal sales approach. Examine whether the target audience consists of business decision-makers evaluating professional solutions or individual consumers making personal purchases. Some offers may blend elements of both, such as professional tools that enhance personal productivity or consumer products sold to small business owners. Your copy should naturally adapt to these nuances rather than forcing a rigid B2B or B2C framework.

Section Development Framework
For each section you create, you must first determine the appropriate depth, tone, and psychological approach based on your analysis of the target market. The documentation will reveal whether your prospects need extensive logical justification, emotional resonance, or a sophisticated blend of both. Let the natural complexity of the buying decision guide your choices rather than applying predetermined templates.

Core Page Architecture
Begin with an opening sequence that immediately qualifies the right audience while creating sufficient intrigue to continue reading. This includes a contextual pre-headline that filters or attracts the right prospects, followed by a main headline that articulates the primary transformation or outcome your offer provides. The sophistication and framing of this promise should match the sophistication of your audience and the nature of the problem being solved.

Develop an introduction that demonstrates deep understanding of the prospect's current situation. This section's length and complexity should mirror the complexity of the problem and the psychological distance the prospect must travel to reach purchase readiness. Simple impulse purchases require brief emotional connections, while complex solutions demand thorough exploration of multi-layered problems.

Present your solution as the natural answer to the problems you've articulated. The mechanism by which your solution works should receive detail proportional to your audience's need to understand it. Technical buyers want to understand systems and processes, while emotional buyers want to understand experiences and outcomes. Many audiences want both, requiring you to layer your explanation accordingly.

Establish credibility in whatever form your specific audience finds most compelling. This might mean personal story and authenticity for some markets, rigorous credentials and case studies for others, or social proof and popularity indicators for still others.

Structure your benefits presentation to match how your audience evaluates value. Rational buyers need benefits tied to measurable outcomes, while emotional buyers need benefits tied to feelings and experiences. Most buyers exist somewhere on this spectrum.

Integrate social proof throughout the page in formats that resonate with your audience.

Address objections naturally as they arise in the prospect's mind rather than in a rigid sequence.

Present your offer with clarity appropriate to its complexity.

Price presentation should account for how your specific audience evaluates cost versus value. Because this is just landing page copy, we need to account for the fact that pricing should not always be revealed for all offers. If the funnel is a sales call funnel, then pricing should not be revealed. If it's a low ticket product where the checkout occurs on the actual page, then pricing should be revealed.

Risk reversal should address the specific fears your audience harbors about moving forward.

Create legitimate urgency that respects your audience's intelligence while motivating action.

Adaptive Tone Calibration
Analyze the provided documentation to determine the appropriate voice along several dimensions. Assess the formality level your audience expects, ranging from highly professional to casually conversational. Determine the appropriate energy level, from calm and measured to enthusiastic and excitable. Gauge the right balance between logical argumentation and emotional appeal. Identify whether your audience responds better to direct, aggressive selling or to soft, consultative approaches.

Output Requirements
For each section you create, provide the complete copy along with a brief notation of whether the content is directly supported by the provided documentation or enhanced based on your expertise. Include a confidence score from 1-10 indicating your assessment of the section's likely conversion impact. Add a strategic note explaining key decisions made in tone, approach, or psychological strategy.

Do not proceed until you have fully read and understood all provided documentation about the Benefits, Value Proposition, Pain Points, Questions, Concerns, and Sales Argument. Allow the true nature of the offer and audience to guide every decision you make in crafting this sales page.
```

---

### [Optional] Turn Sales Page Output into Landing Page Mockup

After generating the B2B sales page copy, you can use this prompt to create a visual mockup:

```
You have been provided with complete B2B sales page copy containing all sections from pre-headline through final call-to-action. Your task is to transform this copy into a professional, high-converting website mockup that adheres to B2B design best practices and maximizes conversion potential for small-to-medium business buyers.

Design Philosophy and Requirements:
You are creating a mockup for a B2B service targeting professional small and mid-market companies. These buyers require designs that communicate competence, stability, and ROI. The design must balance professional credibility with modern engagement techniques.

Core Design Parameters:
- Color Palette: Professional, trust-building color scheme with primary corporate blue or deep teal, complemented by neutral grays and whites. Include one accent color (orange or green) for CTAs only. Maintain 60-30-10 color distribution rule.
- Typography Hierarchy: Headlines: Modern sans-serif (Montserrat, Inter, or similar), bold weight. Body text: Clean serif or sans-serif (Open Sans, Lato, or similar). Maintain clear size hierarchy: H1 (48-56px), H2 (36-42px), H3 (24-28px), Body (16-18px)

Section-by-Section Layout:
1. Hero Section (Above the Fold): Full-width container with subtle gradient or geometric pattern background. Pre-headline in small caps. Main headline prominently displayed. Primary CTA button (high contrast, rounded corners, subtle shadow).
2. Problem Agitation Section: Centered container, maximum 900px width. Generous white space (40-60px).
3. Solution Introduction: Slight background color change. Two-column layout option.
4. Authority/Credibility Block: Horizontal layout with metrics in boxes.
5. Benefits Section: Card-based or alternating left-right layout.
6. Social Proof Section: Logo bar for client companies (grayscale). Testimonial cards.
7. Process/Method Overview: Timeline or stepped diagram layout.
8. Objection Handling Section: FAQ-style expandable cards or accordion.
9. Offer Stack: Table or stacked card layout with checkmarks.
10. Risk Reversal: Distinct visual container with badge or seal graphic.
11. Call-to-Action Sections: Large button, contrasting color. Sticky header CTA after scrolling past hero.
12. FAQ Section: Clean accordion or expandable list.
13. Final Urgency Block: Contained in a highlighted box or banner.

Technical Specifications:
- Create fully responsive design (desktop, tablet, mobile views)
- Consistent spacing system (8px base unit)
- Professional icons from a consistent icon family (Feather, Phosphor, Heroicons)
- Place CTAs at natural decision points after building value
```

---

# PHASE 3: VSL SCRIPT GENERATION

## The 9-Step VSL Framework

### Step 1: Hook Them (First 5-15 seconds)

**Job:** Stop the scroll. Create an open loop. Make them NEED to keep watching.

**Hook Formulas:**
- **The Bold Claim:** "What if I told you [specific result] is possible in [timeframe]... without [common pain]?"
- **The Story Hook:** "3 years ago, I was [relatable struggle]. Today, [impressive result]. Here's what changed."
- **The Pattern Interrupt:** "Everything you've been told about [topic] is wrong. Here's why."
- **The Question:** "Are you still [painful activity] when [better alternative] exists?"
- **The Statistic:** "[X%] of [audience] will never [achieve goal]. But the ones who do all have one thing in common."

**Rules:**
- First sentence MUST create curiosity or emotional reaction
- Never start with your name or credentials (save for Step 2)
- Match the energy to the audience (calm authority for finance, high energy for e-commerce)

### Step 2: Establish Credibility (30-90 seconds)

**Job:** Answer "Why should I listen to you?"

**Include:**
- Personal story (relatable struggle -> discovery -> transformation)
- Credentials (but make them conversational, not resume-like)
- Social proof numbers ("helped 200+ businesses", "managed $X in ad spend")
- Authority by association (clients served, industries, publications)

**Formula:** "I've [credential/experience] and helped [specific people] achieve [specific result]. But more importantly, I was exactly where you are [timeframe] ago."

### Step 3: Sell the Opportunity (2-5 minutes)

**Job:** Make them believe the CATEGORY of solution works, before you sell YOUR specific solution.

**Cover:**
- Why now is the best time (market timing, urgency)
- What's possible (paint the dream state vividly)
- Why most people fail at this (and why it's not their fault)
- The cost of inaction (what happens if they do nothing)
- The unique mechanism (YOUR specific approach that makes this work)

**Key Copywriting Principles:**
- Use "imagine" statements to paint the future
- Quantify the pain ("You're losing $X per month by not doing this")
- Introduce the enemy (what's keeping them stuck)

### Step 4: Present the Offer (2-5 minutes)

**Job:** Clearly explain what they get and why it's worth the investment.

**Structure:**
1. Name the offer
2. Walk through each deliverable (what it is, why it matters)
3. Stack the value (show individual worth)
4. Reveal the price (contrast against total value)
5. Show the ROI math
6. Present guarantee/risk reversal
7. Payment options if applicable

**Always disclose price.** Transparency builds trust and filters unqualified leads.

### Step 5: Handle Objections (2-5 minutes)

**Job:** Proactively address the top 5 objections before the viewer thinks them.

**Universal Objections to Handle:**
1. "It's too expensive" -> ROI reframe, cost of inaction
2. "I don't have time" -> Time savings the solution creates
3. "Will this work for me?" -> Case studies similar to viewer
4. "I've tried something like this before" -> Why this is different (unique mechanism)
5. "I need to think about it" -> What they're really risking by waiting

**Formula per objection:**
- Acknowledge: "You might be thinking..."
- Reframe: "But here's what most people don't realize..."
- Prove: "In fact, [client name] thought the same thing and [result]..."

### Step 6: Qualify the Audience (1-2 minutes)

**Job:** Tell them who this IS and ISN'T for. Exclusion increases desire.

**"This is for you if..."** (3-5 qualifiers)
- You're a [specific avatar] who wants [specific result]
- You're willing to [action required]
- You're currently at [stage] and want to get to [goal]

**"This is NOT for you if..."** (3-5 disqualifiers)
- You're looking for a get-rich-quick scheme
- You're not willing to [minimum commitment]
- You don't have [minimum requirement]

### Step 7: Clear Call to Action (30-60 seconds)

**Job:** Tell them EXACTLY what to do next. Remove all ambiguity.

**CTA Formula:**
"Click the button below to [specific action]. On the next page, you'll [what happens next]. The whole process takes [time estimate]. [Friction reducer]."

**Below the CTA, add friction reducers:**
- Speed: "Takes less than 2 minutes"
- Safety: "No credit card required" or "100% money-back guarantee"
- Social proof: "Join 2,600+ [audience] who already have"

### Step 8: Testimonials & Proof (1-3 minutes)

**Job:** Let other people sell for you.

**Testimonial Framework:**
- Who they are (relatable identity)
- Where they were (the "before")
- What they did (used your solution)
- Where they are now (the "after" with specific results)

**Rules:**
- Use specific numbers ("went from $3K to $15K/month" not "grew my business")
- Variety of testimonial types (video > screenshot > written)
- Match testimonials to the viewer's avatar

### Step 9: Reiterate Value & Close (1-2 minutes)

**Job:** Summarize everything and drive the final decision.

**Structure:**
1. Recap the transformation ("Remember, you came here because [problem]...")
2. Recap the offer ("Here's everything you're getting...")
3. Recap the guarantee ("And it's completely risk-free because...")
4. Final CTA ("So click the button below right now and...")
5. Scarcity/urgency if authentic ("We only take X clients per month")

---

## VSL Format A: Gamma Doc VSL Prompt (Verbatim)

Use this for slide-based VSLs (screen-recorded or used as live sales decks).

```
You are a world-class direct response copywriter and VSL strategist, specializing in creating high-converting Video Sales Letters for B2B offers. You have generated over $500M revenue for your clients by transforming complex offers into clear, persuasive, and visually engaging presentations.

Task Overview
Your task is to create a complete, slide-by-slide script for a Gamma Doc VSL. This VSL will be used in two ways:
1. Screen-recorded video for a landing page
2. Live sales deck for sales calls
Therefore, the content must be both compelling when narrated and clear when read.

Source Materials
You have been provided the following critical components:
- Document 1: Contains the core pain points, desires, value proposition, and sales argument for the offer
- Document 2: Contains the detailed, long-form sales copy for the offer
- Uploaded sales call transcripts: contains the transcripts of actual sales calls conducted with prospects for this offer.

Important: You must synthesize information from only these documents and also what has been generated inside of this chat window. Do not introduce new facts or claims not present in these materials.

Output Structure
You will structure the entire output as a series of 'Cards', where each card represents a slide in the Gamma presentation.

Execution Rules
- Structure: Create a section for each Card listed below, in the exact order provided.
- Content Source: only use content from either the uploaded documents or information established or provided within this chat window.
- Visual Suggestions: Where appropriate, suggest visual elements using the format:
  [VISUAL: Description of the visual element, e.g., a flowchart, client logo, graph showing growth]
  These visuals should be directly inspired by the content

Voice Guidelines
- Tone: Authoritative, clear, and direct
- Perspective: Write as if speaking directly to the prospect
- Language: Use 'You' and 'I' or 'We'
- Style: Professional but conversational

VSL Card Structure

Card 1: The Hook (Headline & Subheadline)
- Use the Main Headline and Subheadline directly from the uploaded documents.
- This should immediately grab attention and communicate the core value proposition
- [VISUAL: Clean, professional background with the company logo subtly visible]

Card 2: The Problem & The Stakes
- Summarize the Problem Agitation Section from the sales page copy
- Condense the paragraphs into 3-4 powerful bullet points
- Capture the essence of external, internal, and philosophical problems
- Start with a headline like "If You're Honest, This Is What Your Growth Looks Like..."
- [VISUAL: A simple but effective graphic showing a jagged, unpredictable line representing 'feast or famine' growth, contrasting with a smooth, upward-trending line labeled 'Predictable Growth']

Card 3: The Opportunity (The Big Idea)
- Introduce the core concept from the Value Proposition section of uploaded documents
- Frame it as a "New Way" of thinking
- Use a headline like "The Problem Isn't You, It's Your Model"
- Explain the concept of our offer and why it's a good opportunity for them
- [VISUAL: A diagram showing a 'before' state with the prospect juggling multiple tasks and an 'after' state where they are focused on high-value work, with the 'System' handling the rest]

Card 4: Authority & Credibility (Why Us?)
- Use the Authority/Credibility Block from the uploaded documents
- Present key points (years of experience, number of clients, industries served) as distinct, impactful statements
- Add a headline that explains what we do. Example: "We Build Predictable Client Acquisition Systems for B2B Experts". But make sure it's relevant to our offer.
- [VISUAL: Professional headshot of the founder or team. Include logos of notable clients if available]

Card 5: How The System Works (The Mechanism)
- Use the Process/Method Overview section from the uploaded documents
- List the 3-5 steps clearly
- For each step, use the Step Name as a sub-headline and briefly explain what happens
- Create a clear, logical flow
- [VISUAL: A numbered flowchart or timeline graphic that visually represents the steps]

Card 6: The Core Benefits
- Pull the Benefit Headlines and their short explanations from the Benefits Section
- Present them as a list or in a 2x2 grid
- Focus on outcome-oriented language (e.g., "Reclaim 10+ Hours Per Week")
- [VISUAL: Use a consistent icon for each benefit]

Card 7: Social Proof & Expected Results
- If source documents contain case studies or testimonials, present the most powerful ones
- Use a direct quote and highlight the single most impressive metric
- If no case studies are present, state: "please provide case studies and social proof here"
- Do not make up case studies or testimonials that are not real
- [VISUAL: A client's headshot next to their quote. If using data, create a simple bar chart]

Card 8: The Offer Stack (What You Get)
- Use the Offer Stack section from the uploaded documents
- List every component of the offer
- Present as a clear, itemized list to build value
- Do not assign a dollar amount to the value
- [VISUAL: A clean table or a series of stacked cards with checkmark icons]

Card 9: The Guarantee (Risk Reversal)
- Use the Risk Reversal section from the uploaded documents
- State the guarantee clearly and confidently
- Use a headline like "Our Pipeline Guarantee: We Don't Succeed Unless You Do", but make it contextual to the offer
- [VISUAL: A prominent guarantee badge or seal. Use a different background color for this card]

Card 10: The Call to Action (The Next Step)
- Use the CTA section from the uploaded documents
- Clearly state what the prospect should do next (e.g., "Book Your Free Strategy Call")
- Explain what will happen on the call to reduce friction and increase conversions
- [VISUAL: A large, high-contrast button with the call-to-action text]

Card 11: FAQ (Objection Handling)
- Select the top 3-4 most critical questions from the FAQ Section and/or Objection Handling Section
- Present them in a simple Q&A format
- [VISUAL: Simple, clean layout with question mark icons]

Card 12: Final Urgency (Why Act Now?)
- Use the Final Urgency/Scarcity Block from the uploaded documents
- Frame it professionally, focusing on a logical reason they need to act now, without fake scarcity
- [VISUAL: A simple, text-focused card. Perhaps a small calendar or capacity-related icon]

Final Instructions
Do not proceed until you have:
1. Reviewed all uploaded documents thoroughly
2. Understood the target audience and offer from the materials
3. Prepared to synthesize the information according to these instructions

Begin with Card 1 and work through each card systematically.

Remember: This VSL will serve as both a video script and a live sales presentation tool, so ensure the content flows naturally when spoken while remaining clear and impactful when read.

In your output, to separate each card, put three dashes like this --- to indicate a separation into a new card.
```

---

## VSL Format B: Talking Head VSL Prompt (Verbatim)

Use this for direct-to-camera VSLs. Adjust the following before using:
- **Remove visual element instructions** if you don't plan on editing with visuals
- **Adjust video length** in the "Video Length" section. Default speaking speed: ~220 words per minute. Adjust for the speaker. 5-6 minute VSLs work. 20-minute VSLs work. For cold traffic, split test short/medium/long.
- **Pricing disclosure:** If sales call funnel, don't reveal pricing in "Offer Architecture Reveal"

```
You have been provided with comprehensive documentation containing the Benefits, Value Proposition, Pain Points, Questions, Concerns, and Sales Argument for our offer. Your task is to transform this information into a compelling video sales letter script that maintains viewer attention, builds desire progressively, and drives conversion through the unique psychological dynamics of video presentation.

Understanding the VSL Medium
Video sales letters operate under fundamentally different constraints than written sales pages. Viewers cannot easily skip ahead, meaning you must maintain engagement every single second or risk losing them entirely. The linear nature of video creates opportunities for strategic reveals, pattern interrupts, and carefully orchestrated emotional journeys that would be impossible in written form. Your script must account for both the auditory and visual channels, creating a synchronized experience that leverages both simultaneously for maximum persuasive impact.

Script Development Framework
Your script should be structured in timed segments, with each segment serving a specific psychological purpose while maintaining sufficient intrigue to prevent abandonment. Unlike written copy where readers can scan, your video script must reward attention moment by moment while building toward an inevitable conclusion that feels both surprising and inevitable.

Video Length
Do your best to make sure the video is roughly 12-15 minutes long. My average speaking time is 220 words per minute. Dynamically adjust the length and depth of each of the following sections in order to fit the constraints of this time limit.

Opening Hook Sequence
Create an opening that immediately disrupts the viewer's pattern and creates an open loop that must be closed. This opening should pose a paradox, present a shocking statement, reveal an unexpected truth, or challenge a fundamental assumption your target audience holds. The goal is not merely to gain attention but to create sufficient cognitive dissonance that clicking away feels like leaving a crucial question unanswered. Include specific verbal pacing notes and any visual directions that enhance the hook's impact.

Credibility Bridge
Quickly establish why the viewer should continue listening without triggering skepticism. This credibility must be demonstrated rather than claimed, using specific details that resonate with your audience's experience. The credibility established here serves as permission to make bolder claims later in the presentation.

Problem Amplification Sequence
Articulate the problem in escalating waves, starting with surface-level frustrations and drilling down to deeper, more painful truths. Each wave should feel like a more profound revelation than the last, creating a sense that you understand their situation better than they understand it themselves. Use specific scenarios and examples that trigger recognition and emotional response. Include instructions for pacing changes and emphasis points that maximize emotional impact.

Failed Solution Acknowledgment
Address why conventional solutions have failed them, demonstrating understanding of their journey while subtly positioning your solution as fundamentally different. This section builds trust by acknowledging their past efforts while creating conceptual space for a new approach. Avoid disparaging competitors directly while making clear why previous attempts were doomed to fail.

Paradigm Shift Moment
Introduce the key insight or mechanism that makes your solution different. This should feel like a revelation that reframes everything that came before. The paradigm shift should be simple enough to grasp immediately but profound enough to justify continued attention. This is where you transition from problem to possibility, creating hope while maintaining credibility.

Solution Revelation Sequence
Unveil your solution progressively, building from concept to specific implementation. Each revelation should answer a question raised by the previous one, creating a chain of satisfaction that maintains engagement. Include specific instructions for visual support elements that reinforce key points without overwhelming the narrative flow. Balance sufficient detail to create understanding with maintaining pace to prevent boredom.

Proof Cascade
Present evidence in multiple forms that compound rather than repeat. Begin with the most universally compelling proof and layer increasingly specific evidence that addresses different skepticism triggers. Include customer stories that feel like documentary moments rather than testimonials, data that tells a story rather than just impressing, and demonstrations that feel revelatory rather than promotional. Each piece of proof should build on the previous one, creating mounting certainty rather than redundant confirmation. If these proof elements are not provided, please conduct deep research in order to find some yourself. Do not make up fake stories, however. If you need more information for this section, return inside your output that you lack sufficient proof in order to fully create this section to the best of your ability.

Benefit Transformation Sequence
Present benefits as a journey of transformation rather than a list of features. Each benefit should be introduced as a scene in the viewer's future life, making the outcome feel tangible and inevitable. Use temporal transitions and future pacing language that helps viewers step into their improved reality. Include specific sensory details that make abstract benefits feel concrete and achievable.

Objection Dissolution Pattern
Address objections preemptively using a pattern that acknowledges, reframes, and dissolves resistance rather than arguing against it. Each objection should be handled as an understandable concern that naturally resolves when viewed from the proper perspective. Use inclusive language that makes viewers feel understood rather than challenged. Include pacing notes that create space for internal processing while maintaining forward momentum.

Offer Architecture Reveal
Present the offer as the logical culmination of everything presented rather than a sales pitch. Structure the reveal to build perceived value progressively, with each component feeling like a necessary piece of the complete solution. Use visual and auditory anchoring to make abstract value feel concrete. We are not revealing the pricing of the offer, so don't do so. Pricing is only revealed on the sales call.

Risk Reversal Reframe
Position the guarantee not as protection against failure but as evidence of confidence in success. The risk reversal should feel like the natural extension of the proof already presented rather than a defensive measure. Frame the real risk as inaction rather than action, making the guarantee feel like a formality rather than a necessity.

Urgency Escalation
Create legitimate urgency that feels helpful rather than manipulative. The urgency should emerge from the viewer's situation rather than arbitrary limits, making delay feel costly rather than just unfortunate. Include specific language that transforms procrastination from a neutral choice to an active decision against their own interests.

Call to Action Sequence
Present the call to action as the beginning of transformation rather than the end of the presentation. Make the next step feel simple, obvious, and inevitable. Include specific instructions for how to maintain energy through the close without feeling repetitive or desperate. The call to action should feel like guidance for eager buyers rather than persuasion for reluctant prospects. Our call to action will be to book in a consult call.

Future Pacing Close
End with a vision of the viewer's future that makes action feel like the only rational choice. This vision should callback to the opening hook, closing the loop while opening a new chapter. The final moments should create a sense of possibility and urgency that persists after the video ends.

Technical Script Requirements
Throughout the script, include specific notations for pacing, emphasis, and tonal shifts. Mark where visual elements should appear and what emotional response each segment should evoke. Include alternative paths for different segment lengths if the video needs to be adjusted for different platforms or attention spans.

Psychological Throughlines
Maintain several psychological threads throughout the presentation that create cohesion and mounting persuasion. These include curiosity loops that open and close at strategic intervals, emotional oscillation between problem and solution states, and progressive commitment patterns that make continuing to watch feel like a series of small agreements leading to the final purchase decision.

Viewer Retention Tactics
Every 30-60 seconds, include a retention mechanism such as a pattern interrupt, a promise of upcoming revelation, or a curiosity spike that prevents abandonment. These should feel natural within the flow rather than obvious attempts to maintain attention. Include specific examples of phrases, transitions, and revelations that serve this purpose while advancing the sales argument.

Output Format Requirements
Provide the complete script with timestamps for each section, word counts to ensure proper pacing, specific notation for emphasis and tonal changes, visual cue suggestions that enhance the narrative, and alternative versions for crucial sections that can be tested. Include confidence scores for each major section and strategic notes explaining key psychological decisions and their intended impact.

The final script should feel like a conversation with a trusted advisor who happens to have the perfect solution to a pressing problem. The progression from opening to close should feel natural and inevitable, with each section building on the previous one to create mounting certainty and desire. The viewer should reach the call to action feeling that purchase is not just logical but necessary for achieving their goals.

Do not proceed until you have fully analyzed the provided documentation to understand the deep psychology of your target audience, the true transformation your offer provides, and the emotional journey required to move viewers from skepticism to enthusiasm.
```

**Notes on VSL editing:**
- Gamma Doc VSLs: generally only need removing blank spaces
- Talking head VSLs: as a starter, remove blank spaces and add captions. Maybe a bit of B-Roll.

---

# PHASE 4: HOOK FORMULAS FROM DIRECT RESPONSE FRAMEWORK

These hook formulas apply to VSLs, video ads, and any direct response content.

## The Universal Ad Flow: Hook -> Reasons -> CTA

All direct response video ads follow this structure:
- **Hook:** The first 3-5 seconds that decide whether people keep watching or scroll away
- **Reasons (Body):** The middle portion that justifies why your viewer should trust you, want your offer, or see your solution as unique
- **CTA:** Tells them exactly what to do next

## In-Market vs Needs-Convinced Framework

**In Market (3-4% of total addressable audience):**
- Already "sold" that they need what you're offering
- Don't need to be told why the overarching industry makes sense
- Need which or who: evaluating which approach or which expert to pick
- Cost to convert is lowest, sales cycles are shortest

**Needs Convinced (30% of your market):**
- Know they want the general outcome but not sure your method is correct
- Need more "why" content, higher cost per conversion
- Higher no-show and churn risk

**Core Lesson:** Begin your campaign structure and messaging for in-market prospects. Master "in market" messaging first, exploit it to the maximum, then expand outward.

## Hook Formulas for In-Market Prospects

### 3.1 The "You Already Know" Opener
"You already know [category] is one of the safest ways to [desired outcome], but have you considered [your specific method] for [specific benefit]?"
- Why it works: Instantly acknowledges their pre-existing belief. You're not pitching the category, you're pitching your method within the category.

### 3.2 The "You're Doing This, But..." Opener
"You've already tried [mainstream method], but it's draining you. There's a simpler approach to [desired result] -- [your method]."
- Why it works: Highlights a mainstream method they already know, then offers a better alternative.

### 3.3 Circumstance Openers
"Your job pays you six figures, but you still want an extra $3k-$5k a month, without messing up your career. Good news -- I found [approach] that fits busy professionals perfectly."
- Why it works: References their life circumstance, shows immediate relevance.

### Qualifying/Disqualifying In the Ad
- "If you already [qualifier], this 2-minute video is for you."
- "This isn't for people who think [category] is too risky or unproven. If you're already convinced, keep watching."

## Objection-First Hook Framework

Flip the usual script: start with the biggest objection as the hook.
- **Time:** "Pressed for time but want to grow? My method runs in about 2 hours a week."
- **Price/Capital:** "Think you need big capital? I started with under $5k total."
- **Credibility:** "Sick of internet 'gurus' who promise millions overnight? Me too. That's why I show raw, real numbers."

## Additional Ad Frameworks

### Classic Talking Head + B-Roll Overlay
1. Hook (talking head, direct camera)
2. Reasons with B-roll segments (showing results, charts, etc.)
3. Return to Head for CTA

### Case Study Snapshot Ad
1. Hook: "How did [person] go from X to Y in just 3 months?"
2. Snapshot: Quick bullet or short footage of their transformation
3. CTA: "Watch the same method. Click below."

### Demo or Screencast Framework
1. Hook: "3 steps I took on my laptop to [result]."
2. Demo: Show your screen doing the key steps
3. CTA: "Ready to replicate this? Click to see the detailed version."

### Question & Answer Style
1. Hook: "A lot of people ask me, '[common question]?' Let's answer that."
2. Body: Provide a short, direct reply with anecdote
3. CTA: "Got more questions? I answer them in my free mini-training."

### 2-Person Interview Style
1. Interviewer lobs questions
2. You answer weaving direct response points
3. Interviewer asks "where can folks learn more?" -> CTA

### Skit or Scenario Framework
1. Hook: "Meet [character]. They're done with [pain point]."
2. Show character struggling, then you appear with solution
3. CTA: "If you feel like [character], watch how we solved it."

---

# PHASE 5: VIDEO AD SCRIPT GENERATION

Use this prompt in the same conversation window after all market research and sales page copy have been produced.

```
Fully ingest this advertising SOP that I've attached including all of the images to fully understand how to make ad creatives. Then, using the offer we've been talking about in this chat, and the instructions and learning you obtain from this SOP, write me 3 ad creatives that each have 5 different hooks
```

**Structure for each ad creative:**
- 3 separate ad bodies (scripts), each with 5 different hook variations
- Total output: 15 unique hook + body combinations
- Format: 9x16 (vertical) for Meta ads
- Length: 30-60 seconds per ad (sweet spot for direct response)
- Each ad follows: Hook (3-5 seconds) -> Reasons/Body (20-50 seconds) -> CTA (5-10 seconds)

**Dynamic Creative Setup:**
- Upload 2-4 short videos
- Enter 2-3 headlines
- Enter 2-3 body copy texts
- Let the platform combine and test

**Ad Matching Rules:**
- Short ads (15-30s): Handle 1 big objection only
- Long ads (60-90s): Can handle 2-3 key objections
- Always finish by pivoting back to CTA -- never end on an objection answer
- Half your assets short, half long -- let the platform decide

---

# PHASE 6: STATIC AD SCRIPT GENERATION

Use this prompt in the same conversation window:

```
I want to test some static ads. These will just be single image ads that are 1080x1080 and just have text on them. It can't be a lot of text though because then you won't be able to read it all. Determine 3 different potential segments of the market that might be relevant for us to target, and then make me 5 different variations of static ads for each. All I need is the static ad text, because I'm going to import it into Canva.
```

**Output:** 15 static ad text variations (3 segments x 5 variations each)
**Format:** Plain text, minimal, readable on a 1080x1080 image
**Design:** Import into Canva. Use Canva AI for additional designs. Plain text image ads with very little design consistently perform well.

---

# PHASE 7: OPT-IN EMAIL SEQUENCE (Companion Deliverable)

For VSL funnels that have an opt-in, use this prompt in the same conversation window:

```
You have been provided with comprehensive documentation about an offer including Benefits, Value Proposition, Pain Points, Questions, Concerns, Sales Argument, and the core VSL script. Your task is to create a strategic five-email sequence for prospects who opted into the VSL funnel but did not immediately book a call. This sequence must work as an integrated system that progressively overcomes resistance while building desire and urgency to schedule a consultation.

Understanding the Psychological Context
These prospects have demonstrated interest by opting in and potentially watching some or all of your VSL, yet something prevented them from taking immediate action. They exist in a specific psychological state characterized by simultaneous interest and hesitation. Your email sequence must diagnose and address the specific barriers preventing action while maintaining the momentum created by the initial engagement. Each email serves as both a continuation of the VSL conversation and a standalone persuasion piece that moves them closer to booking a call.

Email Sequence Architecture and Timing
The sequence should deploy over five days, with strategic spacing that balances persistence with respect. The psychological journey moves from reengagement and curiosity renewal through education and trust building to urgency and final conversion.

Email One: The Reengagement Bridge (Send immediately after opt-in)
- Subject line should acknowledge their interest while creating a new curiosity loop
- Opening should immediately reward their decision to opt in by delivering unexpected value or insight not covered in the VSL
- Reframe their hesitation as intelligent caution while demonstrating why that caution may be costing them
- Include a soft call to action that makes booking a call feel like a natural next step
- Include a low-friction engagement trigger ("Reply with your biggest challenge")

Email Two: The Paradigm Expansion
- Expand their understanding beyond what the VSL covered
- Open with a story, case study, or hypothetical (clearly labeled) chosen to address a common but unspoken concern
- Include a teaching section that provides genuine tactical value they can implement immediately
- Close with a stronger call to action that references their specific situation

Email Three: The Authority Demonstration
- Acknowledge the proliferation of claimed experts in your field
- Systematically demonstrate unique qualifications through specific, verifiable achievements
- Present a detailed case study that mirrors your prospect's situation
- Include a risk reversal element for the call itself (a specific breakthrough they will receive regardless)
- If additional information is needed, add a note in the output

Email Four: The Urgency Catalyst
- Introduce a temporal element to their problem that makes delay genuinely costly
- Present specific examples of prospects who waited too long vs. those who acted decisively
- Introduce any legitimate scarcity elements (calendar availability, cohort timing, resource limitations)

Email Five: The Final Invitation
- Direct but warm acknowledgment that this is the final reach-out in this sequence
- Summarize the complete journey from problem through solution to transformation
- Address the meta-conversation about decision-making itself (analysis paralysis, fear-based procrastination)
- Present a final, enhanced call to action with a limited-time bonus or priority scheduling
- Close with a P.S. that provides one final psychological trigger

Technical Specifications:
- Multiple subject line variations for each email
- Optimal length: 300-600 words for earlier emails, 600-1200 for middle emails, concise for final
- Preview text optimization
- Callback references that create continuity between emails
- Sophistication progression that assumes increasing awareness

Output Format:
For each email provide: complete copy including subject lines, preview text, body copy, and CTA sections. Include strategic notes explaining psychological mechanisms. Provide confidence scores and split-testing recommendations.

Do not proceed until you have fully internalized the offer documentation.
```

---

# PHASE 8: BREAKOUT VIDEOS & PRE-CALL EMAILS (Companion Deliverable)

## Breakout Videos

Breakout videos are placed on the thank-you page after someone schedules a call. Purpose: address questions/objections that typically stop people from showing up. Normally provides a 10-30% absolute increase in show rates.

```
You have been provided with various text transcripts from the client's existing content including sales calls, coaching sessions, marketing materials, customer communications, and other relevant documents. Your task is to analyze these materials to identify the hidden friction points that prevent booked prospects from showing up to sales calls, then generate 10 strategic micro-video scripts that preemptively address these concerns while building anticipation for the call.

Critical Context Understanding
Breakout videos occupy a unique psychological moment. The prospect has just committed to a call (high intent) but hasn't yet invested significant time (low commitment). These videos are not about selling the offer -- that's the call's job. These videos are about selling the value of showing up to the call itself.

Source Material Analysis Protocol
Before generating scripts, identify:
- No-Show Triggers: fear of being "sold to," uncertainty about what the call covers, worry about wasting time, concern about affordability, imposter syndrome, practical confusion about logistics, skepticism about differentiation, fear of confrontation if they need to say no
- Pre-Call Questions: questions from the first 5-10 minutes of sales calls
- Trust Builders: what makes skeptical prospects comfortable
- Excitement Amplifiers: what creates genuine enthusiasm
- Confidence Indicators: what makes prospects feel confident they're making a good decision

Autonomous Video Topic Selection
Based on your analysis, determine the 10 most critical topics. For each, explain WHY it was chosen based on evidence.

Video Script Parameters
- Maximum: 300 words (2 minutes speaking time)
- Target Average: 100-175 words (45-70 seconds speaking time)
- Minimum: 75 words (30 seconds speaking time)

Script Architecture:
- Hook (5-10 seconds): One sentence identifying the concern or opportunity
- Core Value (25-45 seconds): The single most important point that resolves the concern
- Landing (10-15 seconds): Brief closer connecting to the value of attending the call

Output: 10 complete micro-video scripts with topic rationale, word count, speaking time, psychological objective, source evidence, confidence score, and recommended viewing sequence.
```

## Pre-Call Emails

Generally send 1 email immediately after booking, then one 24 hours before the call. Use this prompt in the same chat window where breakout videos were created:

```
Having just analyzed the source materials and generated 10 breakout videos to increase show rates, you now need to create a coordinated email sequence that works synergistically with those videos.

Three emails hit prospects at distinct psychological moments:
- Email 1 (Immediate): Peak excitement, most susceptible to booking regret. Requires confirmation they made the right choice.
- Email 2 (4 hours later): Initial excitement settled, doubt creeps in. Requires rekindling enthusiasm and practical value.
- Email 3 (24 hours later): They've slept on the decision, other priorities compete. Requires renewed urgency and anticipation.

Email 1: Immediate Confirmation & Orientation
- Warm acknowledgment, logistics clarity, immediate value delivery, video navigation, soft engagement trigger, anticipation close

Email 2: Re-Engagement & Depth
- Pattern interrupt opening, story or case study, teaching element, strategic video highlight (reference 1-2 specific videos), call reframe

Email 3: Final Anticipation Builder
- Direct value opening (best insight), preparation empowerment, social proof moment, practical confirmation, video resource summary, powerful close

Length: 200-400 words each. Mobile-optimized with short paragraphs.

Video Integration Strategy:
- Email 1: Mention videos exist as helpful resources (no specific push)
- Email 2: Highlight 2-3 videos most relevant to mid-journey doubts
- Email 3: Suggest 2-3 different videos as final preparation
```

---

# PHASE 9: PROMPT ENGINEERING & EDITING

## Key Principles for AI Copywriting

1. **There is no one "right" prompt.** Whatever is shown can always be improved upon or morphed into something else.

2. **Be "AI Brained."** Understand how to maneuver a model in specific directions. The ability to direct AI is more important than any single prompt.

3. **Context profiles are everything.** Any AI tool is just GPT/Claude/Gemini with a context profile (specific instructions OR specific knowledge documents). When you understand this, you can build your own.

4. **Same chat window rule.** Run market research, sales page, VSL, and ad prompts in the same conversation so the AI retains all context from previous steps.

5. **Never fabricate.** No hallucinated internal facts. Separate SUPPORTED vs INFERRED. Provide confidence scores. No fake stories, case studies, or testimonials. If using examples for illustration, clearly label them as "hypothetical" or "for example."

6. **Do not simply copy from uploaded material.** Come up with your own ideas based off of what you can infer and generate after understanding the uploaded material.

## Editing Workflow

After generating any copy asset:
1. Read the output fully
2. Identify sections that feel generic, weak, or disconnected from the specific offer
3. Provide specific feedback: "Section 3 is too generic -- make it specifically reference [pain point] from the sales call transcripts"
4. Ask for alternative versions of weak sections
5. Test different hooks/openings by requesting 3-5 variations

## Quality Criteria by Output Type

### VSL Script Quality Checks
- [ ] All 9 steps present (no combining, no skipping)
- [ ] Word count appropriate for target length (150 words/min speaking pace)
  - 5 min VSL: ~750 words
  - 15 min VSL: ~2,250 words
  - 30 min VSL: ~4,500 words
- [ ] Hook creates genuine curiosity in first 2 sentences
- [ ] Unique mechanism clearly explained in Step 3
- [ ] Price disclosed transparently in Step 4 (unless sales call funnel)
- [ ] All 5 universal objections addressed in Step 5
- [ ] CTA has friction reducers below it
- [ ] At least 3 testimonial slots included
- [ ] Language matches client's brand voice
- [ ] Reading level: 4th-5th grade (short sentences, simple words)
- [ ] Timestamps included for each section
- [ ] Visual/B-roll suggestions included

### Sales Page Quality Checks
- [ ] All required sections present in correct order
- [ ] Every section labeled [SUPPORTED] or [ENHANCED]
- [ ] Confidence scores provided for each section
- [ ] Headline speaks to primary transformation, not features
- [ ] Problem section escalates from external to internal to philosophical
- [ ] Objections use "Even if..." or "Without..." or "What if..." frameworks
- [ ] CTA is clear, specific, and has friction reducers
- [ ] No fake case studies or testimonials
- [ ] Reading level appropriate (8th grade for B2B, 6th grade for B2C)

### Video Ad Quality Checks
- [ ] 3 ad bodies with 5 hooks each (15 total combinations)
- [ ] Each ad follows Hook -> Reasons -> CTA
- [ ] Hooks are 3-5 seconds max
- [ ] Short ads handle only 1 objection
- [ ] Long ads handle 2-3 objections max
- [ ] CTAs include "so you can" statements
- [ ] Ads speak to in-market audience (not needs-convinced)
- [ ] Environment/visual suggestions match audience's feed

### Static Ad Quality Checks
- [ ] 3 segments identified with rationale
- [ ] 5 variations per segment (15 total)
- [ ] Text is readable at 1080x1080 size
- [ ] Each variation targets a different angle/pain point

### Email Sequence Quality Checks
- [ ] 5 emails with distinct psychological purposes
- [ ] Subject line variations provided for each
- [ ] Callback references create continuity between emails
- [ ] Value delivered in every email (not just sales pitches)
- [ ] No fake stories or fabricated case studies
- [ ] Sophistication progression across the sequence

---

## Output Format

```markdown
# VSL Script: [CLIENT NAME] -- [ANGLE NAME]

> Length: [X] minutes (approx [Y] words)
> Target audience: [avatar]
> Awareness level: [level]
> Primary angle: [angle]

---

## STEP 1: HOOK
[Script text -- what the speaker says]

## STEP 2: CREDIBILITY
[Script text]

## STEP 3: SELL THE OPPORTUNITY
[Script text]

## STEP 4: PRESENT THE OFFER
[Script text]

## STEP 5: HANDLE OBJECTIONS
[Script text]

## STEP 6: QUALIFY THE AUDIENCE
[Script text]

## STEP 7: CALL TO ACTION
[Script text]

## STEP 8: TESTIMONIALS
[Script text with placeholders for video/screenshot testimonials]

## STEP 9: CLOSE
[Script text]

---

## Production Notes
- Recommended pacing: [notes]
- B-roll suggestions: [notes]
- On-screen text callouts: [key stats/quotes to display]
```

---

## Variant: DSL (Deck Sales Letter)

A DSL replaces the video with an **embedded interactive slide deck** (Google Slides or PowerPoint) that prospects control at their own pace.

**When to use DSL vs VSL:**
| Factor | VSL (Video) | DSL (Deck) |
|--------|-------------|------------|
| Audience prefers | Narrative/story flow | Detail/control |
| Prospect type | Emotional buyers | Analytical/B2B buyers |
| Completion rates | 30-50% typical | 20-40% higher than VSL |
| Best for | Emotional products, coaching | High-ticket services, B2B |

**DSL Structure:**
- Same 9-step framework as VSL, but each step becomes slides instead of spoken script
- Final slide: Clear CTA ("Apply below" / "Schedule call" / phone number)
- Embed via Google Slides (File -> Publish to Web -> Embed) or PowerPoint for Web

**DSL Tips:**
- Use Tome.app or AI to generate slide content quickly
- Run A/B split test: duplicate VSL funnel, swap video for deck
- Track completion rates -- DSL should show 20-40% higher engagement
- Works especially well for Mini Webinar 1.0 (product/course) and 2.0 (high-ticket services) templates

**SOP Reference:** `directives/SOPs/extracted/DSL_-_Deck_Sales_Letter_Funnel_Strategy.md`

---

## Variant: Howitzer VSL (Frontloaded CTA)

> Source: Cameron Allen, *The Howitzer Video Sales Letter* (Sell More Online). The name says it all — "A howitzer isn't about precision sniping. It's about dropping massive, decisive firepower early, then keeping up a relentless bombardment until nothing's left standing."

### When to Use Howitzer vs. Standard 9-Step

| Factor | Standard 9-Step | Howitzer |
|--------|----------------|----------|
| **Funnel type** | Any (product, webinar, checkout, call) | Book-a-call funnels specifically |
| **Traffic temperature** | Warm or cold | Cold traffic (strangers) |
| **CTA placement** | Build up, CTA near end (Steps 7-9) | CTA within first 60-180 seconds, repeated throughout |
| **Philosophy** | Educate → convince → convert | Sell immediately → deepen conviction for non-converters |
| **Buyer assumption** | Range from unaware to action-ready | "In-market buyer" who is problem-aware and solution-seeking |
| **Retention reality** | Assumes 40-60% watch-through | Accepts 20-30% average VSL retention; pitches in that window |
| **Price disclosure** | Yes (transparency builds trust) | No — handled on the call ("If it makes sense, I'll tell you about pricing") |

**Key insight:** The Howitzer is designed around the observation that average VSL engagement is 20-30%. Rather than saving the pitch for the end (when most viewers are gone), it treats the first 30% as a standalone sales pitch. If they book off the hook, great. If not, the remaining 70% deepens logic, clarity, and trust.

**Contradiction note — price disclosure:** The standard 9-step framework says "always disclose price" (transparency). The Howitzer says don't reveal price on VSL for sales-call funnels — it's handled on the call. **Resolution:** Both are correct for their context. Disclose price for checkout-on-page funnels (low-ticket, courses, products). Withhold price for book-a-call funnels (high-ticket services) — the call itself is the conversion mechanism, and premature price anchoring kills conversion before the value is fully communicated.

---

### The Howitzer 11-Part Structure

#### Part 1: The Hook (First 60-180 Seconds)

This is the most important part of the entire VSL. We frontload EVERYTHING into the first 1-3 minutes.

**What to accomplish in 60-180 seconds:**
1. Immediately let the ideal prospect know this is for them
2. Talk about the big benefit your product or service delivers
3. Reinforce the outcome that will happen because of the benefit
4. Explain why this works differently than what they've tried
5. Give action takers an opportunity to take action right away
6. Stack proof, relevance, and uniqueness instantly

**We are NOT:**
- Creating intrigue
- Hooking them in
- Bribing them to watch the whole video

**We ARE:** Giving them all the possible information they would need to take action within the first 1-3 minutes. The person watching might be on the toilet, between calls, watching on mute, skeptical as hell, or — most likely — ready to buy but needing the final shove.

**Target buyer — the "In-Market Buyer":**
- Already problem-aware
- Has tried other solutions before
- Actively looking for a solution right now
- Ready to take action when they hear the right things
- Wants clarity, not "free value"
- Will give you money if you show them it's worth it

**Example Hook (Chiropractor niche):**

> If you're a Chiropractor, I will help you get 30-60 new patient appointments every single month, through our "attract, retain, and refer" strategy.
>
> Just like we've done for 134 other Chiropractors like: John, Mary, & Steven
>
> This way you can focus solely on patient care, while your calendar gets automatically filled with potential patients who are ready to pay for high-ticket care packages, and of course have the money for it...
>
> And if you've tried it all before, maybe you've even worked with a "marketing guy" who promised the world but just delivered expensive, low-quality leads...
>
> ...This is completely different. Because we pay for 100% of your ad spend. And we only get paid when a patient PAYS for a high-ticket package.
>
> Not leads. Not calls. Not even appointments.
>
> High-ticket care packages that put cash in your pocket.
>
> Until we deliver cold hard cash for you, we lose money.
>
> If that sounds good to you, and you know this is something you need, there's a button below this video to book in a quick call with me where we'll run through your business and see if this makes sense for you.
>
> If you need a bit more info, stick around and let me tell you about myself, our track record, and how this all works.

---

#### Part 2: Early CTA (Mini Checkpoint)

A quick checkpoint CTA right after the hook — for people who don't need any more convincing. You give "yes" buyers the path forward and make "maybe" buyers feel respected.

**Example Mini CTA:**

> "Now if that sounds like exactly what you've been looking for — if you already know this is something your business needs, there's a button below this video where you can book a call.
>
> We'll walk through your business, see if you're a fit, and I'll show you exactly how we'd roll this out for you — start to finish.
>
> If you're still on the fence or just want to make sure this isn't another BS marketing thing — totally cool. Stick around and I'll show you exactly how this works, why it's different, and what makes it perform."

This CTA reinforces action early without being pushy. It gives "yes" buyers the path forward and makes "maybe" buyers feel respected — keeping them engaged without triggering resistance.

---

#### Part 3: The Introduction

A breathing point after the information-dense hook. Let the cold viewer understand your authority from a high level.

**What to include:**
1. Your name
2. Your experience
3. An implied authority sentence or two
4. Why you're qualified to talk about this

**Example:**

> "Okay, let me take a quick step back and tell you who I am and why you should even listen to me in the first place... My name is Cam Allen, I'm the COO of Sell More Online and I've personally written over 1,000 ad scripts, our company has generated over $38M in directly attributable revenue for our clients and we've worked with industry leaders such as [x], [y] and [z].
>
> I'm not telling you this to brag, I just want to establish why I'm even qualified to talk about this in the first place"

---

#### Part 4: The Core Problem

Articulate their exact situation so precisely they think: "This person GETS me." This is where you achieve **emotional resonance** — the deep, subconscious connection when someone encounters experiences that align with their own feelings.

**If you can articulate their situation and problems clearly — pretty much nothing else matters. You've got them.**

**Critical: High-Frequency Pain Messaging**

Traditional pain messaging (1930s-style fear/doubt/self-pity) does NOT work with the in-market buyer. They are more sophisticated, have less time for BS, and see through typical marketing.

**Emotional Frequency Model — target HIGHER frequency emotions:**

| Target These (Higher Frequency) | Avoid These (Lower Frequency) |
|--------------------------------|-------------------------------|
| Frustration | Fear |
| Anger | Doubt |
| Status | Self-pity |
| Purpose | Desperation |
| Stagnation | Helplessness |
| Pride | Victimhood |
| Willingness | Worry |
| Desire | Anxiety |

**Why:** Frustration is a higher frequency emotion than fear. The in-market buyer operates from a "sure of themselves" level — who are you to tell him how he feels? Targeting lower frequency emotions attracts desperate, nightmare clients who see you as a lifeline, pay the least, and demand the most.

**Example — wrong vs. right:**
- WRONG: "Are you struggling to get qualified leads predictably?"
- RIGHT: "Are you finding it impossible to get your phone ringing with ready-to-book homeowners?"

Use the messaging and words they use. Assimilate into their thinking and brain.

**Inject sales call transcript data:** "If it just feels like [specific quote from transcript]" or "I get it man, you've probably just been [specific quote from transcript]"

---

#### Part 5: Introduce the False Solution (Cognitive Dissonance)

One of the most powerful copywriting techniques:

> "[Problem] isn't because of [common cause], it's actually because of [uncommon cause]"

Or:

> "Most people think the solution to [problem] is [common solution], but it's actually [uncommon solution]"

**Why this works — Cognitive Dissonance:**
1. They believe: "I need more leads to grow"
2. They're acting on that belief: spending on outbound, buying tools, running cold traffic
3. You introduce a contradictory (but believable) idea: "You don't need more leads — you need to fix your offer, pricing, and sales process first"
4. They feel tension — their actions don't align with your insight
5. If they trust you, that tension pulls them into your worldview
6. They think: "Shit. Maybe I don't need more traffic. Maybe I need to charge more and close better."
7. Now they're primed for the next section

**CRITICAL PREREQUISITE:** For cognitive dissonance to work, you MUST have trust built first. They must already think you know what you're on about, you know THEIR situation, and you are the right person to listen to. If you haven't proven that, they'll just dismiss you.

**Example (IT/MSP niche):**

> "Most IT Companies think the reason they can't scale is because they need more leads — so they try hiring cold callers, buying lead lists, running ads, but it just ends up with them constantly working with one-off jobs, getting stuck at $10k-$20k MRR but somehow working 12-14 hour days CONSTANTLY"
>
> "But in reality, you're only stuck because you're charging $100 per seat, have no real sales process or way to attract actual recurring revenue, and you have no offer that justifies charging $300+ per seat."

---

#### Part 6: Introduce the Real Solution + Future Pacing

Not your offer yet — the REASON your solution works. If you sell copywriting, this section explains why copywriting itself is the solution. You're building the "perfect opportunity."

**Example:**

> "What you need is a complete system — built from the ground up, for how your customers actually search and buy — optimized to turn those searches into real phone calls.
>
> A system you don't need to spend months building...
> A system you can actually run yourself...
> A system that gets you a guaranteed return...
> A system that is built in DAYS, not months..."
>
> "And when you have a system like this..."
> - You'll finally have predictability in your pipeline and revenue
> - You won't need to rely on contractors, freelancers, or flaky agencies
> - You'll wake up to booked calls instead of inbox anxiety
> - You'll scale without constantly rebuilding your funnel

---

#### Part 7: Reinstate the Big Promise

The "bring it home" moment. Restate the big promise from the Hook — except this time, they fully understand what it means.

**What to include:**
- Restate your core transformation promise (from the Hook)
- Tie it directly to the mechanism you just explained
- Use emotionally resonant language, not just dry "what we do" copy
- Keep it benefit-rich, not deliverables-heavy (save those for Part 9)

**Example:**

> "And yes — this is exactly what we help you install inside 7 Figure MSP. It's a plug & play sales and marketing system specifically for MSPs, designed to double your MRR within 60-120 days. A system that doesn't rely on referrals or word of mouth. A sales process that lets you charge $300/seat instead of $100."

---

#### Part 8: Case Studies / Proof

Now the only possible doubt is: "Have you done this before? Has this worked for someone like me?"

**3-Part Case Study Formula (keep each to 1-2 sentences max):**
1. Who you helped + industry they're in
2. What you helped them do
3. How you helped them do it

**Example:** "We helped George drop his cost per call by 72% after identifying one single bottleneck in his funnel"

Keep it to 3 specific case studies, then add an implied authority line: "And over 56+ other clients we've helped drop their cost per call and scale predictably..."

**Trust amplifier:** Show social media handles and invite prospects to DM your clients directly. "You can go message them and ask how it was working with us — we've not paid them or anything."

---

#### Part 9: List What They Get (Value Stack)

Make them see exactly what they physically get. Benefits alone aren't enough — they can't touch or feel "an outcome." List concrete deliverables.

**Rules:**
- Only add "so that you can..." statements on abstract features (like coaching)
- Don't explain obvious benefits: "Your entire funnel built completely done for you" doesn't need "so you don't have to touch ClickFunnels"
- Do NOT use "valued at $497" language — it's transparent and kills trust
- Make it feel like A LOT

**Example:**
> "30 days of ongoing coaching so that if you run into any roadblocks, you can just message me and we'll get it solved instantly and you'll feel 100% confident in running this system yourself."

---

#### Part 10: Address Objections (Quickly)

Quickfire style. Be transparent:

> "Look man, if you've not booked a call and you've watched this far it's probably because you have some unanswered questions. Here's the most common..."

List them off and answer truthfully. Use objections from your sales call transcripts.

---

#### Part 11: Final CTA

Close the loop. Make them feel like an irresponsible business owner for not at least hearing you out.

**7-Step Final CTA Formula:**
1. **Reopen the pain loop** (1 sentence): "If you're still stuck with [undesirable status quo]..."
2. **Re-state the transformation promise**: "...and you want to [insert main desire/outcome]..."
3. **Tie it to your mechanism/offer**: "That's exactly what we help you do with [product/service]"
4. **List what happens on the call** (simple, non-threatening): "On the call, we'll look at [X, Y, Z] and I'll show you exactly how we'd roll this out for your business."
5. **Friction-lowering line**: "If it makes sense, we move forward. If not, no hard feelings. You'll still walk away with [deliverable]."
6. **(Optional) Stack the deck**: "If I'm wrong, you'll lose 30 minutes of your day. If I'm right? Well you'll join the 2,000+ other happy [clients]..."
7. **Final CTA**: "So hit the button, pick a time, and let's talk."

**Full Example:**

> "So, if you're still stuck charging $150 per seat, relying on referrals, or constantly chasing one-off break-fix jobs...
>
> And you want to finally install a real sales system that closes $300/seat retainers with ease...
>
> That's exactly what we build with you inside 7 Figure MSP.
>
> We work with you 1-1 to help you reposition your offer, build sales assets, turn your one-off jobs into recurring revenue, and give you everything you could possibly need to double your MRR within 60-120 days.
>
> Just like we've done for over 2,000+ MSPs over the last decade.
>
> On the call we'll look at your pricing, your offer, your sales process — and I'll show you what's broken and how we'd fix it. If it makes sense, I'll tell you all about the program including pricing and everything that's included. If not, no pressure.
>
> If I'm wrong, you'll lose 30 minutes of your day. If I'm right? Well you'll join the 2,000+ other happy MSPs who are scaling predictably and building the businesses they set out to do when they started.
>
> So hit the button below, pick a time, and let's talk."

---

### When to Recommend Howitzer vs. Standard

**Default to Howitzer when:**
- Client runs a book-a-call funnel with cold traffic
- Offer is high-ticket ($2K+)
- Target audience is in-market buyers (problem-aware, solution-seeking)
- Price is NOT disclosed on the page
- Average VSL engagement is expected to be 20-30%

**Default to Standard 9-Step when:**
- Low-ticket product with checkout on-page (price must be disclosed)
- Webinar or challenge funnel (longer education needed)
- Audience is problem-unaware (needs full education arc)
- Client specifically requests value-first, CTA-last structure

**Can combine both:** Use Howitzer structure but include Standard 9-Step depth in the post-hook sections for particularly skeptical or analytical audiences.

**SOP Reference:** `directives/incoming/copy-of-the-howitzer-video-sales-letter.md` -- The Howitzer Video Sales Letter by Cameron Allen (Sell More Online)

---

## Metrics to Track Post-Launch

| Metric | Target | What It Tells You |
|--------|--------|-------------------|
| Play rate | 30-60% | Is the thumbnail/headline compelling? |
| Watch-through rate | 40-60% | Is the content engaging? |
| Drop-off point | After Step 3 | Where are you losing people? |
| CTA click rate | 5-15% | Is the offer compelling? |
| Booking/conversion rate | 10-30% of clicks | Is the CTA page optimized? |
| Cost per 3-second view | Lower = better hook | How well the hook grabs attention |
| CTR (click-through rate) | Above 0.5% | Is ad pulling curiosity? |
| Ad frequency | Below 3-4 | Are you hitting ad fatigue? |

---

## Ad Scaling & Maintenance Framework

**Refresh creatives every 2-4 weeks** or sooner if cost creeps up.

**Dynamic Creative Testing:**
- Upload 2-4 short videos, 2-3 headlines, 2-3 body copy texts
- Let platform combine and test for 5-7 days
- Monitor cost per 3-second view (hook quality) and cost per result (lead quality)
- Swap out losers, scale winners, re-check audience if everything flops

**Scaling approach:**
- Gradual: 10-20% budget increase every 2-3 days
- Aggressive: Double budget if funnel is proven stable for 5-7 days
- Scale by duplication: Clone winning ad set with bigger budget

**Signs of scale fatigue:**
- CPL creeps up 20-30% or more
- Frequency metrics show same audience being hammered
- Sales team reports less qualified leads

**The Hammer Them Strategy (Post-Opt-In):**
Once people opt in or schedule a call, hammer them with short content ads (15-20+ pieces) to build familiarity, preempt objections, and replicate the sense of "they've seen 30 of your videos." This boosts show-up rates, shortens the sales cycle, and ensures they walk into the call warm and trusting you.

---

## Training Data Sources for AI Copy

Always be sourcing new training material. Upload these to the AI for better context:

**Written Assets:** Past marketing emails, existing sales letters or VSL scripts, website copy, landing pages, blog posts, ad copy, sales presentations, product descriptions, course outlines, FAQs, customer testimonials/reviews

**Video & Audio:** YouTube transcripts, podcast transcripts, webinar replays, coaching call recordings/transcripts, client interviews, case study videos, sales/demo call recordings, training videos

**Social Content:** Facebook/Skool group posts, Instagram captions, LinkedIn posts, Twitter/X threads, TikTok scripts, community Q&A posts, replies to customer comments/DMs

**Internal:** SOPs, brand voice guidelines, sales scripts, coaching frameworks, customer survey responses, support tickets, market research reports, notes from discovery calls

---

## SOP References

When deeper context is needed, read:
- `directives/SOPs/extracted/Mastering_VSLs_(Video_Sales_Letters)_SOP.md` -- Full VSL methodology
- `directives/SOPs/extracted/AI_Copywriting_SOP_-_Daniel_Fazio.md` -- Copywriting fundamentals and all prompts
- `directives/SOPs/extracted/Direct_Response_Ad_Creation_Framework_SOP.md` -- Hook and CTA frameworks, scaling strategy
- `directives/SOPs/extracted/Challenge_Funnel_Mastery_SOP.md` -- Funnel context for VSL placement
- `directives/SOPs/extracted/DSL_-_Deck_Sales_Letter_Funnel_Strategy.md` -- DSL variant
- `directives/Vibe-Skills-Claude-Code-v.01/direct-response-copy/SKILL.md` -- Copy frameworks (Schwartz, Hopkins, etc.)
- `directives/incoming/copy-of-the-howitzer-video-sales-letter.md` -- Howitzer VSL (frontloaded CTA variant) by Cameron Allen (Sell More Online)

---

## Connections

- **Requires:** Offer (from offer-creation skill), angles (from positioning-angles skill), avatar research, creative strategy
- **Feeds into:** Landing page (VSL is embedded on the page), ad scripts (ads drive traffic to VSL), email sequences (nurture non-converters)
- **Part of:** Phase III of the client pipeline (see `directives/client_onboarding.md`)
