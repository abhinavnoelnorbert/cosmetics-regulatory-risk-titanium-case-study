# KPI Validation (SQL)

This phase converts EDA insights into locked, dashboard-grade KPIs.
All metrics were validated directly in SQL against the Python-cleaned dataset, ensuring analytical parity and preventing downstream inconsistencies.

This phase establishes the single source of truth used for:

- Power BI modeling
- DAX calculations
- Dashboard KPIs
- Business storytelling

### Market Size KPIs

These represent the full scope of the California cosmetic chemical reporting market.

**KPIs & Value**
- Total regulated products:36,972
- Total unique chemicals:123
- Total companies:604
- Products containing Titanium dioxide:32,010
- Titanium market penetration:86.58%

**Interpretation**

The market is extremely concentrated:

- Only 123 chemicals drive the entire regulatory burden
- Titanium dioxide alone affects nearly 9 out of every 10 products

This indicates a single-chemical dependency risk rather than a fragmented hazard landscape.

### Category Risk KPIs

Titanium dioxide penetration was calculated for each product category.

**Category(Products): Titanium Penetration**
- Non-permanent Makeup (18,096):	96.46%
- Nail Products (6,920): 93.93%
- Oral Hygiene Products (383): 97.13%
- Tattoos & Permanent Makeup	(263): 99.62%
- Sun-Related Products(1,768): 87.39%
- Skin Care Products(5,184): 71.41%
- Bath Products(2,425): 69.53%
- Baby Products(46): 47.83%

**Interpretation**

Certain categories are structurally dependent on Titanium dioxide:

- Tattoo inks
- Toothpaste
- Lipsticks
- Nail polish

These are precisely the products that:
- Stay on the skin
- Enter the mouth
- Or are applied long-term

This creates elevated regulatory and consumer-safety exposure.

### Company Exposure KPIs

Titanium dioxide exposure was measured for all companies with ≥50 products.

Key findings:

- Over 70% of major cosmetic companies have >90% of their product portfolios containing Titanium dioxide
- Several companies show 100% exposure

Examples:

- L’Oréal USA — 100%
- Revlon — 98%
- Procter & Gamble — 98%
- Estée Lauder — 91%
- Shiseido — 100%
- Dior — 98%
- CHANEL — 93%

**Interpretation**

Titanium dioxide is not optional.
It is a core formulation ingredient across the global cosmetics industry.

Any regulatory change would have industry-wide financial and operational impact.

### Chemical Risk Concentration

Market penetration was calculated for all chemicals.

Top chemicals by market share:

Chemical - Market Penetration
- Titanium dioxide	86.58%
- Silica (respirable)	3.67%
- Cocamide diethanolamine	2.43%
- Retinol / retinyl esters	1.96%
- Carbon black	1.94%
- Mica	1.83%
- Talc	1.58%

All remaining chemicals each affect less than 1.5% of products.

**Interpretation**

The chemical risk landscape is not diversified.

It is:

Highly centralized around a single dominant chemical

This makes Titanium dioxide a systemic risk driver rather than one of many hazards.

### Why KPI Validation Matters

This phase ensures:

- All dashboard numbers are auditable
- Every DAX measure traces back to a validated SQL KPI
- Business users see accurate risk exposure

This prevents:

- Metric drift
- Python vs Power BI mismatches
- Stakeholder mistrust