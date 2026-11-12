# Akalat Al-Baraka — Ordering Site for a Home-Style Iraqi Kitchen

Arabic (right-to-left) one-page ordering site for **اكلات البركة**, a Baghdad kitchen selling home-made kibbeh, kebabs, trays and pastries, with catering for occasions.

The whole site is a single self-contained `index.html`: no build step, no framework, no server.

## Features

- **Menu by category** — kibbeh varieties; ʿurook, kebab and trays; pastries — each item with options and prices.
- **Cart** — add items, change quantities, live subtotal, delivery fee by area (Karkh or Rusafa) and grand total.
- **Order through WhatsApp** — name, phone and address are collected, and the order is sent to the kitchen as a formatted WhatsApp message with an order number.
- **Share location** — the customer can attach their GPS location, sent as Google Maps and Waze links so the driver finds them faster.
- **Occasions section** for catering orders, a photo gallery, and an offers section that appears only when offers exist.
- **Optional live data** — menu items, offers, delivery fees and the order phone number can be loaded from Supabase tables (`menu_items`, `offers`, `settings`); with no keys set, the built-in menu is used.

## Run

Open `index.html` in a browser, or host it on any static host (Cloudflare Pages, Netlify, GitHub Pages).

To load the menu from Supabase, set `SUPABASE_URL` and `SUPABASE_ANON_KEY` near the top of the script (anon key only, with Row-Level Security allowing public reads of active items).

## Stack

HTML · CSS · vanilla JavaScript · optional Supabase
