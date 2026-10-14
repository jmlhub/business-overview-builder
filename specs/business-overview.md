# Business Overview Memo Template

## Purpose

Prepare an initial business overview of a public company for a hedge fund analyst. Capture key facts from the materials utilized and present them clearly and concisely. The goal is to help an analyst become familiar with the company, identify key facts and data, and plan future research, not to jump to conclusions from a limited data set. Follow the template below for structure, and the principles to inform what is relevant and how it should be presented.

## Investment principles

Use these insights as a lens for reading the materials and presenting information. For each relevant topic, present the available facts and explain the connection that could be useful to the analyst. A topic can be important even when the supplied materials do not resolve it. Do not apply these principles to jump to conclusions.

1. The value of a business depends on the EPS and FCF per Share over time
2. Other valuation metrics like EV to EBITDA and EV to EBIT can still be useful
3. Identify the few key operational drivers that explain majority of earnings variance 
4. Key drivers are often intuitive but company's also provide information on factors impacting earnings over time which can be instructive
5. Key drivers should be operational metrics, macro variables, key input costs, commodity prices, etc., not simply "revenue" and "gross margin"
6. Developing a view on key drivers is key to projecting earnings
7. Consider operating and financial leverage that magnify impact to bottom line
8. Contextualize earnings: separate the secular, cyclical, temporary factors 
9. Profitability can be heavily impacted by investment cycles, money-losing nascent segments, and similar factors that don't reflect long-term earning power
10. Look for signs as to competitive intensity and shifts in the landscape
11. Shifting balance of supply and demand within a product or service market drives earnings
12. Some companies have untapped pricing power which becomes extremely important
13. Follow the management strategy and investment plans closely - which helps frame potential for value creation, and goalposts against which to evaluate performance
14. Always consider earnings quality (add backs % of total EBITDA and EPS) - some adjustments are truly accounting noise or one-time factors, but companies may add back recurring economic expenses like stock-based compensation or constant restructuring costs 
15. Sell side research reports and models are useful for benchmarks of how analysts think and what the consensus view is - use them as a proxy for expectations, authoritative views
16. Momentum is a key factor - which earnings growth accelerates or decelerates stocks typically follow - so understanding what drives earnings is essential
17. Growth only creates value if return on capital invested is significantly above cost of capital
18. Many companies grow but spend too much or lack durability so value is not created
19. Read disclosures for both content or facts and changes over time 
20. Follow the data - do not trust explanations from the company or management
21. Provide detailed context on potential events (separable assets, strategic interest, spinoffs, strategy or management changes, etc.)
22. Disclose any material risks and liabilities even if not presented as risks or quantifiable today

## Research workflow and source collection

1. **The ingest workflow**. If not provided in the initial user request, ask the user to clarify the following details:
	1. Name of the company or stock ticker if it's US listed.
	2. Light run (only using the latest 10K and filings since it was filed), or heavy run (last 3 10-K reports, last 3 10-Q reports, and filings since the latest 10-Q). 
	3. Memo, screen-friendly slide deck, or printer-friendly slide deck format (follow the Donerail presentation formats which already have a skill in the plugin)
	4. Remind user to provide any helpful documents before the process begins, such as consensus estimates, historical trading multiples, earnings call transcripts, sell-side analyst reports and models, and industry research
2. **Pull the necessary SEC filings**. The Donerail Plugin already includes a script to access the SEC API which can be re-used. Pull the SEC filings relevant for the specified light or heavy run. Always read the last 4 earnings releases provided in form 8-K. Also use the SEC API to pull 20 years of revenue, operating income, D&A (to calculate GAAP EBITDA), net income, and EPS data, to evaluate long-term earnings trends (this may be called the SEC EDGAR XBRL API or Company Concept API). Pull stock price history if possible and present it in a chart with the past 3 years of data (or less if that's all that's available). 
3. **Read the filings, data, and supplementary materials provided by the user**. Consider the facts and data presented, as well as what has changed over time. SEC filings and earnings calls should be viewed as a source of key facts (potentially with management "spin" applied). Sell side analyst research and models are used to frame consensus. Use limited web searches to fill in key knowledge gaps (swings in macro data, resolution of news such as potential M&A, etc.)
4. **Build the business overview presentation.** Use the template below. Organize key evidence. Quote useful facts and data along with their source documents, speakers, and dates. Use footnotes to provide source information and detail. 
	1. Be concise: about 15 pages for a heavy run, fewer for a light run, including tables, charts and footnotes.
	2. Put minor clarifying detail and every source in footnotes, never in bullets or lines of their own; footnote the source of estimates. When a footnote cites an earnings call transcript or a research analyst's note, quote the relevant passage and name the speaker or analyst.
	3. Do not state what the reader can infer (e.g. that a year marked `YYYYE` is not yet reported).
	4. Follow the Donerail memo template's formats. In tables, labels and notes go in the left column and numbers only in the value columns, right-aligned; key totals (Market Capitalization, Enterprise Value, etc.) are bold; row labels are short; a table moves to the next page rather than split.

## 1. Financial Summary

[a compact, two-part financial exhibit]

### Current valuation

[Market Cap = Share Price x Ending Shares Outstanding (include each share class with economic rights)]
[Enterprise value = Market Cap Less Cash Plus Debt, Finance Leases, Preferred Equity, and Minority Interests]

| Item                                                     | Value                   |
| -------------------------------------------------------- | ----------------------- |
| Share Price                                              | [Value(s)]              |
| Shares Outstanding                                       | [Class and share count] |
| Market Capitalization                                    | [Value]                 |
| Less: Cash                                               | [Value]                 |
| Plus: Debt                                               | [Value]                 |
| Plus: Finance Leases / Capitalized Financing Obligations | [Value]                 |
| Plus: Preferred Equity                                   | [Value]                 |
| Plus: Minority Interests                                 | [Value]                 |
| Plus: Other Items, Including Treatment of Securities     | [Value and treatment]   |
| Enterprise Value                                         | [Value]                 |
### Historical and forecast performance

Show two actual years and, when supplied or readily available, two estimate years, labeled `YYYYA` and `YYYYE`. Attribute estimates, in a footnote, to management, a named analyst, a consensus source, or a user-provided model. Use only the metrics actually covered by that source. If estimates are unavailable, retain the historical information and label the estimate cells unavailable; do not create a forecast to complete the table. Include adjusted EPS and FCF per share alongside the operating metrics.

| FYE: [Month]                       | [YYYYA — prior actual] | [YYYYA — latest actual] | [YYYYE — first estimate] | [YYYYE — second estimate] |
| ---------------------------------- | ---------------------- | ----------------------- | ------------------------ | ------------------------- |
| Revenue                            | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| Growth Y-Y                         | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| Adjusted EBITDA                    | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| Adjusted EBITDA margin             | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| EV/EBITDA                          | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| Adjusted EBIT                      | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| Adjusted EBIT margin               | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| EV/EBIT                            | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| Adjusted EPS                       | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| Free Cash Flow (Adj. if Available) | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| FCF per Share (Adj. if Available)  | [Value]                | [Value]                 | [Value]                  | [Value]                   |
| Stock-Based Compensation           | [Value]                | [Value]                 | [Value]                  | [Value]                   |
**Special cases:**
- If a company has multiple operating segments, show "Note:" rows which break down each metric possible by segment (generally, Revenue, and Adj. EBITDA and/or Adj. EBIT). 
- If a company reports EBITDAR, then show EBITDAR and EBITDA, and Enterprise Value Before and After Capitalized Rent.
- If a company has a specialized business model where Enterprise Value is not used, adapt this financial summary as necessary (banks use book value and net income not EV or EBITDA)

**Time frame for forecasts:**
- If consensus or sell side estimates are available: show two years of historical data and 3 years of forecasts
- If only management guidance for current year is available: show 4 years of historical data and 1 year of guidance
- If neither are available, show 4 years of historical data and LTM financials through the latest quarter

## 2. Share Price History

Insert a historical share-price chart using clean, split-adjusted prices when available. Otherwise, skip this section and renumber the others accordingly.

Annotate stock chart with material reported events, earnings beats or misses, guidance revisions, or other market-moving factors if available. Highlight observed acceleration or deceleration in relevant metrics where the available data supports it (e.g. shares have declined by 30% in the last 6 months as EPS growth slowed from 20% to 5% in last 2 quarters). 

[Historical share-price chart and relevant factual context]

## 3. Business Model Breakdown

### Business Model Overview

Provide a concise breakdown of the business model, which should answer the following:

- What product or service is provided
- What value is created for customers
- How the company makes money (revenue model, unit economics, cost structure)
- Key operating and financial metrics
- Detail on competitive and product positioning vs. peers
- Is the company heavily regulated? If so, what are key regulators and constraints

### Additional Context

- Highlight any information that makes a company unique from peers in the same industry and other industries
- Quantify metrics available that frame how the business is unique: key customers and suppliers, customer or supplier concentration, customer demographics, product metrics, pricing data, scale vs. peers, outsized R&D spending, etc.
- 10-K reports typically include a multitude of these variables that help frame what makes a company unique
- e.g. does a company serve enterprise or SMB customers? Does a company use a diversified base of 30 suppliers, or buy most of its product from one supplier? Does a company use a stated low price strategy or seek product differentiation? How many SKUs does the company sell? These type of details should be included.

## 4. Stated Management Strategy

Describe management's stated strategy for creating value and related context:

- **Stated objectives:** What management says it is trying to achieve, including financial or operating targets and their timeframes.
- **Actions and priorities:** Products, customers, markets, pricing, cost actions, operational changes, investment programs, acquisitions, divestitures, and capital allocation.
- **Intended path to value:** How management says the actions should affect revenue, margins, capital efficiency, cash flow, or per-share results.
- **Required resources and dependencies:** Disclosed spending, capital needs, execution requirements, and dependencies.
- **Progress and changes:** Reported results or milestones alongside the corresponding stated goals; revisions, delays, abandoned initiatives, or changes in emphasis.

Distinguish intentions and targets from achieved results. Report straightforward comparisons with stated milestones when the measures and periods match. The section should equip the analyst to evaluate the targets, financial impact if they are achieved, success or failure milestones so far; it does not require an independent judgment that the strategy will work.

## 5. Valuation Details

Include additional detail that is helpful to understand valuation.

Potential sections as relevant based on situation and available information:

- Sum-of-the-Parts valuation
	- If the company has multiple segments it is useful to value them separately
	- Can use sell-side report or model SOTP analysis if available
	- Otherwise build a simple one when relevant: a table applying a multiple to each segment's earnings, with unallocated corporate cost valued at the segments' blended multiple. Where useful, back into the value implied for one segment (e.g. "if UTI were worth 10x 2027 EBITDA, Concorde would be free")
- Value of potentially separable assets
	- If incremental to segment analysis, include this
	- Business may own separable assets (real estate that could be sold, etc.)
- Valuation excluding Losses
	- If a company has a major money-losing business segment, or money losing venture embedded within a segment, if possible, show the valuation multiples when excluding these losses 
	- The logic: losses will flip to income or the venture will eventually be shut down
- Chart with historical trading multiples (if data was provided)
- Public Company Quality of Earnings Analysis
	- Bridge from GAAP to Adjusted financial metrics (EBITDA, Net Income, etc.)
	- Total adjustments as % of Adjusted financial metrics 
	- Identify which of these adjustments are likely economic recurring costs (SBC, etc.)
	- Management may label expenses as "One-Time Restructuring" but incur them every period

## 6. Key Factors Impacting Earnings

Provide context as to the forces which have impacted recent earnings in recent periods. The goal is to understand historical and current earnings, to form a basis for projections, but not to actually make the projections in this report.

Key sources of this information:
- Key drivers identified above
- 10-K and 10-Q reports with sections which compare current period earnings to prior period and list the factors causing the changes
- Earnings releases and call transcripts

As possible and relevant, provide:
- Chart with long-term historical operating income or EBITDA (can use GAAP measures for efficiency since these can be pulled from SEC API); below each year, show Total Revenue, Operating Margin and EBITDA Margin
- Bridges between Adj EBITDA or Adj EBIT across time periods, showing the factors which impacted earnings between periods to identify key drivers
- Other schedules or charts as necessary

### Recent performance and expectations

- Compare recent results with the preceding periods when data is available.
- Present operating metrics alongside revenue, Adj. EBITDA, Adj. EBIT, etc.
- Summarize management's explanation of changes, guidance revisions, and disclosed impacts.
- Include reported beats or misses when the dated comparison benchmark is available.
- Attribute estimates and views from supplied research.
- Do not substitute an independent forecast for unavailable consensus.
- Highlight observed acceleration, deceleration, or changing comparisons.

### Sources of earnings change

| Category            | Information to capture from the materials                                                                             |
| ------------------- | --------------------------------------------------------------------------------------------------------------------- |
| Secular             | Disclosed industry growth, longer-term share or pricing trends, and changes to the business model.                    |
| Cyclical            | Demand, supply, capacity, utilization, inventories, pricing, and management's explanation of cyclical conditions.     |
| Temporary / one-off | Disclosed temporary benefits or burdens, including items that remain in adjusted metrics.                             |
| Competitive changes | Reported changes in competitors' spending, funding, capacity, entry, or exit and any described effect on the company. |
| Investment cycle    | Spending, segment losses, ramp schedules, closures, and management's stated timing of benefits.                       |

Identify the source and period of each important fact. Explain why it could matter to earnings or FCF, while leaving the magnitude or future direction open where not supported.

### Sensitivity to Key Drivers

If provided or possible to estimate, provide information on how key drivers would impact Adj. EBITDA or Adj. EBIT or Adj. Net Income or Adj. EPS.

This depends largely on: nature of the key driver, fixed vs. variable costs (can require estimating nature of each P&L line item), and financial leverage.

In some cases, small changes in volumes, pricing, gross margins, etc. can cause large swings in EPS and FCF, and this should be noted.

Examples:
- A 1% increase in volumes could increase EPS by 3%
- A 1% increase in pricing could increase EPS by 6%
- A 1% increase in resin prices could reduce EPS by 3%

| Driver and illustrative change                                   | Disclosed relationship / simple assumptions | Likely EBITDA impact  | Likely EPS impact               | Basis, source, and limitations                   |
| ---------------------------------------------------------------- | ------------------------------------------- | --------------------- | ------------------------------- | ------------------------------------------------ |
| [Price, volume, spread, cost, or other driver; change and units] | [Mechanism; held-constant assumptions]      | [Amount or direction] | [Per-share amount or direction] | [Disclosed / calculated / directional; citation] |

Explain the role of starting margins, fixed versus variable costs, and financing where the information is available. A quantified EBITDA impact does not automatically provide a quantified EPS impact: EPS may also require depreciation, interest, tax, and share-count inputs. Leave unsupported amounts unquantified.

Keep the work proportional to an initial overview. Do not build a full operating model, assume the shock will occur, or translate the sensitivity into a stock-price forecast.

[Sensitivity summary]

## 7. Macro Backdrop

**Structure:**

- Provide a brief explanation of the key macro and industry variables that likely impact key operational drivers and therefore earnings of the company
- Include bullet points with context to help the analyst frame the macro situation (recent macro trends, where key macro variables are vs. historical levels, publicly available forecasts for the industry, etc.)

**Process:**

- The company filings may identify certain key macro and industry variables
- Claude should use this and research on the business and key drivers to estimate the key macro and industry variables that drive earnings for the company
- If necessary, perform targeted research using the internet to add context regarding these key drivers
- The key focus is understanding factors like where we are in the cycle for key variables, recent trends, and the outlook from credible sources
- Often this analysis will be straightforward: for a homebuilder, the key macro variables would likely be new home sales, mortgage rates, and labor costs. Claude could briefly search and uncover that there is a widespread belief that there is a deficit of homes in the US, but rising mortgage rates are impacting the short-term outlook.
- This section should be concise and illuminate key issues for future research.

## 8. Key Risks and Liabilities

Surface risks, liabilities, and exposures a portfolio manager needs to understand before investing.

- Cover material business risks, balance-sheet liabilities, and off-balance-sheet exposures, including leases and unquantified litigation.
- Include disclosed amounts, maturities, commitments, contingencies, and the company's explanation of the exposure where available.
- Highlight new or changed disclosures and risks already discussed in supplied investment research.
- Explain the mechanism through which a risk could affect the business or shareholders, without estimating losses that the available information cannot support.
- Include risk factors disclosed in the 10-K (beyond boiler plate or immaterial ones), as well as risk factors that are inferred by Claude.
- Exposures = risk. If a company has high exposure to certain customers or customer segments, suppliers, etc. then this should be included.

Distinguish quantified disclosures, unquantified exposures, and missing information. A lack of disclosure in the reviewed materials does not establish that no exposure exists.

## 9. Recent News and Events

Use one row per material event. Keep searches focused on consequential developments. Review the IR press release page.

Apply this baseline priority order:

1. Major M&A, including a sale, spinoff, or divestiture. Capture the first documented bid or rumor, material updates, and any conclusion.
2. Stakes or Schedule 13D filings by potential activists or strategic acquirers, where relevant to an event.
3. Major management changes.
4. Major strategy changes.
5. Major changes in business conditions.
6. Earnings releases associated with stock moves of 10% or more, when price data is available.
7. Other developments material to a hedge fund analyst.

| Date (Mmm-yy) | Source   | Event description | Stock price at event   |
| ------------- | -------- | ----------------- | ---------------------- |
| [Date]        | [Source] | [Event]           | [Price or unavailable] |

Identify relevant unanswered questions without assigning independent deal probabilities or building event-return scenarios.

## 10. Analyst Perspectives

When research is supplied, summarize the views and the facts they cite. Do not expand the assignment to obtain unavailable research.

Repeat for each relevant analyst:

- **Bank, analyst, and report date:** [Details]
- **Investment thesis:** [Attributed view]
- **Valuation perspective:** [Attributed view and available basis]
- **Position on key debates:** [View and cited evidence]

Distinguish a named analyst's estimate from a defined consensus measure. Include documented buyside views if available; do not infer a consensus from price behavior. Lay out disagreements and the information that would help an analyst examine them, without requiring Claude to resolve the debate.

## 11. Source Documents and Follow-up Questions

List the documents and data sources actually used, including filing or publication dates and the periods covered.

- [Document or data source; date; location]
- [Document or data source; date; location]

Close with a short list of material questions the supplied information does not answer, such as missing cost sensitivities, unclear investment returns, or an unresolved liability. These are directions for subsequent analyst work, not unfinished requirements to expand this initial overview.

