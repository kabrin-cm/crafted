
---

## 8. EMAIL DELIVERABILITY & SPAM PROTECTION

# Skill: Spam & Bot Traffic Protection

> Complete tactical SOP for identifying, eliminating, and preventing spam and bot traffic that burns your pixel, spams your calendar, and destroys campaign performance. Covers immediate fix protocol, pixel recovery, Cloudflare IP blocking, trap funnel strategy, and last-resort measures. Extracted from Evan Seech's *Spam & Bot Traffic Blocking SOP* (Sell More Online).

## Trigger Keywords

`spam traffic`, `bot traffic`, `spam leads`, `bot leads`, `spam blocking`, `bot blocking`, `pixel spam`, `burned pixel`, `fake leads`, `spam bookings`, `bot bookings`, `spam calls`, `low CPM`, `high CTR no conversions`, `spam protection`, `clickcease`, `CAPI`, `conversion API`, `trap funnel`, `IP blocking`, `spam calendar`, `pixel recovery`

---

## Core Job

Help anyone running ads eliminate bot and spam traffic if they get affected by it, so they can get back to normal fast -- covering identification, immediate response, pixel recovery, preventive infrastructure, and trap funnels to neutralize persistent attackers.

---

## Target Audience

Anyone who is running ads and dealing with spam leads and/or a ton of clicks to their landing page and no conversions. Personal Brands, High Ticket Product or Service Businesses, Digital Marketers, Agencies, and Entrepreneurs running paid traffic on Meta, Google, or any ad platform.

---

## Inputs Required

| Input | Required? | Source |
|-------|-----------|--------|
| Ad platform access (Meta, Google, etc.) | Yes | User |
| CRM / calendar access | Yes | User |
| Current funnel URL(s) | Yes | User |
| Pixel / tracking setup details | Yes | User |
| Domain registrar access | Yes | User |
| Cloudflare account (or willingness to set up) | Helpful | User |
| Hyros or other tracking tool access | Helpful | User |
| Recent campaign performance data (CPM, CTR, conversions) | Yes | Ad platform |
| Lead submission logs with timestamps | Yes | CRM / form tool |
| Confirmation page event setup details | Yes | User / pixel setup |

---

## Signs of Potential "Bot" Traffic

It will be pretty darn clear when you get spam/bot traffic coming in. But here are the indicators that show you have a high likelihood of bot traffic hitting your funnel.

**Important distinction:** If you get a few "funnel hackers" in a day, that is most likely NOT spam/bot traffic. Spam/bot traffic is a **deliberate attempt by somebody to burn your pixel and spam your calendar.**

### Bot Traffic Indicators

| Indicator | What It Looks Like |
|-----------|-------------------|
| **Abnormally low CPMs** | CPMs drop well below your historical average without a corresponding improvement in targeting or creative. The platform is serving impressions to low-quality traffic. |
| **Spam lead submissions** | Applications and/or call bookings flooding in -- not just a handful, we are talking **5-10+ in a short period of time.** These are deliberate spam entries. |
| **Abnormally low cost per call** | Cost per booked call drops to suspiciously cheap levels because bots are completing the booking flow. |
| **Abnormally high CTR (10%+)** | Click-through rates spike to 10% or higher, combined with low Typeform starts and low application completions. Lots of clicks, no real engagement. |
| **Tons of confirmation page clicks without conversions** | Massive clicks to your confirmation page causing pixel fires but no real downstream conversions. This is what burns your pixel -- it trains on garbage data. |

---

## Immediate Fix Protocol

If you're getting bot traffic, do ALL of the following. **Pause everything and block off 1 hour to fix things ASAP.**

### Step 1: Pause ALL Campaigns Immediately

Do not let another dollar spend while bots are active. Pause every campaign across every ad set. This stops the bleeding.

### Step 2: Remove the Standard Event Code from the Confirmation Page

The standard event on your confirmation page is what the bots are triggering. Every time they click through to your confirmation page, it fires a conversion event that poisons your pixel data. Remove the standard event code immediately to stop false conversion signals.

### Step 3: Switch to a Full CAPI (Conversion API) Setup

Replace the standard pixel event with a full server-side Conversion API (CAPI) setup. CAPI sends conversion data server-to-server rather than through the browser, which makes it much harder for bots to trigger false events. This is your new standard going forward.

### Step 4: Buy a New Domain

The bots have your current domain. Purchase a new domain for your funnel. Do not reuse the compromised domain for running traffic.

### Step 5: Switch the Domain on the Funnel

Update your funnel to use the new domain. All funnel pages should now resolve on the new domain.

### Step 6: Switch the Domain in Your Typeform & Ads

Update the domain in:
- Your Typeform or application form (embedded URLs, redirect URLs)
- All ad creatives (destination URLs, display URLs)
- Any other integrations that reference the old funnel URL

### Step 7: Set Up Redirects from Old Domain

If the old domain was out in the wild on socials, emails, etc., set up redirects. **Critical:** Do NOT redirect the old domain to your new domain. Instead:
- Duplicate your funnel on ANOTHER domain (a third domain)
- Redirect the old domain to that third domain
- This keeps the new domain you are running traffic to protected and unknown to the attacker

### Step 8: Delete All Spam Leads

Delete all spam leads from:
- Your CRM
- Your calendar (Calendly, etc.)
- Any other systems where spam entries exist

Clean the pipeline completely so your sales team is not wasting time on fake bookings.

### Step 9: Duplicate Any Affected Campaigns/Ad Sets

Do not restart the old campaigns. Duplicate them fresh. This gives the algorithm a clean slate rather than continuing to optimize around poisoned data.

### Step 10: Block IPs and Emails

If you can identify the attacker's IP addresses or email addresses:
- Block them at the platform level
- Block them in your funnel/hosting
- If you use **Hyros**, you can find IP and email data for the spam entries there

---

## Pixel Recovery

### When to Create a New Pixel vs Retrain the Old One

**Decision threshold: 50+ spam conversions.**

- If you ignored the problem for days and accumulated **50+ conversions** from spam traffic that hit in a very short period of time, your pixel is severely poisoned.
- In this case:
  1. **Create a new pixel** and optimize around it in the short term
  2. **Keep the old pixel on the page** as well so it continues to collect data and "retrain" on real conversions
  3. Optimize campaigns around the new pixel
  4. Once quality has stabilized on the old pixel (it's learning from real conversions again), you can switch back to it

- If the spam volume was lower (under 50 conversions), you can likely recover the existing pixel by:
  1. Removing the standard event (already done in Step 2)
  2. Switching to CAPI (already done in Step 3)
  3. Feeding it clean conversion data going forward
  4. Monitoring for quality stabilization over 1-2 weeks

---

## Additional Protection Methods

### Cloudflare Hosting for IP Blocking

Host your funnel on **Cloudflare**. This gives you the ability to:
- Manually block IP addresses that come through as spam
- Set up firewall rules to filter suspicious traffic
- Potentially have someone build an **agentic AI** to automatically detect and block spam IPs for you (automated IP blocking based on behavior patterns)

Cloudflare is a proactive measure -- set it up even before you get hit, so you have the infrastructure in place when you need it.

### Trap Funnel Strategy

This is an offensive counter-measure. You set up a decoy so the attacker wastes their time on a fake funnel while your real traffic goes to a clean one.

#### Step-by-Step Trap Setup

**Step 1:** Duplicate out your funnel, form, and scheduler. You now have two copies of everything.

**Step 2:** Add a **"dummy closer"** to your scheduler (Calendly). This is a fake user/team member -- not a real salesperson.

**Step 3:** On the **original scheduler** (the one being attacked), add the newly created dummy closer.

**Step 4:** Set the original scheduler to allow bookings **14-21 days out**. This makes the attacker think they're still booking real calls, but the bookings go nowhere and are far enough out to be meaningless.

**Step 5:** On the **newly duplicated funnel** (with the newly duplicated application and scheduler), duplicate out your campaigns to point to the new page URL (new funnel).

**Step 6:** Remove ALL real salespeople or closers from the original scheduler. Only the dummy closer/fake user should remain on the original scheduler to accept bookings.

**Step 7:** The result:
- **Original funnel** = the "trap." Bots and spammers book on nothing. The dummy closer absorbs all fake bookings 14-21 days out.
- **New duplicated funnel** = where you direct real traffic. Your actual sales team (real users) are only on this scheduler.

**Step 8:** If the attacker finds the new funnel, **repeat the process.** Duplicate again, set up a new trap, move real traffic to the newest funnel.

### ClickCease (Last Resort)

If everything else continues to be an issue:
- Install **ClickCease** (clickcease.com)
- This is a dedicated click fraud prevention tool that automatically detects and blocks fraudulent clicks
- Use this as a last resort after you've already implemented CAPI, new domain, Cloudflare, and trap funnels
- ClickCease adds cost and complexity, so exhaust the other methods first

---

## Response Priority Order

When bot traffic is detected, execute in this order:

```
1. PAUSE all campaigns (immediate -- stop the bleeding)
2. REMOVE standard event from confirmation page (stop pixel poisoning)
3. SWITCH to full CAPI setup (prevent future browser-based spam triggers)
4. BUY new domain + switch funnel + switch ads (escape the compromised domain)
5. SET UP redirects from old domain (protect new domain)
6. DELETE spam leads from CRM & calendar (clean the pipeline)
7. DUPLICATE affected campaigns (fresh algorithm start)
8. BLOCK IPs/emails if identifiable (targeted defense)
9. ASSESS pixel damage (new pixel if 50+ spam conversions)
10. SET UP Cloudflare (ongoing IP blocking infrastructure)
11. DEPLOY trap funnel (offensive counter-measure for persistent attackers)
12. INSTALL ClickCease (last resort if attacks continue)
```

---

## Monitoring & Detection Checklist

Use this checklist to catch bot traffic early before it causes major damage:

### Daily Monitoring (During Active Campaigns)

- [ ] Check CPMs against historical average -- flag any abnormal drops
- [ ] Review lead submissions for obvious spam patterns (fake names, gibberish emails, rapid-fire submissions)
- [ ] Check CTR -- flag anything above 10% with low downstream engagement
- [ ] Review confirmation page event fires vs actual legitimate bookings
- [ ] Check cost per call -- flag any abnormal drops

### Weekly Review

- [ ] Compare lead quality this week vs last week
- [ ] Review any blocked IPs/emails (if Cloudflare or Hyros is set up)
- [ ] Confirm CAPI is functioning correctly (server-side events firing)
- [ ] Check pixel health -- conversion quality score in ad platform

---

## Output Format

When responding to a bot traffic incident for a client, deliver:

```markdown
# Bot Traffic Response Plan: [CLIENT NAME]

## Incident Assessment
- Date detected: [X]
- Indicators present: [list which of the 5 indicators are showing]
- Estimated spam volume: [X leads / X confirmation page fires]
- Pixel damage assessment: [Under 50 spam conversions / Over 50 -- new pixel needed]
- Duration of exposure: [How long before detection]

## Immediate Actions (Execute Now)
1. [ ] Pause all campaigns
2. [ ] Remove standard event from confirmation page
3. [ ] Switch to CAPI setup
4. [ ] New domain purchased: [domain]
5. [ ] Funnel switched to new domain
6. [ ] Typeform/ads updated with new domain
7. [ ] Old domain redirected to third domain (NOT new domain)
8. [ ] Spam leads deleted from CRM and calendar
9. [ ] Campaigns duplicated fresh
10. [ ] IPs/emails blocked (if identifiable)

## Pixel Recovery Plan
[New pixel needed? Steps to create and dual-run with old pixel]
[Or: existing pixel recovery timeline and monitoring plan]

## Preventive Infrastructure
- [ ] Cloudflare hosting set up for IP blocking
- [ ] Trap funnel deployed (if persistent attacker)
- [ ] ClickCease installed (if needed as last resort)

## Ongoing Monitoring Plan
[Daily and weekly checks to catch future incidents early]
```

---

## Quality Checks

- [ ] All 5 bot traffic indicators are being monitored
- [ ] Campaigns paused immediately upon detection (no continued spend during bot attack)
- [ ] Standard event removed from confirmation page
- [ ] CAPI setup confirmed functional (server-side events only)
- [ ] New domain purchased and funnel migrated
- [ ] Old domain NOT redirected to new domain (redirected to third domain or nowhere)
- [ ] All spam leads purged from CRM and calendar
- [ ] Campaigns duplicated fresh (not restarted from poisoned state)
- [ ] IPs/emails blocked where identifiable
- [ ] Pixel damage assessed against 50-conversion threshold
- [ ] New pixel created if threshold exceeded, with old pixel still collecting data for retraining
- [ ] Cloudflare hosting in place for ongoing IP blocking capability
- [ ] Trap funnel deployed if attacker is persistent (dummy closer, 14-21 day booking window)
- [ ] Real salespeople removed from original (trap) scheduler
- [ ] ClickCease installed only as last resort after other methods exhausted
- [ ] Sales team notified about spam incident and cleaned pipeline
- [ ] Daily monitoring checklist in use for early detection going forward

---

## Edge Cases

### Attacker Finds New Domain Quickly
Repeat the trap funnel process. Duplicate everything again, move real traffic to newest funnel, convert previous funnel into new trap. This is a war of attrition -- each iteration costs the attacker time and reveals nothing about your real funnel.

### Pixel Damage Uncertain (Near 50 Threshold)
When in doubt, create the new pixel. It's better to spend a few days training a clean pixel than to continue optimizing around a potentially poisoned one. Keep the old pixel on the page to retrain in parallel.

### Client Has No Cloudflare Setup
Set up Cloudflare first as part of the response. It's free for basic plans and gives you immediate IP blocking capability. This should become standard infrastructure for all clients running paid traffic.

### Spam Leads Already Contacted by Sales Team
Notify the sales team immediately. Flag which leads were spam so closers stop wasting time. Review any calls that were conducted with spam leads to ensure no sensitive information was shared.

### Multiple Ad Platforms Affected
Execute the fix protocol per platform. Each platform has its own pixel/CAPI setup. New domain and funnel migration covers all platforms simultaneously, but pixel recovery and campaign duplication must be done per platform.

### Bot Traffic During a Launch or Promo
Critical timing issue. Execute Steps 1-3 immediately (pause, remove event, switch to CAPI). For Steps 4-7 (new domain, migration), move fast but verify everything before reactivating. A botched migration during a launch is worse than a brief pause.

---

## SOP References

- `directives/incoming/copy-of-spam-bot-traffic-blocking-sop.md` -- Full spam and bot traffic blocking SOP by Evan Seech (Sell More Online)
- `directives/Vibe-Skills-Claude-Code-v.01/meta-ad-strategy/SKILL.md` -- Ad strategy (campaigns that may be affected)
- `directives/Vibe-Skills-Claude-Code-v.01/landing-page/SKILL.md` -- Landing page and funnel setup (domain migration)

---

## Connections

- **Requires:** Ad platform access, CRM access, domain registrar access, funnel builder access, pixel/tracking setup details
- **Pairs with:** Meta ad strategy (campaign management during and after bot attack), landing-page (funnel duplication and domain migration), confirmation-page (event code removal and CAPI setup)
- **Part of:** Campaign health and maintenance -- this is a reactive and preventive skill that protects all active paid traffic
- **Feeds into:** Clean campaign data, accurate pixel optimization, protected sales pipeline, reliable cost-per-acquisition metrics
