# MarketView Landing Documentation Guide

**Quick reference for updating landing page documentation when features change.**

---

## 📋 When to Update This Repo

Update MarketView-landing documentation when:
- ✅ New feature is added to the bot
- ✅ Existing feature is updated or enhanced
- ✅ Command syntax changes
- ✅ Feature moves from premium to free (or vice versa)
- ✅ New commands are added
- ✅ Alert types or notifications change

---

## 📁 File Structure

```
MarketView-landing/
├── index.md                    # Main landing page
├── QUICK_START.md             # Quick start guide
├── FREE_FEATURES.md           # All free features
├── EXAMPLES.md                # Premium features examples
├── FEATURES_COMPARISON.md     # Free vs Premium comparison
├── USER_GUIDE.md              # Complete user guide
└── DOCUMENTATION_GUIDE.md     # This file
```

---

## 🔄 Update Locations by Feature Type

### For FREE Features

| File | Section | What to Update |
|------|---------|----------------|
| `index.md` | FREE features table | Add row with feature name and description |
| `index.md` | Free Commands section | Add command with syntax |
| `QUICK_START.md` | Free Commands table | Add command and description |
| `QUICK_START.md` | FREE Features section | Add feature with details |
| `FREE_FEATURES.md` | New section | Full feature documentation |

### For PREMIUM Features

| File | Section | What to Update |
|------|---------|----------------|
| `index.md` | PREMIUM features list | Add feature with link to EXAMPLES.md |
| `index.md` | Premium Commands section | Add command with syntax |
| `QUICK_START.md` | Premium Commands table | Add command and description |
| `QUICK_START.md` | PREMIUM Features section | Add feature with details |
| `EXAMPLES.md` | New section | Full feature documentation |
| `EXAMPLES.md` | Feature lists | Add to feature lists |

---

## ✍️ Content Templates

### Template: FREE Feature Section (FREE_FEATURES.md)

```markdown
## 🔍 Feature Name

**Command**: `/commandname <arguments>`
OR
**Trigger**: Automatic

Brief description of what the feature does.

### Examples

\`\`\`
/commandname example1
/commandname example2
\`\`\`

### Sample Response

\`\`\`
[Formatted sample output showing what users will see]
\`\`\`

### What You Get

- Benefit 1
- Benefit 2
- Benefit 3
- **100% FREE** - No premium required!

### How to Use

1. Step 1
2. Step 2
3. Step 3

### Tips

- Tip 1
- Tip 2
```

### Template: PREMIUM Feature Section (EXAMPLES.md)

```markdown
## 📅 Feature Name

**Command**: `/commandname ARGUMENTS`
OR
**Trigger**: Automatic (Premium Only)

Brief description of premium feature.

### Examples

\`\`\`
/commandname EXAMPLE1
/commandname EXAMPLE2
\`\`\`

### Sample Response

\`\`\`
[Formatted sample output showing premium feature data]
\`\`\`

### What You Get (Premium Only)

- Premium benefit 1
- Premium benefit 2
- Premium benefit 3

### Use Cases

1. Trading use case
2. Investment use case
3. Analysis use case

### Automated Broadcasts (if applicable)

Premium users receive these alerts **automatically** when [condition].
```

### Template: index.md FREE Feature Entry

```markdown
| 🔍 **Feature Name** | `/command` - Brief description |
| | Additional details about the feature |
```

### Template: index.md PREMIUM Feature Entry

```markdown
- 📅 **[Feature Name](EXAMPLES.md#anchor-link)** - Brief description with details
```

### Template: Command Table Entry

```markdown
| `/commandname ARGS` | What the command does |
```

---

## 📝 Writing Guidelines

### Command Descriptions

**Good:**
```markdown
/ipo NAME - Get detailed IPO info (GMP, prices, dates, RHP)
```

**Bad:**
```markdown
/ipo - IPO command
```

### Feature Benefits

**Good:**
- Real-time alerts for new IPOs
- Complete IPO details including GMP and RHP link
- Automatic notifications for status changes

**Bad:**
- Get IPO info
- Notifications

### Sample Responses

**Always include:**
- Actual formatted output (as users will see it)
- Emojis and symbols used in the bot
- All sections of the message
- Realistic data

---

## 🎯 Common Update Scenarios

### Scenario 1: New Free Command Added

**Example:** `/ipo` command

**Steps:**
1. ✅ Add to `index.md` FREE features table
2. ✅ Add to `index.md` Free Commands section
3. ✅ Add to `QUICK_START.md` Free Commands table
4. ✅ Add to `QUICK_START.md` FREE Features section
5. ✅ Create full section in `FREE_FEATURES.md`

### Scenario 2: New Premium Command Added

**Example:** `/unlock` command

**Steps:**
1. ✅ Add to `index.md` PREMIUM features list (with link)
2. ✅ Add to `index.md` Premium Commands section
3. ✅ Add to `QUICK_START.md` Premium Commands table
4. ✅ Add to `QUICK_START.md` PREMIUM Features section
5. ✅ Create full section in `EXAMPLES.md`
6. ✅ Add to feature lists in `EXAMPLES.md`

### Scenario 3: New Automatic Alert (Free)

**Example:** IPO status change notifications

**Steps:**
1. ✅ Add to `index.md` FREE features table
2. ✅ Add to `QUICK_START.md` FREE Features section
3. ✅ Create full section in `FREE_FEATURES.md`
4. ✅ Explain trigger conditions and sample alerts

### Scenario 4: New Automatic Alert (Premium)

**Example:** VIP/HNI bulk deal alerts

**Steps:**
1. ✅ Add to `index.md` PREMIUM features list
2. ✅ Add to `QUICK_START.md` PREMIUM Features section
3. ✅ Create full section in `EXAMPLES.md`
4. ✅ Add to automated broadcasts section
5. ✅ Include sample alert messages

---

## 🔍 Quality Checklist

Before committing documentation updates, verify:

- [ ] All command syntax is correct
- [ ] Sample responses match actual bot output
- [ ] FREE vs PREMIUM is clearly marked
- [ ] Links to other sections work
- [ ] Markdown formatting is correct
- [ ] Emojis are used consistently
- [ ] No typos or grammatical errors
- [ ] Benefits are clear and specific
- [ ] Examples are realistic and helpful

---

## 🚀 Publishing Updates

### Commit Message Template

```bash
git commit -m "Add [feature name] documentation

[Detailed description of what was added/changed]

- Updated index.md with feature overview
- Updated QUICK_START.md with commands
- Added complete section to [FREE_FEATURES.md or EXAMPLES.md]

🤖 Generated with [Claude Code](https://claude.com/claude-code)

Co-Authored-By: Claude <noreply@anthropic.com>"
```

### Deployment

```bash
cd /path/to/MarketView-landing
git add .
git commit -m "..."
git push origin main
```

**GitHub Pages will automatically update** (usually within 1-2 minutes).

---

## 📞 Cross-Reference

**Main codebase checklist:**
`/Users/nimxor/PycharmProjects/MarketView/FEATURE_UPDATE_CHECKLIST.md`

This checklist covers bot code updates. The documentation guide (this file) focuses on landing page updates only.

---

## 🎨 Style Guide

### Emojis

Use consistent emojis for feature types:
- 📊 Market data
- 🔍 Search/query
- 🔔 Notifications/alerts
- 💼 Bulk deals
- 📅 Results/calendar
- 🔓 Unlocks
- 🌟 VIP/premium exclusive
- 🎯 Tracking/monitoring
- 💎 Premium/upgrade

### Headings

- Use `##` for main sections
- Use `###` for subsections
- Use `####` for minor subsections
- Keep heading structure consistent

### Code Blocks

Use triple backticks with no language for command examples:
```
/command example
```

Use `markdown` for documentation snippets:
```markdown
**Bold text**
```

### Links

Internal links:
```markdown
[Link Text](FILE.md#section-anchor)
```

External links:
```markdown
[Link Text](https://example.com)
```

---

**Last Updated:** November 2025
