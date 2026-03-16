# JD Davenport - Booking Page

Self-hosted booking page with dark terminal aesthetic.

## Features

- **3 Event Types:**
  - 15 min Free - Quick chat
  - 30 min $75 - Strategy session (popular)
  - 60 min $150 - Deep dive consulting

- **Design:**
  - Dark terminal aesthetic matching jddavenport.com
  - Fully responsive
  - No dependencies (pure HTML/CSS/JS)

- **Integrations:**
  - Google Calendar (for availability)
  - Stripe (for paid sessions)
  - Cal.com or self-hosted booking backend

## Deployment

### Option 1: Vercel (Recommended)
```bash
vercel --prod
```

### Option 2: GitHub Pages
1. Push to GitHub
2. Enable GitHub Pages in repo settings
3. Done

## File Structure

```
.
├── index.html          # Main booking page
├── README.md           # This file
└── .github/
    └── workflows/      # CI/CD if needed
```

## Domain Setup

### For jddavenport.com/book
Add to your main site's `vercel.json`:
```json
{
  "rewrites": [
    { "source": "/book", "destination": "https://jddavenport-booking.vercel.app/" }
  ]
}
```

### Or as subdomain
Point `book.jddavenport.com` to this deployment.

## Integration Checklist

- [ ] Add Google Calendar embed or Cal.com
- [ ] Add Stripe payment links
- [ ] Connect to booking backend
- [ ] Set up email notifications
- [ ] Test end-to-end booking flow

## Version History

| Date | Version | Notes |
|------|---------|-------|
| 2026-03-16 | v1.0 | Initial rebuild after data loss |

---

**Never lose this again.** This repo is the source of truth.