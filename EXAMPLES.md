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

## 📈 Filter Results by Date and Type

**Command**: `/result_on_date DD-MM-YYYY [EXCHANGE] [TYPE]`

Query and filter quarterly results scheduled for a specific date by exchange and/or expectation type.

### Command Formats

```
/result_on_date DATE TYPE          - Filter by result type
/result_on_date DATE EXCHANGE      - Filter by exchange only
/result_on_date DATE EXCHANGE TYPE - Filter by both exchange and type
```

### Examples

**Filter by Result Type:**
```
/result_on_date 05-11-2025 strong
/result_on_date 10-11-2025 good
/result_on_date 15-11-2025 all
/result_on_date 20-11-2025 weak
```

**Filter by Exchange:**
```
/result_on_date 05-11-2025 sme
/result_on_date 05-11-2025 mainboard
```

**Filter by Both Exchange and Type:**
```
/result_on_date 05-11-2025 sme strong
/result_on_date 05-11-2025 sme good
/result_on_date 05-11-2025 sme neutral
/result_on_date 05-11-2025 mainboard strong
/result_on_date 05-11-2025 mainboard good
/result_on_date 05-11-2025 mainboard neutral
```

### Available Filters

**Exchanges:**
- **`mainboard`** - NSE/BSE mainboard stocks only
- **`sme`** - SME platform stocks only

**Result Types:**
- **`strong`** - Strong Positive (YoY growth > 20%)
- **`good`** - Good Expected (YoY growth 0-20%)
- **`neutral`** - Neutral (missing data)
- **`weak`** - Weak (YoY growth < 0%)
- **`all`** - Show all results for the date

### Sample Response

```
  ╔══════════════════════════╗
    🟢 Strong Positive
  ╚══════════════════════════╝

  📅 Date: 05 Nov 2025
  📈 Total: 12 companies

  ━━━━━━━━━━━━━━━━━━━━━━━━━

  🏢 MAINBOARD (8 companies)

  Reliance Industries Limited
  Tata Consultancy Services
  Infosys Limited
  HDFC Bank Limited
  ICICI Bank Limited
  Bharti Airtel Limited
  State Bank of India
  Larsen & Toubro Limited

  ━━━━━━━━━━━━━━━━━━━━━━━━━

  🏪 SME (4 companies)

  ABC Technologies Limited
  XYZ Manufacturing Limited
  PQR Solutions Limited
  LMN Industries Limited
```

**Note:** All company names are clickable links to Screener.in for detailed analysis.

### What You Get
- Filter by specific date (DD-MM-YYYY format)
- Filter by exchange (mainboard/SME)
- Filter by expectation type (strong/good/neutral/weak/all)
- Combine exchange and type filters for precise targeting
- Grouped by mainboard and SME
- Clean list of company names (no clutter)
- All company names are clickable links to Screener.in
- Quick overview of which companies have results on a specific day
- Plan your trades based on upcoming results

### Use Cases
- **Pre-Market Planning**: Check strong results for the day
- **SME Focus**: Use `/result_on_date DATE sme` to see only SME results
- **Mainboard Only**: Filter mainboard stocks with `/result_on_date DATE mainboard`
- **Targeted Search**: Combine filters like `/result_on_date DATE sme strong` for SME stocks with strong growth
- **Earnings Season**: Track multiple results on busy days
- **Filter Weak Results**: Identify companies with poor expectations
- **All Results View**: See complete result calendar for any date

### Tips
- Use `strong` filter before market opens to spot potential movers
- Check `sme strong` for high-growth SME opportunities
- Use `mainboard good` for safer large-cap plays
- Check `all` results on Fridays for weekend analysis
- Compare `good` vs `weak` counts to gauge market sentiment
- Filter by exchange when you have specific portfolio constraints

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

## 🌟 VIP/HNI Bulk Deal Alerts (NEW!)

**Trigger**: Automatic (Premium Only)

Get instant notifications when VIP clients or HNIs make bulk deals in IPO stocks!

### What Triggers Alerts

Premium users automatically receive alerts when:
- **VIP clients** appear in bulk deals for IPO stocks
- **HNI traders** make significant moves
- **Known operators** enter or exit positions

### Sample VIP Client Alert

```
🌟 VIP CLIENT BULK DEAL ALERT

📊 JAYESH LOGISTICS (JAYESH)
📅 Date: 01 Nov 2025

━━━━━━━━━━━━━━━━━━━━━━━━━

⭐ VIP CLIENT ACTIVITY

🟢 BUY
Client: PREMIUM INVESTMENT TRUST
Qty: 50,000 @ ₹125.50
Value: ₹62.75L
Exchange: NSE

━━━━━━━━━━━━━━━━━━━━━━━━━

🔍 Why This Matters:
This client has history of profitable exits
in recent IPOs. Their entry often signals
confidence in the stock.

━━━━━━━━━━━━━━━━━━━━━━━━━
```

### What You Get (Premium Only)

- **Real-time alerts** when VIP clients trade
- **Client identification** with track record
- **Deal details**: Quantity, price, value
- **Exchange information** (NSE/BSE)
- **Context**: Why this deal matters
- **Historical insights** on client performance

### Automated Broadcasts

Premium users receive these alerts **automatically** every 30 minutes when:
- New bulk deals are detected
- VIP clients are involved
- Deal value exceeds thresholds

---

## 🎯 Anchor Entry/Exit Alerts (NEW!)

**Trigger**: Automatic (Premium Only)

Get instant notifications when anchor investors enter or exit positions!

### What Triggers Alerts

Premium users automatically receive alerts when:
- **Anchor investors** buy back into IPO stocks (re-entry)
- **Anchor investors** exit positions (sell)
- **Significant anchor activity** detected

### Sample Anchor Entry Alert

```
✅ ANCHOR ENTRY ALERT

📊 ORKLA INDIA (ORKLAINDIA)
📅 Date: 01 Nov 2025

━━━━━━━━━━━━━━━━━━━━━━━━━

🟢 ANCHOR RE-ENTRY

Client: CITIGROUP GLOBAL MARKETS
Qty: 1,00,000 @ ₹785.00
Value: ₹7.85Cr
Exchange: NSE

🌟 Signal: BULLISH

━━━━━━━━━━━━━━━━━━━━━━━━━

🔍 Analysis:
Anchor re-entering after lock-in period
often indicates strong confidence in
fundamentals. Historically positive signal.

IPO Details:
Listed: 06 Nov 2025
Listing Gain: +8.2%
Current GMP: +₹68

━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Sample Anchor Exit Alert

```
⚠️ ANCHOR EXIT ALERT

📊 ABC TECH LTD (ABCTECH)
📅 Date: 01 Nov 2025

━━━━━━━━━━━━━━━━━━━━━━━━━

🔴 ANCHOR EXIT

Client: KOTAK INSTITUTIONAL EQUITIES
Qty: 2,50,000 @ ₹425.50
Value: ₹10.64Cr
Exchange: NSE

🌟 Signal: CAUTION

━━━━━━━━━━━━━━━━━━━━━━━━━

🔍 Analysis:
Anchor exiting shortly after lock-in
expiry. May indicate profit booking or
reduced confidence. Monitor for
continued selling pressure.

IPO Details:
Listed: 28 Oct 2025
Days Since Listing: 4 days
Listing Gain: +15.2%
Lock-in: 30 days (expired)

━━━━━━━━━━━━━━━━━━━━━━━━━
```

### What You Get (Premium Only)

- **Instant alerts** for anchor activity
- **Entry/Exit signals** (Bullish/Bearish/Caution)
- **Deal details**: Client name, quantity, value
- **IPO context**: Listing date, gains, lock-in status
- **Analysis**: Why this matters for your trading
- **Historical patterns**: How similar moves performed

### Automated Broadcasts

Premium users receive these alerts **automatically** every 30 minutes when:
- Anchor investors make bulk deals
- Both entries and exits are tracked
- Deals are in IPO stocks (listed in last 365 days)

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

Premium users receive **6 separate unlock notifications**:

**1-Month Anchor Unlocks (Daily, Mon-Fri):**
- 🔸 SME IPOs: 3:30 PM IST
- 🔸 Mainboard IPOs: 3:32 PM IST
- Alert window: Next 10 days

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

**3-Month Anchor Unlocks (Daily, Mon-Fri):**
- 🔹 SME IPOs: 3:15 PM IST
- 🔹 Mainboard IPOs: 3:17 PM IST
- Alert window: Next 15 days

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

**Pre-IPO Unlocks (Weekly, Saturday):**
- 🔺 SME IPOs (1-year lock-in): 3:00 PM IST
- 🔺 Mainboard IPOs (6-month lock-in): 3:02 PM IST
- Alert window: Next 30 days

---

## 📅 Query Unlock Dates for Any IPO

**Command**: `/unlock SYMBOL or COMPANY NAME`

Get all anchor unlock dates (30-day, 90-day, and 1-year) for any listed IPO instantly!

### Examples

```
/unlock PREMIERENE
/unlock Premier Energies
/unlock WAAREE
/unlock Orkla India
```

### Sample Response

```
🔓 Anchor Unlock Dates

PREMIERENE
Premier Energies Limited

📅 Listing Date: 03 Sep 2024

━━━━━━━━━━━━━━━━━━━━━━━━━
🔸 1 Month Anchor Unlock
📆 03 Oct 2024
✅ Unlocked (29 days ago)

━━━━━━━━━━━━━━━━━━━━━━━━━
🔹 3 Month Anchor Unlock
📆 02 Dec 2024
⏳ In 32 days

━━━━━━━━━━━━━━━━━━━━━━━━━
🔺 Pre-IPO Unlock (1 Year)
📆 03 Sep 2025
⏳ In 307 days
━━━━━━━━━━━━━━━━━━━━━━━━━

Unlock dates are approximate and based on listing date
```

### What You Get

- **All unlock dates** in one place (30-day, 90-day, 1-year)
- **Unlock status** - Already unlocked or days remaining
- **Listing date** for reference
- **Smart search** - Works with symbol or company name
- **Instant calculation** - No need to calculate manually
- **Historical tracking** - Shows when unlocks already happened

### Use Cases

1. **Planning trades** - Know when selling pressure might come
2. **Risk assessment** - Check all unlock dates before investing
3. **Exit strategy** - Plan exits before major unlocks
4. **Quick lookup** - Instantly see all unlock dates
5. **Historical analysis** - See which unlocks already passed

### Unlock Status Indicators

- ✅ **Unlocked** - Already passed (shows days ago)
- 🔔 **Unlocking Today!** - Happening today
- ⏳ **In X days** - Future unlock date

### Smart Fuzzy Matching

Just like other commands, `/unlock` supports fuzzy search:

```
/unlock PREMIERENE         → Exact symbol match
/unlock Premier            → Partial name match
/unlock Premier Energies   → Full name match
/unlock WAAREE            → Symbol
/unlock Waaree Energies   → Name
```

---

## ⚓ Query Anchor Investors

**Command**: `/anchor SYMBOL or COMPANY NAME`

View the complete list of anchor investors for any IPO with allocation details.

### Examples

```
/anchor PREMIERENE
/anchor Premier Energies
/anchor WAAREE
/anchor Swiggy
```

### Sample Response

```
⚓ Anchor Investors

PREMIERENE
Premier Energies Limited

━━━━━━━━━━━━━━━━━━━━━━━━━
📊 Summary
├ Total Anchors: 56
├ Total Allocation: ₹1,342.50 Cr
└ Anchor Price: ₹450.00

━━━━━━━━━━━━━━━━━━━━━━━━━
📈 By Type

🏦 Mutual Funds: 28 investors (₹756.25 Cr)
🏢 Insurance: 8 investors (₹285.50 Cr)
🌍 FII: 12 investors (₹198.75 Cr)
💼 Others: 8 investors (₹102.00 Cr)

━━━━━━━━━━━━━━━━━━━━━━━━━
🏆 Top 15 Investors

1. HDFC Mutual Fund - ₹125.50 Cr
2. SBI Mutual Fund - ₹98.25 Cr
3. ICICI Prudential MF - ₹87.50 Cr
...
```

### What You Get

- **Complete anchor list** with allocation amounts
- **Summary statistics**: Total anchors, total allocation, anchor price
- **Breakdown by investor type**: MFs, Insurance, FIIs, Others
- **Top 15 investors** by allocation amount
- **Smart search**: Works with symbol or company name

### Use Cases

1. **Pre-investment research**: Check who invested as anchors
2. **Quality signal**: Strong anchor participation indicates confidence
3. **Unlock planning**: Know who might sell after lock-in
4. **Pattern analysis**: Compare anchor participation across IPOs

---

## 🔍 Anchor Portfolio Lookup

**Command**: `/anchor_info INVESTOR NAME`

Search any anchor investor's complete IPO investment history across all IPOs.

### Examples

```
/anchor_info HDFC
/anchor_info Saint Capital
/anchor_info Rajasthan Global
/anchor_info Goldman Sachs
```

### Sample Response

```
🏦 Anchor Investor Info

HDFC MUTUAL FUND (3 entities)

📊 Summary
├ Total IPOs: 45
└ Total Investment: ₹2,856.75 Cr

📈 Recent Investments

1. PREMIERENE Premier Energies
   ₹125.50 Cr | 03 Sep 24

2. WAAREE Waaree Energies
   ₹98.25 Cr | 28 Oct 24

3. SWIGGY Swiggy
   ₹156.00 Cr | 13 Nov 24

...and 42 more IPOs

📋 Matching Entities
• HDFC Mutual Fund
• HDFC Life Insurance
• HDFC Bank Limited
```

### What You Get

- **Complete investment history** across all IPOs
- **Summary**: Total IPOs invested, total investment amount
- **Recent investments**: Last 15 IPO investments with details
- **Entity grouping**: Groups similar names (HDFC Bank, HDFC MF, etc.)
- **Partial search**: Search with partial name like "HDFC", "Saint", "SBI"

### Use Cases

1. **Track smart money**: See where top investors are putting money
2. **Pattern analysis**: Identify investor preferences
3. **Quality signal**: Repeated investments by same anchor
4. **Due diligence**: Research investor track record

---

## 🏢 Lead Manager Portfolio

**Command**: `/lm LEAD MANAGER NAME`

View all IPOs managed by any lead manager with performance statistics.

### Examples

```
/lm HDFC Bank
/lm Emkay
/lm Pantomath
/lm SBI Capital
/lm Axis Capital
```

### Sample Response

```
🏢 Lead Manager Info

Pantomath Capital Advisors

📊 Portfolio Summary
├ Total IPOs: 89
├ Listed: 72 | Active: 5 | Upcoming: 12
├ Avg GMP: +18.5%
└ Avg Listing Gains: +22.3%

📈 Recent IPOs

1. ✅ ABCTECH ABC Technologies
   15 Nov 24 | +35.2%

2. ✅ XYZIND XYZ Industries
   10 Nov 24 | +18.5%

3. 🟢 PQRSME PQR Solutions
   TBA | GMP: +25.0%

4. 📅 LMNIPO LMN Limited
   20 Dec 24

...and 85 more IPOs

📋 Matching Entities
• Pantomath Capital Advisors Private Limited
• Pantomath Capital
```

### What You Get

- **Portfolio summary**: Total IPOs, listed/active/upcoming breakdown
- **Performance metrics**: Average GMP, average listing gains
- **Recent IPOs**: Last 15 IPOs with status and performance
- **Status indicators**: ✅ Listed, 🟢 Active, 📅 Upcoming
- **Entity grouping**: Groups similar lead manager names

### Use Cases

1. **Manager reputation**: Check lead manager's track record
2. **Performance analysis**: Compare avg gains across managers
3. **IPO selection**: Prefer IPOs from successful managers
4. **Research**: Understand manager's focus (SME vs Mainboard)

### Status Indicators

- ✅ **Listed**: IPO has listed, shows listing gains
- 🟢 **Active**: IPO currently open for subscription
- 📅 **Upcoming**: IPO announced but not yet open
- ⏸️ **Other**: Withdrawn or delayed IPOs

---

## 🔸 ESM Surveillance History

**Command**: `/esm SYMBOL or COMPANY NAME`

Get complete Enhanced Surveillance Measure (ESM) history for any stock - track all surveillance stages, movements, and exits!

### What is ESM?

ESM (Enhanced Surveillance Measure) is a surveillance framework used by NSE and BSE to monitor stocks showing unusual price movements or trading patterns. Stocks under ESM face additional restrictions to protect investors.

**ESM Stages:**
- **ESM Stage 1**: First-level surveillance with additional price bands
- **ESM Stage 2**: Stricter surveillance with trade-for-trade settlement
- **ESM2 → ESM1**: Stock improved, moved from Stage 2 back to Stage 1
- **Exit ESM**: Stock removed from surveillance completely

### Examples

```
/esm RELIANCE
/esm Reliance Industries
/esm 540145
/esm Tata Steel
/esm TATASTEEL
```

### Sample Response - NSE Stock

```
🔸 ESM History

TATASTEEL
Tata Steel Limited

━━━━━━━━━━━━━━━━━━━━━━
NSE Exchange (8 events)
━━━━━━━━━━━━━━━━━━━━━━

📅 15 Sep 2024
🔸 ESM Stage 1 Entry

📅 22 Sep 2024
🔹 ESM Stage 2 Entry

📅 10 Oct 2024
🔄 ESM2 → ESM1

📅 31 Oct 2024
✅ Exit ESM

━━━━━━━━━━━━━━━━━━━━━━
Total ESM Events: 8
Period: Sep 2024 - Oct 2024
```

### Sample Response - BSE Stock

```
🔸 ESM History

540145
Reliance Industries Limited

━━━━━━━━━━━━━━━━━━━━━━
BSE Exchange (5 events)
━━━━━━━━━━━━━━━━━━━━━━

📅 01 Sep 2024
🔸 ESM Stage 1 Entry

📅 15 Sep 2024
🔹 ESM Stage 2 Entry
_Effective from: 16 Sep 2024_

📅 01 Oct 2024
🔄 ESM2 → ESM1

📅 15 Oct 2024
✅ Exit ESM

━━━━━━━━━━━━━━━━━━━━━━
Total ESM Events: 5
Period: Sep 2024 - Oct 2024
```

### What You Get

- 📊 **Complete History**: All ESM events for a stock from Sept 2024 onwards
- 📅 **Chronological Order**: Events sorted by date (oldest to newest)
- 🔍 **Detailed Info**: Event dates, effective dates, action types
- 🌍 **Multi-Exchange**: Separate sections for NSE and BSE
- 📈 **Status Tracking**: See if stock entered, exited, or moved between stages
- 🔸 **Risk Assessment**: Understand stock's surveillance history before investing

### Use Cases

1. **Pre-Investment Research**: Check if stock has ESM history before buying
2. **Risk Management**: Track if your holdings ever entered ESM
3. **Trading Decisions**: Avoid stocks with frequent ESM entries
4. **Exit Planning**: Know when stocks typically exit ESM
5. **Pattern Analysis**: Identify stocks with recurring surveillance issues
6. **Compliance Tracking**: Monitor regulatory actions on stocks

### ESM Stage Impact

**ESM Stage 1:**
- Additional price bands (5-10%)
- Higher margin requirements
- Increased exchange scrutiny
- Daily surveillance monitoring

**ESM Stage 2:**
- Stricter price bands (2-5%)
- **Trade-for-trade** settlement (no intraday)
- **100% margin** required upfront
- **Physical delivery** mandatory
- Cannot use for F&O trading
- Higher transaction costs

### Smart Fuzzy Matching

The `/esm` command supports smart search for both NSE and BSE stocks:

**NSE Stocks (Alphabetic Symbols):**
```
/esm RELIANCE          → Exact symbol match
/esm Reliance          → Company name search
/esm Reliance Industries → Full name match
```

**BSE Stocks (Numeric Scrip Codes):**
```
/esm 540145            → Direct scrip code match
/esm Reliance          → Searches by company name
/esm Reliance Industries → Full company name
```

### Tips

💡 **Check Before Buying**: Always check ESM history before investing in a stock
💡 **Free Daily Updates**: Get automatic ESM updates for all stocks at 7:30 PM IST (free feature)
💡 **Stage 2 Warning**: Stocks in ESM Stage 2 have severe trading restrictions
💡 **Exit Timing**: Stocks exiting ESM may see improved liquidity and lower volatility
💡 **Historical Patterns**: Frequent ESM entries indicate high-risk stocks
💡 **BSE Search**: For BSE stocks, search by company name if you don't know the scrip code

### Why ESM Matters

1. **Trading Restrictions**: ESM stocks have additional trading constraints
2. **Higher Costs**: Increased margins and delivery requirements
3. **Risk Indicator**: ESM placement signals unusual trading activity
4. **Liquidity Impact**: ESM stocks may have lower liquidity
5. **Price Discovery**: Trade-for-trade settlement affects price discovery
6. **Investment Decision**: Important factor in buy/sell decisions

### Related Features

- **Free Daily ESM Updates**: Get automatic daily notifications at 7:30 PM IST (all users)
- **Historical Data**: Complete ESM history from September 2024 onwards
- **Multi-Exchange**: Covers both NSE and BSE surveillance measures

---

## ⭐ Early Access to New Features

Premium subscribers get **first access** to all new features before they're released to free users.

### Current Early Access Features

All the features above were initially released to premium users as early access:

- **Query Results** (`/results`) - Query any stock's upcoming results
- **Query Bulk Deals** (`/deals`) - Search bulk deals for any stock
- **Query Unlock Dates** (`/unlock`) - Get all unlock dates for any IPO
- **Query Anchor Investors** (`/anchor`) - View anchor list for any IPO
- **Anchor Portfolio Lookup** (`/anchor_info`) - Search anchor investor's history
- **Lead Manager Portfolio** (`/lm`) - View lead manager's IPO portfolio
- **Query ESM History** (`/esm`) - Complete surveillance history for any stock
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

All query commands (`/results`, `/deals`, `/unlock`, `/anchor`, `/anchor_info`, `/lm`, and `/esm`) support **fuzzy matching** for easy searching.

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
- `/unlock SYMBOL` - Get all unlock dates
- `/anchor SYMBOL` - View anchor investor list
- `/anchor_info NAME` - Search anchor portfolio
- `/lm NAME` - View lead manager portfolio
- `/esm SYMBOL` - Check ESM surveillance history
- `/trading_session` - View trading sessions
- `/anchor_1m` - View 30-day unlocks
- `/anchor_3m` - View 90-day unlocks
- `/preipo_unlock` - View 1-year unlocks

**Automated Broadcasts** (Daily/Weekly):
Premium users automatically receive unlock notifications:
- 🔸 1M Anchor Unlock: Daily 3:30 PM IST (SME & Mainboard)
- 🔹 3M Anchor Unlock: Daily 3:15 PM IST (SME & Mainboard)
- 🔺 Pre-IPO Unlock: Weekly Saturday 3:00 PM IST (SME 1-year, Mainboard 6-month)

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

**Last Updated**: December 2025
