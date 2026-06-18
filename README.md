# GSE Terminal — Telegram Bot

Ghana Stock Exchange live data bot for Telegram.
Search stocks, track prices, get news — all inside Telegram.

---

## What the bot does

| Command | What it does |
|---|---|
| `/start` | Welcome screen with quick buttons |
| `/market` | Full market overview — gainers, losers, volume |
| `/top` | Top 5 gainers and top 5 losers |
| `/search MTNGH` | Quick price lookup |
| `/ticker GCB` | Full equity profile (cap, EPS, DPS, P/E) |
| `/news` | Latest Ghana business headlines |
| `/watch GOIL` | Add to your personal watchlist |
| `/watchlist` | View all your saved stocks |
| `/unwatch TICK` | Remove from watchlist |
| Just type `MTNGH` | Auto-detects ticker, shows price |

---

## Setup in 5 steps

### Step 1 — Get a bot token
1. Open Telegram, search **@BotFather**
2. Send `/newbot`
3. Give it a name: `GSE Terminal`
4. Give it a username: `GSETerminalBot` (must end in "bot")
5. BotFather sends you a token like `7123456789:AAH...`
6. Copy that token

### Step 2 — Set your token
```bash
# Option A: environment variable (recommended)
export BOT_TOKEN="7123456789:AAH..."

# Option B: create .env file
echo 'BOT_TOKEN=7123456789:AAH...' > .env
```

### Step 3 — Install dependencies
```bash
pip install -r requirements.txt
```

### Step 4 — Run the bot
```bash
python bot.py
```

You'll see: `🚀 GSE Terminal Bot is running…`

### Step 5 — Test it
Open Telegram, search your bot username, send `/start`

---

## Deploy for FREE (so it runs 24/7 without your phone)

### Option A — Railway.app (easiest, free tier)
1. Go to **railway.app** → New Project → Deploy from GitHub
2. Upload this folder to a GitHub repo
3. Add environment variable: `BOT_TOKEN = your_token`
4. Railway auto-deploys — bot runs 24/7

### Option B — Render.com (also free)
1. Go to **render.com** → New → Background Worker
2. Connect your GitHub repo
3. Build command: `pip install -r requirements.txt`
4. Start command: `python bot.py`
5. Add env var: `BOT_TOKEN`

### Option C — Run on your phone (Termux)
```bash
# Install Termux from F-Droid
pkg install python
pip install -r requirements.txt
export BOT_TOKEN="your_token"
python bot.py
```

---

## Contact
- Email: attah.godsway999@gmail.com
- Phone/WhatsApp: +233 53 383 3623
