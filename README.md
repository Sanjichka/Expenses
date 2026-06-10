💸 Personal Expense Analytics (Feb 2023 – Present)
I've logged every personal expense since February, 2023. What started as a habit turned into a full project - from raw logging, through cleaning, to an interactive dashboard that finally makes three-plus years of spending readable.
I use dummy expense values for this project, but the concept and all the other categories are real.

Google Sheets + Apps Script - logging the data
Since it's all for personal use, the whole thing lives in Google Sheets, with a custom entry form built in Apps Script. Every time I spend something I open the form, fill it in, and hit submit - it lands as a new row in the sheet.

Each expense becomes one row with these columns:
Description - what it was
Price - how much
Needed/Satisfaction - essential or just nice to have
Date - when I paid
Cash/Card - how I paid
Category - which bucket it falls into
Special – a manual flag I set directly in the sheet for one-off outliers. When something is genuinely rare and perhaps expensive, a new laptop - its size would otherwise skew my conclusions and send me hunting for a "problem" that isn't one. It's a good investment I make once in a blue moon, not a leak in my normal spending. Flagging it as Special lets me set those outliers aside and keep the focus on my everyday habits.

Looker Studio - the dashboard
Six pages, each answering a different question. The date ranges, filters, and drill-downs update the visuals live and make everything interactive.
📌 1. Lifetime Overview
The big-picture page. Two scorecards up top (Total Spent, Average Daily Spend) so the headline numbers hit first. A ranked Spending by Category bar, two donuts for Needs vs Wants and Payment Method, and a Spending Over Time line from 2023 to now. My favorite panel is the Spending DNA scatter: each category is a bubble placed by average transaction size vs how often I buy it - which neatly splits the cheap-but-constant stuff (food, sanjatime) from the rare-but-pricey stuff (accessories, education).
🔎 2. Period Details
The drill-down page. Pick a date range and filter by category or description, and everything recalculates: total spent with an average line, the change vs last month (−67.3% in June), donuts scoped to the period, and a full transactions table with a running total. This is where I answer "where did this month actually go?"
🗂️ 3. Category Breakdown
Two takes on category mix. A treemap sizes each category by its share of the month (food 38%, hangout 23%…) for instant proportion. Below it, a this-month-vs-last-month bar shows what I cut and what held - market dropping from 157 to 15 jumps right out.
⚖️ 4. Needs vs Wants
The question I care about most: how much is essential vs just nice to have. A stacked bar splits "needed" from "satisfaction" in real numbers (176 vs 42), and a donut shows the same as a percentage (80.7% / 19.3%). Watching this ratio over time is basically my personal KPI.


I have two more pages, they are used in my personal analysis where I simultaneously want to compare all the months throughout the years, or when I am interested in detailed analysis annually with a special focus on the categories and whether I started spending more/less per a specific category.
📅 5. Monthly Trends
Twelve mini charts, one per calendar month, each stacking that month across years. Putting January next to January, February next to February, takes seasonality out of the picture and shows the real year-over-year drift (e.g. February: 423 → 532 → 763 → 872).
📆 6. Annual Breakdown
The long view. Every category gets its own yearly chart, plus summary panels for total spend, payment method, and needs vs wants by year - so multi-year patterns (what's grown, faded, or stayed flat) finally show up.
