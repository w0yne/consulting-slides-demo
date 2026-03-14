---
theme: apple-basic
title: "Consulting Presentation Patterns — A Visual Reference Guide"
info: |
  A comprehensive visual reference of consulting presentation patterns used by McKinsey, BCG, and Bain
colorSchema: light
drawings:
  persist: false
transition: slide-left
mdc: true
---

<CoverSlide
  title="Consulting Presentation Patterns"
  subtitle="A Visual Reference Guide"
  tagline="McKinsey · BCG · Bain — The Complete Pattern Library"
/>

---

# Agenda

<CardGrid :columns="3">
  <AgendaCard number="1" title="Cover & Structure" description="Agenda, exec summary<br/>section dividers" />
  <AgendaCard number="2" title="Core Charts" description="Waterfall, bar, line<br/>combo, scatter" />
  <AgendaCard number="3" title="Advanced Charts" description="Marimekko, tornado<br/>Harvey balls, heatmap" />
  <AgendaCard number="4" title="Frameworks & Matrices" description="2×2, BCG, process<br/>pyramid, value chain" />
  <AgendaCard number="5" title="Comparison & Analysis" description="T-chart, timeline<br/>Gantt, decision tree" />
  <AgendaCard number="6" title="Storytelling & Special" description="Insight slides, case study<br/>KPI dashboard, risk" />
</CardGrid>

---

# Executive Summary

<SlideHeading title="" subtitle="Four key findings from our strategic assessment" />

<CardGrid variant="summary">
  <SummaryCard
    number="1"
    title="Revenue growth is decelerating — organic CAGR fell from 12% to 7%"
    description="Core business growth has slowed due to market saturation in the primary segment. Adjacent markets represent a $2.4B untapped opportunity requiring strategic investment."
  />
  <SummaryCard
    number="2"
    title="Operational margins can improve by 350bps through procurement optimization"
    description="Benchmarking reveals significant procurement inefficiency vs. peers. Consolidating suppliers and renegotiating contracts could yield $45M in annual savings."
  />
  <SummaryCard
    number="3"
    title="Digital channel penetration at 23% vs. industry benchmark of 45%"
    description="Accelerating digital adoption would reduce CAC by 30% and improve customer retention by 2.5x. Requires $15M investment over 18 months."
  />
  <SummaryCard
    number="4"
    title="M&A pipeline should prioritize two targets in adjacent verticals"
    description="Two acquisition candidates at 6-8x EBITDA multiples would add $180M revenue and provide cross-sell opportunities into the existing customer base."
  />
</CardGrid>

---
layout: section
---

<SectionDivider
  section="Section One"
  title="Core Charts"
  subtitle="The fundamental chart types used in every consulting engagement"
/>

---

# Revenue Bridge — Waterfall Chart

<SlideHeading subtitle="FY2024 revenue walk from $100M to $135M, showing key growth and decline drivers" />

<WaterfallChart
  :bars="[
    { label: 'FY23', sublabel: 'Base', value: '$100M', height: 200, color: '#0284c7', isTotal: true },
    { label: 'Volume', sublabel: 'Growth', value: '+$18M', height: 36, color: '#16a34a', offset: 120 },
    { label: 'Price', sublabel: 'Increase', value: '+$12M', height: 24, color: '#16a34a', offset: 156 },
    { label: 'New', sublabel: 'Products', value: '+$15M', height: 30, color: '#16a34a', offset: 180 },
    { label: 'Customer', sublabel: 'Churn', value: '−$5M', height: 10, color: '#ef4444', offset: 180 },
    { label: 'FX', sublabel: 'Impact', value: '−$5M', height: 10, color: '#ef4444', offset: 170 },
    { label: 'FY24', sublabel: 'Total', value: '$135M', height: 270, color: '#0284c7', isTotal: true }
  ]"
  :showCallout="true"
  calloutText="Net growth of +35% driven primarily by volume and new product launches"
/>

---

# Cost Build-Up — Waterfall Chart

<SlideHeading subtitle="Total cost structure breakdown showing cumulative build-up to $82M operating cost" />

<div style="display: flex; align-items: flex-end; justify-content: center; gap: 0.5rem; height: 260px; margin-top: 1rem;">
  <div style="text-align: center;">
    <div style="font-size: 0.7rem; font-weight: 600; margin-bottom: 0.3rem;">$32M</div>
    <div style="width: 80px; height: 102px; background: #0284c7; border-radius: 4px 4px 0 0;"></div>
    <div style="font-size: 0.65rem; color: #888; margin-top: 0.3rem;">Raw<br/>Materials</div>
  </div>
  <div style="text-align: center;">
    <div style="font-size: 0.7rem; font-weight: 600; margin-bottom: 0.3rem;">$22M</div>
    <div style="width: 80px; height: 172px; background: #7c3aed; border-radius: 4px 4px 0 0;"></div>
    <div style="font-size: 0.65rem; color: #888; margin-top: 0.3rem;">Labor</div>
  </div>
  <div style="text-align: center;">
    <div style="font-size: 0.7rem; font-weight: 600; margin-bottom: 0.3rem;">$12M</div>
    <div style="width: 80px; height: 210px; background: #d97706; border-radius: 4px 4px 0 0;"></div>
    <div style="font-size: 0.65rem; color: #888; margin-top: 0.3rem;">Overhead</div>
  </div>
  <div style="text-align: center;">
    <div style="font-size: 0.7rem; font-weight: 600; margin-bottom: 0.3rem;">$8M</div>
    <div style="width: 80px; height: 236px; background: #db2777; border-radius: 4px 4px 0 0;"></div>
    <div style="font-size: 0.65rem; color: #888; margin-top: 0.3rem;">SG&A</div>
  </div>
  <div style="text-align: center;">
    <div style="font-size: 0.7rem; font-weight: 600; margin-bottom: 0.3rem;">$8M</div>
    <div style="width: 80px; height: 260px; background: #16a34a; border-radius: 4px 4px 0 0;"></div>
    <div style="font-size: 0.65rem; color: #888; margin-top: 0.3rem;">R&D</div>
  </div>
</div>

<Legend :items="[
  { color: '#0284c7', label: 'Materials 39%' },
  { color: '#7c3aed', label: 'Labor 27%' },
  { color: '#d97706', label: 'Overhead 15%' },
  { color: '#db2777', label: 'SG&A 10%' },
  { color: '#16a34a', label: 'R&D 10%' }
]" />

---

# Market Composition — Stacked Bar Chart

<SlideHeading subtitle="Market share by segment across years showing shifting competitive dynamics" />

<StackedBarChart
  :bars="[
    { label: '2020', total: '$80B', segments: [{ value: 30, color: '#16a34a' }, { value: 42, color: '#d97706' }, { value: 48, color: '#0284c7' }, { value: 60, color: '#7c3aed' }] },
    { label: '2021', total: '$95B', segments: [{ value: 32, color: '#16a34a' }, { value: 43, color: '#d97706' }, { value: 57, color: '#0284c7' }, { value: 64, color: '#7c3aed' }] },
    { label: '2022', total: '$110B', segments: [{ value: 33, color: '#16a34a' }, { value: 41, color: '#d97706' }, { value: 66, color: '#0284c7' }, { value: 66, color: '#7c3aed' }] },
    { label: '2023', total: '$125B', segments: [{ value: 29, color: '#16a34a' }, { value: 38, color: '#d97706' }, { value: 75, color: '#0284c7' }, { value: 75, color: '#7c3aed' }] },
    { label: '2024E', total: '$140B', segments: [{ value: 26, color: '#16a34a' }, { value: 37, color: '#d97706' }, { value: 84, color: '#0284c7' }, { value: 84, color: '#7c3aed' }] }
  ]"
  :legend="[
    { label: 'Enterprise', color: '#7c3aed' },
    { label: 'Mid-Market', color: '#0284c7' },
    { label: 'SMB', color: '#d97706' },
    { label: 'Consumer', color: '#16a34a' }
  ]"
/>

---

# Segment Mix — 100% Stacked Bar

<SlideHeading subtitle="Revenue composition by channel showing digital acceleration trend" />

<StackedBarChart
  variant="percentage"
  :height="240"
  :barWidth="100"
  :bars="[
    { label: '2020', segments: [{ value: 12, color: '#16a34a', showLabel: true }, { value: 20, color: '#d97706', showLabel: true }, { value: 28, color: '#0284c7', showLabel: true }, { value: 40, color: '#7c3aed', showLabel: true }] },
    { label: '2022', segments: [{ value: 18, color: '#16a34a', showLabel: true }, { value: 22, color: '#d97706', showLabel: true }, { value: 28, color: '#0284c7', showLabel: true }, { value: 32, color: '#7c3aed', showLabel: true }] },
    { label: '2024E', segments: [{ value: 30, color: '#16a34a', showLabel: true }, { value: 22, color: '#d97706', showLabel: true }, { value: 25, color: '#0284c7', showLabel: true }, { value: 23, color: '#7c3aed', showLabel: true }] },
    { label: '2026E', segments: [{ value: 42, color: '#16a34a', showLabel: true }, { value: 20, color: '#d97706', showLabel: true }, { value: 23, color: '#0284c7', showLabel: true }, { value: 15, color: '#7c3aed', showLabel: true }] }
  ]"
  :legend="[
    { label: 'Retail Stores', color: '#7c3aed' },
    { label: 'Wholesale', color: '#0284c7' },
    { label: 'Marketplace', color: '#d97706' },
    { label: 'Direct Digital', color: '#16a34a' }
  ]"
/>

---

# Competitor Ranking — Horizontal Bar Chart

<SlideHeading subtitle="Market share by competitor (%), FY2024 — our client ranks #3 with room to grow" />

<HorizontalBarChart
  :bars="[
    { label: 'Alpha Corp', value: '28%', width: 82, color: '#0284c7' },
    { label: 'Beta Inc', value: '22%', width: 64, color: '#0284c7' },
    { label: 'Our Client', value: '18%', width: 53, color: '#d97706', highlight: true },
    { label: 'Gamma Ltd', value: '13%', width: 38, color: '#94a3b8' },
    { label: 'Delta SA', value: '10%', width: 29, color: '#94a3b8' },
    { label: 'Others', value: '9%', width: 26, color: '#cbd5e1' }
  ]"
/>

---

# Year-over-Year Performance — Grouped Bar Chart

<SlideHeading subtitle="Revenue ($M) by business unit, FY2023 vs FY2024 — showing strongest growth in Digital" />

<GroupedBarChart
  :groups="[
    { label: 'North', sublabel: 'America', bars: [{ value: '$45M', height: 180, color: '#94a3b8' }, { value: '$52M', height: 208, color: '#0284c7' }] },
    { label: 'Europe', bars: [{ value: '$28M', height: 112, color: '#94a3b8' }, { value: '$35M', height: 140, color: '#0284c7' }] },
    { label: 'APAC', bars: [{ value: '$15M', height: 60, color: '#94a3b8' }, { value: '$22M', height: 88, color: '#0284c7' }] },
    { label: 'Digital', bars: [{ value: '$12M', height: 48, color: '#94a3b8' }, { value: '$26M', height: 104, color: '#0284c7' }] }
  ]"
  :legend="[
    { label: 'FY2023', color: '#94a3b8' },
    { label: 'FY2024', color: '#0284c7' }
  ]"
  :highlights="[
    { text: 'Digital +117% YoY', color: '#16a34a', bgColor: '#f0fdf4' }
  ]"
/>

---

# Revenue Trend — Line Chart with CAGR

<SlideHeading subtitle="5-year revenue trajectory ($M) with compound annual growth rate annotation" />

<LineChart
  :points="[
    { x: 2, y: 40, value: '$82M' },
    { x: 22, y: 50, value: '$95M' },
    { x: 42, y: 58, value: '$108M' },
    { x: 62, y: 72, value: '$125M' },
    { x: 82, y: 88, value: '$145M' }
  ]"
  :labels="['2020', '2021', '2022', '2023', '2024E']"
  :annotation="{ title: 'CAGR', value: '15.3%', subtitle: '2020–2024' }"
/>

---

# Cumulative Growth — Area Chart

<SlideHeading subtitle="Cumulative customer acquisition (thousands) showing accelerating adoption curve" />

<AreaChart
  svgPath="M 30 240 Q 100 235, 150 220 Q 200 200, 250 170 Q 300 130, 350 80 Q 400 35, 470 15"
  fillPath="M 30 240 Q 100 235, 150 220 Q 200 200, 250 170 Q 300 130, 350 80 Q 400 35, 470 15 L 470 260 L 30 260 Z"
  :points="[
    { cx: 30, cy: 240 },
    { cx: 150, cy: 220 },
    { cx: 250, cy: 170 },
    { cx: 350, cy: 80 },
    { cx: 470, cy: 15 }
  ]"
  :labels="['Q1 23', 'Q2 23', 'Q3 23', 'Q4 23', 'Q1 24']"
  :valueLabels="[
    { x: '4%', y: '8%', value: '5K' },
    { x: '27%', y: '18%', value: '15K' },
    { x: '48%', y: '38%', value: '35K' },
    { x: '67%', y: '70%', value: '68K' },
    { x: '93%', top: '2%', value: '95K' }
  ]"
  :gridLabels="[
    { y: '25%', label: '25K' },
    { y: '50%', label: '50K' },
    { y: '75%', label: '75K' }
  ]"
/>

---

# Revenue vs. Margin — Combo Chart

<SlideHeading subtitle="Revenue ($M, bars) and EBITDA margin (%, line) showing improving profitability" />

<ComboChart
  :bars="[
    { value: '$82M', height: 140 },
    { value: '$95M', height: 162 },
    { value: '$108M', height: 184 },
    { value: '$125M', height: 214 },
    { value: '$145M', height: 248 }
  ]"
  linePath="M 50 200 L 150 175 L 250 145 L 350 110 L 450 75"
  :linePoints="[
    { cx: 50, cy: 200, label: '18%' },
    { cx: 150, cy: 175, label: '21%' },
    { cx: 250, cy: 145, label: '24%' },
    { cx: 350, cy: 110, label: '27%' },
    { cx: 450, cy: 75, label: '31%' }
  ]"
  :labels="['2020', '2021', '2022', '2023', '2024E']"
  :legend="[
    { label: 'Revenue ($M)', color: '#0284c7', type: 'bar' },
    { label: 'EBITDA Margin (%)', color: '#ef4444', type: 'line' }
  ]"
/>

---

# Market Positioning — Scatter Plot with Quadrants

<SlideHeading subtitle="Competitive landscape: Market share vs. growth rate with bubble size = revenue" />

<ScatterQuadrant
  :quadrants="[
    { position: 'top-left', label: 'Low Share / High Growth', style: 'italic' },
    { position: 'top-right', label: 'Stars ★', color: '#16a34a', fontWeight: 500 },
    { position: 'bottom-left', label: 'Dogs', color: '#ef4444' },
    { position: 'bottom-right', label: 'Cash Cows', style: 'italic' }
  ]"
  :bubbles="[
    { x: '82%', y: '18%', size: 60, label: 'Alpha', color: '#0284c7' },
    { x: '32%', y: '28%', size: 50, label: 'Client', color: '#d97706' },
    { x: '78%', y: '75%', size: 55, label: 'Beta', color: '#6b7280' },
    { x: '15%', y: '15%', size: 40, label: 'NewCo', color: '#16a34a' },
    { x: '18%', y: '80%', size: 35, label: 'Delta', color: '#ef4444' }
  ]"
  xAxisLabel="Market Share →"
  yAxisLabel="Growth Rate →"
/>

---
layout: section
---

<SectionDivider
  section="Section Three"
  title="Advanced Charts"
  subtitle="Specialized visualizations for deeper analysis"
/>

---

# Market Landscape — Marimekko Chart

<SlideHeading subtitle="Market size by region (width) and segment share (height) — column width proportional to market size" />

<MarimekkoChart
  :columns="[
    { width: '40%', label: 'North America ($56B)', segments: [
      { flex: 35, color: '#0284c7', label: 'Enterprise 35%' },
      { flex: 40, color: '#60a5fa', label: 'Mid-Market 40%' },
      { flex: 25, color: '#93c5fd', label: 'SMB 25%', labelColor: '#1e40af' }
    ]},
    { width: '30%', label: 'Europe ($42B)', segments: [
      { flex: 50, color: '#d97706', label: 'Enterprise 50%' },
      { flex: 30, color: '#fbbf24', label: 'Mid-Mkt 30%', labelColor: '#78350f' },
      { flex: 20, color: '#fde68a', label: 'SMB 20%', labelColor: '#78350f' }
    ]},
    { width: '20%', label: 'APAC ($28B)', segments: [
      { flex: 20, color: '#16a34a', label: 'Ent 20%' },
      { flex: 35, color: '#4ade80', label: 'Mid 35%', labelColor: '#14532d' },
      { flex: 45, color: '#bbf7d0', label: 'SMB 45%', labelColor: '#14532d' }
    ]},
    { width: '10%', label: 'RoW', segments: [
      { flex: 60, color: '#7c3aed', label: '' },
      { flex: 25, color: '#a78bfa', label: '' },
      { flex: 15, color: '#ddd6fe', label: '' }
    ]}
  ]"
/>

---

# Sensitivity Analysis — Tornado Chart

<SlideHeading subtitle="Impact of key assumptions on NPV ($M) — showing which variables matter most" />

<TornadoChart
  centerLabel="NPV = $120M"
  :rows="[
    { label: 'Revenue Growth', leftWidth: 70, leftValue: '−$35M', rightWidth: 65, rightValue: '+$32M' },
    { label: 'Discount Rate', leftWidth: 55, leftValue: '−$28M', rightWidth: 50, rightValue: '+$25M' },
    { label: 'Op. Margin', leftWidth: 40, leftValue: '−$20M', rightWidth: 38, rightValue: '+$19M' },
    { label: 'Market Share', leftWidth: 30, leftValue: '−$15M', rightWidth: 28, rightValue: '+$14M' },
    { label: 'CapEx', leftWidth: 18, leftValue: '−$9M', rightWidth: 16, rightValue: '+$8M' }
  ]"
/>

---

# Vendor Assessment — Harvey Balls Matrix

<SlideHeading subtitle="Capability comparison across five evaluation criteria — ● Full ◕ High ◑ Medium ◔ Low ○ None" />

<div style="margin: 1rem auto; max-width: 700px;">
  <table style="width: 100%; border-collapse: collapse; font-size: 0.8rem;">
    <thead>
      <tr style="border-bottom: 2px solid #111;">
        <th style="text-align: left; padding: 0.6rem 0.8rem; font-weight: 600;">Vendor</th>
        <th style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 600;">Scalability</th>
        <th style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 600;">Security</th>
        <th style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 600;">Cost</th>
        <th style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 600;">UX</th>
        <th style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 600;">Support</th>
        <th style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 600;">Overall</th>
      </tr>
    </thead>
    <tbody>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.6rem 0.8rem; font-weight: 500;">Vendor A</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">●</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">●</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◑</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◕</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">●</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 700; color: #16a34a;">★ Best</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.6rem 0.8rem; font-weight: 500;">Vendor B</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◕</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◕</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">●</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◑</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◕</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 500; color: #d97706;">Runner-up</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.6rem 0.8rem; font-weight: 500;">Vendor C</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◑</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">●</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◕</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">●</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◑</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 500; color: #888;">Adequate</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.6rem 0.8rem; font-weight: 500;">Vendor D</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◔</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◑</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">●</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◔</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◔</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 500; color: #ef4444;">Weak</td>
      </tr>
      <tr>
        <td style="padding: 0.6rem 0.8rem; font-weight: 500;">Vendor E</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◑</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◔</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◕</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">◑</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-size: 1.3rem;">○</td>
        <td style="text-align: center; padding: 0.6rem 0.5rem; font-weight: 500; color: #ef4444;">Not Rec.</td>
      </tr>
    </tbody>
  </table>
</div>

---

# Team Competency — Radar Chart

<SlideHeading subtitle="Skill assessment across six dimensions — current state vs. target state" />

<div style="display: flex; flex-direction: column; align-items: center;">
  <div style="position: relative; width: 300px; height: 300px;">
    <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); width: 60px; height: 60px; border: 1px solid #e5e7eb; border-radius: 50%;"></div>
    <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); width: 120px; height: 120px; border: 1px solid #e5e7eb; border-radius: 50%;"></div>
    <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); width: 180px; height: 180px; border: 1px solid #e5e7eb; border-radius: 50%;"></div>
    <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); width: 240px; height: 240px; border: 1px solid #e5e7eb; border-radius: 50%;"></div>
    <svg viewBox="0 0 300 300" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
      <polygon points="150,30 255,90 255,210 150,270 45,210 45,90" fill="rgba(2, 132, 199, 0.08)" stroke="#0284c7" stroke-width="2"/>
      <polygon points="150,55 230,100 230,200 150,245 70,200 70,100" fill="none" stroke="#ef4444" stroke-width="2" stroke-dasharray="6,3"/>
    </svg>
    <div style="position: absolute; top: -5px; left: 140px; font-size: 0.7rem; font-weight: 600; color: #333;">Strategy</div>
    <div style="position: absolute; top: 22%; right: -10px; font-size: 0.7rem; font-weight: 600; color: #333;">Analytics</div>
    <div style="position: absolute; bottom: 22%; right: -15px; font-size: 0.7rem; font-weight: 600; color: #333;">Technology</div>
    <div style="position: absolute; bottom: -5px; left: 130px; font-size: 0.7rem; font-weight: 600; color: #333;">Operations</div>
    <div style="position: absolute; bottom: 22%; left: -15px; font-size: 0.7rem; font-weight: 600; color: #333;">Leadership</div>
    <div style="position: absolute; top: 22%; left: -5px; font-size: 0.7rem; font-weight: 600; color: #333;">Innovation</div>
  </div>
  <div style="display: flex; justify-content: center; gap: 2rem; margin-top: 0.5rem;">
    <div style="display: flex; align-items: center; gap: 0.3rem;"><div style="width: 16px; height: 3px; background: #0284c7; border-radius: 2px;"></div><span style="font-size: 0.7rem; color: #888;">Target State</span></div>
    <div style="display: flex; align-items: center; gap: 0.3rem;"><div style="width: 16px; height: 3px; border: 2px dashed #ef4444; border-radius: 2px;"></div><span style="font-size: 0.7rem; color: #888;">Current State</span></div>
  </div>
</div>

---

# Performance Heat Map

<SlideHeading subtitle="Regional performance by metric — darker = stronger performance" />

<div style="margin: 1rem auto; max-width: 700px;">
  <table style="width: 100%; border-collapse: collapse; font-size: 0.78rem;">
    <thead>
      <tr style="border-bottom: 2px solid #111;">
        <th style="text-align: left; padding: 0.5rem 0.6rem; font-weight: 600;"></th>
        <th style="text-align: center; padding: 0.5rem 0.6rem; font-weight: 600;">Revenue<br/>Growth</th>
        <th style="text-align: center; padding: 0.5rem 0.6rem; font-weight: 600;">Margin</th>
        <th style="text-align: center; padding: 0.5rem 0.6rem; font-weight: 600;">Market<br/>Share</th>
        <th style="text-align: center; padding: 0.5rem 0.6rem; font-weight: 600;">NPS</th>
        <th style="text-align: center; padding: 0.5rem 0.6rem; font-weight: 600;">Employee<br/>Retention</th>
      </tr>
    </thead>
    <tbody>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.5rem 0.6rem; font-weight: 500;">North America</td>
        <td style="text-align: center; padding: 0.5rem; background: #15803d; color: white; font-weight: 600;">18%</td>
        <td style="text-align: center; padding: 0.5rem; background: #16a34a; color: white; font-weight: 600;">32%</td>
        <td style="text-align: center; padding: 0.5rem; background: #15803d; color: white; font-weight: 600;">28%</td>
        <td style="text-align: center; padding: 0.5rem; background: #22c55e; color: white; font-weight: 600;">72</td>
        <td style="text-align: center; padding: 0.5rem; background: #16a34a; color: white; font-weight: 600;">91%</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.5rem 0.6rem; font-weight: 500;">Europe</td>
        <td style="text-align: center; padding: 0.5rem; background: #22c55e; color: white; font-weight: 600;">12%</td>
        <td style="text-align: center; padding: 0.5rem; background: #86efac; color: #14532d; font-weight: 600;">24%</td>
        <td style="text-align: center; padding: 0.5rem; background: #22c55e; color: white; font-weight: 600;">22%</td>
        <td style="text-align: center; padding: 0.5rem; background: #15803d; color: white; font-weight: 600;">78</td>
        <td style="text-align: center; padding: 0.5rem; background: #86efac; color: #14532d; font-weight: 600;">85%</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.5rem 0.6rem; font-weight: 500;">APAC</td>
        <td style="text-align: center; padding: 0.5rem; background: #15803d; color: white; font-weight: 600;">25%</td>
        <td style="text-align: center; padding: 0.5rem; background: #fbbf24; color: #78350f; font-weight: 600;">15%</td>
        <td style="text-align: center; padding: 0.5rem; background: #fbbf24; color: #78350f; font-weight: 600;">12%</td>
        <td style="text-align: center; padding: 0.5rem; background: #22c55e; color: white; font-weight: 600;">65</td>
        <td style="text-align: center; padding: 0.5rem; background: #22c55e; color: white; font-weight: 600;">88%</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.5rem 0.6rem; font-weight: 500;">LatAm</td>
        <td style="text-align: center; padding: 0.5rem; background: #86efac; color: #14532d; font-weight: 600;">8%</td>
        <td style="text-align: center; padding: 0.5rem; background: #ef4444; color: white; font-weight: 600;">8%</td>
        <td style="text-align: center; padding: 0.5rem; background: #fbbf24; color: #78350f; font-weight: 600;">10%</td>
        <td style="text-align: center; padding: 0.5rem; background: #fbbf24; color: #78350f; font-weight: 600;">52</td>
        <td style="text-align: center; padding: 0.5rem; background: #ef4444; color: white; font-weight: 600;">72%</td>
      </tr>
      <tr>
        <td style="padding: 0.5rem 0.6rem; font-weight: 500;">MEA</td>
        <td style="text-align: center; padding: 0.5rem; background: #fbbf24; color: #78350f; font-weight: 600;">5%</td>
        <td style="text-align: center; padding: 0.5rem; background: #ef4444; color: white; font-weight: 600;">5%</td>
        <td style="text-align: center; padding: 0.5rem; background: #ef4444; color: white; font-weight: 600;">4%</td>
        <td style="text-align: center; padding: 0.5rem; background: #ef4444; color: white; font-weight: 600;">42</td>
        <td style="text-align: center; padding: 0.5rem; background: #fbbf24; color: #78350f; font-weight: 600;">78%</td>
      </tr>
    </tbody>
  </table>
</div>

<Legend :items="[
  { color: '#ef4444', label: 'Critical' },
  { color: '#fbbf24', label: 'Below Target' },
  { color: '#86efac', label: 'On Target' },
  { color: '#22c55e', label: 'Strong' },
  { color: '#15803d', label: 'Excellent' }
]" />

---

# KPI Status — Traffic Light Dashboard

<SlideHeading subtitle="Q4 2024 performance against targets — executive-level status at a glance" />

<div style="display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem; margin-top: 1.5rem;">
  <MetricCard status="green" title="Revenue" value="$135M" target="$130M" delta="+3.8% above target" />
  <MetricCard status="green" title="EBITDA Margin" value="28.5%" target="27%" delta="+1.5pp above target" />
  <MetricCard status="yellow" title="Customer NPS" value="62" target="70" delta="−11.4% below target" />
  <MetricCard status="red" title="Digital Adoption" value="23%" target="40%" delta="−42.5% below target" />
</div>

<div style="display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem; margin-top: 0.8rem;">
  <MetricCard status="green" title="Employee Retention" value="92%" target="90%" />
  <MetricCard status="yellow" title="Market Share" value="18.2%" target="20%" />
  <MetricCard status="green" title="Cash Flow" value="$42M" target="$38M" />
  <MetricCard status="red" title="Time to Market" value="14 mo" target="9 mo" />
</div>

---

# Progress Gauge — Speedometer

<SlideHeading subtitle="Digital transformation progress — overall program completion at 67%" />

<div style="display: flex; justify-content: center; gap: 3rem; margin-top: 2rem;">
  <GaugeChart :value="78" label="Phase 1: Foundation" sublabel="On Track" color="#16a34a" />
  <GaugeChart :value="52" label="Phase 2: Migration" sublabel="At Risk" color="#d97706" />
  <GaugeChart :value="15" label="Phase 3: Optimization" sublabel="Behind Schedule" color="#ef4444" />
</div>

<div style="text-align: center; margin-top: 2rem; padding: 0.8rem; background: #f8fafc; border-radius: 8px;">
  <span style="font-size: 0.85rem; font-weight: 500;">Overall Program: <strong style="color: #d97706;">67% Complete</strong> — Phase 2 requires executive intervention to meet Q2 deadline</span>
</div>

---

# Regional Comparison — Small Multiples

<SlideHeading subtitle="Quarterly revenue trend by region — same scale for easy comparison" />

<div style="display: grid; grid-template-columns: repeat(4, 1fr); gap: 1.2rem; margin-top: 1.5rem;">
  <SparklineCard
    title="North America"
    trend="↑ 15% YoY"
    trendColor="#16a34a"
    :bars="[
      { height: '55%', color: '#bae6fd' },
      { height: '62%', color: '#bae6fd' },
      { height: '70%', color: '#bae6fd' },
      { height: '78%', color: '#0284c7' },
      { height: '72%', color: '#bae6fd' },
      { height: '80%', color: '#bae6fd' },
      { height: '88%', color: '#bae6fd' },
      { height: '95%', color: '#0284c7' }
    ]"
  />
  <SparklineCard
    title="Europe"
    trend="↑ 8% YoY"
    trendColor="#16a34a"
    :bars="[
      { height: '50%', color: '#bae6fd' },
      { height: '48%', color: '#bae6fd' },
      { height: '55%', color: '#bae6fd' },
      { height: '58%', color: '#0284c7' },
      { height: '52%', color: '#bae6fd' },
      { height: '56%', color: '#bae6fd' },
      { height: '60%', color: '#bae6fd' },
      { height: '65%', color: '#0284c7' }
    ]"
  />
  <SparklineCard
    title="APAC"
    trend="↑ 28% YoY"
    trendColor="#16a34a"
    :bars="[
      { height: '30%', color: '#bae6fd' },
      { height: '38%', color: '#bae6fd' },
      { height: '45%', color: '#bae6fd' },
      { height: '52%', color: '#0284c7' },
      { height: '55%', color: '#bae6fd' },
      { height: '65%', color: '#bae6fd' },
      { height: '78%', color: '#bae6fd' },
      { height: '90%', color: '#0284c7' }
    ]"
  />
  <SparklineCard
    title="LatAm"
    trend="↓ 3% YoY"
    trendColor="#ef4444"
    :bars="[
      { height: '40%', color: '#bae6fd' },
      { height: '42%', color: '#bae6fd' },
      { height: '38%', color: '#bae6fd' },
      { height: '44%', color: '#0284c7' },
      { height: '40%', color: '#fca5a5' },
      { height: '36%', color: '#fca5a5' },
      { height: '38%', color: '#fca5a5' },
      { height: '35%', color: '#ef4444' }
    ]"
  />
</div>

---
layout: section
---

<SectionDivider
  section="Section Four"
  title="Frameworks & Matrices"
  subtitle="Classic consulting frameworks for strategic analysis"
/>

---

# Prioritization — 2×2 Matrix

<SlideHeading subtitle="Initiative prioritization by impact vs. effort — focus on Quick Wins and Major Projects" />

<Matrix2x2
  xAxisLabel="Effort →"
  yAxisLabel="Impact →"
  :cells="[
    { title: 'Quick Wins ★', subtitle: 'High Impact / Low Effort', color: '#16a34a', bgColor: '#f0fdf4', items: ['Pricing Optimization', 'Cross-sell Automation'], itemBorderColor: '#bbf7d0' },
    { title: 'Major Projects', subtitle: 'High Impact / High Effort', color: '#0284c7', bgColor: '#f0f9ff', items: ['Platform Migration', 'M&A Integration'], itemBorderColor: '#bae6fd' },
    { title: 'Fill-Ins', subtitle: 'Low Impact / Low Effort', color: '#d97706', bgColor: '#fef3c7', items: ['Office Redesign', 'Reporting Update'], itemBorderColor: '#fde68a' },
    { title: 'Thankless Tasks', subtitle: 'Low Impact / High Effort', color: '#ef4444', bgColor: '#fef2f2', items: ['Legacy Rewrite', 'Full ERP Swap'], itemBorderColor: '#fecaca' }
  ]"
/>

---

# Portfolio Strategy — BCG Growth-Share Matrix

<SlideHeading subtitle="Business unit portfolio classification — invest, hold, harvest, or divest" />

<Matrix2x2
  xAxisLabel="Relative Market Share →"
  yAxisLabel="Market Growth →"
  :cells="[
    { title: '❓ Question Marks', subtitle: 'High Growth / Low Share', color: '#d97706', bgColor: '#fef3c7' },
    { title: '★ Stars', subtitle: 'High Growth / High Share', color: '#16a34a', bgColor: '#f0fdf4' },
    { title: '🐕 Dogs', subtitle: 'Low Growth / Low Share', color: '#ef4444', bgColor: '#fef2f2' },
    { title: '🐄 Cash Cows', subtitle: 'Low Growth / High Share', color: '#0284c7', bgColor: '#f0f9ff' }
  ]"
/>

---

# Strategic Attractiveness — GE/McKinsey 9-Box

<SlideHeading subtitle="Business units mapped by industry attractiveness and competitive strength" />

<Matrix3x3
  :xAxisLabels="{ left: 'Strong', center: 'Competitive Strength →', right: 'Weak' }"
  :cells="[
    { label: 'INVEST', sublabel: 'Grow', color: 'white', sublabelColor: 'rgba(255,255,255,0.7)', bgColor: '#15803d' },
    { label: 'INVEST', sublabel: 'Grow', color: 'white', sublabelColor: 'rgba(255,255,255,0.7)', bgColor: '#16a34a' },
    { label: 'SELECTIVE', sublabel: 'Earn', color: '#78350f', sublabelColor: '#92400e', bgColor: '#fbbf24' },
    { label: 'INVEST', sublabel: 'Grow', color: 'white', sublabelColor: 'rgba(255,255,255,0.7)', bgColor: '#16a34a' },
    { label: 'SELECTIVE', sublabel: 'Earn', color: '#78350f', sublabelColor: '#92400e', bgColor: '#fbbf24' },
    { label: 'HARVEST', sublabel: 'Divest', color: 'white', sublabelColor: 'rgba(255,255,255,0.7)', bgColor: '#ef4444' },
    { label: 'SELECTIVE', sublabel: 'Earn', color: '#78350f', sublabelColor: '#92400e', bgColor: '#fbbf24' },
    { label: 'HARVEST', sublabel: 'Divest', color: 'white', sublabelColor: 'rgba(255,255,255,0.7)', bgColor: '#ef4444' },
    { label: 'DIVEST', sublabel: 'Exit', color: 'white', sublabelColor: 'rgba(255,255,255,0.7)', bgColor: '#991b1b' }
  ]"
/>

---

# Transformation Journey — Process Arrows

<SlideHeading subtitle="5-phase digital transformation roadmap with key milestones" />

<ProcessChevrons
  :steps="[
    { label: 'Phase 1', sublabel: 'Assess', detail: 'Wk 1-4', color: '#0c4a6e' },
    { label: 'Phase 2', sublabel: 'Design', detail: 'Wk 5-10', color: '#0369a1' },
    { label: 'Phase 3', sublabel: 'Build', detail: 'Wk 11-22', color: '#0284c7' },
    { label: 'Phase 4', sublabel: 'Deploy', detail: 'Wk 23-30', color: '#0ea5e9' },
    { label: 'Phase 5', sublabel: 'Optimize', detail: 'Ongoing', color: '#38bdf8', textColor: '#0c4a6e' }
  ]"
  :details="[
    { borderColor: '#0c4a6e', items: ['Current state analysis', 'Stakeholder interviews', 'Gap assessment'] },
    { borderColor: '#0369a1', items: ['Target operating model', 'Technology selection', 'Business case'] },
    { borderColor: '#0284c7', items: ['Agile development', 'Integration testing', 'Change management'] },
    { borderColor: '#0ea5e9', items: ['Pilot launch', 'User training', 'Full rollout'] },
    { borderColor: '#38bdf8', items: ['KPI monitoring', 'Continuous improvement', 'Scale & expand'] }
  ]"
/>

---

# Strategic Hierarchy — Pyramid

<SlideHeading subtitle="Three-layer strategic framework — vision cascades into execution" />

<Pyramid
  :levels="[
    { label: 'Vision', sublabel: 'Market leadership by 2027', width: '200px', color: '#0c4a6e' },
    { label: 'Strategy', sublabel: 'Digital-first · Adjacent markets · Operational excellence · Talent acquisition', width: '380px', color: '#0284c7' },
    { label: 'Execution', sublabel: 'Platform build · M&A pipeline · Procurement optimization · Hiring plan · KPI tracking', width: '560px', color: '#38bdf8', textColor: '#0c4a6e' }
  ]"
  :annotations="[
    { label: 'Why', sublabel: 'Purpose & Direction', color: '#0c4a6e' },
    { label: 'What', sublabel: 'Strategic Pillars', color: '#0284c7' },
    { label: 'How', sublabel: 'Initiatives & Actions', color: '#38bdf8' }
  ]"
/>

---

# Value Chain — Porter's Model

<SlideHeading subtitle="Primary and support activities with margin analysis" />

<ValueChain
  :supportActivities="[
    { label: 'Firm Infrastructure', sublabel: 'Finance, Legal, Planning', color: '#ede9fe' },
    { label: 'Human Resources', sublabel: 'Recruiting, Training', color: '#ede9fe' },
    { label: 'Technology Development', sublabel: 'R&D, IT Systems', color: '#ede9fe' },
    { label: 'Procurement', sublabel: 'Purchasing, Sourcing', color: '#ede9fe' }
  ]"
  :primaryActivities="[
    { label: 'Inbound Logistics', sublabel: 'Receiving, Warehousing', color: '#0284c7' },
    { label: 'Operations', sublabel: 'Manufacturing, Assembly', color: '#0369a1' },
    { label: 'Outbound Logistics', sublabel: 'Distribution, Delivery', color: '#0c4a6e' },
    { label: 'Marketing & Sales', sublabel: 'Advertising, Channels', color: '#0369a1' },
    { label: 'Service', sublabel: 'Support, Warranty', color: '#0284c7' }
  ]"
  marginValue="28%"
/>

---

# Innovation Horizons — Concentric Circles

<SlideHeading subtitle="Three horizons of growth — core, adjacent, and transformational" />

<ConcentricCircles
  :width="380"
  :height="380"
  :circles="[
    { label: 'Transformational', sublabel: '10% of R&D', size: 360, color: '#7c3aed', labelPosition: 'top' },
    { label: 'Adjacent', sublabel: '20% of R&D', size: 250, color: '#0284c7', labelPosition: 'top-right' },
    { label: 'Core', sublabel: '70% of R&D', size: 140, color: '#16a34a', textColor: '#16a34a' }
  ]"
/>

---

# Capability Maturity — 5-Level Model

<SlideHeading subtitle="Digital maturity assessment across functional areas — current state highlighted" />

<MaturityModel
  :levels="[
    { number: 1, sublabel: 'Initial' },
    { number: 2, sublabel: 'Developing' },
    { number: 3, sublabel: 'Defined' },
    { number: 4, sublabel: 'Managed' },
    { number: 5, sublabel: 'Optimized' }
  ]"
  :dimensions="[
    { label: 'Data & Analytics', currentLevel: 4, color: '#0284c7' },
    { label: 'Customer Exp.', currentLevel: 2, color: '#d97706' },
    { label: 'Operations', currentLevel: 3, color: '#16a34a' },
    { label: 'Technology', currentLevel: 5, color: '#16a34a' },
    { label: 'Culture', currentLevel: 1, color: '#ef4444' }
  ]"
/>

---

# Strategic Overlap — Venn Diagram

<SlideHeading subtitle="Finding the sweet spot at the intersection of market need, capability, and profitability" />

<VennDiagram
  :circles="[
    { label: 'Market Need', color: '#0284c7', size: 220, position: { top: '15%', left: '10%' }, labelPosition: { top: '18%', left: '15%' } },
    { label: 'Core Capability', color: '#16a34a', size: 220, position: { top: '15%', right: '10%' }, labelPosition: { top: '18%', right: '15%' } },
    { label: 'Profit Potential', color: '#d97706', size: 220, position: { bottom: '5%', left: '90px' }, labelPosition: { bottom: '8%', left: '160px' } }
  ]"
  centerLabel="Sweet Spot"
  :width="400"
  :height="350"
/>

---

# Growth Engine — Flywheel

<SlideHeading subtitle="Self-reinforcing growth loop, each element accelerates the next" />

<Flywheel :size="350" :items="[{ label: 'Better Product', color: '#0284c7' }, { label: 'More Users', color: '#0369a1' }, { label: 'More Data', color: '#0c4a6e' }, { label: 'Better Insights', color: '#0c4a6e' }, { label: 'More Revenue', color: '#0369a1' }, { label: 'More R&D', color: '#0284c7' }]" />

---
layout: section
---

<SectionDivider
  section="Section Five"
  title="Comparison & Analysis"
  subtitle="Side-by-side evaluation and planning tools"
/>

---

# Current vs. Future State — T-Chart

<SlideHeading subtitle="Operating model transformation — from siloed functions to integrated platform" />

<TChart
  leftTitle="Current State"
  rightTitle="Future State"
  :leftItems="[
    { text: 'Siloed data across 12 systems' },
    { text: 'Manual reporting — 5 day cycle' },
    { text: 'Reactive customer service' },
    { text: 'Waterfall development — 18mo cycles' },
    { text: 'On-premise infrastructure' }
  ]"
  :rightItems="[
    { text: 'Unified data platform — single source of truth' },
    { text: 'Real-time dashboards — self-serve analytics' },
    { text: 'Predictive engagement — AI-powered NPS' },
    { text: 'Agile squads — 2-week sprints' },
    { text: 'Cloud-native — auto-scaling multi-region' }
  ]"
/>

---

# Implementation Roadmap — Swim Lane Timeline

<SlideHeading subtitle="18-month transformation plan across four workstreams" />

<SwimLaneTimeline
  :periods="['Q1 25', 'Q2 25', 'Q3 25', 'Q4 25', 'Q1 26', 'Q2 26']"
  :lanes="[
    { label: 'Technology', color: '#0284c7', segments: [
      { span: 1, label: 'Platform Selection' },
      { span: 2, label: 'Core Development' },
      { span: 1, label: 'Testing' },
      { span: 2, label: 'Rollout & Optimization' }
    ]},
    { label: 'Process', color: '#16a34a', segments: [
      { span: 2, label: 'Process Mapping & Redesign' },
      { span: 2, label: 'Pilot & Iterate' },
      { span: 2, label: 'Full Implementation' }
    ]},
    { label: 'People', color: '#d97706', segments: [
      { span: 1, label: 'Assess' },
      { span: 2, label: 'Training Programs' },
      { span: 3, label: 'Change Management & Coaching' }
    ]},
    { label: 'Governance', color: '#7c3aed', segments: [
      { span: 1, label: 'Setup PMO' },
      { span: 5, label: 'Ongoing Monitoring, Reporting & Stakeholder Management' }
    ]}
  ]"
  :milestones="[
    { text: 'Key milestone: Q2 25 Pilot launch' },
    { text: 'Key milestone: Q4 25 Go-live' },
    { text: 'Key milestone: Q2 26 Full optimization' }
  ]"
/>

---

# Project Timeline — Gantt Chart

<SlideHeading subtitle="Detailed project plan with dependencies and critical path highlighted" />

<GanttChart
  :months="['J', 'F', 'M', 'A', 'M', 'J', 'J', 'A', 'S', 'O', 'N', 'D']"
  :tasks="[
    { label: 'Discovery & Planning', bars: [{ start: 0, span: 2, color: '#0284c7' }] },
    { label: 'Vendor Selection', bars: [{ start: 1, span: 2, color: '#0369a1' }] },
    { label: 'Core Development', critical: true, bars: [{ start: 3, span: 5, color: '#ef4444' }] },
    { label: 'Integration Testing', bars: [{ start: 8, span: 2, color: '#d97706' }] },
    { label: 'User Training', bars: [{ start: 9, span: 2, color: '#16a34a' }] },
    { label: 'Go-Live', critical: true, bars: [{ start: 11, span: 1, color: '#ef4444' }] }
  ]"
  :legend="[
    { label: 'Critical Path', color: '#ef4444' },
    { label: 'On Track', color: '#0284c7' },
    { label: 'Testing', color: '#d97706' },
    { label: 'Training', color: '#16a34a' }
  ]"
/>

---

# Decision Logic — Decision Tree

<SlideHeading subtitle="Market entry strategy decision framework — binary branching to recommended action" />

<DecisionTree
  rootQuestion="Market Size > $1B?"
  :branches="[
    {
      answer: 'Yes',
      answerColor: '#16a34a',
      question: 'Existing Capability?',
      outcomes: [
        { answer: 'Yes', answerColor: '#16a34a', label: 'Organic Entry ★', color: '#16a34a', bgColor: '#f0fdf4' },
        { answer: 'No', answerColor: '#ef4444', label: 'Acquire Target', color: '#0284c7', bgColor: '#f0f9ff' }
      ]
    },
    {
      answer: 'No',
      answerColor: '#ef4444',
      question: 'Niche with >30% margins?',
      outcomes: [
        { answer: 'Yes', answerColor: '#16a34a', label: 'Partnership / JV', color: '#d97706', bgColor: '#fef3c7' },
        { answer: 'No', answerColor: '#ef4444', label: 'Do Not Enter ✕', color: '#ef4444', bgColor: '#fef2f2' }
      ]
    }
  ]"
/>

---

# Tradeoff Analysis — Pros & Cons Table

<SlideHeading subtitle="Build vs. Buy vs. Partner evaluation for new platform capability" />

<ProsConsTable
  :options="[
    {
      title: 'Build',
      headerColor: '#0284c7',
      pros: ['Full customization', 'IP ownership', 'Long-term cost advantage', 'Deep integration'],
      cons: ['18-24 month timeline', '$8-12M investment', 'Talent acquisition risk', 'Ongoing maintenance']
    },
    {
      title: 'Buy',
      headerColor: '#16a34a',
      recommended: true,
      pros: ['Immediate capability', 'Proven technology', 'Vendor support', 'Faster time-to-market'],
      cons: ['$3-5M annual license', 'Vendor dependency', 'Limited customization', 'Integration complexity']
    },
    {
      title: 'Partner',
      headerColor: '#d97706',
      pros: ['Shared risk/investment', 'Market access', 'Complementary skills', 'Flexible structure'],
      cons: ['Alignment challenges', 'Shared economics', 'Governance overhead', 'Exit complexity']
    }
  ]"
/>

---

# Strategic Options — Scenario Comparison

<SlideHeading subtitle="Three strategic scenarios evaluated across key dimensions" />

<ScenarioTable
  :columns="[
    { title: 'Scenario A', subtitle: 'Conservative' },
    { title: 'Scenario B ★', subtitle: 'Balanced', recommended: true, color: '#16a34a' },
    { title: 'Scenario C', subtitle: 'Aggressive' }
  ]"
  :rows="[
    { label: 'Investment', values: [{ text: '$15M' }, { text: '$35M', highlight: true }, { text: '$60M' }] },
    { label: 'Revenue Uplift', values: [{ text: '+8%' }, { text: '+22%', highlight: true }, { text: '+35%' }] },
    { label: 'Payback Period', values: [{ text: '18 months' }, { text: '24 months', highlight: true }, { text: '36 months' }] },
    { label: 'Risk Level', values: [{ text: '● Low', color: '#16a34a' }, { text: '● Medium', color: '#d97706', highlight: true }, { text: '● High', color: '#ef4444' }] },
    { label: 'Market Position', values: [{ text: 'Maintain #3' }, { text: 'Reach #2', highlight: true }, { text: 'Challenge #1' }] },
    { label: 'NPV (5yr)', values: [{ text: '$22M' }, { text: '$68M', color: '#16a34a', highlight: true }, { text: '$85M' }] }
  ]"
  :footer="{ text: '★ Recommendation: Scenario B offers the best risk-adjusted return at 2.9x MOIC' }"
/>

---
layout: section
---

<SectionDivider
  section="Section Six"
  title="Storytelling & Special"
  subtitle="High-impact slides for executive communication"
/>

---

# The "So What?" — Key Insight Slide

<InsightSlide
  insight="Companies that invest in digital <strong>before</strong> market pressure forces them<br/>see <strong style='color: #0284c7;'>3.2× higher</strong> returns<br/>than reactive adopters."
  soWhat="So what? → Our client must accelerate digital investment by Q2 2025 to capture the proactive premium. Delay costs ~$12M in unrealized value per quarter."
/>

---

# Case Study — Client Transformation

<SlideHeading subtitle="Global manufacturing company — 18-month digital transformation" />

<TChart
  leftTitle="Before"
  rightTitle="After (18 months)"
  :leftItems="[
    { text: 'Revenue: $420M' },
    { text: 'EBITDA Margin: 18%' },
    { text: 'NPS: 32' },
    { text: 'Digital Revenue: 8%' },
    { text: 'Time to Market: 18 months' }
  ]"
  :rightItems="[
    { text: 'Revenue: $540M', highlight: '(+29%)' },
    { text: 'EBITDA Margin: 26%', highlight: '(+800bps)' },
    { text: 'NPS: 71', highlight: '(+39 pts)' },
    { text: 'Digital Revenue: 35%', highlight: '(+27pp)' },
    { text: 'Time to Market: 6 months', highlight: '(−67%)' }
  ]"
/>

<div style="text-align: center; margin-top: 1rem; padding: 0.6rem; background: #f8fafc; border-radius: 8px;">
  <span style="font-size: 0.8rem; font-weight: 500;">Investment: $35M over 18 months → ROI: <strong style="color: #16a34a;">3.4× in 3 years</strong></span>
</div>

---

# Financial Summary

<SlideHeading subtitle="5-year P&L projection under recommended scenario ($M)" />

<div style="margin: 0.8rem auto; max-width: 700px;">
  <table style="width: 100%; border-collapse: collapse; font-size: 0.75rem;">
    <thead>
      <tr style="border-bottom: 2px solid #111;">
        <th style="text-align: left; padding: 0.5rem 0.6rem; font-weight: 600;">Metric</th>
        <th style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 600; color: #888;">FY24A</th>
        <th style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 600;">FY25E</th>
        <th style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 600;">FY26E</th>
        <th style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 600;">FY27E</th>
        <th style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 600;">FY28E</th>
      </tr>
    </thead>
    <tbody>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.5rem 0.6rem; font-weight: 600;">Revenue</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #888;">135</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">158</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">185</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">212</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 600;">240</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.5rem 0.6rem; color: #888;">&nbsp;&nbsp;YoY Growth</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #888;">—</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #16a34a;">+17%</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #16a34a;">+17%</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #16a34a;">+15%</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #16a34a;">+13%</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.5rem 0.6rem;">Gross Profit</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #888;">78</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">95</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">115</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">136</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">158</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.5rem 0.6rem;">EBITDA</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #888;">38</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">48</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">60</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">72</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 600;">84</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb; background: #f8fafc;">
        <td style="padding: 0.5rem 0.6rem; font-weight: 600;">EBITDA Margin</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #888;">28%</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 500;">30%</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 500;">32%</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 500;">34%</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 600; color: #16a34a;">35%</td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 0.5rem 0.6rem;">Free Cash Flow</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #888;">25</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">18</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">35</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">52</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">65</td>
      </tr>
      <tr>
        <td style="padding: 0.5rem 0.6rem; font-weight: 600;">Cumulative FCF</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; color: #888;">25</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">43</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">78</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem;">130</td>
        <td style="text-align: right; padding: 0.5rem 0.6rem; font-weight: 600; color: #16a34a;">195</td>
      </tr>
    </tbody>
  </table>
</div>

---

# Risk Assessment — 5×5 Matrix

<SlideHeading subtitle="Project risks mapped by likelihood and impact — red zone requires immediate mitigation" />

<RiskMatrix
  :cells="[
    { color: '#fbbf24' }, { color: '#ef4444' }, { color: '#ef4444', label: 'R1', textColor: 'white' }, { color: '#991b1b' }, { color: '#991b1b' },
    { color: '#86efac' }, { color: '#fbbf24', label: 'R3', textColor: '#78350f' }, { color: '#ef4444' }, { color: '#ef4444', label: 'R2', textColor: 'white' }, { color: '#991b1b' },
    { color: '#86efac' }, { color: '#86efac' }, { color: '#fbbf24', label: 'R4', textColor: '#78350f' }, { color: '#ef4444' }, { color: '#ef4444' },
    { color: '#16a34a' }, { color: '#86efac' }, { color: '#86efac' }, { color: '#fbbf24' }, { color: '#ef4444' },
    { color: '#16a34a' }, { color: '#16a34a' }, { color: '#86efac', label: 'R5', textColor: '#14532d' }, { color: '#86efac' }, { color: '#fbbf24' }
  ]"
  :risks="[
    { id: 'R1', description: 'Talent attrition during transformation' },
    { id: 'R2', description: 'Technology vendor failure' },
    { id: 'R3', description: 'Budget overrun >20%' },
    { id: 'R4', description: 'Regulatory changes' },
    { id: 'R5', description: 'Competitor response' }
  ]"
/>

---

# Organization Structure — Org Chart

<SlideHeading subtitle="Proposed transformation office structure — dotted lines show matrix reporting" />

<OrgChart
  :root="{ title: 'CEO', color: '#111' }"
  :branches="[
    { title: 'CFO', color: '#0284c7', children: [{ label: 'Finance' }, { label: 'FP&A' }] },
    { title: 'COO', color: '#16a34a', children: [{ label: 'Operations' }, { label: 'Supply Chain' }] },
    { title: 'CTO', color: '#d97706', children: [{ label: 'Engineering' }, { label: 'Data' }] },
    { title: 'CMO', color: '#7c3aed', children: [{ label: 'Marketing' }, { label: 'Digital' }] }
  ]"
/>

---

# KPI Dashboard — Executive View

<SlideHeading subtitle="Real-time business health at a glance — March 2025" />

<div style="display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem; margin-top: 1rem;">
  <div style="padding: 1rem; border: 1px solid #e5e7eb; border-radius: 10px;">
    <div style="font-size: 0.7rem; color: #888; text-transform: uppercase; letter-spacing: 0.05em;">Revenue (MTD)</div>
    <div style="font-size: 1.5rem; font-weight: 700; margin: 0.3rem 0;">$12.4M</div>
    <div style="font-size: 0.7rem; color: #16a34a; font-weight: 500;">↑ 12% vs. plan</div>
    <div style="margin-top: 0.5rem; display: flex; align-items: flex-end; gap: 2px; height: 30px;">
      <div style="flex: 1; height: 50%; background: #bae6fd; border-radius: 2px;"></div>
      <div style="flex: 1; height: 65%; background: #bae6fd; border-radius: 2px;"></div>
      <div style="flex: 1; height: 55%; background: #bae6fd; border-radius: 2px;"></div>
      <div style="flex: 1; height: 70%; background: #bae6fd; border-radius: 2px;"></div>
      <div style="flex: 1; height: 80%; background: #bae6fd; border-radius: 2px;"></div>
      <div style="flex: 1; height: 75%; background: #bae6fd; border-radius: 2px;"></div>
      <div style="flex: 1; height: 90%; background: #0284c7; border-radius: 2px;"></div>
    </div>
  </div>
  <div style="padding: 1rem; border: 1px solid #e5e7eb; border-radius: 10px;">
    <div style="font-size: 0.7rem; color: #888; text-transform: uppercase; letter-spacing: 0.05em;">Gross Margin</div>
    <div style="font-size: 1.5rem; font-weight: 700; margin: 0.3rem 0;">62.3%</div>
    <div style="font-size: 0.7rem; color: #16a34a; font-weight: 500;">↑ 2.1pp YoY</div>
    <div style="margin-top: 0.5rem; height: 30px; background: #f1f5f9; border-radius: 4px; overflow: hidden;">
      <div style="width: 62.3%; height: 100%; background: #16a34a; border-radius: 4px;"></div>
    </div>
  </div>
  <div style="padding: 1rem; border: 1px solid #e5e7eb; border-radius: 10px;">
    <div style="font-size: 0.7rem; color: #888; text-transform: uppercase; letter-spacing: 0.05em;">Active Customers</div>
    <div style="font-size: 1.5rem; font-weight: 700; margin: 0.3rem 0;">8,420</div>
    <div style="font-size: 0.7rem; color: #16a34a; font-weight: 500;">↑ 340 net new</div>
    <div style="margin-top: 0.5rem; display: flex; align-items: flex-end; gap: 2px; height: 30px;">
      <div style="flex: 1; height: 40%; background: #bbf7d0; border-radius: 2px;"></div>
      <div style="flex: 1; height: 50%; background: #bbf7d0; border-radius: 2px;"></div>
      <div style="flex: 1; height: 45%; background: #bbf7d0; border-radius: 2px;"></div>
      <div style="flex: 1; height: 60%; background: #bbf7d0; border-radius: 2px;"></div>
      <div style="flex: 1; height: 70%; background: #bbf7d0; border-radius: 2px;"></div>
      <div style="flex: 1; height: 75%; background: #bbf7d0; border-radius: 2px;"></div>
      <div style="flex: 1; height: 90%; background: #16a34a; border-radius: 2px;"></div>
    </div>
  </div>
  <div style="padding: 1rem; border: 1px solid #e5e7eb; border-radius: 10px;">
    <div style="font-size: 0.7rem; color: #888; text-transform: uppercase; letter-spacing: 0.05em;">Churn Rate</div>
    <div style="font-size: 1.5rem; font-weight: 700; margin: 0.3rem 0;">2.1%</div>
    <div style="font-size: 0.7rem; color: #ef4444; font-weight: 500;">↑ 0.3pp vs. target</div>
    <div style="margin-top: 0.5rem; display: flex; align-items: flex-end; gap: 2px; height: 30px;">
      <div style="flex: 1; height: 30%; background: #fecaca; border-radius: 2px;"></div>
      <div style="flex: 1; height: 35%; background: #fecaca; border-radius: 2px;"></div>
      <div style="flex: 1; height: 40%; background: #fecaca; border-radius: 2px;"></div>
      <div style="flex: 1; height: 45%; background: #fecaca; border-radius: 2px;"></div>
      <div style="flex: 1; height: 50%; background: #fecaca; border-radius: 2px;"></div>
      <div style="flex: 1; height: 55%; background: #fecaca; border-radius: 2px;"></div>
      <div style="flex: 1; height: 65%; background: #ef4444; border-radius: 2px;"></div>
    </div>
  </div>
</div>

---

# Thank You

<CoverSlide
  variant="thank-you"
  title="Thank you for your time."
  subtitle="Questions, discussion, and next steps"
>
  <StatHighlight
    :stats="[
      { value: '46', label: 'Slide patterns' },
      { value: '6', label: 'Categories' },
      { value: 'MBB', label: 'Inspired' }
    ]"
  />
  <div style="margin-top: 3rem; font-size: 0.85rem; color: #999;">
    Consulting Presentation Patterns — A Visual Reference Guide
  </div>
</CoverSlide>

---

# Appendix

<SlideHeading subtitle="Supporting data, methodology notes, and additional analysis" />

<div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.2rem; margin-top: 1rem;">
  <div style="padding: 1.2rem; border: 1px solid #e5e7eb; border-radius: 10px;">
    <div style="font-size: 0.75rem; color: #999; text-transform: uppercase; letter-spacing: 0.1em;">Data Sources</div>
    <div style="font-size: 0.75rem; color: #666; margin-top: 0.5rem; line-height: 1.6;">
      Company financials (10-K filings)<br/>
      Industry reports (Gartner, IDC)<br/>
      Expert interviews (n=24)<br/>
      Customer surveys (n=1,200)
    </div>
  </div>
  <div style="padding: 1.2rem; border: 1px solid #e5e7eb; border-radius: 10px;">
    <div style="font-size: 0.75rem; color: #999; text-transform: uppercase; letter-spacing: 0.1em;">Methodology</div>
    <div style="font-size: 0.75rem; color: #666; margin-top: 0.5rem; line-height: 1.6;">
      DCF analysis (WACC: 9.5%)<br/>
      Monte Carlo simulation<br/>
      Benchmarking vs. top quartile<br/>
      Sensitivity on 5 key drivers
    </div>
  </div>
  <div style="padding: 1.2rem; border: 1px solid #e5e7eb; border-radius: 10px;">
    <div style="font-size: 0.75rem; color: #999; text-transform: uppercase; letter-spacing: 0.1em;">Key Assumptions</div>
    <div style="font-size: 0.75rem; color: #666; margin-top: 0.5rem; line-height: 1.6;">
      Market CAGR: 8-12%<br/>
      Terminal growth: 3%<br/>
      Tax rate: 25%<br/>
      Implementation: 18 months
    </div>
  </div>
</div>

<div style="margin-top: 1.5rem; padding: 0.8rem 1.2rem; border: 1px solid #e5e7eb; border-radius: 8px; background: #f8fafc;">
  <div style="font-size: 0.75rem; color: #888;">
    <strong>Disclaimer:</strong> This document contains forward-looking statements and projections based on current assumptions. Actual results may differ materially. All financial figures are illustrative and for reference purposes only.
  </div>
</div>

<style>
:root {
  --slidev-slide-container-background: #f1f5f9;
}
#slide-container {
  background: #f1f5f9 !important;
}
</style>
