# MarketView Free Features - Examples & Commands

Complete guide with real examples for all free features available in MarketView Telegram Bot.

---

## 🆕 Automatic IPO Notifications (NEW!)

**Trigger**: Automatic when IPO status changes

Get real-time notifications for all IPO events - completely free!

### What Triggers Notifications

✅ **New IPO Added** - When a new IPO is added to our database
✅ **IPO Opening** - When bidding starts (upcoming → active)
✅ **IPO Closing** - When bidding ends (active → closed)
✅ **IPO Listed** - When stock gets listed (closed → listed)

### Sample New IPO Notification

```
🆕 New IPO Added

🏢 Orkla India Ltd (MAINBOARD)
📝 Symbol: ORKLAINDIA

📊 Type: Main Board
✅ Status: ACTIVE

💰 PRICING:
   Price Band: ₹695 - ₹730
   Lot Size: 20 shares

📈 GMP: ₹68 (+9.3%)

📅 IMPORTANT DATES:
   Open: 29 Oct 2025
   Close: 31 Oct 2025
   Listing: 06 Nov 2025

🏦 LEAD MANAGER:
   Citigroup Global Markets India Private Limited

📄 View RHP Document
🔗 View Full Details
```

### Sample Status Change Notification

```
✅ IPO Now OPEN

🏢 Jayesh Logistics Ltd. (NSE SME)
📝 Symbol: JAYESH

📊 Type: SME
✅ Status: ACTIVE

💰 PRICING:
   Price Band: ₹116 - ₹122
   Min Investment: ₹116,000
   Max Investment: ₹122,000
   Lot Size: 1000 shares

📈 GMP: ₹9 (+7.4%)
   Expected Listing: ₹131

📅 IMPORTANT DATES:
   Open: 27 Oct 2025
   Close: 29 Oct 2025
   Listing: 03 Nov 2025

⏱️ Closes in 2 days

🏦 LEAD MANAGER:
   Indcap Advisors Pvt. Ltd.

📄 View RHP Document
🔗 View Full Details
```

### What You Get (All Free!)

- **Real-time alerts** for new IPOs
- **Status change notifications** (Opening, Closing, Listed)
- **Complete IPO details**:
  - Price band and lot size
  - Grey Market Premium (GMP)
  - Expected listing price
  - Important dates with countdowns
  - Lead manager information
  - RHP document link
- **No premium required** - 100% free for all users!

### How to Enable

1. Start the bot: [@marketview_ipostream_bot](https://t.me/marketview_ipostream_bot)
2. Send `/subscribe` to enable notifications
3. You're all set! Notifications are automatic.

To disable: `/unsubscribe`

---

## 📊 IPO Details Command (NEW!)

**Command**: `/ipo <name or symbol>`

Search and get detailed information about any IPO - past, present, or upcoming!

### Examples

```
/ipo orkla
/ipo JAYESH
/ipo reliance
/ipo premji invest
```

### Sample Response

```
╔══════════════════════════╗
  📊 IPO DETAILS
╚══════════════════════════╝

🏢 Orkla India Ltd (MAINBOARD)
📝 Symbol: ORKLAINDIA
✅ Status: OPEN FOR BIDDING
🏷️ Type: Main Board

━━━━━━━━━━━━━━━━━━━━━━━━━
💰 PRICING DETAILS

   Price Band: ₹695 - ₹730
   Min Investment: ₹13,900
   Max Investment: ₹14,600
   Lot Size: 20 shares

💹 GREY MARKET PREMIUM

📈 GMP: ₹68 (+9.3%)
   Expected Listing: ₹798

━━━━━━━━━━━━━━━━━━━━━━━━━
📅 IMPORTANT DATES

   Open: 29 Oct 2025
   Close: 31 Oct 2025
   Listing: 06 Nov 2025

━━━━━━━━━━━━━━━━━━━━━━━━━
🏦 LEAD MANAGER

   Citigroup Global Markets India Private Limited

━━━━━━━━━━━━━━━━━━━━━━━━━
🔗 USEFUL LINKS

📄 View RHP Document

━━━━━━━━━━━━━━━━━━━━━━━━━

Use /ipos to see all active IPOs
Use /subscribe to get IPO alerts
```

### Smart Search Features

**Fuzzy Matching** - Don't need exact names:
```
/ipo jayesh          → Finds "Jayesh Logistics"
/ipo orkla          → Finds "Orkla India Ltd"
/ipo premji         → Finds "Premji Invest"
```

**Symbol or Name** - Works with both:
```
/ipo ORKLAINDIA     → By symbol
/ipo Orkla India    → By name
```

**Multiple Results** - Shows list if multiple matches:
```
/ipo reliance

🔍 Found 3 IPOs matching 'reliance':

1. 🎉 Reliance Industries
   Symbol: RELIANCE | Status: LISTED
   /ipo RELIANCE

2. 🔜 Reliance Power
   Symbol: RPOWER | Status: UPCOMING
   /ipo RPOWER

3. 🔒 Reliance Infra
   Symbol: RINFRA | Status: CLOSED
   /ipo RINFRA
```

### What You Get

- **Complete pricing details** with min/max investment
- **Grey Market Premium (GMP)** with percentage and expected listing
- **Important dates** with countdown timers
- **Lead manager** information
- **RHP document** link for detailed prospectus
- **Listing performance** (for listed IPOs)
- **100% FREE** - No premium required!

---

## 📋 Active IPOs List

**Command**: `/ipos`

View all currently active and upcoming IPOs in one place.

### Example

```
/ipos
```

### Sample Response

```
╔══════════════════════════╗
  📊 Active IPOs
╚══════════════════════════╝

✅ ORKLA INDIA LTD
📝 ORKLAINDIA
📅 Close: 31 Oct 2025
💰 ₹695 - ₹730
📈 GMP: +₹68 (9.3%)

✅ JAYESH LOGISTICS
📝 JAYESH
📅 Close: 29 Oct 2025
💰 ₹116 - ₹122
📈 GMP: +₹9 (7.4%)

━━━━━━━━━━━━━━━━━━━━━━━━━

╔══════════════════════════╗
  🔜 Upcoming IPOs
╚══════════════════════════╝

🔜 PREMIUM INVEST LTD
📝 PREMIUMINV
📅 Opens: 05 Nov 2025
💰 ₹250 - ₹265

━━━━━━━━━━━━━━━━━━━━━━━━━

╔══════════════════════════╗
  🎉 Recent Listings (7d)
╚══════════════════════════╝

🎉 ABC TECH LTD
📝 ABCTECH
📅 Listed: 28 Oct 2025
💰 Listed: ₹425 (+15.2%)
```

### What You Get

- **Active IPOs** currently open for bidding
- **Upcoming IPOs** opening soon (next 30 days)
- **Recent listings** from last 7 days
- **GMP data** for all IPOs
- **Quick view** of prices and dates
- Use `/ipo <symbol>` for full details

---

## 📈 Today's Market Summary

**Command**: `/today`

Get a comprehensive snapshot of today's market activity.

### Example

```
/today
```

### Sample Response

```
📊 Market Summary
📅 01 Nov 2025

━━━━━━━━━━━━━━━━━━━━━━━━━

📈 Market Indices

🟢 NIFTY 50: 19,875.20 (+1.24%)
🟢 SENSEX: 66,428.10 (+1.15%)
🔴 BANKNIFTY: 44,230.50 (-0.32%)
🟢 NIFTY IT: 32,145.80 (+2.10%)

━━━━━━━━━━━━━━━━━━━━━━━━━

🎯 Active IPOs (2)

✅ Orkla India Ltd
   Close: 31 Oct 2025
   GMP: +₹68 (9.3%)

✅ Jayesh Logistics
   Close: 29 Oct 2025
   GMP: +₹9 (7.4%)

━━━━━━━━━━━━━━━━━━━━━━━━━

📅 Results Today (3)

RELIANCE - Strong Expected
TCS - Good Expected
INFY - Neutral

━━━━━━━━━━━━━━━━━━━━━━━━

💼 Top Bulk Deals

🟢 TATASTEEL
   Buy: ₹5.53Cr by ABC Trust

🔴 HDFCBANK
   Sell: ₹12.4Cr by XYZ Fund

━━━━━━━━━━━━━━━━━━━━━━━━

Use /ipo, /ipos for detailed IPO info
Use /subscribe for automatic alerts
```

### What You Get

- **Market indices** with % changes
- **Active IPOs** with GMP
- **Results calendar** for today
- **Top bulk deals** of the day
- **All sections** with quick links to detailed views

---

## ⚙️ Settings & Preferences

**Command**: `/settings`

Customize your notification preferences.

### Example

```
/settings
```

### Sample Response

```
⚙️ Notification Settings

Current Settings:
✅ IPO Alerts: ON
✅ Active: Subscribed

Manage Your Alerts:
• /subscribe - Resume all alerts
• /unsubscribe - Pause all alerts

━━━━━━━━━━━━━━━━━━━━━━━━━

Want more features?
Use /premium to upgrade
```

### Available Settings

- **Enable/Disable** all notifications
- **Subscribe/Unsubscribe** with one command
- **Check status** of your subscription

---

## 📊 Subscription Status

**Command**: `/status`

Check your current subscription status and tier.

### Example

```
/status
```

### Sample Response (Free User)

```
╔══════════════════════════╗
  📊 Subscription Status
╚══════════════════════════╝

👤 User: @yourhandle
🆔 ID: 123456789

━━━━━━━━━━━━━━━━━━━━━━━━━

🎯 Tier: FREE
✅ Status: Active
🔔 Alerts: ON

━━━━━━━━━━━━━━━━━━━━━━━━━

📊 Free Features Available:
✅ IPO Notifications
✅ /ipo command
✅ /ipos command
✅ /today summary

━━━━━━━━━━━━━━━━━━━━━━━━━

💎 Upgrade to Premium:
/premium - View premium features
```

---

## 🆘 Help & Support

**Command**: `/help`

View all available commands and features.

### Example

```
/help
```

### Sample Response

```
╔══════════════════════════╗
  🤖 MarketView Commands
╚══════════════════════════╝

━━━━━━━━━━━━━━━━━━━━━━━━━
📊 MARKET DATA (FREE)
━━━━━━━━━━━━━━━━━━━━━━━━━
• /today - Today's market summary
• /ipos - Active & upcoming IPOs
• /ipo NAME - Get IPO details

━━━━━━━━━━━━━━━━━━━━━━━━━
👑 PREMIUM FEATURES
━━━━━━━━━━━━━━━━━━━━━━━━━
• /results SYMBOL - Check result date
• /deals SYMBOL - Latest bulk deals
• /trading_session - SME IPOs (10 sessions)
• /anchor_1m - 30-day anchor unlocks
• /anchor_3m - 90-day anchor unlocks
• /preipo_unlock - 1-year pre-IPO unlocks

━━━━━━━━━━━━━━━━━━━━━━━━━
⚙️ SETTINGS & STATUS
━━━━━━━━━━━━━━━━━━━━━━━━━
• /settings - Configure preferences
• /status - Subscription status
• /myid - Get your Telegram ID
• /subscribe - Resume notifications
• /unsubscribe - Pause notifications

━━━━━━━━━━━━━━━━━━━━━━━━━
ℹ️ SUPPORT
━━━━━━━━━━━━━━━━━━━━━━━━━
• /help - Show this menu
• /feedback - Send feedback

━━━━━━━━━━━━━━━━━━━━━━━━━
💎 UPGRADE TO PREMIUM
━━━━━━━━━━━━━━━━━━━━━━━━━
Use /premium to view plans & subscribe
✓ Exclusive market insights

━━━━━━━━━━━━━━━━━━━━━━━━━
MarketView - Your AI Market Companion
```

---

## 🔄 Subscribe/Unsubscribe

### Subscribe Command

**Command**: `/subscribe`

Resume all notifications (they're on by default for new users).

```
/subscribe

✅ Subscribed!

You'll now receive:
• New IPO alerts
• IPO status updates
• Market notifications

Use /unsubscribe to pause alerts
```

### Unsubscribe Command

**Command**: `/unsubscribe`

Pause all notifications temporarily.

```
/unsubscribe

⏸️ Notifications Paused

You won't receive alerts until you:
• /subscribe - Resume notifications

Your account remains active.
```

---

## 💡 Tips for Best Results

### 1. Enable Notifications for Best Experience
```
/subscribe
```
Get real-time IPO alerts automatically!

### 2. Use Commands for Quick Lookup
```
/ipo <name>    - Get detailed IPO info
/ipos          - See all active IPOs
/today         - Market summary
```

### 3. Search Works with Partial Names
```
✅ /ipo orkla
✅ /ipo jayesh
✅ /ipo premji
All work perfectly!
```

### 4. Check Multiple IPOs Quickly
```
/ipo ORKLA
/ipo JAYESH
/ipo PREMIUM
Fast and easy!
```

---

## 🆘 Command Not Working?

### If notifications aren't coming:

1. Check if you're subscribed:
   ```
   /status
   ```

2. Subscribe if needed:
   ```
   /subscribe
   ```

3. Check Telegram notification settings

### If /ipo search doesn't work:

1. Try using the symbol instead
2. Check spelling
3. Try a shorter search term
4. The IPO might not be in our database yet

---

## 📞 Need Help?

**Support Contact**: [@nimxor_marketview](https://t.me/nimxor_marketview)

**Business Hours**: Mon-Fri, 10 AM - 6 PM IST

**For Technical Issues**:
- Notification problems
- Search not working
- General questions

---

## 🔸 Daily ESM Updates

**Trigger**: Automatic daily at 7:30 PM IST (Weekdays)

Get daily Enhanced Surveillance Measure (ESM) updates for both NSE and BSE stocks - completely free!

### What is ESM?

ESM (Enhanced Surveillance Measure) is a framework used by stock exchanges to monitor stocks that show unusual price movements or trading patterns. Exchanges place stocks under surveillance to protect investors from excessive volatility.

**Two ESM Stages:**
- **ESM Stage 1**: First level surveillance - stocks show abnormal trading activity
- **ESM Stage 2**: Stricter surveillance - stocks continue to show concerning patterns

### What Triggers Notifications

✅ **ESM Stage 1 Entry** - Stock enters first level surveillance
✅ **ESM Stage 2 Entry** - Stock enters stricter surveillance
✅ **ESM2 → ESM1 Movement** - Stock moved from Stage 2 back to Stage 1
✅ **ESM Exit** - Stock removed from surveillance framework

### Sample ESM Notification

```
🔸 ESM Updates - 31 Oct 2025

━━━━━━━━━━━━━━━━━━━━━━━━━
NSE Exchange (17 stocks)
━━━━━━━━━━━━━━━━━━━━━━━━━

🔸 ESM Stage 1 Entry (3)
• EXAMPLE1
• EXAMPLE2
• EXAMPLE3

🔄 ESM2 → ESM1 (7)
• STOCK1
• STOCK2
• STOCK3
• STOCK4
• STOCK5
• STOCK6
• STOCK7

✅ Exit ESM (7)
• FREED1
• FREED2
• FREED3
• FREED4
• FREED5
• FREED6
• FREED7

━━━━━━━━━━━━━━━━━━━━━━━━━
BSE Exchange (54 stocks)
━━━━━━━━━━━━━━━━━━━━━━━━━

🔸 ESM Stage 1 Entry (2)
• 540145 - Reliance Industries
• 500325 - Tata Steel

🔹 ESM Stage 2 Entry (2)
• 532174 - ICICI Bank
• 500180 - HDFC Bank

🔄 ESM2 → ESM1 (25)
• [List of stocks...]

✅ Exit ESM (25)
• [List of stocks...]

━━━━━━━━━━━━━━━━━━━━━━━━━
📊 Total Updates: 71 stocks
```

### What You Get

- 📅 **Daily Updates**: Automatic notifications every trading day at 7:30 PM IST
- 🔍 **Complete Coverage**: Both NSE and BSE stocks
- 📊 **Categorized**: Clear grouping by action type (Entry, Exit, Movement)
- ⚡ **Real-time**: Same-day updates from exchange circulars
- 🆓 **Free**: No premium subscription needed

### Why It Matters

1. **Risk Awareness**: Know when stocks you track enter surveillance
2. **Trading Decisions**: ESM stocks have additional trading restrictions
3. **Exit Indicators**: Track when stocks are removed from surveillance
4. **Market Insight**: Understand which stocks are showing unusual patterns

### Use Cases

1. **Portfolio Monitoring**: Check if your holdings are under ESM
2. **Pre-Trade Due Diligence**: Avoid buying stocks under strict surveillance
3. **Exit Planning**: Know when it's safer to exit ESM stocks
4. **Market Analysis**: Track overall market volatility patterns

### ESM Impact on Trading

**For ESM Stage 1:**
- Additional price bands may apply
- Higher margin requirements
- Increased scrutiny from exchanges

**For ESM Stage 2:**
- Even stricter price bands
- Trade-for-trade settlement (no intraday)
- Physical delivery mandatory
- Cannot use for derivatives

### Tips

💡 **Stay Informed**: Check daily notifications to track surveillance changes
💡 **Premium Benefit**: Upgrade to premium for `/esm SYMBOL` command to check any stock's complete ESM history
💡 **Research First**: ESM stocks require extra caution before trading
💡 **Monitor Exits**: Stocks exiting ESM may indicate improving conditions

---

## 🚀 Ready to Get Started?

Visit [@marketview_ipostream_bot](https://t.me/marketview_ipostream_bot) and send `/start`!

All features above are **100% FREE** - no credit card required!

---

## 💎 Want More?

Upgrade to **Premium** for:
- Results calendar with expectations
- Bulk deals query for any stock
- ESM history query for any stock (`/esm SYMBOL`)
- VIP/HNI bulk deal alerts
- Anchor buy/sell tracking
- Trading session alerts
- Anchor unlock notifications

Send `/premium` to view plans!

---

**Last Updated**: November 2025
