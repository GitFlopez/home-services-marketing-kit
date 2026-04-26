# Prompt 3: Referral & Review System

Copy and paste the prompt below into Claude. This builds your complete review generation and referral engine.

---

## The Prompt

```
You are a customer experience strategist for local home service businesses. Build a complete referral and review generation system for the following business.

BUSINESS INFO:
- Company Name: [Name]
- Service Type: [HVAC / Plumbing / Electrical / Roofing / Landscaping / Pool / Pest / Cleaning / Handyman]
- City: [City, State]
- Current Google Reviews: [e.g., "47 reviews, 4.2 stars" OR "just starting, 0 reviews"]
- Technician/Service Rep Name Variable: [use [TECH_NAME] as placeholder]
- Service Variable: [use [SERVICE_PERFORMED] as placeholder, e.g., "AC tune-up", "drain cleaning", "roof inspection"]
- Referral Reward for Referrer: [e.g., "$25 Visa gift card", "$50 off next service", "free filter replacement", "enter to win $500 quarterly drawing"]
- Reward for New Customer: [e.g., "$25 off first service", "free inspection", "no service fee"]
- Primary Review Platform: [Google Business Profile / Yelp / Facebook / All three]
- Primary Contact Method for Follow-Up: [Text/SMS / Email / Both]
- Timing Window: [e.g., "Send review request same day tech leaves" OR "24 hours after job completion"]

Generate:

1. POST-SERVICE REVIEW REQUEST SEQUENCE (3-touch)

   Touch 1 — SMS (send 30-60 minutes after technician leaves):
   [Under 160 characters total — count them]
   Rules:
   - Open with technician's first name: "Hi, [TECH_NAME] just finished up at your place."
   - Reference what was done: [SERVICE_PERFORMED]
   - One specific ask: 1-click link placeholder [REVIEW_LINK]
   - No exclamation points. No emojis. Friendly, direct.
   Write 2 variants (A/B test):
   Variant A — direct ask
   Variant B — satisfaction check first, then ask

   Touch 2 — Email (send 24-48 hours after service, only if no review submitted yet):
   Subject line option A: [under 50 chars, reference service]
   Subject line option B: [under 50 chars, softer follow-up]
   Subject line option C: [under 45 chars, last resort / curiosity]
   Preview text (under 90 chars)
   Body (80-110 words):
   - Open with: what was done + hope it's working well
   - Why reviews matter (humanize it — "helps homeowners like you find us")
   - Single CTA: [REVIEW_LINK] with anchor text "Share Your Experience"
   - Sign off from: [TECH_NAME] or office manager (not "The [Company] Team")
   Rule: No "As a valued customer." No "We hope you're enjoying your experience." Write like a text from a person.

   Touch 3 — Final SMS (send 72-96 hours after service, only if still no review):
   [Under 130 characters — count them]
   Rules:
   - No guilt-tripping. No "we really need your help."
   - Acknowledge it might not be the right time
   - Leave the door open (no more follow-up after this)
   Write 1 variant only.

2. REVIEW QR CARD (physical leave-behind, business card size — 3.5" × 2")

   Front of card:
   - Headline: "How did we do?" OR "Rate our service" (choose better one for this business type)
   - 5-star icon row (graphic placeholder)
   - QR code placeholder labeled: [QR_CODE → links to Google review page]
   - Company name + phone number (small footer)
   
   Back of card:
   Title: "What helps other homeowners:"
   3 short bullets guiding what to include in the review:
   - [e.g., "What we fixed and how fast" — helps conversion]
   - [e.g., "Whether the tech explained what they did" — builds trust signal]
   - [e.g., "Would you call us for your next issue?" — prompts recommendation language]
   Rule: Total word count under 60. The goal is to coach customers to write better reviews, not to write it for them (which violates Google's policy).

3. REFERRAL PROGRAM STRUCTURE

   Program Name: [2-3 word name — memorable, not cheesy, e.g., "Neighbor Rewards", "The Good Neighbor Program", "Refer & Save"]
   
   Reward for Referrer (the customer who refers):
   - [Exact reward, e.g., "$25 Visa gift card mailed within 5 business days of referred customer's first completed job"]
   
   Reward for New Customer (the person being referred):
   - [Exact reward, e.g., "$25 off first service call"]
   
   Program Rules (3 bullets — simple enough to explain verbally in 30 seconds):
   - Rule 1: how to refer (give our name, use referral code, or text us their name + address)
   - Rule 2: when the reward pays out (after referred customer's first completed service)
   - Rule 3: any limits (max referrals per year, geographic area, etc.)
   
   Expiration: [e.g., "No expiration" OR "Referral rewards issued within 90 days of referral"]
   
   Tax note (if reward over $600): [Include for high-reward programs: "Gift cards over $600 cumulative per year may require a 1099. We'll let you know if you hit that threshold — which means you've referred a LOT of neighbors!"]

4. REFERRAL CARD COPY

   Physical Card (business card size, leave-behind after every job):
   
   Front:
   - Program name + tagline (e.g., "Neighbor Rewards — Give your neighbor $25 off their first service")
   - Simple visual: two neighbor houses icon description
   - Company name + phone
   
   Back:
   - How to redeem (2 steps max):
     Step 1: [Give this card to your neighbor OR text us their address]
     Step 2: [They mention your name when they book — you both save]
   - Referral code placeholder: [REF-XXXXX]
   - Expiration: [see program rules]
   - Fine print (1 line max): "One reward per referred household. Clark County service area."
   
   Digital Version (easy-forward SMS):
   [Under 160 chars. Should be easily forwarded by a satisfied customer to a neighbor.]
   Example format: "Just had [Company] fix my [SERVICE]. They're legit. Use code [CODE] for $25 off your first call: [BOOKING_LINK]"
   Write 2 variants — one casual, one slightly more formal (for different customer demographics).

5. GOOGLE REVIEW RESPONSE TEMPLATES (6 templates)

   IMPORTANT RULES for all templates:
   - Max 120 words per response
   - Never "We take pride in" or "We're sorry you feel that way"
   - Never admit fault for 1-star without knowing full context
   - Always move 3-star and 1-star conversations offline
   - Address the reviewer by first name when visible
   - Responses are written for future readers as much as the reviewer

   5-Star Glowing Review — Template A (highlight specific details mentioned):
   [Open with thanks, echo back 1-2 specifics from the review, reinforce the company value, brief forward-looking CTA for next service need]

   5-Star Glowing Review — Template B (brief + community-forward):
   [Shorter response, thank them, connect to the neighborhood/community angle, soft referral nudge]

   3-Star "It was fine, nothing special" Review — Template A (invite conversation):
   [Thank them, acknowledge "fine" isn't the goal, invite a call to understand what would have made it a 5-star experience, phone number or email to reach out]

   3-Star "One thing was great, one thing wasn't" Review — Template B (address + move offline):
   [Thank them for the positive part, acknowledge the specific issue mentioned, offer to make it right, move to offline contact — no defensiveness]

   1-Star "Something went wrong" Review — Template A (de-escalate, no admission):
   [Thank them for the feedback, express genuine concern (not legal-defensive concern), state you want to understand what happened, invite them to call/email directly, do NOT respond to the specific accusation in the public response]

   1-Star "Seems like wrong business" or "Didn't use us" Review — Template B (factual, empathetic):
   [Note that you don't have a record of the service address or date, invite them to call to verify, keep it short and non-defensive — this response is mainly for other readers to see the discrepancy]
```

---

## Tips for Best Results

- **Timing matters most.** A review request sent 30 minutes after the tech leaves converts 3–4× better than one sent the next morning. Build this into your dispatch process.
- **The QR card beats the link.** Customers are more likely to scan a card the tech hands them in person than click a link in a text hours later. Use both.
- **$25 is the magic referral number.** It feels meaningful without being expensive. $10 feels cheap. $50 raises questions about your margins.
- **Review responses are for future readers.** Write every response assuming 100 homeowners will read it before deciding whether to call you.

## Implementation Checklist

- [ ] Create a Google Business Profile short link for reviews (GBP → Get More Reviews → Share review form)
- [ ] Design the QR card using Canva (search "business card" template, portrait orientation)
- [ ] Add referral card to every tech's truck toolkit
- [ ] Set SMS review request in your CRM or set a phone reminder to send after each job
- [ ] Train techs: "Hand the card before you leave. Say: 'If you got good service today, this is how to let people know.'"
