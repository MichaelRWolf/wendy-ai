# Facebook Sales Campaigns

## Resources

- [Facebook Conversion Campaign Guide](https://www.facebook.com/business/m/conversion-campaign)
- [Facebook Conversions Playbook PDF](https://scontent-msp1-1.xx.fbcdn.net/v/t39.8562-6/394497629_346601301211150_6997970709125168462_n.pdf/ConversionsPlaybook.pdf?_nc_cat=108&ccb=1-7&_nc_sid=e280be&_nc_ohc=K_hkaUxtfnsQ7kNvwHpU8TW&_nc_oc=Adrz3AB3akQTh_DPNYVMJbhgl-QYfpSNiZMfYoVMPeIUHKTFY2WBBfA1-UBXkPiPAWg&_nc_zt=14&_nc_ht=scontent-msp1-1.xx&_nc_gid=-hYY2H1bgutJ2TW-PRgRQg&_nc_ss=7b2a8&oh=00_AQDCo47wlkhohYz-TPJOOvx_hQjLKR3_D-T9ZiCfZFnRJw&oe=6A604D4C)

## Planning Context

This document captures the technical foundation for Facebook ad campaigns, extracted from ChatGPT guidance on Meta's ad setup and tracking architecture. The conversation evolved from exploring Tony Robbins and Dean Graziosi's approach toward Wendy-specific testing frameworks.

## ChatGPT Guidance: Separation of Concerns

The starting principle: separate "getting it running" from "building the ideal tracking system" because Meta makes it harder than necessary.

### Phase 1: Simple Traffic Test (This Month)

**Don't touch:** Pixels, conversions, Events Manager yet.

**Just do:**

1. Write a good invitation
2. Create a Mailchimp signup page
3. Open Ads Manager
4. Choose Traffic objective
5. Paste in the Mailchimp URL
6. Spend $5-10/day for a few days
7. See what happens

### Phase 2: Conversion Optimization (If Phase 1 Shows Promise)

Learn one thing: How to get Meta to optimize for registrations instead of clicks. This involves Pixels and thank-you pages.

### Phase 3: Scaling (If Phase 2 Works)

Then optimize.

## The Full Technical Setup (For Reference)

### Part 1: Prepare the Signup Destination

Use a registration page specific to each gathering containing:

- Your image
- The invitation
- Date and time
- "Online through Zoom" (if applicable)
- Name and email fields
- One clear button (e.g., "Join Us")
- Brief assurance that registering sends Zoom information

Ideally send registrants to a distinct thank-you page:

```text
wendyrwolf.com/soul-gym-thank-you
```

### Part 2: Open Ads Manager

Meta Business Suite → All Tools → Ads Manager

Do not begin from the Facebook Event's Boost button.

### Part 3: Campaign Objective

Select: **Traffic**

Name the campaign something recognizable:

```text
Soul GYM - Amusement - July 2026 - Traffic Test
```

Leave these off initially unless Meta requires them:

- Advantage campaign budget
- A/B test
- Special ad category

### Part 4: Configure the Ad Set

**Conversion location:** Website

**Performance goal:** Maximize number of landing page views (not Link Clicks, Daily Unique Reach, or Impressions)

### Part 5: Set a Real Test Budget

For a modest first test: $5-$10 per day for 4-7 days. This gives Meta room to distribute and you enough activity to observe.

### Part 6: Build the Audience

**Location:** United States and Canada (or adjust for your market)

**Age:** Genuine range likely to participate (e.g., 35-70+)

**Gender:** All (unless specifically designed for a particular population)

**Detailed targeting:** Start broad with related signals:

- Meditation
- Personal development
- Spirituality
- Mindfulness
- Emotional intelligence

Allow Advantage+ Audience to expand, but keep geographic and age boundaries sensible.

### Part 7: Placements

Use: **Advantage+ placements**

This shows across Facebook and Instagram. Later, inspect whether registrations come disproportionately from Feed, Stories, or Reels.

### Part 8: Create the Ad

1. Select your Facebook Page and Instagram account
2. Choose Single image or video
3. Upload the image
4. Add the registration-page URL
5. Choose a button: Sign Up, Learn More, or Register

**Primary text:** Shorter version of your invitation. First lines matter most.

**Headline:** Straightforward and action-oriented

**Description:** Brief logistics summary, e.g., "Live online practice • Newcomers welcome"

### Part 9: Add Tracking to the URL

Even before installing Meta Pixel, add tracking parameters:

```text
https://your-registration-page.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=soul_gym_amusement_july_2026
```

Or use Meta's URL parameters box:

```text
utm_source={{site_source_name}}&utm_medium=paid_social&utm_campaign=soul_gym_amusement_july_2026&utm_content={{ad.name}}
```

### Part 10: Preview Carefully

Check across:

- Facebook Feed
- Instagram Feed
- Mobile
- Stories

Verify text is not cut off, image is readable, button works, page loads on phone, form is not difficult, and date/time/timezone are unmistakable.

## Advanced Setup: Full Pixel Tracking (When Ready)

### Events Manager Setup

Meta Business Suite → All Tools → Events Manager

1. Click Connect Data Sources
2. Choose Web → Meta Pixel
3. Name it (e.g., "BLOOM Website Pixel")
4. Enter your website
5. Follow WordPress installation (plugin or partner integration preferred over manual code)

### Custom Conversion Setup

1. Open Custom Conversions
2. Click Create custom conversion
3. Select your Pixel
4. Use a rule: URL contains → thank-you-soul-gym
5. Name it: Soul GYM Registration
6. Choose category: Lead or Complete Registration

### Ideal Long-Term Architecture

Facebook ad → registration page on wendyrwolf.com → Mailchimp form embedded on that page → thank-you page on wendyrwolf.com → confirmation email with Zoom information

This gives:

- Control of the page
- Meta tracking
- Your own domain
- Mailchimp list growth
- Coherent welcome experience
- Cleaner measurement

## Measurement Framework (Phase 1)

Track only these numbers initially:

| Stage                | Number |
|:---------------------|:-------|
| Ad reach             |        |
| Landing-page views   |        |
| Registrations        |        |
| Attendees            |        |
| First-time attendees |        |
| People who return    |        |

This reveals whether the largest problem is the advertisement, the registration page, the reminder process, the timing, or the leap between registering and attending.

## Core Principle: Message Before Mechanics

The bigger issue isn't technology--it's finding the message that reliably makes the right people say "Yes."

Technology amplifies. It rarely rescues.

Rather than spending 20 hours installing Meta Pixel, spend 2 hours asking: Which invitation gets 5× the registrations?

If the invitation isn't landing, better tracking just helps you spend money more efficiently on the wrong message.

## Test One Variable at a Time

You and Wendy have spent time discovering a new way to talk about the work. Don't change ten things at once. Test the new language first. If registrations improve, you've learned something valuable. If they don't, then examine the mechanics.
