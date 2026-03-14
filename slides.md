---
theme: seriph
title: Consulting Presentation Patterns
info: A visual reference guide to McKinsey/BCG/Bain-style slide patterns
class: text-center
drawings:
  persist: false
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Consulting Presentation Patterns

### A Visual Reference Guide

<div class="abs-br m-6 text-sm opacity-50">
McKinsey / BCG / Bain Style Templates
</div>

<style>
h1 {
  color: #1B3A5C !important;
  font-weight: 700;
}
h3 {
  color: #2E86AB;
}
</style>

---
layout: default
---

# Key findings indicate three strategic priorities to capture $35M incremental revenue

<div class="grid grid-cols-1 gap-4 mt-6">

<div class="flex items-start gap-3 p-4 rounded-lg" style="background: #f0f7fa; border-left: 4px solid #2E86AB;">
  <div class="text-2xl font-bold" style="color: #E85D04;">1</div>
  <div>
    <div class="font-bold" style="color: #1B3A5C;">Expand into adjacent market segments to unlock $18M in untapped demand</div>
    <div class="text-sm mt-1 opacity-70">Current penetration is only 12% in SMB segment vs. 45% in enterprise</div>
  </div>
</div>

<div class="flex items-start gap-3 p-4 rounded-lg" style="background: #f0f7fa; border-left: 4px solid #2E86AB;">
  <div class="text-2xl font-bold" style="color: #E85D04;">2</div>
  <div>
    <div class="font-bold" style="color: #1B3A5C;">Optimize pricing architecture to capture $10M through value-based tiers</div>
    <div class="text-sm mt-1 opacity-70">Benchmarking shows 15-20% pricing gap vs. comparable solutions</div>
  </div>
</div>

<div class="flex items-start gap-3 p-4 rounded-lg" style="background: #f0f7fa; border-left: 4px solid #2E86AB;">
  <div class="text-2xl font-bold" style="color: #E85D04;">3</div>
  <div>
    <div class="font-bold" style="color: #1B3A5C;">Reduce churn by 3pp through dedicated customer success investment ($7M impact)</div>
    <div class="text-sm mt-1 opacity-70">Top-quartile peers achieve 95% retention vs. our current 88%</div>
  </div>
</div>

</div>

<div class="abs-bl m-4 text-xs opacity-40">EXECUTIVE SUMMARY</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
</style>

---
layout: section
---

# Strategic Growth Analysis

<div style="color: #2E86AB; font-size: 1.2rem;">Revenue Drivers & Market Opportunity</div>

<style>
h1 { color: #1B3A5C !important; }
</style>

---
layout: default
---

# Revenue grew from $100M to $135M, driven primarily by new products and geographic expansion

<div class="waterfall-chart mt-4">
  <div class="bar-group">
    <div class="bar-container">
      <div class="bar base" style="height: 250px;">
        <span class="bar-label">$100M</span>
      </div>
      <div class="bar-title">FY22<br>Revenue</div>
    </div>
    <div class="bar-container">
      <div class="spacer" style="height: 250px;"></div>
      <div class="bar positive" style="height: 50px;">
        <span class="bar-label">+$20M</span>
      </div>
      <div class="bar-title">New<br>Products</div>
    </div>
    <div class="bar-container">
      <div class="spacer" style="height: 300px;"></div>
      <div class="bar positive" style="height: 37px;">
        <span class="bar-label">+$15M</span>
      </div>
      <div class="bar-title">Geo<br>Expansion</div>
    </div>
    <div class="bar-container">
      <div class="spacer" style="height: 337px;"></div>
      <div class="bar positive" style="height: 20px;">
        <span class="bar-label">+$8M</span>
      </div>
      <div class="bar-title">Price<br>Increase</div>
    </div>
    <div class="bar-container">
      <div class="spacer" style="height: 345px;"></div>
      <div class="bar negative" style="height: 20px;">
        <span class="bar-label neg">−$8M</span>
      </div>
      <div class="bar-title">Lost<br>Clients</div>
    </div>
    <div class="bar-container">
      <div class="bar base end" style="height: 337px;">
        <span class="bar-label">$135M</span>
      </div>
      <div class="bar-title">FY23<br>Revenue</div>
    </div>
  </div>
  <div class="baseline"></div>
</div>

<div class="abs-bl m-4 text-xs opacity-40">Source: Company financials, FY22–FY23 actuals</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.waterfall-chart { position: relative; height: 380px; }
.bar-group {
  display: flex; align-items: flex-end; justify-content: center;
  height: 360px; gap: 18px; position: relative;
}
.bar-container { display: flex; flex-direction: column; align-items: center; width: 90px; }
.bar {
  position: relative; width: 70px; border-radius: 3px 3px 0 0;
  display: flex; align-items: center; justify-content: center;
}
.bar.base { background: #1B3A5C; }
.bar.base.end { background: #1B3A5C; }
.bar.positive { background: #2E86AB; }
.bar.negative { background: #E85D04; border-radius: 0 0 3px 3px; }
.spacer { width: 70px; }
.bar-label {
  color: white; font-weight: 700; font-size: 0.75rem; white-space: nowrap;
  position: absolute; top: -22px; color: #1B3A5C;
}
.bar-label.neg { color: #E85D04; }
.bar.base .bar-label, .bar.base.end .bar-label { top: 8px; color: white; }
.bar-title { font-size: 0.7rem; margin-top: 6px; text-align: center; color: #666; }
.baseline { position: absolute; bottom: 18px; left: 10%; right: 10%; border-bottom: 2px solid #ddd; }
</style>

---
layout: default
---

# Market composition shifted toward digital segments, now representing 45% of total

<div class="stacked-chart mt-6">
  <div class="chart-area">
    <div class="y-axis">
      <span>100%</span><span>75%</span><span>50%</span><span>25%</span><span>0%</span>
    </div>
    <div class="bars">
      <div class="stacked-bar">
        <div class="segment seg-d" style="height: 25%"><span>25%</span></div>
        <div class="segment seg-c" style="height: 15%"></div>
        <div class="segment seg-b" style="height: 25%"></div>
        <div class="segment seg-a" style="height: 35%"><span>35%</span></div>
        <div class="x-label">2020</div>
      </div>
      <div class="stacked-bar">
        <div class="segment seg-d" style="height: 30%"><span>30%</span></div>
        <div class="segment seg-c" style="height: 18%"></div>
        <div class="segment seg-b" style="height: 22%"></div>
        <div class="segment seg-a" style="height: 30%"><span>30%</span></div>
        <div class="x-label">2021</div>
      </div>
      <div class="stacked-bar">
        <div class="segment seg-d" style="height: 37%"><span>37%</span></div>
        <div class="segment seg-c" style="height: 18%"></div>
        <div class="segment seg-b" style="height: 20%"></div>
        <div class="segment seg-a" style="height: 25%"><span>25%</span></div>
        <div class="x-label">2022</div>
      </div>
      <div class="stacked-bar">
        <div class="segment seg-d" style="height: 45%"><span>45%</span></div>
        <div class="segment seg-c" style="height: 15%"></div>
        <div class="segment seg-b" style="height: 18%"></div>
        <div class="segment seg-a" style="height: 22%"><span>22%</span></div>
        <div class="x-label">2023</div>
      </div>
    </div>
  </div>
  <div class="legend">
    <span><i class="leg seg-d-bg"></i> Digital</span>
    <span><i class="leg seg-c-bg"></i> Services</span>
    <span><i class="leg seg-b-bg"></i> Hybrid</span>
    <span><i class="leg seg-a-bg"></i> Traditional</span>
  </div>
</div>

<div class="abs-bl m-4 text-xs opacity-40">Source: Industry reports, market sizing analysis 2020–2023</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.stacked-chart { display: flex; flex-direction: column; align-items: center; }
.chart-area { display: flex; height: 300px; width: 80%; }
.y-axis {
  display: flex; flex-direction: column; justify-content: space-between;
  font-size: 0.65rem; color: #8B8B8B; padding-right: 8px; text-align: right;
}
.bars { display: flex; flex: 1; justify-content: space-around; align-items: flex-end; border-left: 1px solid #ccc; border-bottom: 1px solid #ccc; padding: 0 20px; }
.stacked-bar { display: flex; flex-direction: column; width: 80px; position: relative; }
.segment { display: flex; align-items: center; justify-content: center; font-size: 0.65rem; font-weight: 600; color: white; }
.seg-a { background: #8B8B8B; }
.seg-b { background: #2E86AB; }
.seg-c { background: #E85D04; }
.seg-d { background: #1B3A5C; }
.x-label { font-size: 0.75rem; text-align: center; margin-top: 6px; color: #666; position: absolute; bottom: -22px; width: 100%; }
.legend { display: flex; gap: 20px; margin-top: 30px; font-size: 0.75rem; color: #555; }
.leg { display: inline-block; width: 12px; height: 12px; border-radius: 2px; margin-right: 4px; vertical-align: middle; }
.seg-d-bg { background: #1B3A5C; }
.seg-c-bg { background: #E85D04; }
.seg-b-bg { background: #2E86AB; }
.seg-a-bg { background: #8B8B8B; }
</style>

---
layout: default
---

# Company A leads on revenue but lags in customer satisfaction vs. key competitors

<div class="h-bar-chart mt-6">
  <div class="metric-group">
    <div class="metric-title">Revenue ($M)</div>
    <div class="h-bar"><span class="label">Company A</span><div class="fill" style="width: 85%; background: #1B3A5C;">$850M</div></div>
    <div class="h-bar"><span class="label">Company B</span><div class="fill" style="width: 72%; background: #2E86AB;">$720M</div></div>
    <div class="h-bar"><span class="label">Company C</span><div class="fill" style="width: 58%; background: #8B8B8B;">$580M</div></div>
    <div class="h-bar"><span class="label">Company D</span><div class="fill" style="width: 41%; background: #8B8B8B;">$410M</div></div>
  </div>
  <div class="metric-group mt-4">
    <div class="metric-title">Customer Satisfaction (NPS)</div>
    <div class="h-bar"><span class="label">Company A</span><div class="fill" style="width: 52%; background: #E85D04;">52</div></div>
    <div class="h-bar"><span class="label">Company B</span><div class="fill" style="width: 71%; background: #2E86AB;">71</div></div>
    <div class="h-bar"><span class="label">Company C</span><div class="fill" style="width: 68%; background: #2E86AB;">68</div></div>
    <div class="h-bar"><span class="label">Company D</span><div class="fill" style="width: 78%; background: #1B3A5C;">78</div></div>
  </div>
</div>

<div class="abs-bl m-4 text-xs opacity-40">Source: Public filings, proprietary NPS survey (n=2,400)</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.h-bar-chart { padding: 0 20px; }
.metric-group { margin-bottom: 8px; }
.metric-title { font-size: 0.8rem; font-weight: 700; color: #1B3A5C; margin-bottom: 6px; }
.h-bar { display: flex; align-items: center; margin-bottom: 5px; height: 28px; }
.h-bar .label { width: 100px; font-size: 0.7rem; color: #555; text-align: right; padding-right: 10px; flex-shrink: 0; }
.h-bar .fill {
  height: 100%; border-radius: 0 4px 4px 0; color: white;
  font-size: 0.7rem; font-weight: 600; display: flex; align-items: center;
  padding-left: 8px; transition: width 0.5s;
}
</style>

---
layout: default
---

# Digital adoption is accelerating while traditional channels plateau across all segments

```mermaid {theme: 'neutral', scale: 0.85}
xychart-beta
    title "Channel Performance Trends (2019–2023)"
    x-axis [2019, 2020, 2021, 2022, 2023]
    y-axis "Revenue ($M)" 0 --> 200
    line "Digital" [45, 68, 95, 140, 185]
    line "Hybrid" [60, 65, 72, 78, 82]
    line "Traditional" [120, 115, 108, 100, 95]
```

<div class="abs-bl m-4 text-xs opacity-40">Source: Internal channel reporting, FY19–FY23</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
</style>

---
layout: default
---

# Capability assessment reveals critical gaps in data analytics and AI/ML readiness

<div class="harvey-matrix mt-4">
<table>
  <thead>
    <tr>
      <th>Capability</th>
      <th>Company A</th>
      <th>Company B</th>
      <th>Company C</th>
      <th>Best-in-Class</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Cloud Infrastructure</td><td class="ball">●</td><td class="ball">◕</td><td class="ball">◑</td><td class="ball">●</td></tr>
    <tr><td>Data Analytics</td><td class="ball warn">◔</td><td class="ball">◕</td><td class="ball">●</td><td class="ball">●</td></tr>
    <tr><td>AI / ML</td><td class="ball warn">○</td><td class="ball">◑</td><td class="ball">◕</td><td class="ball">●</td></tr>
    <tr><td>Cybersecurity</td><td class="ball">◕</td><td class="ball">●</td><td class="ball">◑</td><td class="ball">●</td></tr>
    <tr><td>DevOps Maturity</td><td class="ball">◑</td><td class="ball">◕</td><td class="ball">◕</td><td class="ball">●</td></tr>
    <tr><td>Customer Platform</td><td class="ball">●</td><td class="ball">◑</td><td class="ball">◔</td><td class="ball">●</td></tr>
  </tbody>
</table>

<div class="scale mt-4">
  <span>● Full</span> <span>◕ Strong</span> <span>◑ Moderate</span> <span>◔ Weak</span> <span>○ None</span>
</div>
</div>

<div class="abs-bl m-4 text-xs opacity-40">Source: Capability maturity assessment, Q3 2023</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.harvey-matrix table { width: 90%; margin: 0 auto; border-collapse: collapse; font-size: 0.8rem; }
.harvey-matrix th { background: #1B3A5C; color: white; padding: 8px 12px; text-align: center; font-weight: 600; }
.harvey-matrix th:first-child { text-align: left; }
.harvey-matrix td { padding: 8px 12px; border-bottom: 1px solid #e5e5e5; }
.harvey-matrix td.ball { text-align: center; font-size: 1.4rem; color: #1B3A5C; }
.harvey-matrix td.ball.warn { color: #E85D04; }
.harvey-matrix tr:hover { background: #f8fafb; }
.scale { text-align: center; font-size: 0.75rem; color: #8B8B8B; display: flex; gap: 16px; justify-content: center; }
</style>

---
layout: default
---

# North America dominates market share but APAC is the fastest-growing region

<div class="marimekko mt-6">
  <div class="mekko-header">
    <span style="width: 40%">North America (40%)</span>
    <span style="width: 30%">Europe (30%)</span>
    <span style="width: 20%">APAC (20%)</span>
    <span style="width: 10%">RoW</span>
  </div>
  <div class="mekko-row">
    <div class="mekko-cell" style="width: 40%;">
      <div class="seg" style="height: 50%; background: #1B3A5C;"><span>Company A<br>50%</span></div>
      <div class="seg" style="height: 30%; background: #2E86AB;"><span>Company B<br>30%</span></div>
      <div class="seg" style="height: 20%; background: #8B8B8B;"><span>Others</span></div>
    </div>
    <div class="mekko-cell" style="width: 30%;">
      <div class="seg" style="height: 35%; background: #1B3A5C;"><span>Co. A 35%</span></div>
      <div class="seg" style="height: 40%; background: #2E86AB;"><span>Co. B 40%</span></div>
      <div class="seg" style="height: 25%; background: #8B8B8B;"><span>Others</span></div>
    </div>
    <div class="mekko-cell" style="width: 20%;">
      <div class="seg" style="height: 20%; background: #1B3A5C;"></div>
      <div class="seg" style="height: 25%; background: #2E86AB;"></div>
      <div class="seg" style="height: 55%; background: #E85D04;"><span>Local 55%</span></div>
    </div>
    <div class="mekko-cell" style="width: 10%;">
      <div class="seg" style="height: 15%; background: #1B3A5C;"></div>
      <div class="seg" style="height: 15%; background: #2E86AB;"></div>
      <div class="seg" style="height: 70%; background: #8B8B8B;"></div>
    </div>
  </div>
  <div class="mekko-legend mt-3">
    <span><i style="background:#1B3A5C"></i> Company A</span>
    <span><i style="background:#2E86AB"></i> Company B</span>
    <span><i style="background:#E85D04"></i> Local Players</span>
    <span><i style="background:#8B8B8B"></i> Others</span>
  </div>
</div>

<div class="abs-bl m-4 text-xs opacity-40">Source: Gartner market share data, 2023</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.marimekko { padding: 0 30px; }
.mekko-header { display: flex; font-size: 0.7rem; font-weight: 600; color: #1B3A5C; margin-bottom: 4px; text-align: center; }
.mekko-header span { text-align: center; }
.mekko-row { display: flex; height: 280px; gap: 2px; }
.mekko-cell { display: flex; flex-direction: column; }
.mekko-cell .seg {
  display: flex; align-items: center; justify-content: center;
  color: white; font-size: 0.6rem; font-weight: 600; text-align: center;
  border: 1px solid rgba(255,255,255,0.3);
}
.mekko-legend { display: flex; gap: 18px; font-size: 0.7rem; color: #555; justify-content: center; }
.mekko-legend i { display: inline-block; width: 10px; height: 10px; border-radius: 2px; margin-right: 4px; vertical-align: middle; }
</style>

---
layout: section
---

# Strategic Frameworks

<div style="color: #2E86AB; font-size: 1.2rem;">Analytical Tools & Decision Models</div>

<style>
h1 { color: #1B3A5C !important; }
</style>

---
layout: default
---

# Initiatives should be prioritized based on impact potential and implementation effort

<div class="matrix mt-2">
  <div class="y-label">IMPACT →</div>
  <div class="grid-container">
    <div class="quadrant q2">
      <div class="q-title">Quick Wins</div>
      <div class="q-desc">High Impact · Low Effort</div>
      <div class="bubble b1">Pricing<br>optimization</div>
      <div class="bubble b2">Cross-sell<br>program</div>
    </div>
    <div class="quadrant q1">
      <div class="q-title">Major Projects</div>
      <div class="q-desc">High Impact · High Effort</div>
      <div class="bubble b3">Digital<br>platform</div>
    </div>
    <div class="quadrant q3">
      <div class="q-title">Fill-ins</div>
      <div class="q-desc">Low Impact · Low Effort</div>
      <div class="bubble b4">Process<br>tweaks</div>
    </div>
    <div class="quadrant q4">
      <div class="q-title">Deprioritize</div>
      <div class="q-desc">Low Impact · High Effort</div>
      <div class="bubble b5">Legacy<br>migration</div>
    </div>
  </div>
  <div class="x-label">EFFORT →</div>
</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.matrix { position: relative; display: flex; flex-direction: column; align-items: center; }
.y-label { position: absolute; left: 30px; top: 50%; transform: rotate(-90deg) translateX(-50%); font-size: 0.7rem; font-weight: 700; color: #8B8B8B; letter-spacing: 2px; }
.x-label { font-size: 0.7rem; font-weight: 700; color: #8B8B8B; letter-spacing: 2px; margin-top: 8px; }
.grid-container { display: grid; grid-template-columns: 1fr 1fr; grid-template-rows: 1fr 1fr; width: 550px; height: 340px; gap: 2px; }
.quadrant { position: relative; padding: 16px; border-radius: 6px; }
.q1 { background: #f0f7fa; }
.q2 { background: #e8f5e9; }
.q3 { background: #fff8e1; }
.q4 { background: #fce4ec; }
.q-title { font-size: 0.85rem; font-weight: 700; color: #1B3A5C; }
.q-desc { font-size: 0.6rem; color: #8B8B8B; }
.bubble {
  position: absolute; border-radius: 50%; display: flex; align-items: center; justify-content: center;
  font-size: 0.55rem; font-weight: 600; color: white; text-align: center; line-height: 1.2;
}
.b1 { width: 70px; height: 70px; background: #2E86AB; bottom: 30px; left: 40px; }
.b2 { width: 55px; height: 55px; background: #2E86AB; bottom: 20px; right: 30px; }
.b3 { width: 80px; height: 80px; background: #1B3A5C; bottom: 40px; left: 60px; }
.b4 { width: 50px; height: 50px; background: #8B8B8B; top: 50px; left: 60px; }
.b5 { width: 60px; height: 60px; background: #E85D04; top: 50px; right: 40px; }
</style>

---
layout: default
---

# The transformation follows five sequential phases from assessment through sustained optimization

<div class="chevrons mt-12">
  <div class="chevron c1">
    <div class="c-num">01</div>
    <div class="c-title">Assess</div>
    <div class="c-desc">Baseline & diagnostics</div>
  </div>
  <div class="chevron c2">
    <div class="c-num">02</div>
    <div class="c-title">Design</div>
    <div class="c-desc">Solution architecture</div>
  </div>
  <div class="chevron c3">
    <div class="c-num">03</div>
    <div class="c-title">Pilot</div>
    <div class="c-desc">Test & validate</div>
  </div>
  <div class="chevron c4">
    <div class="c-num">04</div>
    <div class="c-title">Scale</div>
    <div class="c-desc">Full rollout</div>
  </div>
  <div class="chevron c5">
    <div class="c-num">05</div>
    <div class="c-title">Optimize</div>
    <div class="c-desc">Continuous improvement</div>
  </div>
</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.chevrons { display: flex; justify-content: center; gap: 6px; padding: 0 20px; }
.chevron {
  flex: 1; padding: 30px 20px 30px 35px; text-align: center; position: relative;
  clip-path: polygon(0 0, calc(100% - 20px) 0, 100% 50%, calc(100% - 20px) 100%, 0 100%, 20px 50%);
  color: white;
}
.chevron:first-child { clip-path: polygon(0 0, calc(100% - 20px) 0, 100% 50%, calc(100% - 20px) 100%, 0 100%); padding-left: 20px; }
.c1 { background: #1B3A5C; }
.c2 { background: #245578; }
.c3 { background: #2E86AB; }
.c4 { background: #E85D04; }
.c5 { background: #8B8B8B; }
.c-num { font-size: 0.65rem; opacity: 0.7; }
.c-title { font-size: 1rem; font-weight: 700; margin: 4px 0; }
.c-desc { font-size: 0.6rem; opacity: 0.8; }
</style>

---
layout: default
---

# Organizational value is built on three foundational layers, each enabling the next

<div class="pyramid-container mt-6">
  <div class="pyramid">
    <div class="layer layer-1">
      <div class="layer-content">
        <strong>Strategic Vision</strong>
        <span>Market leadership & innovation</span>
      </div>
    </div>
    <div class="layer layer-2">
      <div class="layer-content">
        <strong>Operational Excellence</strong>
        <span>Scalable processes, talent & technology</span>
      </div>
    </div>
    <div class="layer layer-3">
      <div class="layer-content">
        <strong>Foundation</strong>
        <span>Culture, governance & core infrastructure</span>
      </div>
    </div>
  </div>
</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.pyramid-container { display: flex; justify-content: center; }
.pyramid { display: flex; flex-direction: column; align-items: center; width: 600px; }
.layer {
  display: flex; align-items: center; justify-content: center; color: white; text-align: center;
  clip-path: polygon(15% 0%, 85% 0%, 95% 100%, 5% 100%);
}
.layer-1 { width: 45%; height: 100px; background: #1B3A5C; }
.layer-2 { width: 70%; height: 100px; background: #2E86AB; margin-top: -2px; }
.layer-3 { width: 95%; height: 100px; background: #8B8B8B; margin-top: -2px; }
.layer-content { padding: 10px; }
.layer-content strong { display: block; font-size: 0.9rem; }
.layer-content span { font-size: 0.65rem; opacity: 0.85; }
</style>

---
layout: default
---

# Implementation roadmap spans 18 months across three parallel workstreams

<div class="swimlane mt-4">
  <div class="lane">
    <div class="lane-label" style="background: #1B3A5C;">Technology</div>
    <div class="lane-track">
      <div class="task" style="left: 0%; width: 25%; background: #1B3A5C;">Platform selection</div>
      <div class="task" style="left: 28%; width: 35%; background: #1B3A5C;">Build & integrate</div>
      <div class="task" style="left: 66%; width: 34%; background: #1B3A5C; opacity: 0.7;">Optimize & scale</div>
    </div>
  </div>
  <div class="lane">
    <div class="lane-label" style="background: #2E86AB;">Process</div>
    <div class="lane-track">
      <div class="task" style="left: 0%; width: 20%; background: #2E86AB;">Map current state</div>
      <div class="task" style="left: 22%; width: 30%; background: #2E86AB;">Redesign</div>
      <div class="task" style="left: 55%; width: 45%; background: #2E86AB; opacity: 0.7;">Roll out & monitor</div>
    </div>
  </div>
  <div class="lane">
    <div class="lane-label" style="background: #E85D04;">People</div>
    <div class="lane-track">
      <div class="task" style="left: 5%; width: 22%; background: #E85D04;">Skills assessment</div>
      <div class="task" style="left: 30%; width: 40%; background: #E85D04;">Training program</div>
      <div class="task" style="left: 73%; width: 27%; background: #E85D04; opacity: 0.7;">Change mgmt</div>
    </div>
  </div>
  <div class="timeline">
    <span>Q1 2024</span><span>Q2 2024</span><span>Q3 2024</span><span>Q4 2024</span><span>Q1 2025</span><span>Q2 2025</span>
  </div>
  <div class="milestones">
    <div class="milestone" style="left: 25%;">▲ MVP</div>
    <div class="milestone" style="left: 55%;">▲ Pilot Complete</div>
    <div class="milestone" style="left: 90%;">▲ Full Deploy</div>
  </div>
</div>

<div class="abs-bl m-4 text-xs opacity-40">Source: Program management office, preliminary timeline</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.swimlane { padding: 0 30px; }
.lane { display: flex; margin-bottom: 12px; align-items: center; }
.lane-label {
  width: 100px; flex-shrink: 0; color: white; font-size: 0.7rem; font-weight: 700;
  padding: 8px; text-align: center; border-radius: 4px;
}
.lane-track { flex: 1; position: relative; height: 36px; margin-left: 10px; background: #f5f5f5; border-radius: 4px; }
.task {
  position: absolute; top: 4px; height: 28px; border-radius: 4px; color: white;
  font-size: 0.6rem; font-weight: 600; display: flex; align-items: center; padding: 0 8px;
  white-space: nowrap; overflow: hidden;
}
.timeline { display: flex; justify-content: space-between; margin-left: 110px; margin-top: 8px; font-size: 0.65rem; color: #8B8B8B; }
.milestones { position: relative; margin-left: 110px; height: 20px; margin-top: 4px; }
.milestone { position: absolute; font-size: 0.6rem; font-weight: 700; color: #E85D04; transform: translateX(-50%); }
</style>

---
layout: default
---

# Digital transformation will close performance gaps across five critical dimensions

<div class="comparison mt-4">
<table>
  <thead>
    <tr>
      <th>Dimension</th>
      <th>Current State</th>
      <th></th>
      <th>Future State</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="dim">Order Processing</td>
      <td class="current">Manual, 48hr cycle time</td>
      <td class="arrow">→</td>
      <td class="future">Automated, 4hr cycle time</td>
    </tr>
    <tr>
      <td class="dim">Data Analytics</td>
      <td class="current">Spreadsheet-based, monthly</td>
      <td class="arrow">→</td>
      <td class="future">Real-time dashboards, AI-driven</td>
    </tr>
    <tr>
      <td class="dim">Customer Experience</td>
      <td class="current">NPS 52, reactive support</td>
      <td class="arrow">→</td>
      <td class="future">NPS 75+, proactive engagement</td>
    </tr>
    <tr>
      <td class="dim">Supply Chain</td>
      <td class="current">3-week lead time, 85% OTIF</td>
      <td class="arrow">→</td>
      <td class="future">1-week lead time, 97% OTIF</td>
    </tr>
    <tr>
      <td class="dim">Cost Structure</td>
      <td class="current">SG&A at 28% of revenue</td>
      <td class="arrow">→</td>
      <td class="future">SG&A at 20% of revenue</td>
    </tr>
  </tbody>
</table>
</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.comparison table { width: 95%; margin: 0 auto; border-collapse: collapse; font-size: 0.78rem; }
.comparison th { background: #1B3A5C; color: white; padding: 10px 14px; text-align: left; }
.comparison td { padding: 12px 14px; border-bottom: 1px solid #e8e8e8; }
.comparison .dim { font-weight: 700; color: #1B3A5C; width: 150px; }
.comparison .current { color: #8B8B8B; background: #fafafa; }
.comparison .future { color: #2E86AB; font-weight: 600; background: #f0f7fa; }
.comparison .arrow { text-align: center; color: #E85D04; font-weight: 700; font-size: 1.1rem; width: 30px; }
.comparison tr:hover td { background: #f0f7fa; }
</style>

---
layout: default
---

# Decision framework determines optimal market entry approach based on two key criteria

<div class="tree mt-4">
  <div class="node root">Market Attractiveness<br>>$500M?</div>
  <div class="branches">
    <div class="branch left">
      <div class="edge-label yes">YES</div>
      <div class="node l1">Existing<br>Capabilities?</div>
      <div class="branches">
        <div class="branch left">
          <div class="edge-label yes">YES</div>
          <div class="node leaf go">Organic<br>Growth</div>
        </div>
        <div class="branch right">
          <div class="edge-label no">NO</div>
          <div class="node leaf go">Acquire /<br>Partner</div>
        </div>
      </div>
    </div>
    <div class="branch right">
      <div class="edge-label no">NO</div>
      <div class="node l1">Strategic<br>Fit?</div>
      <div class="branches">
        <div class="branch left">
          <div class="edge-label yes">YES</div>
          <div class="node leaf wait">Monitor &<br>Reassess</div>
        </div>
        <div class="branch right">
          <div class="edge-label no">NO</div>
          <div class="node leaf stop">Do Not<br>Enter</div>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.tree { display: flex; flex-direction: column; align-items: center; }
.node {
  padding: 12px 20px; border-radius: 8px; text-align: center;
  font-size: 0.75rem; font-weight: 600; line-height: 1.3;
}
.node.root { background: #1B3A5C; color: white; }
.node.l1 { background: #2E86AB; color: white; }
.node.leaf { padding: 10px 16px; font-size: 0.7rem; }
.node.leaf.go { background: #e8f5e9; color: #2e7d32; border: 2px solid #2e7d32; }
.node.leaf.wait { background: #fff8e1; color: #f57f17; border: 2px solid #f57f17; }
.node.leaf.stop { background: #fce4ec; color: #c62828; border: 2px solid #c62828; }
.branches { display: flex; gap: 40px; margin-top: 8px; justify-content: center; }
.branch { display: flex; flex-direction: column; align-items: center; }
.edge-label { font-size: 0.65rem; font-weight: 700; margin-bottom: 4px; }
.edge-label.yes { color: #2e7d32; }
.edge-label.no { color: #c62828; }
</style>

---
layout: section
---

# Signature Elements

<div style="color: #2E86AB; font-size: 1.2rem;">Callouts, Insights & Benchmark Patterns</div>

<style>
h1 { color: #1B3A5C !important; }
</style>

---
layout: default
---

# Customer acquisition cost decreased 32% YoY, outpacing the industry benchmark of 18%

<div class="callout-layout mt-6">
  <div class="metric-card main">
    <div class="metric-value">$127</div>
    <div class="metric-label">Customer Acquisition Cost</div>
    <div class="metric-delta positive">▼ 32% vs. prior year</div>
  </div>
  <div class="metric-card">
    <div class="metric-value small">$187</div>
    <div class="metric-label">Industry Average</div>
  </div>
  <div class="metric-card">
    <div class="metric-value small">3.2x</div>
    <div class="metric-label">LTV/CAC Ratio</div>
    <div class="metric-delta positive">vs. 2.1x target</div>
  </div>
  <div class="annotation">
    <div class="arrow">←</div>
    <div class="note">Driven by shift to digital channels<br>and improved conversion funnel (12% → 18%)</div>
  </div>
</div>

<div class="so-what">
  <strong>So what?</strong> The CAC improvement creates runway to invest $4M in growth while maintaining unit economics above target thresholds.
</div>

<div class="abs-bl m-4 text-xs opacity-40">Source: Marketing analytics, FY23 actuals vs. FY22</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.callout-layout { display: flex; gap: 20px; align-items: flex-start; padding: 0 20px; flex-wrap: wrap; }
.metric-card {
  background: #f8fafb; border-radius: 8px; padding: 20px 24px; text-align: center;
  border: 1px solid #e0e0e0;
}
.metric-card.main { border: 2px solid #2E86AB; background: #f0f7fa; }
.metric-value { font-size: 2.5rem; font-weight: 800; color: #1B3A5C; line-height: 1; }
.metric-value.small { font-size: 1.8rem; }
.metric-label { font-size: 0.7rem; color: #8B8B8B; margin-top: 4px; }
.metric-delta { font-size: 0.75rem; font-weight: 600; margin-top: 4px; }
.metric-delta.positive { color: #2e7d32; }
.annotation { display: flex; align-items: center; gap: 8px; margin-left: auto; }
.arrow { font-size: 2rem; color: #E85D04; }
.note { font-size: 0.7rem; color: #555; border-left: 3px solid #E85D04; padding-left: 10px; line-height: 1.5; }
.so-what {
  position: absolute; bottom: 50px; right: 40px; max-width: 400px;
  background: #fff8e1; border: 1px solid #E85D04; border-radius: 6px;
  padding: 12px 16px; font-size: 0.72rem; color: #333; line-height: 1.5;
}
.so-what strong { color: #E85D04; }
</style>

---
layout: default
---

# Current performance trails best-in-class benchmarks, with largest gap in digital maturity

<div class="ghost-chart mt-6">
  <div class="ghost-row">
    <div class="ghost-label">Revenue Growth</div>
    <div class="ghost-bars">
      <div class="ghost-bar benchmark" style="width: 80%;"><span class="bench-label">12%</span></div>
      <div class="ghost-bar actual" style="width: 58%;"><span>8.5%</span></div>
    </div>
  </div>
  <div class="ghost-row">
    <div class="ghost-label">EBITDA Margin</div>
    <div class="ghost-bars">
      <div class="ghost-bar benchmark" style="width: 72%;"><span class="bench-label">28%</span></div>
      <div class="ghost-bar actual" style="width: 60%;"><span>23%</span></div>
    </div>
  </div>
  <div class="ghost-row">
    <div class="ghost-label">Digital Revenue %</div>
    <div class="ghost-bars">
      <div class="ghost-bar benchmark" style="width: 90%;"><span class="bench-label">65%</span></div>
      <div class="ghost-bar actual" style="width: 45%;"><span>32%</span></div>
    </div>
    <div class="gap-callout">33pp gap</div>
  </div>
  <div class="ghost-row">
    <div class="ghost-label">Customer NPS</div>
    <div class="ghost-bars">
      <div class="ghost-bar benchmark" style="width: 85%;"><span class="bench-label">78</span></div>
      <div class="ghost-bar actual" style="width: 55%;"><span>52</span></div>
    </div>
  </div>
  <div class="ghost-row">
    <div class="ghost-label">Employee Engagement</div>
    <div class="ghost-bars">
      <div class="ghost-bar benchmark" style="width: 88%;"><span class="bench-label">82%</span></div>
      <div class="ghost-bar actual" style="width: 65%;"><span>61%</span></div>
    </div>
  </div>
  <div class="ghost-legend mt-4">
    <span><i class="gl actual-l"></i> Current</span>
    <span><i class="gl bench-l"></i> Best-in-class benchmark</span>
  </div>
</div>

<div class="so-what">
  <strong>So what?</strong> The 33pp digital revenue gap represents the single largest value creation lever — closing half this gap would add ~$50M in annual revenue.
</div>

<div class="abs-bl m-4 text-xs opacity-40">Source: McKinsey benchmarking database, peer group analysis 2023</div>

<style>
h1 { color: #1B3A5C !important; font-size: 1.15rem !important; line-height: 1.5 !important; }
.ghost-chart { padding: 0 30px; }
.ghost-row { display: flex; align-items: center; margin-bottom: 14px; }
.ghost-label { width: 150px; font-size: 0.75rem; font-weight: 600; color: #1B3A5C; text-align: right; padding-right: 12px; flex-shrink: 0; }
.ghost-bars { flex: 1; position: relative; height: 30px; }
.ghost-bar {
  position: absolute; top: 0; left: 0; height: 100%; border-radius: 4px;
  display: flex; align-items: center; font-size: 0.7rem; font-weight: 700;
}
.ghost-bar.benchmark {
  background: repeating-linear-gradient(90deg, #ddd 0px, #ddd 4px, transparent 4px, transparent 8px);
  border: 2px dashed #bbb; color: #999; justify-content: flex-end; padding-right: 8px;
}
.ghost-bar.actual { background: #2E86AB; color: white; padding-left: 10px; z-index: 1; }
.bench-label { font-size: 0.65rem; color: #999; }
.gap-callout {
  font-size: 0.7rem; font-weight: 700; color: #E85D04; margin-left: 8px;
  background: #fff3e0; padding: 2px 8px; border-radius: 4px; white-space: nowrap;
}
.ghost-legend { display: flex; gap: 20px; font-size: 0.7rem; color: #666; margin-left: 162px; }
.gl { display: inline-block; width: 20px; height: 10px; border-radius: 2px; margin-right: 4px; vertical-align: middle; }
.gl.actual-l { background: #2E86AB; }
.gl.bench-l { background: repeating-linear-gradient(90deg, #ccc 0px, #ccc 3px, transparent 3px, transparent 6px); border: 1px dashed #bbb; }
.so-what {
  position: absolute; bottom: 50px; right: 40px; max-width: 380px;
  background: #fff8e1; border: 1px solid #E85D04; border-radius: 6px;
  padding: 12px 16px; font-size: 0.72rem; color: #333; line-height: 1.5;
}
.so-what strong { color: #E85D04; }
</style>

---
layout: center
class: text-center
---

# Thank You

<div style="color: #2E86AB; font-size: 1.1rem; margin-top: 10px;">
Consulting Presentation Patterns — A Visual Reference Guide
</div>

<div style="margin-top: 30px; color: #8B8B8B; font-size: 0.8rem;">
These templates are designed to be reused and adapted.<br>
Fork this repo and make them your own.
</div>

<style>
h1 { color: #1B3A5C !important; font-size: 2.5rem !important; }
</style>
