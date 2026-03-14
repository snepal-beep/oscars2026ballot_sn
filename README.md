# 🏆 98th Academy Awards — Watch Party Ballot 2026

A real-time, multi-device Oscar watch party ballot for friends in different cities.  
Built on Firebase Realtime Database + GitHub Pages (100% free, no server needed).

---

## ✨ Features

- **Real-time sync** — everyone's picks and the leaderboard update live across all devices
- **Room codes** — create a room and share the link or 6-character code with friends
- **Host mode** — the host reveals winners live during the ceremony; all ballots update instantly
- **Leaderboard** — live standings with points as winners are revealed
- **All 24 categories** — every 2026 nominee preloaded
- **Mobile-friendly** — works on phones and tablets

---

## 🚀 Setup (5 minutes, one time only)

### Step 1 — Create a free Firebase project

1. Go to [console.firebase.google.com](https://console.firebase.google.com)
2. Click **Add project** → name it `oscars-party` → click Continue → Create project
3. In the left sidebar: **Build → Realtime Database**
4. Click **Create Database** → choose any region → select **Start in test mode** → Enable

### Step 2 — Get your Firebase config

1. Click the ⚙️ gear icon → **Project Settings**
2. Scroll to **Your apps** → click the **`</>`** (web) icon
3. Name the app `oscars-ballot` → click **Register app**
4. Copy the `firebaseConfig` object that appears

### Step 3 — Paste config into index.html

Open `index.html` in any text editor. Find this block near the top:

```js
const firebaseConfig = {
  apiKey:            "PASTE_YOUR_API_KEY",
  authDomain:        "PASTE_YOUR_AUTH_DOMAIN",
  databaseURL:       "PASTE_YOUR_DATABASE_URL",
  projectId:         "PASTE_YOUR_PROJECT_ID",
  storageBucket:     "PASTE_YOUR_STORAGE_BUCKET",
  messagingSenderId: "PASTE_YOUR_MESSAGING_SENDER_ID",
  appId:             "PASTE_YOUR_APP_ID"
};
```

Replace every `PASTE_YOUR_*` value with your real Firebase values.

---

## 🌐 Deploy to GitHub Pages

1. Go to [github.com](https://github.com) → sign in → click **+** → **New repository**
2. Name it `oscars-party` → set to **Public** → **Create repository**
3. Click **uploading an existing file** → drag in `index.html` and `README.md` → **Commit changes**
4. Go to **Settings → Pages** → under *Branch* select `main` → **Save**
5. Your URL: `https://YOUR-USERNAME.github.io/oscars-party`

Share that URL with all your friends — they open it on their phone, enter their name + the room code, and they're in!

---

## 🎬 Party Night Instructions

1. **Host** opens the URL → enters name → leaves room code blank → room is created
2. **Host** copies the share link or 6-letter code and sends it to friends
3. **Friends** open the link → enter their name → they join the room instantly
4. **Everyone** fills in their ballot → clicks **Lock In My Picks** before the show
5. **During the show** → Host uses the gold **✦ HOST** bar under each category to reveal winners
6. **Leaderboard** updates live for everyone as winners are announced 🎉

---

## 💰 Cost: Completely Free

Firebase free tier covers 100 simultaneous connections — more than enough for any watch party.
GitHub Pages is free for public repos.
