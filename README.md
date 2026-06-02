# Sammy's Auto Repair Centre — Website Package

## Files

| File | Description |
|------|-------------|
| `index.html` | Main landing page (hero, services, reviews, CTA) |
| `booking.html` | 4-step online booking form |
| `admin.html` | Admin dashboard (appointments, revenue, calendar) |
| `style.css` | Shared styles across all pages |

## How to Use

1. **Local**: Just open `index.html` in any browser — no server needed.
2. **Host**: Upload all 4 files to any web host (Netlify, Vercel, cPanel, etc.) keeping them in the same folder.

## Customization Checklist

### Contact Info (update in all files)
- Phone: `(613) 327-6181` → your number
- Address: `2535 Blackwell St, Ottawa, ON K1B 4E4`
- Hours: Mon–Fri 8:00 AM – 5:00 PM

### Colors (`style.css` line 8–21)
```css
--red:    #C8102E;   /* main brand red */
--black:  #0A0A0A;   /* backgrounds */
--silver: #C0C0C0;   /* accents */
```

### Booking Form
- `booking.html` currently runs as a demo (no backend).
- To make it actually send bookings, connect to:
  - **Formspree** (free): wrap form in `<form action="https://formspree.io/f/YOUR_ID">`
  - **EmailJS**: call EmailJS API in the `submitBooking()` function
  - **Your own backend**: POST to your server endpoint

### Admin Dashboard
- `admin.html` uses static demo data.
- For a live admin panel, connect to a backend (Node.js/PHP/Firebase) and replace the table rows with fetched data.

## Pages Overview

### index.html
- Fixed navigation with Call Now CTA
- Full-screen hero with animated stats
- Scrolling red marquee with services
- 12 service cards with hover effects
- "Built on Trust" section with visual accent block
- 6 customer review cards
- Big CTA section with phone number
- Footer with links and hours

### booking.html
- Step 1: Select service (12 options)
- Step 2: Pick date (working calendar) + time slot
- Step 3: Enter name, phone, email, vehicle info
- Step 4: Confirmation screen
- Live booking summary sidebar

### admin.html
- Fixed sidebar navigation
- 4 KPI stat cards (appointments, completions, pending, revenue)
- Tabbed appointment table (Today / Upcoming / Pending / Completed)
- CSS revenue bar chart (12 months)
- Mini calendar with appointment indicators
- Services breakdown list
- "New Appointment" modal
- Shop info quick panel

## Design System
- **Fonts**: Oswald (headings), Barlow Condensed (labels), Barlow (body)
- **Brand colors**: Red `#C8102E`, Black `#0A0A0A`, Silver `#C0C0C0`
- **Style**: Dark industrial premium — confident, trustworthy, fast

---
Built for Sammy's Auto Repair Centre, Ottawa ON · (613) 327-6181
