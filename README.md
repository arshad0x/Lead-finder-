# LeadHunter AI

Find active local businesses that **don't have a website yet**, and write a personalised pitch for each one with AI. Built as a mobile-first web app that can be packaged as an Android APK.

**Live app:** https://arshad0x.github.io/Lead-finder-/

## Features

- **Lead search** by city and business type (gym, salon, clinic, furniture, carpenter and more)
- **Multiple data sources**
  - Google Places API
  - OpenStreetMap (free, no key needed)
  - Open Places API
  - Or combine them
- **Smart filtering**: keeps only businesses that are open, have a phone number, and have no real website (Instagram, Facebook or Justdial pages count as "no website")
- **AI pitch writer**: generates a short WhatsApp message in Hinglish using the Claude API, with an offline template as fallback
- **Lead tracker**: save leads and mark them New, Contacted, Interested or Closed
- **One-tap actions**: call, open in Maps, or send the pitch on WhatsApp
- **CSV export** of saved leads
- **Light and Dark theme** (Settings)

## How to use

1. Open the app and go to **Settings**.
2. Add your API keys (all optional, see below).
3. Go to **Khojo**, enter a city and business type, pick a data source and tap **Leads dhundo**.
4. Tap the sparkle button on a lead to generate a pitch, then send it on WhatsApp.

## API keys

| Key | Used for | Required? |
|-----|----------|-----------|
| Google Places API (New) | Best data: phone, website, rating, reviews | Optional |
| Open Places API | Alternative data source | Optional |
| Claude API | AI-written pitches | Optional |

Keys are stored only in your own browser or phone (localStorage). They are never sent anywhere except to the respective API.

**Tips**
- Restrict your Google key to Places API only and set a budget alert in Google Cloud.
- OpenStreetMap works without any key but has less data in smaller cities.
- Open Places API covers only a limited set of countries (India is not included).

## Run it

It is a single `index.html` file. Open it in a browser, or host it free with **GitHub Pages**:

1. Repo **Settings >
