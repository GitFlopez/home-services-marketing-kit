# Prompt 2: Service Page Copy Generator

Copy and paste the prompt below into Claude. Fill in the bracketed fields.

One run = one complete service page. Run separately for each service (AC repair, AC installation, furnace repair, etc.)

---

## The Prompt

```
You are a conversion copywriter who specializes in local home service websites. Write a complete, SEO-optimized service page for the following business and service. The page must rank in Google Search and Google Maps for local searches AND convert visitors to calls or bookings.

BUSINESS INFO:
- Company Name: [Name]
- City/Metro: [City, State]
- Service: [Specific service — be precise, e.g., "AC Repair", "AC Replacement / New Installation", "Drain Cleaning", "Water Heater Replacement", "Electrical Panel Upgrade", "Roof Repair (shingle)", "Weekly Lawn Maintenance", "Pool Opening Service"]
- Primary Keyword: [The exact phrase people search, e.g., "AC repair Las Vegas", "emergency plumber Henderson NV", "roof repair after storm Summerlin"]
- Secondary Keywords: [2-3 related phrases, e.g., "air conditioner not cooling", "HVAC repair near me", "same-day AC fix"]
- Pricing (if you display it): [e.g., "$89 diagnostic fee applied to repair", "free estimates", "$150-300 typical drain cleaning", "no upfront pricing — quote after inspection"]
- Certifications & Licenses: [e.g., "NATE-certified", "Nevada State Contractor License #12345", "EPA 608 certified", "C-10 licensed", "GAF Master Elite Certified", "licensed and bonded in Nevada"]
- Guarantee: [e.g., "1-year parts and labor warranty", "100% satisfaction or we return for free", "if we can't fix it, you don't pay"]
- Emergency/After-Hours Service: [Yes — 24/7 / Yes — weekends only / No]
- Years in Business: [X years]
- Common Objections: [e.g., "worried about hidden fees", "not sure if repair or replace is better", "afraid tech will upsell unnecessary parts"]

Generate a complete service page with the following 9 sections:

1. SEO METADATA
   Page Title (55-60 chars exactly): [Primary keyword] | [Company Name] [City abbrev]
   Meta Description (150-160 chars exactly): Lead with main benefit + proof + CTA. Include city name.
   URL slug suggestion (lowercase, hyphenated): /[service]-[city-state]
   
   Show character count in brackets after each field: [Title: 58 chars]

2. H1 HEADLINE
   Must: include city name, core benefit, and either a number/stat or timeframe
   Format A: [Action verb] [Service] in [City] — [Benefit] + [Proof]
   Format B: [City]'s [Trust signal] [Service] — [Primary benefit]
   
   Write both formats, then recommend which converts better for this specific service.

3. ABOVE-THE-FOLD COPY (60-80 words)
   Structure:
   - Sentence 1: Name the customer's pain (not the company's capabilities)
   - Sentence 2-3: State what you do about it + key differentiator
   - Sentence 4: Proof point (years, reviews, certifications, or guarantee)
   - Sentence 5: Call to action with phone number in format (XXX) XXX-XXXX
   Rule: No "We are proud to offer." No "Your satisfaction is our priority." Write what the customer is thinking, not what the company wants to say.

4. BENEFITS SECTION (3 columns, appears below the fold)
   Each column: icon label (1-2 words) + benefit headline (max 8 words) + supporting sentence (max 20 words)
   
   Column ideas: Speed / Pricing Transparency / Warranty / Emergency Availability / Local/Licensed / Satisfaction Guarantee
   Choose the 3 most relevant for THIS service and THIS market.

5. SERVICE DETAILS
   Subheading: "What's Included in Our [Service Name]"
   Included (6-8 bullet points, specific — not vague):
   - [e.g., "Full 21-point system inspection" not "thorough inspection"]
   - [e.g., "Refrigerant level check + top-off up to 1 lb included" not "refrigerant check"]
   
   NOT Included (2-3 bullets — transparency builds trust):
   - [What requires a separate quote or service call]
   
   Typical Duration: [X hours / Half day / Full day — be specific]
   Emergency surcharge (if applicable): [e.g., "After-hours emergency calls: $X additional diagnostic fee"]

6. HOW IT WORKS (3-4 numbered steps)
   Each step: Bold title (4-6 words) + 1-sentence description (under 20 words)
   Must feel sequential and effortless — remove friction in every step
   Step 1 should be: call/book online (make it easy)
   Last step should end with: the resolution (working system, clean drain, fixed roof)

7. FAQ (5 questions)
   Q1: "How much does [service] cost in [city]?"
   Q2: "How long does [service] take?"
   Q3: "Do I need to be home during the service?"
   Q4: "Is your work guaranteed?"
   Q5: [Most common pre-purchase objection for THIS specific service — write the real question customers ask]
   
   Rule: Each answer 40-75 words. Specific. No "it depends" without a range. No corporate speak. Write the answer your best tech would give in a text message.

8. TRUST SECTION
   Certifications list (formatted as a badge/tag list, e.g., "✓ NATE-Certified" "✓ Nevada Licensed #XXXXX" "✓ EPA 608 Certified")
   Insurance statement: "Licensed, bonded, and insured in [State]. License #[PLACEHOLDER]. $X million liability coverage."
   Rating bar: [Google: X.X stars (XXX reviews) — PLACEHOLDER for actual numbers]
   Guarantee box (stand-alone callout): 
   - Box title: "[Company Name] [Service] Guarantee"
   - Body: [Exact guarantee language, specific — what happens if they're not satisfied, what the company will do, within what timeframe]
   - No asterisks. No fine print.

9. CTA SECTION
   Primary CTA block:
   - Headline (1 line): creates urgency or removes risk
   - Body (2 sentences max): reinforce guarantee + next step
   - Phone number (large, prominent): (XXX) XXX-XXXX
   - Alternative: "Prefer to book online? [Schedule here →]" with link placeholder
   
   Secondary CTA (for visitors not ready to call):
   - "Get a Free Estimate" form — 3 fields only: Name / Service Address / What's the issue? (text field)
   - Submit button: "Send My Estimate Request"
   
   Urgency bar (optional, A/B test this):
   - "[Month] Appointment Slots Filling Fast — [X] openings remaining this week"
   Rule: No countdown timers. No fake urgency. Use real slot availability or seasonal demand framing.
```

---

## Tips for Best Results

- **Run once per service.** "AC Repair" and "AC Installation" are different pages with different keywords, different buyer intent, and different conversion copy. Don't combine them.
- **Use the exact primary keyword** people type into Google. Check Google Search Console or type the service in Google and look at the autocomplete suggestions.
- **Be honest in the "Not Included" section.** Listing what's NOT included builds more trust than leaving it out — customers fear hidden fees more than limitations.
- **Plug in real numbers.** Replace every placeholder (license number, review count, star rating) before publishing.

## After You Have the Copy

1. Paste into your CMS (WordPress, Squarespace, Wix, ServiceTitan's website builder)
2. Add the page title and meta description in your SEO plugin (Yoast, RankMath, or built-in tools)
3. Upload 2-3 job photos as supporting images (label them: "[service]-[city]-[company].jpg" for SEO)
4. Submit the URL to Google Search Console after publishing: "URL Inspection → Request Indexing"
