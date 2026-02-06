# Spec-Check
Working demo version of a doc checker

# 🎯 Spec-Check Premortem Assistant

A real-time AI-powered tool that red-teams Product Requirements Documents (PRDs) to identify blind spots, edge cases, and stakeholder misalignments **before** they derail your sprint.

![Spec-Check Preview](https://via.placeholder.com/800x450/0a0e17/4a9eff?text=Spec-Check+Preview)

---

## 📦 Two Versions Included

### 1. **Demo Version** (`spec-check-assistant.html`)
**USE THIS FOR:** Portfolio demos, interviews, GitHub Pages hosting

✅ **Features:**
- Smart keyword-based mock analysis
- Instant results (no API needed)
- Works offline
- Free forever
- Perfect for showcasing your product thinking

🎯 **Best for:** Sharing with hiring managers, adding to your portfolio site

---

### 2. **Personal API Version** (`spec-check-assistant-api.html`)
**USE THIS FOR:** Your actual PM work with your own Claude API credits

✅ **Features:**
- Real Claude Sonnet 4 analysis
- Genuinely intelligent insights
- Your API key stored locally
- ~$0.003 per analysis (300+ PRDs for $1)
- Production-quality feedback

🎯 **Best for:** Your daily work analyzing real PRDs

---

## 🚀 Quick Start

### Personal API Version (For Real Work)

1. **Get Your Claude API Key:**
   - Go to [console.anthropic.com](https://console.anthropic.com/)
   - Create an account or sign in
   - Navigate to API Keys → Create Key
   - Copy your key (starts with `sk-ant-api03-...`)

2. **Open the API Version:**
   - Open `spec-check-assistant-api.html` in your browser
   - Click "⚙️ API Key" in the header
   - Paste your API key
   - Click "Save API Key"

3. **Use It:**
   - Write or paste your PRD
   - Click "🔍 Analyze Document"
   - Get real AI insights in ~3-5 seconds

---

## 💡 Features

### ✨ Core Functionality
- **Readiness Radar Chart** - 5-axis visualization of PRD quality
- **Smart Insight Cards** - Color-coded by type (Edge Cases, Stakeholders, Metrics, Mental Models)
- **Real-time Scoring** - Overall readiness percentage
- **Interactive Filtering** - Click radar axes or use filter buttons
- **Export Reports** - Generate shareable HTML readiness reports

### 🎨 Design Highlights
- Dark, professional aesthetic
- Smooth animations and micro-interactions
- Responsive layout
- Production-grade UI polish

---

## 📊 How It Works

### Demo Version Analysis Logic
The demo version uses intelligent keyword detection:

**Edge Cases** trigger on:
- `checkout`, `payment`, `user`, `customer`
- Missing accessibility considerations

**Stakeholder Alerts** trigger on:
- `refund`, `ops`, `legal`, `privacy`, `data`
- Payment/auth integrations

**Metric Gaps** trigger on:
- Missing `failure metric`, `rollback` plan
- Weak success metrics

**Mental Models** trigger on:
- `assume`, `expect`, `quick`, `fast`
- Mobile without tablet/desktop specs

### API Version Analysis
Sends your PRD to Claude Sonnet 4 with this prompt structure:
```
You are a senior PM reviewing a PRD for:
1. Edge Cases - scenarios that might break
2. Stakeholder Alerts - teams to inform
3. Metric Gaps - missing success criteria
4. Mental Model Issues - assumptions to validate

[Your PRD]

Return JSON with structured insights
```

One API call = All insights returned at once.

---

## 💰 Cost Breakdown (API Version)

**Claude Sonnet 4 Pricing:**
- Input: $3 per million tokens
- Output: $15 per million tokens

**Example Analysis:**
- 500-word PRD = ~700 tokens
- Claude's response = ~800 tokens
- Total: ~1,500 tokens = **$0.003 per analysis**

**Bottom line:** You can analyze 300+ PRDs for $1.

---

## 🛠️ Technical Details

**Built with:**
- React 18 (via CDN)
- Chart.js (radar visualization)
- Vanilla CSS (no frameworks)
- localStorage (API key storage)

**Browser Support:**
- Chrome/Edge: ✅
- Firefox: ✅
- Safari: ✅

**File Size:**
- Demo version: ~35KB
- API version: ~38KB

---

## 🔐 Security Notes

### API Version
- Your API key is stored in browser localStorage
- Never sent anywhere except Anthropic's official API
- Not shared with any third parties
- Can be cleared anytime via browser dev tools

### Demo Version
- No external API calls
- No data storage
- 100% client-side JavaScript
- Works completely offline

---

## 🚧 Future Enhancements

Potential additions:
- [ ] Save/load PRD drafts
- [ ] Custom quality frameworks
- [ ] Integration with Notion/Confluence
- [ ] Team collaboration features
- [ ] Historical PRD comparison
- [ ] Slack/Teams export

---

## 📝 License

MIT License - Free for personal and commercial use

---

## 🤝 Contributing

This is a portfolio project, but if you have ideas:
1. Fork the repo
2. Make your changes
3. Submit a PR

---

## 📧 Contact

Built by [Your Name]
- Portfolio: [your-site.com]
- LinkedIn: [linkedin.com/in/yourname]
- Email: [your@email.com]

---

## 🙏 Acknowledgments

Built with:
- Claude (Anthropic) for AI analysis
- Chart.js for radar visualization
- Inspiration from real PM workflow pain points

---

**Questions?** Open an issue or reach out!
