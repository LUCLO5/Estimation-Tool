# Vaughn Construction Co. — Cost Estimator

Internal new-build cost estimation tool for Vaughn Construction Co., Waco, TX.

**This software is proprietary. See [LICENSE](LICENSE) for terms.**

---

## What It Does

Generates custom home build estimates based on actual cost data from 9 completed builds. Select square footage, estimate tier (Q1 / Median / Q3), and markup percentage to produce a full line-item cost breakdown by construction category.

## Data Source

All cost data is sourced from BuilderTrend Job Costing Budget actuals. Only cost codes appearing in 2 or more completed builds are included.

| Build | Sq Ft |
|-------|-------|
| Hammond | 3,186 |
| De La Pena | 2,074 |
| Ogles JR | 1,762 |
| Ogles SR | 1,316 |
| Heatherly | 5,189 |
| Martinez | 3,513 |
| Simcik | 2,535 |
| McAfee | 2,197 |
| Arscott | 2,778 |

**77 cost codes** across 17 categories. Median total: ~$194.96/sf.

## Deploy

### Netlify (easiest)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag this folder onto the page
3. Live in 30 seconds

### GitHub Pages
1. Push to GitHub
2. Settings → Pages → Source: main branch
3. Live at `https://[username].github.io/vaughn-estimator`

### Vercel
1. Connect GitHub repo at [vercel.com](https://vercel.com)
2. Import and deploy

## Updating Data

Edit the `D` array in `index.html`. Each entry:

```javascript
["Cost Code Name", avgPerSqFt, q1, median, q3, numberOfProjects, "Category"]
```

Recalculate from BuilderTrend actuals when new builds complete.

## Brand

- Navy: `#152c35`
- Powder: `#f7f6f2`
- Bronze: `#876a4b`
- Moss: `#7f7a5f`
- Fog: `#949d9d`
- Headings: Montserrat 500, uppercase, 3px letter-spacing
- Display: Cormorant Garamond (Proyale substitute)
- Body: Montserrat 400

## License

Proprietary. See [LICENSE](LICENSE). Unauthorized use prohibited. Custom builds available — contact howdy@vaughnwtx.com.
