# AiMetrics — 50 Key Investor Metrics for AI Startups

> A comprehensive reference for investors evaluating AI startups. Research and development performed by **Von AI**. [LinkedIn profile of the developer](https://www.linkedin.com/in/warren-harding-29a0a673).

---

## Table of Contents

### Section 1: AI-Specific Metrics (20 Metrics)
- [1. Inference Cost per Token (CPM)](#1-inference-cost-per-token-cpm)
- [2. Compute Costs as % of Revenue](#2-compute-costs-as--of-revenue)
- [3. GPU Utilization Rate](#3-gpu-utilization-rate)
- [4. Inference Latency (Time to First Token)](#4-inference-latency-time-to-first-token)
- [5. Model Accuracy / Precision / Recall / F1 Score](#5-model-accuracy--precision--recall--f1-score)
- [6. Model Improvement Velocity](#6-model-improvement-velocity)
- [7. Proprietary Data Assets / Data Quality](#7-proprietary-data-assets--data-quality)
- [8. Data Moat Velocity](#8-data-moat-velocity)
- [9. Data Flywheel Evidence](#9-data-flywheel-evidence)
- [10. Dependency Risk (Single Model/Provider Exposure)](#10-dependency-risk-single-modelprovider-exposure)
- [11. Fully-Loaded Cost per Unit](#11-fully-loaded-cost-per-unit)
- [12. COGS Stack Breakdown](#12-cogs-stack-breakdown)
- [13. Token Efficiency Metrics](#13-token-efficiency-metrics)
- [14. Orchestration Overhead Multiplier](#14-orchestration-overhead-multiplier)
- [15. Compute Runway](#15-compute-runway)
- [16. AI Gross Margin](#16-ai-gross-margin)
- [17. Data Moat Premium](#17-data-moat-premium)
- [18. Model Drift/Maintenance Cost](#18-model-driftmaintenance-cost)
- [19. Technical Risk Discount](#19-technical-risk-discount)
- [20. Regulatory Compliance Score](#20-regulatory-compliance-score)

### Section 2: Software / SaaS Metrics (15 Metrics)
- [21. MRR (Monthly Recurring Revenue)](#21-mrr-monthly-recurring-revenue)
- [22. ARR (Annual Recurring Revenue)](#22-arr-annual-recurring-revenue)
- [23. NRR/NDR (Net Revenue Retention)](#23-nrrndr-net-revenue-retention)
- [24. GRR (Gross Revenue Retention)](#24-grr-gross-revenue-retention)
- [25. LTV:CAC Ratio](#25-ltvcac-ratio)
- [26. CAC Payback Period](#26-cac-payback-period)
- [27. Rule of 40](#27-rule-of-40)
- [28. Burn Multiple](#28-burn-multiple)
- [29. Logo Churn (Monthly)](#29-logo-churn-monthly)
- [30. ARR per Employee](#30-arr-per-employee)
- [31. Activation Rate](#31-activation-rate)
- [32. Time-to-Value (TTV)](#32-time-to-value-ttv)
- [33. DAU/MAU Ratio (Stickiness)](#33-dau mau-ratio-stickiness)
- [34. Product Market Fit Score](#34-product-market-fit-score)
- [35. NPS (Net Promoter Score)](#35-nps-net-promoter-score)

### Section 3: General Business / Financial Metrics (15 Metrics)
- [36. Revenue Growth Rate (YoY)](#36-revenue-growth-rate-yoy)
- [37. Gross Margin](#37-gross-margin)
- [38. EBITDA Margin](#38-ebitda-margin)
- [39. Free Cash Flow (FCF)](#39-free-cash-flow-fcf)
- [40. Gross Burn Rate](#40-gross-burn-rate)
- [41. Net Burn Rate](#41-net-burn-rate)
- [42. Cash Runway](#42-cash-runway)
- [43. LTV (Customer Lifetime Value)](#43-ltv-customer-lifetime-value)
- [44. CAC (Customer Acquisition Cost)](#44-cac-customer-acquisition-cost)
- [45. Magic Number](#45-magic-number)
- [46. EV/Revenue Multiple](#46-evrevenue-multiple)
- [47. TAM (Total Addressable Market)](#47-tam-total-addressable-market)
- [48. Revenue Concentration](#48-revenue-concentration)
- [49. S&M as % of Revenue](#49-sm-as--of-revenue)
- [50. Efficiency Score](#50-efficiency-score)

---

## Introduction

Evaluating AI startups requires a dual lens: traditional SaaS and financial metrics that any software investor understands, plus AI-specific indicators that capture the unique unit economics, technical risk, and defensibility of artificial intelligence businesses. This repository compiles **50 key investor metrics** organized into three categories:

1. **AI-Specific Metrics** — 20 metrics covering inference economics, model quality, data moats, compute runway, and regulatory risk.
2. **Software / SaaS Metrics** — 15 metrics covering recurring revenue health, retention, efficiency, and product-market fit.
3. **General Business / Financial Metrics** — 15 metrics covering growth, margins, cash management, valuation, and market opportunity.

Each metric includes benchmarks, target ranges, and investor relevance notes to support due diligence and portfolio monitoring.

---

## Section 1: AI-Specific Metrics

### 1. Inference Cost per Token (CPM)

**Definition:** The cost incurred to generate one million output tokens from a model, measured in dollars per million tokens (CPM). This encompasses both self-hosted inference on dedicated hardware and third-party API-based inference.

**Typical Ranges:** Self-hosted inference on optimized hardware generally runs $0.10–$0.50 per million tokens, whereas third-party API providers charge $0.60–$15.00 depending on the model size, capability tier, and provider pricing strategy.

**Why Investors Care:** Inference cost is the single most important unit economics driver for AI companies. Every interaction a user has with the product carries a direct variable cost tied to token consumption. If CPM does not trend downward over time — through model optimization, hardware upgrades, caching strategies, or migration to cheaper models — the business becomes unsustainable at scale. Investors should look for evidence of declining CPM trajectories and clear strategies for cost reduction.

---

### 2. Compute Costs as % of Revenue

**Definition:** The proportion of total revenue consumed by compute expenses, including GPU leasing, cloud infrastructure fees, and related processing costs.

**Typical Ranges:** Early-stage AI startups typically see compute costs consume 50–80% of revenue. As the business matures and achieves pricing power or operational efficiency, this ratio should decline toward 20–30%.

**Why Investors Care:** This metric reveals whether the company's fundamental economics can support profitability. A compute cost ratio above 70% signals that the company is spending most of its revenue just to run the product, leaving little for growth, R&D, or profit. Investors should track this ratio over time and demand a clear downward trajectory as a condition of the investment thesis.

---

### 3. GPU Utilization Rate

**Definition:** The percentage of available GPU compute capacity that is actively processing inference or training workloads during a given period.

**Typical Ranges:** Well-optimized dedicated infrastructure targets utilization above 70%. The industry average for cloud GPU instances sits between 30–50%, reflecting significant idle capacity.

**Why Investors Care:** Low GPU utilization means the company is paying for compute it is not using, directly eroding margins. High utilization indicates operational discipline and efficient capital deployment. Investors should ask about workload scheduling, auto-scaling policies, and whether the company rightsizes its infrastructure to match demand patterns.

---

### 4. Inference Latency (Time to First Token)

**Definition:** The elapsed time between a user's request and the first token of the model's response being returned, measured in milliseconds.

**Typical Ranges:** Real-time applications target ≤100ms time-to-first-token. Chat-based applications tolerate up to ≤250ms. Batch or asynchronous workloads may accept higher latencies.

**Why Investors Care:** Latency is a direct driver of user experience and, consequently, retention. Users abandon slow interfaces; even small increases in perceived wait time can reduce engagement. For AI startups competing on product quality, latency is as important as model accuracy. Investors should verify that the company measures and optimizes this metric across its infrastructure stack.

---

### 5. Model Accuracy / Precision / Recall / F1 Score

**Definition:** Standard statistical measures of model quality. Accuracy reflects overall correctness; precision measures the rate of true positive predictions among all positive predictions; recall measures the rate of true positives captured among all actual positives; F1 score is the harmonic mean of precision and recall.

**Typical Ranges:** Varies by domain and task. In competitive AI markets, a 5-point superiority gap over rivals can justify a 30–50% price premium.

**Why Investors Care:** Model quality is the product. If the model does not outperform alternatives on quantifiable metrics, the company has no defensible product advantage. Investors should insist on independent benchmarking data and understand how the company's metrics compare to open-source baselines and commercial competitors.

---

### 6. Model Improvement Velocity

**Definition:** The rate at which the company's models demonstrate measurable performance gains over time, typically tracked through benchmark scores, internal evaluation metrics, or customer outcome improvements.

**Typical Ranges:** Leading AI companies demonstrate quarterly or monthly improvement cycles. Slower improvement rates may indicate R&D bottlenecks or diminishing returns.

**Why Investors Care:** In a rapidly evolving field, standing still means falling behind. Improvement velocity signals the effectiveness of the company's R&D engine and its ability to sustain a competitive edge. Investors should look for structured evaluation frameworks, regular model release cadences, and evidence that improvements translate to customer-facing value.

---

### 7. Proprietary Data Assets / Data Quality

**Definition:** The volume, labeling accuracy, diversity, and freshness of the training data the company controls exclusively. This includes curated datasets, labeled corpora, and domain-specific data collections.

**Typical Ranges:** Varies widely. The key differentiator is not raw volume but the uniqueness and relevance of the data to the company's target domain.

**Why Investors Care:** Proprietary data is the foundation of a defensible AI moat. Open-source models can replicate general capabilities, but domain-specific data advantages are harder to copy. Investors should assess the data pipeline: how is data acquired, cleaned, labeled, and updated? Is the data pipeline itself a competitive advantage?

---

### 8. Data Moat Velocity

**Definition:** The rate at which the company's proprietary data advantage grows over time. A positive data moat velocity means the company is accumulating harder-to-replicate data faster than competitors can catch up.

**Typical Ranges:** Companies with self-reinforcing data flywheels can justify valuation premiums of 40–80% over peers with static data assets.

**Why Investors Care:** A data moat that grows over time is far more valuable than a static dataset. If each customer interaction generates new training data that improves the product, the company's competitive position strengthens with every user. Investors should look for evidence of accelerating data accumulation and improving model performance correlated with data growth.

---

### 9. Data Flywheel Evidence

**Definition:** Whether the company's product usage generates proprietary training data that improves the model, which in turn drives additional usage — creating a self-reinforcing cycle.

**Typical Ranges:** Binary signal — either the flywheel exists with measurable evidence, or it does not.

**Why Investors Care:** Data flywheels are the strongest form of defensibility in AI. Companies like Google Search and Uber benefited from this dynamic historically. For AI startups, a proven flywheel means the product gets better the more it is used, creating switching costs and compounding advantages. Investors should demand concrete examples: what data is collected from usage, how is it incorporated into model training, and what measurable improvements result?

---

### 10. Dependency Risk (Single Model/Provider Exposure)

**Definition:** The concentration risk arising from reliance on a single external LLM provider (e.g., OpenAI, Anthropic, Google) for core product functionality.

**Typical Ranges:** Companies dependent on one provider face significant supply chain risk. Diversified stacks using multiple providers or self-hosted models reduce this exposure.

**Why Investors Care:** A provider price increase, API change, or service disruption could cripple a company built on a single dependency. Investors should assess the company's provider diversification strategy, the feasibility of migrating workloads, and whether the company has proprietary models that reduce third-party reliance.

---
### 11. Fully-Loaded Cost per Unit

**Definition:** The total cost of goods sold (COGS) per billable unit of service, encompassing inference costs, retrieval overhead, orchestration, infrastructure, and any human-in-the-loop expenses.

**Typical Ranges:** For chat-based AI products, fully-loaded costs typically range from $0.05 to $0.30 per conversation. For more complex agentic tasks involving multi-step reasoning and tool use, costs range from $0.50 to $5.00 per task.

**Why Investors Care:** This metric establishes the pricing floor for the product. If the fully-loaded cost per unit exceeds the price charged to customers, the company loses money on every transaction. Investors should verify that pricing strategies provide adequate margin above fully-loaded costs and that the company has a plan to drive unit costs down through optimization.

---

### 12. COGS Stack Breakdown

**Definition:** A detailed decomposition of the cost of goods sold into its component categories: model inference, RAG retrieval, orchestration overhead, infrastructure hosting, and human-in-the-loop operations.

**Typical Ranges:** Varies by product architecture. Inference typically dominates, but orchestration overhead in agentic systems can consume a significant share.

**Why Investors Care:** Understanding the COGS stack reveals where optimization efforts should be focused. If orchestration overhead is the largest cost driver, the company should invest in reducing agent loop iterations. If inference dominates, model distillation or hardware optimization may be the priority. Investors should ask for a clear COGS breakdown and a roadmap for cost reduction in the largest categories.

---

### 13. Token Efficiency Metrics

**Definition:** Measures of how effectively the company uses tokens in its prompts, context windows, and model outputs. Includes prompt optimization quality, context window utilization, and output verbosity control.

**Typical Ranges:** Well-optimized systems can reduce token consumption by 30–60% compared to naive implementations through techniques like prompt compression, selective context loading, and output constraints.

**Why Investors Care:** Token efficiency is a direct lever for reducing inference costs without sacrificing output quality. Companies that invest in prompt engineering, context management, and output control demonstrate operational sophistication. Investors should look for evidence of systematic token optimization and measurable cost savings from these efforts.

---

### 14. Orchestration Overhead Multiplier

**Definition:** The multiplier applied to base inference costs due to agent loops, tool calls, retries, and multi-step reasoning chains in agentic AI systems. Each additional loop iteration compounds the cost.

**Typical Ranges:** Agentic workflows can add a 5–20x cost multiplier per user request compared to a single model call. Complex multi-agent systems may exceed this range.

**Why Investors Care:** This is one of the most dangerous cost traps for AI startups building agentic products. A feature that requires 10 tool calls and 3 retry attempts costs 30x more than a single inference call. Investors should understand the typical orchestration multiplier for the company's product and whether there is a strategy to reduce unnecessary iterations.

---

### 15. Compute Runway

**Definition:** The amount of time the company's available compute resources (GPUs, cloud credits, reserved instances) will last given the current rate of compute consumption, separate from overall cash runway.

**Typical Ranges:** Varies by company stage and infrastructure commitments. Some AI startups can run out of accessible compute before running out of cash.

**Why Investors Care:** Compute constraints can kill an AI startup faster than cash shortages. If a company's GPUs are fully allocated and cloud budgets are exhausted, product development and customer service grind to a halt regardless of remaining bank balance. Investors should assess compute runway independently from cash runway and ensure the company has a plan for scaling infrastructure.

---

### 16. AI Gross Margin

**Definition:** Gross margin calculated specifically for AI companies, where COGS is dominated by inference and compute costs rather than traditional software delivery costs.

**Typical Ranges:** AI startups typically achieve 50–60% gross margins, compared to 75%+ for traditional SaaS companies. Margins below 50% signal unit economics challenges that must be addressed.

**Why Investors Care:** Gross margin is the primary indicator of whether a business model can achieve profitability. AI companies start with lower margins than traditional SaaS due to compute costs, but margins should expand over time through optimization, scale, and pricing power. Investors should demand a clear path to margin expansion and track margin trends quarterly.

---

### 17. Data Moat Premium

**Definition:** The valuation premium assigned to a company based on the uniqueness, quality, and defensibility of its proprietary datasets relative to competitors.

**Typical Ranges:** Companies with strong data moats can command valuation premiums of 15–65% above base enterprise value estimates, depending on data uniqueness and the difficulty of replication.

**Why Investors Care:** Data advantages are among the hardest competitive positions to replicate. A company with exclusive access to high-quality domain data can sustain superior model performance even as open-source models improve. Investors should evaluate the exclusivity of the data, the cost and time required for competitors to assemble comparable datasets, and whether the data advantage is growing or static.

---

### 18. Model Drift / Maintenance Cost

**Definition:** The ongoing cost required to retrain, fine-tune, and maintain models to preserve performance levels as data distributions shift and user expectations evolve.

**Typical Ranges:** Typically 8–15% of revenue. Companies that fail to account for maintenance costs risk 20–30% overvaluation.

**Why Investors Care:** Models degrade over time without active maintenance. A company that delivered strong performance six months ago may be underperforming today if it has not invested in continuous retraining. Investors should verify that the company budgets for model maintenance, monitors performance drift, and has a structured retraining pipeline.

---

### 19. Technical Risk Discount

**Definition:** A valuation adjustment applied to reflect the percentage of the company's technical roadmap that remains unproven or unvalidated in production environments.

**Typical Ranges:** Companies with validated production models command 2–3x valuation premiums over those with only lab-stage or research-grade results.

**Why Investors Care:** There is a significant gap between research prototypes and production-ready AI systems. Models that perform well in controlled benchmarks may fail under real-world conditions with diverse inputs, edge cases, and scale. Investors should discount valuations proportionally to the amount of unproven technology in the roadmap and prioritize companies with demonstrated production track records.

---

### 20. Regulatory Compliance Score

**Definition:** An assessment of the company's compliance posture with relevant data protection regulations (GDPR, HIPAA, CCPA) and emerging AI-specific regulations such as the EU AI Act.

**Typical Ranges:** Companies operating in high-risk AI categories within regulated markets may face 10–25% valuation discounts if compliance is inadequate.

**Why Investors Care:** Regulatory risk is rising rapidly for AI companies. Non-compliance can result in fines, product bans, or forced architectural changes that destroy competitive advantages. Investors should evaluate the company's regulatory strategy, compliance investments, and exposure to jurisdictions with strict AI regulations.

---

## Section 2: Software / SaaS Metrics

### 21. MRR (Monthly Recurring Revenue)

**Definition:** The normalized, predictable subscription income a company generates each month, adjusted for one-time fees, deferred revenue, and contract variations. MRR smooths out irregularities to provide a clean view of recurring revenue health.

**Typical Ranges:** Varies dramatically by stage. Pre-seed startups may have $0–$10K MRR. Series A companies typically demonstrate $80K–$250K+ MRR. Growth-stage companies often exceed $1M MRR.

**Why Investors Care:** MRR is the foundational metric for subscription businesses. It provides the baseline for measuring month-over-month growth, forecasting annual revenue, and assessing the stability of the income stream. Investors should examine MRR composition — how much comes from new logos versus expansion, and whether the revenue is concentrated among a small number of customers. Consistent MRR growth signals product-market fit and scalable go-to-market execution.

---

### 22. ARR (Annual Recurring Revenue)

**Definition:** Annualized recurring revenue, calculated as MRR multiplied by 12. ARR is the primary metric used for annual contracts, board reporting, fundraising milestones, and valuation benchmarks.

**Typical Ranges:** Series A fundraising typically requires $1M–$3M+ ARR. Series B companies often range from $5M–$20M ARR. Late-stage and pre-IPO SaaS companies frequently exceed $50M ARR.

**Why Investors Care:** ARR provides the annual revenue anchor that investors use to apply valuation multiples and compare companies across their portfolio. It is the primary signal of scale. Investors should look at ARR growth trajectory, the mix of contract lengths contributing to ARR, and whether ARR is supported by strong retention or is being propped up by aggressive new customer acquisition.

---

### 23. NRR / NDR (Net Revenue Retention / Net Dollar Retention)

**Definition:** The percentage of recurring revenue retained from existing customers in a given period, accounting for expansion (upsells and cross-sells), contraction (downgrades), and churn (cancellations). An NRR above 100% means existing customers are generating more revenue over time despite any losses.

**Typical Ranges:** Venture-backed SaaS median is approximately 106%. Top-quartile companies achieve 120%+ NRR. Below 100% NRR indicates the company is losing revenue from its existing base.

**Why Investors Care:** NRR is arguably the most important retention metric for growth-stage SaaS companies. High NRR means the company can grow profitably from its existing customer base without proportional increases in acquisition spend. Companies with NRR above 120% can effectively "grow their way" to profitability. Investors should dig into the drivers of NRR: is expansion coming from genuine product value or from one-time add-ons that may not recur?

---

### 24. GRR (Gross Revenue Retention)

**Definition:** The percentage of revenue retained from existing customers excluding any expansion revenue. GRR isolates the pure stickiness of the product by measuring how much revenue is lost to churn and downgrades alone.

**Typical Ranges:** The median for private SaaS companies is approximately 91%. Strong products achieve 95%+ GRR. Below 85% signals significant product or customer satisfaction issues.

**Why Investors Care:** GRR reveals the underlying product quality independent of sales-driven expansion. A company with high NRR but low GRR is relying on new upsells to offset significant churn — a fragile growth model. Investors should view GRR as the true measure of product stickiness and customer satisfaction. Consistently high GRR means the product is essential enough that customers stay and pay even without active sales engagement.

---

### 25. LTV:CAC Ratio

**Definition:** The ratio of Customer Lifetime Value (LTV) to Customer Acquisition Cost (CAC). This is the primary unit economics test for subscription businesses, measuring how much revenue a customer generates over their lifetime relative to the cost of acquiring them.

**Typical Ranges:** A minimum threshold of 3:1 is widely accepted. The B2B SaaS median is 3.2:1–3.6:1. Top-quartile companies achieve 4:1–6:1. Ratios above 5:1 may indicate the company is underinvesting in growth.

**Why Investors Care:** This ratio determines whether the company's growth model is fundamentally profitable. A ratio below 3:1 means the company loses money on each customer over time, making growth a path to bankruptcy rather than scale. Ratios above 5:1 suggest the company could afford to spend more on acquisition to capture market share faster. Investors should verify that LTV calculations use realistic churn assumptions and that CAC includes fully-loaded sales and marketing costs.

---

### 26. CAC Payback Period

**Definition:** The number of months required to recover the customer acquisition cost through the gross margin contributed by that customer. Shorter payback periods mean faster capital recovery and less reliance on external funding.

**Typical Ranges:** The 2025 median for SaaS companies is 15–20 months. The target for healthy businesses is under 12 months. Best-in-class companies achieve 6–8 month payback.

**Why Investors Care:** CAC payback directly impacts capital efficiency and fundraising cadence. A long payback period means the company must continuously raise capital to fund growth, increasing dilution and execution risk. Investors should assess whether the company has strategies to shorten payback — such as increasing pricing, improving gross margins, or targeting higher-value customer segments.

---

### 27. Rule of 40

**Definition:** The sum of a company's revenue growth rate (as a percentage) and its profit margin (typically EBITDA margin). A combined score of 40 or above indicates a healthy balance between growth and profitability.

**Typical Ranges:** Only about 20% of public SaaS companies exceed a score of 40. Scores above 60 are rare and command 2–3x higher valuation multiples.

**Why Investors Care:** The Rule of 40 provides a single-number health check that balances growth ambition with financial discipline. A company growing 50% with -10% EBITDA margin scores 40 — acceptable. A company growing 20% with 25% EBITDA margin also scores 45 — also healthy, but through efficiency. Investors use this metric to assess whether a company is operating at an appropriate point on the growth-profitability spectrum for its stage.

---

### 28. Burn Multiple

**Definition:** Net burn (cash consumed) divided by net new ARR generated in the same period. This measures how much capital the company spends to produce each dollar of new recurring revenue.

**Typical Ranges:** Below 1.5x is considered great capital efficiency. Below 2.5x is acceptable. AI-native SaaS companies typically achieve 0.8x–1.2x due to lower incremental infrastructure costs at scale.

**Why Investors Care:** Burn multiple reveals the true capital efficiency of growth. A company adding $1M in ARR while burning $3M has a 3x burn multiple — meaning it is spending three dollars of cash for every dollar of new revenue. This is unsustainable. Investors should track burn multiple over time and look for a declining trend as the company achieves operational leverage.

---

### 29. Logo Churn (Monthly)

**Definition:** The percentage of customers lost in a given month, calculated as (Customers Lost / Starting Customers) × 100. Unlike revenue churn, logo churn treats every customer equally regardless of contract size.

**Typical Ranges:** Elite companies achieve under 2% monthly logo churn. Strong performance is 3–5%. Acceptable range is 5–7%. Above 10% signals serious product or market-fit problems.

**Why Investors Care:** High logo churn among small customers can mask itself in revenue metrics if a few large accounts remain. Logo churn reveals whether the company is systematically losing customers, which will compound into revenue problems over time. Investors should segment logo churn by customer size and cohort to identify whether churn is concentrated among new customers (onboarding problem) or mature customers (product value problem).

---

### 30. ARR per Employee

**Definition:** Total annual recurring revenue divided by the number of full-time employees. This measures organizational revenue efficiency and scalability.

**Typical Ranges:** Private SaaS median is $129K–$130K per employee. Public SaaS companies average $283K. Top-quartile performers exceed $369K per employee.

**Why Investors Care:** ARR per employee reveals how efficiently the organization converts headcount into revenue. Low ratios suggest the company is overstaffed relative to its revenue generation, which becomes a margin drag as it scales. Investors should watch this metric closely during hiring sprees — rapid headcount growth without proportional ARR growth is a warning sign of operational inefficiency.

---

### 31. Activation Rate

**Definition:** The percentage of new signups or trial users who reach a defined "aha moment" or key value milestone within the product. Activation marks the transition from a prospect to an engaged user who perceives value.

**Typical Ranges:** B2B SaaS median is approximately 36%. Companies achieving above 60% activation are considered strong. Below 20% suggests fundamental onboarding or product clarity issues.

**Why Investors Care:** Activation rate is a leading indicator of future retention and expansion. Users who activate are significantly more likely to convert to paying customers and remain long-term. Low activation rates mean the company is wasting acquisition spend on users who never experience product value. Investors should understand how the company defines activation and whether it invests in onboarding optimization.

---

### 32. Time-to-Value (TTV)

**Definition:** The number of days (or hours) from initial signup or implementation to the user's first meaningful product outcome. Shorter TTV correlates with higher activation, retention, and expansion rates.

**Typical Ranges:** Simple products target under 24 hours. Complex B2B platforms may require up to one week. Products requiring more than two weeks to deliver value face significantly higher churn risk.

**Why Investors Care:** TTV is a critical lever for improving the entire customer lifecycle. Every day of delay between signup and value delivery increases the probability of abandonment. Investors should assess whether the company measures TTV, what it is, and whether there is an active initiative to reduce it. For AI startups especially, demonstrating value quickly can differentiate the product in a crowded market.

---

### 33. DAU/MAU Ratio (Stickiness)

**Definition:** The ratio of Daily Active Users to Monthly Active Users. This measures how habit-forming the product is — a higher ratio means users engage frequently rather than sporadically.

**Typical Ranges:** B2B SaaS median is approximately 13%. Products achieving above 25% are considered sticky. Consumer products typically target 50%+.

**Why Investors Care:** Stickiness is a strong predictor of retention. Products that users engage with daily or near-daily create deeper integration into workflows and higher switching costs. For AI startups, daily usage also means more data generation, fueling the data flywheel. Investors should segment this metric by customer tier to understand whether stickiness varies by product plan or use case.

---

### 34. Product-Market Fit Score

**Definition:** Measured using the Sean Ellis test — surveying users on how they would feel if they could no longer use the product. The percentage responding "very disappointed" serves as the product-market fit indicator.

**Typical Ranges:** Above 40% "very disappointed" responses indicates product-market fit has been achieved. Below 20% suggests the product has not yet found a strong market need.

**Why Investors Care:** Product-market fit is the single most important milestone for early-stage companies. Without PMF, scaling go-to-market efforts is pouring money into a leaky bucket. Investors should treat PMF as a prerequisite for significant growth investment and verify the score through direct customer surveys rather than proxy metrics.

---

### 35. NPS (Net Promoter Score)

**Definition:** The percentage of promoters (users who would rate the product 9–10 on a recommendation scale) minus the percentage of detractors (users who would rate it 0–6). NPS measures overall customer sentiment and willingness to advocate for the product.

**Typical Ranges:** B2B SaaS median is approximately 29. Scores above 50 are considered excellent. Negative NPS signals widespread customer dissatisfaction.

**Why Investors Care:** NPS is a leading indicator of retention, expansion, and organic growth through referrals. Companies with high NPS benefit from word-of-mouth acquisition, reducing CAC. Investors should look at NPS trends over time and segment by customer cohort to identify whether satisfaction is improving or deteriorating among newer customers.

---

## Section 3: General Business / Financial Metrics

### 36. Revenue Growth Rate (YoY)

**Definition:** The year-over-year percentage increase in total revenue. This measures the pace at which the company is scaling its top line and is the primary signal of market traction and demand.

**Typical Ranges:** Top-quartile early-stage companies achieve 300%+ YoY revenue growth. The SaaS industry median is approximately 25%. Growth rates naturally decelerate as the revenue base expands, so context around stage and absolute revenue matters.

**Why Investors Care:** Revenue growth is the most visible and scrutinized metric in any investment thesis. It demonstrates whether the market wants the product and whether the company can capture demand. For AI startups especially, rapid growth can offset concerns about lower initial margins by demonstrating the path to scale. Investors should examine the quality of growth — is it driven by new logos, expansion revenue, or pricing increases? — and whether the growth is sustainable given the total addressable market.

---

### 37. Gross Margin

**Definition:** The percentage of revenue remaining after subtracting the cost of goods sold (COGS), calculated as (Revenue − COGS) / Revenue × 100. This measures the inherent profitability of each dollar of sales before operating expenses.

**Typical Ranges:** Traditional SaaS targets 70–85% gross margins. AI startups typically achieve 50–70% in early stages due to higher compute costs. Margins should show an improving trajectory as the company optimizes its cost structure.

**Why Investors Care:** Gross margin sets the ceiling for overall profitability. Even the best go-to-market execution cannot compensate for structurally low margins. For AI companies, the key question is whether gross margins will expand toward traditional SaaS levels over time through compute optimization, model efficiency gains, and pricing power. Investors should demand a credible margin expansion plan and monitor quarterly trends closely.

---

### 38. EBITDA Margin

**Definition:** Earnings before interest, taxes, depreciation, and amortization, expressed as a percentage of revenue. This provides a view of operating profitability stripped of financing decisions, tax regimes, and non-cash accounting items.

**Typical Ranges:** The SaaS industry average is approximately 29–30%. Margins above 30% are considered strong. Each 10-percentage-point improvement in EBITDA margin correlates with roughly 1.1x higher EV/Revenue multiples.

**Why Investors Care:** EBITDA margin reveals whether the company's core operations are profitable after accounting for all operating expenses. For growth-stage companies, negative EBITDA is common and acceptable if growth rates are high, but the trajectory should trend positive. Investors should assess whether the company has a clear path to positive EBITDA and at what revenue scale it becomes achievable.

---

### 39. Free Cash Flow (FCF)

**Definition:** Operating cash flow minus capital expenditures. FCF represents the actual cash the company generates after funding its operations and maintaining its asset base. Positive FCF indicates the business can self-fund its growth.

**Typical Ranges:** Early-stage companies typically operate at negative FCF as they invest heavily in growth. Mature companies should achieve positive FCF. The transition point varies by business model.

**Why Investors Care:** Positive free cash flow is the ultimate profitability signal. It means the company generates more cash than it consumes, enabling self-funded growth, debt repayment, shareholder returns, and reduced dilution from future fundraising. For AI startups with high compute costs, achieving positive FCF is particularly significant and commands premium valuations. Investors should model the FCF inflection point and assess whether it is achievable within a reasonable timeframe.

---

### 40. Gross Burn Rate

**Definition:** The total monthly operating expenses incurred by the company, including payroll, office rent, cloud infrastructure, sales and marketing spend, R&D, and general and administrative costs. This represents the total cash outflow before any revenue is considered.

**Typical Ranges:** Varies widely by company size and stage. Seed-stage companies may burn $20K–$100K/month. Series B companies commonly burn $500K–$2M/month.

**Why Investors Care:** Gross burn rate establishes the baseline cash consumption of the business. Combined with the cash balance, it determines runway. Investors should scrutinize the composition of burn — a high proportion allocated to revenue-generating activities (sales, product development) is preferable to excessive G&A or unproductive overhead. Rapid increases in gross burn without corresponding revenue growth are a warning sign.

---

### 41. Net Burn Rate

**Definition:** Gross burn rate minus monthly revenue. This represents the actual net rate at which the company is consuming cash each month, accounting for the revenue that partially offsets expenses.

**Typical Ranges:** Negative net burn (i.e., the company generates more revenue than it spends) is the target for mature companies. Growth-stage companies typically operate at positive net burn.

**Why Investors Care:** Net burn is the key input for runway calculations and fundraising timing. A declining net burn rate signals improving unit economics and a path to self-sufficiency. Investors should track net burn trends and ensure the company has a realistic plan to reduce it. Sudden spikes in net burn — from hiring accelerations, pricing pressure, or compute cost increases — should trigger immediate investigation.

---

### 42. Cash Runway

**Definition:** The number of months the company can continue operating at its current net burn rate before exhausting its cash reserves, calculated as Cash Balance / Net Monthly Burn.

**Typical Ranges:** The target at the time of a funding raise is 18–24 months of runway. Below 12 months requires active fundraising. Below 6 months is considered an emergency situation.

**Why Investors Care:** Cash runway determines the company's time horizon for achieving milestones and its negotiating position in future fundraising. Running out of cash forces distressed financing on unfavorable terms or forces the company into shutdown. Investors should monitor runway continuously, stress-test it against downside scenarios, and ensure the company begins fundraising well before runway drops below 12 months.

---

### 43. LTV (Customer Lifetime Value)

**Definition:** The total gross profit a single customer generates over the entire duration of their relationship with the company. Calculated as (Average Revenue Per Account × Gross Margin %) / Monthly Churn Rate.

**Typical Ranges:** Varies widely by pricing, margins, and retention. The key benchmark is the LTV:CAC ratio (see metric #25), where LTV should be at least 3x CAC.

**Why Investors Care:** LTV determines how much the company can profitably spend to acquire each customer. Higher LTV enables greater investment in sales and marketing, fueling faster growth. For AI startups, LTV is particularly sensitive to churn assumptions — a small increase in churn can dramatically reduce LTV. Investors should verify that LTV calculations use conservative churn rates and realistic gross margin projections.

---

### 44. CAC (Customer Acquisition Cost)

**Definition:** The total sales and marketing spend divided by the number of new customers acquired in the same period. CAC should be fully loaded, including sales and marketing salaries, commissions, advertising spend, tools, and overhead allocations.

**Typical Ranges:** Varies by market, pricing, and sales model. The critical benchmark is CAC relative to LTV (see metric #25) and the CAC payback period (see metric #26).

**Why Investors Care:** CAC determines the efficiency of the company's go-to-market engine. Rising CAC can signal market saturation, increased competition, or declining marketing effectiveness. Investors should examine CAC trends over time, segment CAC by channel to identify the most efficient acquisition paths, and ensure that CAC calculations include all relevant costs rather than just advertising spend.

---

### 45. Magic Number

**Definition:** Net new ARR generated in the current quarter divided by sales and marketing spend in the previous quarter. This measures the return on each dollar of go-to-market investment.

**Typical Ranges:** A magic number above 0.75 is considered healthy. Above 1.0 indicates the company is generating more than a dollar of new ARR for every dollar spent on sales and marketing — potentially meaning the company could afford to spend more to accelerate growth.

**Why Investors Care:** The magic number isolates go-to-market efficiency from other operational factors. A declining magic number suggests the company is paying more for each dollar of new revenue, which may indicate market saturation or competitive pressure. A magic number above 1.0 signals strong operational leverage and the potential to accelerate growth by increasing S&M investment. Investors should track this metric quarterly and compare it to industry benchmarks.

---

### 46. EV/Revenue Multiple

**Definition:** Enterprise value (market capitalization plus debt minus cash) divided by total revenue. This is the primary valuation metric used for growth companies, expressing how much the market is willing to pay for each dollar of revenue.

**Typical Ranges:** AI companies currently trade at 6.2x–22.8x revenue multiples. Traditional SaaS companies trade at 16x–20x. Multiples vary significantly based on growth rate, profitability, market position, and macro conditions.

**Why Investors Care:** The EV/Revenue multiple determines the potential return on investment at exit. Higher multiples reward faster growth, stronger margins, and more defensible market positions. Investors should benchmark the company against comparable public and private transactions and understand which factors — growth rate, margin profile, market size — drive the multiple expansion or compression.

---

### 47. TAM (Total Addressable Market)

**Definition:** The total revenue opportunity available if the company achieved 100% market share in its target market. TAM sets the ceiling for the company's revenue potential and informs the scale of the opportunity.

**Typical Ranges:** Venture capital investors typically expect category-defining startups to address a $1B+ TAM. Smaller markets can support successful companies but may cap the upside for investors seeking 10x+ returns.

**Why Investors Care:** TAM determines whether the company can grow large enough to deliver the returns investors require. A small TAM means even dominant market share produces limited revenue. Investors should assess whether the company's TAM calculation is realistic, whether the addressable market is expanding (e.g., AI adoption creating new demand), and whether the company has a credible strategy to capture a meaningful share.

---

### 48. Revenue Concentration

**Definition:** The percentage of total revenue derived from the company's largest customer or a small group of customers. High concentration means the loss of a single customer would materially impact the business.

**Typical Ranges:** More than 20% of revenue from a single customer is considered a material risk factor. Well-diversified companies have no single customer exceeding 5–10% of revenue.

**Why Investors Care:** Revenue concentration creates existential risk. Losing a major customer can trigger cash flow crises, valuation write-downs, and loss of investor confidence. Investors should examine the top-10 customer concentration, the contractual security of large accounts (multi-year contracts vs. month-to-month), and the company's strategy for diversifying its customer base.

---

### 49. S&M as % of Revenue

**Definition:** Total sales and marketing expenses expressed as a percentage of total revenue. This measures how much of each revenue dollar is being reinvested into customer acquisition and brand building.

**Typical Ranges:** Early-stage companies typically spend 40–60% of revenue on S&M as they build their customer base. Mature companies target 20–30%. A declining S&M percentage signals operational leverage — the company is generating more revenue from each dollar of marketing spend.

**Why Investors Care:** S&M intensity reveals the company's growth investment strategy and go-to-market efficiency. Persistently high S&M spend as a percentage of revenue suggests the company cannot grow profitably without continuous marketing investment. A declining trend indicates the company is achieving scale and operational leverage. Investors should compare S&M intensity to peers and assess whether the level is appropriate for the company's growth stage.

---

### 50. Efficiency Score

**Definition:** Net new ARR generated divided by the sum of sales & marketing, R&D, and G&A expenses. This measures how much new recurring revenue each dollar of total operating expense generates.

**Typical Ranges:** An efficiency score above 0.5 is considered good. Scores above 1.0 indicate the company is generating more new recurring revenue than it spends on operations — a sign of exceptional capital efficiency.

**Why Investors Care:** The efficiency score provides a holistic view of how well the company converts operating spend into revenue growth. It combines go-to-market effectiveness (S&M), product investment (R&D), and organizational overhead (G&A) into a single metric. Companies with high efficiency scores can grow faster with less capital, reducing dilution and extending runway. Investors should track this metric over time and use it to compare capital efficiency across portfolio companies.

---

## Conclusion

These 50 metrics provide a comprehensive framework for evaluating AI startups across three dimensions: AI-specific unit economics and technical risk, SaaS operational health, and general business and financial fundamentals. No single metric tells the whole story — investors should assess them as an interconnected system where weakness in one area can compound problems in another.

For AI startups specifically, the interplay between compute costs, data moats, and traditional SaaS metrics creates a unique evaluation landscape. Companies that demonstrate strong AI-specific fundamentals alongside healthy SaaS and financial metrics represent the most compelling investment opportunities.

---

*Research and development performed by **Von AI**. [LinkedIn profile of the developer](https://www.linkedin.com/in/warren-harding-29a0a673).*
