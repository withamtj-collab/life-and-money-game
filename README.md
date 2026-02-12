# 💸 Life & Money — Financial Literacy Game

An interactive classroom game that teaches students about real financial decisions: education, careers, budgeting, home buying, investing, and retirement planning.

## Features

- **8 Education Paths** — from Ivy League ($280K debt) to Military/GI Bill ($0)
- **96 Career Options** — matched to student interests, with real salary data
- **Paycheck Anatomy** — interactive breakdown of taxes, deductions, take-home pay
- **Home Buying** — 10 real neighborhoods near Erlanger, KY with actual prices and tax rates
- **Mortgage Calculator** — adjustable down payment, interest rates, PMI, insurance
- **Investment Portfolio** — 6 asset classes with risk/return profiles and market simulation
- **Retirement Planning** — 40-year projection with 401(k), investments, Social Security
- **Life Events** — random financial surprises test emergency funds
- **Teacher Dashboard** — control pauses, market conditions, boost/penalize students

## Teacher Controls

- 🔓 **Pause Points** — lock/unlock 4 discussion gates throughout the game
- 📊 **Market Controls** — adjust stock returns and mortgage interest rates for all students
- ⚡ **Boost/Penalize** — give raises, adjust credit scores, add money, trigger events
- 🎲 **Quick Events** — pre-built templates for rewards and consequences
- 👨‍🎓 **Student Overview** — see all students' progress and financial snapshots

## Quick Start

```bash
npm install
npm run dev
```

Then open `http://localhost:5173` in your browser.

## Deploy for Classroom Use

### Netlify (free, easiest)
1. Push this repo to GitHub
2. Go to [netlify.com](https://netlify.com) → "Add new site" → "Import from Git"
3. Select this repo
4. Build command: `npm run build`
5. Publish directory: `dist`
6. Click Deploy — get a shareable URL for students

### Vercel (free alternative)
1. Go to [vercel.com](https://vercel.com) → "New Project" → Import from GitHub
2. It auto-detects Vite — just click Deploy

## Data Storage

Student progress and teacher settings are saved in `localStorage`. This means:
- Progress persists across browser refreshes and sessions
- Each student signs in with their name
- **Important**: Data is per-browser. If students switch devices, they start over unless you use the same browser.

For multi-device classroom use, consider deploying with a backend database (Firebase, Supabase, etc.).

## Built With

- React 18
- Vite
- No external UI libraries — pure inline styles

## Real Data Sources

- Erlanger, KY housing prices (2024-2025 market data)
- Kenton County property tax rates (~1.07% effective)
- Standard federal tax brackets (2024)
- Historical average investment returns
- Social Security benefit estimates

## License

MIT — Free for educational use.
