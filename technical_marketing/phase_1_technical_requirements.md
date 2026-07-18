# Phase 1 Technical Requirements & Data Output

## The Principle

"Separate 'getting it running' from 'building the ideal tracking system' because Meta makes it harder than necessary."

**Phase 1 deliberately avoids:** Pixels, conversion tracking, Events Manager, automations, complex integrations.

---

## Systems That Need Configuration

### 1. Mailchimp (Existing or New)

**What to do:**

- Create or use existing signup form
- Create a dedicated landing page in Mailchimp specifically for this event/offer
- Add fields: name, email (required), optional timezone or how they heard about it

**Time to set up:** 30 min (if you have a Mailchimp account)

**Cost:** $0-20/month (free tier works for small lists)

**What it does:** Captures registrations + sends confirmation email with Zoom link

---

### 2. Facebook Ads Manager (Meta Business Suite)

**What to do:**

1. Go to Meta Business Suite → All Tools → Ads Manager
2. Create new Campaign with **Traffic** objective (NOT Conversions, NOT Leads)
3. Name it: "Soul GYM - Amusement - July 2026 - Traffic Test"
4. Set budget: $5-10/day for 4-7 days
5. Choose ad set options:
   - Conversion location: Website
   - Performance goal: **Maximize landing page views** (not clicks, not reach)
6. Build audience:
   - Location: US & Canada
   - Age: 35-70+
   - Gender: All
   - Interests: Meditation, spirituality, personal development, mindfulness, emotional intelligence
   - Placements: Advantage+ (Facebook + Instagram, all placements)
7. Upload ad creative (image + text + headline)
8. Paste Mailchimp signup page URL as destination
9. Publish

**Time to set up:** 1-2 hours (first time; faster after)

**Cost:** $50 total ($5-10/day × 5-7 days)

**What it provides (automatically):** Ad reach, impressions, clicks, click-through rate (CTR), cost per click, landing page views, cost per landing page view

---

### 3. Landing Page (Mailchimp or Website)

**What to include:**

- Your image
- Invitation text (1-2 paragraphs)
- Date and time
- "Online via Zoom"
- Name and email fields
- One clear button ("Join Us" or "Register")
- Brief line: "Registering sends you the Zoom link"

**No tracking pixels needed yet.**

**Time to set up:** 30 min (Mailchimp form) to 1 hour (custom website page)

**Cost:** $0 (if using Mailchimp) to hosting cost (if on your website)

---

### 4. UTM Parameters (Optional but Recommended)

**What to do:**

- Add to Mailchimp signup page URL:

  ```text
  ?utm_source=facebook&utm_medium=paid_social&utm_campaign=soul_gym_amusement_july_2026
  ```

**Time to set up:** 5 min

**Cost:** $0

**What it does:** Helps you distinguish Facebook ad traffic from other sources in analytics (if you use Google Analytics)

---

### 5. Manual Tracking (Spreadsheet or Mailchimp Automation)

**What to track manually:**

- How many registered (Mailchimp shows this)
- How many actually attended (check Zoom attendee list after the event)
- Any repeat attendees

**Time to set up:** 5 min (a simple spreadsheet)

**Cost:** $0

---

## What Data Phase 1 Provides

### From Facebook Ads Manager (Automatic)

| Data Point                     | What It Shows                            | Use                                  |
|--------------------------------|------------------------------------------|--------------------------------------|
| **Impressions**                | How many times the ad was shown          | Scale of audience reached            |
| **Clicks**                     | How many people clicked the ad           | Interest level                       |
| **Click-Through Rate (CTR)**   | Clicks ÷ Impressions                     | Is the ad compelling? (target: 1-3%) |
| **Landing Page Views**         | How many people actually loaded the page | Did they get there?                  |
| **Cost Per Click**             | $ spent ÷ Clicks                         | Efficiency of the ad                 |
| **Cost Per Landing Page View** | $ spent ÷ Page views                     | Efficiency at the next step          |

**How to access:** Ads Manager → Campaigns → View detailed breakdown

---

### From Mailchimp (Automatic)

| Data Point                  | What It Shows                 | Use                 |
|-----------------------------|-------------------------------|---------------------|
| **Form Submissions**        | Total registrations           | Did people say yes? |
| **Email Subscribers Added** | New contacts on your list     | List growth         |
| **Unsubscribes or Bounces** | Problems with email addresses | Data quality        |

**How to access:** Mailchimp → Form → Stats

---

### From Zoom (Manual Check)

| Data Point           | What It Shows                   | Use                                           |
|----------------------|---------------------------------|-----------------------------------------------|
| **Attendees**        | Who showed up                   | Registration → attendance rate (target: >60%) |
| **Repeat Attendees** | How many you've seen before     | Is this reaching new people?                  |
| **No-Shows**         | Registrations who didn't attend | Reminder/timing problem?                      |

**How to access:** Zoom → Meeting Reports → Participants

---

## What You DON'T Track Yet

**Deliberately excluded from Phase 1:**

- ❌ Meta Pixel installation
- ❌ Conversion events (paid registration, course enrollment, etc.)
- ❌ Custom conversions
- ❌ Events Manager
- ❌ Advanced audiences or lookalike audiences
- ❌ Multi-touch attribution
- ❌ Automated remarketing

**Why:** "Technology amplifies. It rarely rescues." If the *message* doesn't work, better tracking just helps you spend money on the wrong thing.

---

## Data Analysis: What Each Metric Tells You

### If Few People Click the Ad

→ Problem is the **ad itself** (image, headline, or targeting is off)

**Fix:** Change the ad creative or targeting, not the offer

### If People Click but Few Land on Page

→ Problem is **landing page load** or **link destination**

**Fix:** Check the URL works, page loads fast, no broken links

### If People Land but Few Register

→ Problem is the **registration page or offer** (unclear, too many fields, not compelling)

**Fix:** Simplify the form, clarify the invitation, remove friction

### If People Register but Few Attend

→ Problem is **reminder, timing, or setup**

**Fix:** Better reminder email before event, clearer Zoom instructions, better day/time

### If Few Register + Few Attend

→ Problem is the **message itself** -- people don't actually want this

**Fix:** Different invitation text, different offer, different targeting, or different product entirely

---

## Total Time & Cost for Phase 1

| Component               | Time             | Cost     |
|-------------------------|------------------|----------|
| Mailchimp signup page   | 30 min           | $0       |
| Facebook ad setup       | 1-2 hours        | $50      |
| Landing page/invitation | 30 min           | $0       |
| UTM parameters          | 5 min            | $0       |
| Manual tracking sheet   | 5 min            | $0       |
| **Total**               | **~2.5-3 hours** | **~$50** |

---

## What Phase 1 DOESN'T Require

✅ You don't need a website
✅ You don't need coding
✅ You don't need a developer
✅ You don't need to understand marketing funnels
✅ You don't need automation or workflows
✅ You don't need analytics expertise
✅ You don't need a business plan
✅ You just need: Mailchimp (free), Facebook Ads Manager (free), $50, and 3 hours

---

## Bottom Line

**Phase 1 is intentionally simple.** It answers one question: "Does this message move people to register?"

Everything else (optimization, automation, advanced tracking) comes only if Phase 1 says "yes."
