# 🐾 ScavengerHound

**Tagline:** A React + Firebase scavenger‑hunt platform for teams, GPS check‑ins, photos, trivia, and automated rewards — built for dog lovers and city explorers.

> Built from a forked foundation and actively evolving toward a hosted SaaS + open template for community hunts.

---

## 🚀 Purpose

ScavengerHound helps organizers spin up location‑based scavenger hunts in minutes — from dog‑friendly neighborhood walks to downtown brand activations. Players join with a game code, form teams, complete GPS/photo/trivia challenges, and earn points and rewards.

---

## 🎯 Core Features

* Team join + game code rooms
* GPS proximity check‑ins with map pins
* Photo uploads + gallery moderation
* Trivia challenges with scoring + bonuses
* Real‑time admin dashboard: start/stop game, points control
* Anonymous auth + rejoin logic
* Firebase Cloud Functions for automations (emails, rewards)

Planned:

* Social boosts (#ScavengerHound) with bonus points
* Sponsor tiers (QR clues, coupon drops, links)
* Automated reward delivery (Marketing Boost, Dining, Hotel Savings)
* City templates and pet‑themed hunts

---

## 🧱 Tech Stack

* **Frontend:** React + Vite
* **Backend:** Firebase (Auth, Firestore, Storage, Functions)
* **Maps/GPS:** Google Maps JavaScript API + Geolocation
* **CI/CD:** GitHub Actions (planned)
* **Infra:** Firebase Hosting (starter), Render/Netlify optional

---

## 📦 Quick Start (Local)

```bash
# 1) Clone and enter
git clone https://github.com/jesseboudreau80/ScavengerHound.git
cd ScavengerHound

# 2) Install deps
npm install

# 3) Env vars (create .env.local)
# See ".env.example" for keys

# 4) Run dev server
npm run dev
```

### Required environment variables

Create **.env.local** at project root:

```
VITE_FIREBASE_API_KEY=
VITE_FIREBASE_AUTH_DOMAIN=
VITE_FIREBASE_PROJECT_ID=
VITE_FIREBASE_STORAGE_BUCKET=
VITE_FIREBASE_MESSAGING_SENDER_ID=
VITE_FIREBASE_APP_ID=
VITE_GOOGLE_MAPS_API_KEY=
```

---

## ☁️ Deploy (Firebase Hosting + Functions)

```bash
# Login & init (once)
npm i -g firebase-tools
firebase login
firebase use <your-project-id>

# Deploy hosting only
firebase deploy --only hosting

# Deploy functions only (Node 20 recommended)
firebase deploy --only functions

# Or deploy both
firebase deploy
```

---

## 🧭 How It Works (Workflow)

```
Organizer creates game ➜ Adds challenges (GPS, Photo, Trivia)
             │
Players join via game code ➜ Form/auto-assign teams
             │
Live game: teams complete challenges ➜ Upload photos / answer trivia / move to pins
             │
Admin dashboard: approve photos, adjust points, start/stop, monitor map
             │
Cloud Functions: send emails, drop coupons, reward winners
```

---

## 🗺️ Roles

* **Player:** Join, submit, view progress
* **Moderator:** Review photos, flag content
* **Admin/Host:** Configure game, manage points, start/stop

---

## 💸 Monetization + Business Model (MVP)

* **Hunt Packs:** Paid city or theme templates (one‑time)
* **Hosted Events:** Flat fee per event or per team
* **Sponsor Slots:** QR clues, branded challenges, coupon drops
* **Rewards Add‑on:** Automated coupon/vacation incentives via Zapier/Functions
* **White‑Label:** Partner mode for tourism/venues

---

## 🔐 Privacy & Safety (baseline)

* Anonymous player IDs by default
* Photo moderation queue before public gallery
* No precise location stored without consent; use hashed/geofenced coords
* COPPA/child‑safety note for public events; parental consent guidance

---

## 🧪 Roadmap

* [ ] Maps + GPS proximity validation
* [ ] Challenge builder UX (drag‑drop)
* [ ] Social proofing: hashtag verification (server‑side later)
* [ ] Reward pipelines (Marketing Boost / Dining / Hotel Savings)
* [ ] Multi‑event org dashboard + billing
* [ ] Analytics (pageviews, completions, heatmaps)

---

## 📁 Repo Structure (high‑level)

```
public/                 static assets
src/
  components/           UI building blocks
  pages/                routes & screens
  lib/                  firebase, api, utils
  features/
    game/               game state, scoring, team mgmt
    challenges/         gps, photo, trivia modules
functions/              Firebase Cloud Functions
```

---

## 🧑‍💻 Contributing

PRs welcome after initial MVP. Please open an issue first to propose changes. Add tests where possible.

---

## 📜 License

MIT (proposed)

---

## 🙌 Credits

* Original foundation: @theNatePi (scavenger‑hunt)
* New direction & productization: @jesseboudreau

---

## 📣 Contact & Links

* Project: [https://github.com/jesseboudreau80/ScavengerHound](https://github.com/jesseboudreau80/ScavengerHound)
* Updates & demos: [https://jesseboudreau.com](https://jesseboudreau.com)
* Email: [jesse@jesseboudreau.com](mailto:jesse@jesseboudreau.com)

---

### Appendix: Sponsor Options (Draft)

* Bronze: One QR clue + coupon link
* Silver: Two challenges + logo on map
* Gold: Branded prize + social campaign co‑post
