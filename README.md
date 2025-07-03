# 🐾 ScavengerHound

Originally built by Nate for CTC — now being extended and reimagined as **ScavengerHound**:  
A location-based scavenger hunt platform built for dog lovers, community explorers, and creative marketers.

---

## 🌟 What Is ScavengerHound?

ScavengerHound is a **web-based, mobile-friendly scavenger hunt platform** with:
- Game code entry and team formation
- GPS-aware checkpoints on a dynamic map
- Multiple check-in types: 📸 photo, 🧠 trivia, 📍 location proximity, 🏷️ social sharing
- Admin panel for real-time monitoring, point control, and content review
- Cloud function support for **prizes, email triggers, and vacation reward delivery**

---

## 🔥 New Features (Planned or In Progress)

- 🗺️ Google Maps pins with GPS proximity validation
- 🧠 Trivia engine with bonus rewards (e.g., free next hunt)
- 🏷️ Social media integration: #ScavengerHound for bonus check-ins
- 🐕 Pet-friendly themes and customizable city-based hunts
- 🧾 Business sponsor tiers and QR-based partner promos
- 🎁 MarketingBoost vacation/gift card integration via Zapier/Firebase

---

## ✨ Current Features (Inherited from Original Repo)

- Dynamic game rooms supporting unlimited players
- Anonymous user authentication and rejoin logic
- Real-time updates across teams
- Image upload and gallery view
- Admin interface for game control and team review
- Points system per submission

---

## 📸 App Screenshots (Original Build)

### Start Page – Game Code Entry
<img src="https://github.com/user-attachments/assets/807aeeab-fd96-4ee4-aad7-4d260afa3cfa" width="200" />

### Team Sorting
<img src="https://github.com/user-attachments/assets/30e273d3-b77b-4b73-85dc-b98055362ad3" width="200" />

### Game Home Page
<img src="https://github.com/user-attachments/assets/aad5e0dc-cbf5-4ad5-857f-6ce5f229e29b" width="200" />

### Challenge Check-In Page
<img src="https://github.com/user-attachments/assets/c706ec95-84a6-480d-9c27-87b1b7659b92" width="200" />

### Admin Game Control
<img src="https://github.com/user-attachments/assets/cc609396-9985-4940-a5bd-631ea0c6f82a" width="200" />

### Admin Team Review
<img src="https://github.com/user-attachments/assets/da3b8738-d1e6-4e32-97b6-3447c44d23e8" width="200" />

---

## 🛠️ Getting Started

```bash
# clone this fork
git clone https://github.com/yourusername/ScavengerHound.git
cd ScavengerHound

# install client dependencies
npm install

# run frontend locally
npm run dev

# Firebase CLI setup required for backend deploys
firebase deploy --only functions

🔗 Live Demos & Contact
Coming soon at: jesseboudreau.com/scavenger-survey
Learn more about the project, upcoming hunt locations, and join the adventure.

Original Author: @theNatePi
New Direction & Expansion by: @jesseboudreau

💬 Want to sponsor or be featured in a ScavengerHound hunt?
Contact jesse@jesseboudreau.com or visit jesseboudreau.com

yaml
Copy
Edit

---

Would you like this pushed into a new repo scaffold? I can also add:
- LICENSE (MIT?)
- `CONTRIBUTING.md` if you open it up for collaborators
- Or a `TODO.md` to track phases like:
  - Google Maps integration
  - Trivia engine
  - Marketing Boost reward flow setup
