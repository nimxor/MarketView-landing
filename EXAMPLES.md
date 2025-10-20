# MarketView Premium Features - Examples & Commands

Complete guide with real examples for all premium features available in MarketView Telegram Bot.

---

## 📊 Live Result Updates

**Command**: `/results SYMBOL`

Query upcoming quarterly results for any company with performance expectations.

### Examples

```
/results RELIANCE
/results Reliance Industries
/results TCS
/results Tata Consultancy Services
```

### Sample Response

```
╔══════════════════════════╗
  📊 Results Lookup
╚══════════════════════════╝

RELIANCE
Reliance Industries

━━━━━━━━━━━━━━━━━━━━━━━━━
📅 Result Date: 15 Jan 2025
🔔 Status: 📅 UPCOMING
━━━━━━━━━━━━━━━━━━━━━━━━━

🟢 STRONG RESULTS EXPECTED
Strong performance anticipated

📋 Type: Quarterly
```

### What You Get
- Exact result announcement date
- Performance expectations (Strong/Good/Neutral/Weak)
- Special events (Dividend, Bonus, Fundraising)
- Works with partial names (fuzzy matching)
- Cross-exchange lookup (NSE ↔ BSE)

---

## 💼 Query Bulk Deals

**Command**: `/deals SYMBOL`

Search and analyze bulk deal data for any stock on the most recent trade date.

### Examples

```
/deals TATASTEEL
/deals Tata Steel
/deals INFY
/deals Infosys
```

### Sample Response

```
╔══════════════════════════╗
  💼 Bulk Deals
╚══════════════════════════╝

TATASTEEL
📅 Date: 15 Oct 2025
💰 Total: 3 deals

━━━━━━━━━━━━━━━━━━━━━━━━━

🟢 Buys (2)

📊 ABC Investment Trust
   Qty: 500,000 @ ₹110.50
   Value: ₹5.53Cr

📊 XYZ Mutual Fund
   Qty: 250,000 @ ₹110.75
   Value: ₹2.77Cr

━━━━━━━━━━━━━━━━━━━━━━━━━

🔴 Sells (1)

📊 DEF Ventures ⚠️
   Qty: 300,000 @ ₹110.00
   Value: ₹3.30Cr
   Note: ANCHOR EXIT

━━━━━━━━━━━━━━━━━━━━━━━━━
⚠️ Indicates anchor investor activity
```

### What You Get
- All bulk deals for the stock
- Separated by buys and sells
- Quantity, price, and total value
- Anchor investor activity highlighted
- Recent trade date data

---

## 📈 Trading Sessions Alerts

**Command**: `/trading_session`

Get alerts for SME IPOs approaching their 10th trading session (circuit filter removal).

### Example

```
/trading_session
```

### Sample Response

```
╔══════════════════════════╗
  📈 10 Trading Sessions
╚══════════════════════════╝
━━━━━━━━━━━━━━━━━━━━━━━━━
👑 PREMIUM ALERT
━━━━━━━━━━━━━━━━━━━━━━━━━

🔴 ABC SME URGENT
   📊 Session: 9/10
   ⏰ Days Left: 1
   📅 Listed: 2025-10-04

🟡 XYZ SME Soon
   📊 Session: 7/10
   ⏰ Days Left: 3
   📅 Listed: 2025-10-08

🟢 PQR SME On Track
   📊 Session: 5/10
   ⏰ Days Left: 5
   📅 Listed: 2025-10-10

━━━━━━━━━━━━━━━━━━━━━━━━━
🔴 Urgent | 🟡 Soon | 🟢 On Track
```

### What You Get
- Current session number (e.g., 9/10)
- Days remaining until 10th session
- Listing date for reference
- Urgency indicators (Urgent/Soon/On Track)
- Critical for SME investors (circuit filters removed after 10 sessions)

### Automated Broadcasts
Premium users receive daily broadcasts with these alerts automatically.

---

## 🔓 Anchor Unlock Alerts (30-Day Lock-in)

**Command**: `/anchor_1m`

View anchor investors whose 30-day lock-in period is expiring within the next 7 days.

### Example

```
/anchor_1m
```

### Sample Response

```
╔══════════════════════════╗
  🔓 30-Day Anchor Unlocks
╚══════════════════════════╝
━━━━━━━━━━━━━━━━━━━━━━━━━
👑 PREMIUM ALERT
━━━━━━━━━━━━━━━━━━━━━━━━━

⏰ UNLOCKING IN 2 DAYS

🏢 ABC IPO LTD
   📅 Unlock: 17 Oct 2025
   🎯 Lock: 30 Days
   📊 Listed: 17 Sep 2025

━━━━━━━━━━━━━━━━━━━━━━━━━

⏰ UNLOCKING IN 5 DAYS

🏢 XYZ TECHNOLOGIES
   📅 Unlock: 20 Oct 2025
   🎯 Lock: 30 Days
   📊 Listed: 20 Sep 2025

━━━━━━━━━━━━━━━━━━━━━━━━━
⚠️ Potential selling pressure ahead
```

### What You Get
- Companies with anchors unlocking soon
- Exact unlock date
- Days remaining countdown
- Listing date for context
- Early warning for potential volatility

### Automated Broadcasts
Premium users receive automated alerts 7 days before 30-day anchor unlocks.

---

## 🔓 Anchor Unlock Alerts (90-Day Lock-in)

**Command**: `/anchor_3m`

View anchor investors whose 90-day lock-in period is expiring within the next 15 days.

### Example

```
/anchor_3m
```

### Sample Response

```
╔══════════════════════════╗
  🔓 90-Day Anchor Unlocks
╚══════════════════════════╝
━━━━━━━━━━━━━━━━━━━━━━━━━
👑 PREMIUM ALERT
━━━━━━━━━━━━━━━━━━━━━━━━━

⏰ UNLOCKING IN 8 DAYS

🏢 DEF INDUSTRIES
   📅 Unlock: 23 Oct 2025
   🎯 Lock: 90 Days
   📊 Listed: 25 Jul 2025

━━━━━━━━━━━━━━━━━━━━━━━━━

⏰ UNLOCKING IN 12 DAYS

🏢 GHI SOLUTIONS
   📅 Unlock: 27 Oct 2025
   🎯 Lock: 90 Days
   📊 Listed: 29 Jul 2025

━━━━━━━━━━━━━━━━━━━━━━━━━
⚠️ Prepare for potential price impact
```

### What You Get
- Companies with 90-day anchor unlocks coming
- 15-day advance notice
- Unlock date and countdown
- Listing date reference
- Time to plan trading strategy

### Automated Broadcasts
Premium users receive automated alerts 15 days before 90-day anchor unlocks.

---

## 🔍 Pre-IPO Unlock Notifications (1-Year Lock-in)

**Command**: `/preipo_unlock`

Get notified about pre-IPO shareholders whose 1-year lock-in period is expiring within the next 30 days.

### Example

```
/preipo_unlock
```

### Sample Response

```
╔══════════════════════════╗
  🔍 Pre-IPO Unlocks (1Y)
╚══════════════════════════╝
━━━━━━━━━━━━━━━━━━━━━━━━━
👑 PREMIUM ALERT
━━━━━━━━━━━━━━━━━━━━━━━━━

⏰ UNLOCKING IN 15 DAYS

🏢 JKL ENTERPRISES
   📅 Unlock: 30 Oct 2025
   🎯 Lock: 365 Days (1 Year)
   📊 Listed: 30 Oct 2024

━━━━━━━━━━━━━━━━━━━━━━━━━

⏰ UNLOCKING IN 25 DAYS

🏢 MNO TECH
   📅 Unlock: 09 Nov 2025
   🎯 Lock: 365 Days (1 Year)
   📊 Listed: 09 Nov 2024

━━━━━━━━━━━━━━━━━━━━━━━━━
⚠️ Major unlock event - plan accordingly
```

### What You Get
- Pre-IPO investors unlocking in next 30 days
- Exact unlock date
- One-year anniversary tracking
- 30-day advance warning
- Critical for planning around major unlock events

### Automated Broadcasts
Premium users receive automated alerts 30 days before 1-year pre-IPO unlocks.

---

## ⭐ Early Access to New Features

Premium subscribers get **first access** to all new features before they're released to free users.

### Current Early Access Features

All the features above were initially released to premium users as early access:

- **Query Results** (`/results`) - Query any stock's upcoming results
- **Query Bulk Deals** (`/deals`) - Search bulk deals for any stock
- **Trading Sessions** (`/trading_session`) - SME circuit filter alerts
- **Anchor Unlocks** (`/anchor_1m`, `/anchor_3m`) - Lock-in expiry tracking
- **Pre-IPO Unlocks** (`/preipo_unlock`) - 1-year unlock notifications

### Future Features Coming Soon

Premium users will get early access to:
- **Advanced Filters** - Filter by market type, result expectations, deal types
- **Customization** - Choose which alerts to receive, notification preferences
- **Analytics Dashboard** - Track received alerts, market trends, performance metrics

---

## 🎯 Smart Fuzzy Matching

All query commands (`/results` and `/deals`) support **fuzzy matching** for easy searching.

### How It Works

You don't need to type the exact symbol or company name. The bot intelligently matches:

#### Example: Searching for Reliance Industries

All these work:
```
/results RELIANCE
/results reliance
/results Reliance Industries
/results Reliance Ind
/results RIL
```

#### Example: Searching for Tata Consultancy Services

All these work:
```
/results TCS
/results tcs
/results Tata Consultancy
/results Tata Consultancy Services
/results TATACONSULT
```

### Matching Priority

1. **Exact symbol match** - Highest priority
2. **Exact company name match** - High priority
3. **Partial company name** - Medium priority
4. **Fuzzy symbol similarity** - Lower priority
5. **Fuzzy name similarity** - Lowest priority

Minimum 50% match confidence required.

---

## 🔄 Cross-Exchange Lookup

If a stock isn't found on NSE, the bot automatically searches BSE and vice versa.

### Example

```
You: /results SOMESME
Bot: Not found on NSE, checking BSE...
Bot: ✅ Found on BSE!
```

This ensures you get results even if you don't know which exchange the stock is listed on.

---

## 📱 How to Use Premium Commands

### Step 1: Subscribe to Premium

```
/premium
```

Choose your plan and complete payment.

### Step 2: Use Any Premium Command

Once your premium subscription is active, you can use any of these commands:

**Query Commands** (On-Demand):
- `/results SYMBOL` - Check result dates
- `/deals SYMBOL` - Check bulk deals
- `/trading_session` - View trading sessions
- `/anchor_1m` - View 30-day unlocks
- `/anchor_3m` - View 90-day unlocks
- `/preipo_unlock` - View 1-year unlocks

**Automated Broadcasts** (Daily):
Premium users automatically receive daily broadcasts for:
- Trading sessions approaching 10th session
- Anchor unlocks (30-day, 90-day, 1-year)

### Step 3: Check Your Status

```
/status
```

View your subscription tier, expiration date, and days remaining.

---

## 💡 Tips for Best Results

### 1. Use Stock Symbols for Faster Results
```
✅ /results RELIANCE
❌ /results Reliance Industries Limited
```

### 2. Partial Names Work Great
```
✅ /deals TATA
✅ /deals Tata Steel
Both work fine!
```

### 3. Case Doesn't Matter
```
/results INFY
/results infy
/results Infy
All the same!
```

### 4. Check Multiple Stocks Quickly
```
/results RELIANCE
/results TCS
/results INFY
/results HDFCBANK
```

---

## 🆘 Command Not Working?

### If you get "Premium Required" message:

1. Check your subscription:
   ```
   /status
   ```

2. If expired, renew:
   ```
   /premium
   ```

3. If active but not working, contact support:
   - Telegram: [@nimxor_marketview](https://t.me/nimxor_marketview)

### If you get "Stock Not Found":

1. Try using the stock symbol instead of full name
2. Check spelling
3. Try a partial name
4. The stock might not be in our database yet

---

## 📞 Need Help?

**Support Contact**: [@nimxor_marketview](https://t.me/nimxor_marketview)

**Business Hours**: Mon-Fri, 10 AM - 6 PM IST

**For Premium Issues**:
- Payment verification
- Subscription activation
- Technical support

---

## 🚀 Ready to Get Started?

Visit [@marketview_ipostream_bot](https://t.me/marketview_ipostream_bot) and send `/premium` to subscribe!

---

**Last Updated**: October 2025
