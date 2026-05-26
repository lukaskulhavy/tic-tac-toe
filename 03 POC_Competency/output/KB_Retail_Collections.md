# Knowledge Base: Retail Collections

**Source document:** ABC Collections Guideline, Version 2.0 (Sberbank Europe, 11 July 2013)  
**Extracted:** 2026-05-26  
**Domain:** Retail Banking – Credit Risk / Collections  
**Audience:** Consultants (junior through senior)

---

> **About this document**
> The source is a 2013 group-level guideline from Sberbank Europe. The core framework — lifecycle stages, segmentation logic, communication escalation, KPI design, legal process flow — remains largely sound practice. However, several sections reference outdated technology, governance structures, and regulatory contexts. Each such item is flagged inline with a `⚠️ OUTDATED` callout, and a consolidated list appears in the final appendix.
>
> Sberbank Europe as a legal entity no longer exists following the 2022 divestiture tied to EU/US sanctions on Russia. Any references to "SBEU approval" or "group policy" are therefore obsolete governance references. The underlying operational knowledge is independent of that context.

---

## Table of Contents

1. [Key Terms & Glossary](#1-key-terms--glossary)
2. [Collections Lifecycle Overview](#2-collections-lifecycle-overview)
3. [Portfolio Scope and Segmentation](#3-portfolio-scope-and-segmentation)
4. [Communication Channels & Templates](#4-communication-channels--templates)
5. [Collection Tools — Pre-Collections Stage](#5-collection-tools--pre-collections-stage)
6. [Collection Tools — Early Collections (1–90 DPD)](#6-collection-tools--early-collections-190-dpd)
7. [Collection Tools — Late Collections (90–180 DPD)](#7-collection-tools--late-collections-90180-dpd)
8. [Collection Tools — Workout Stage (180+ DPD)](#8-collection-tools--workout-stage-180-dpd)
9. [KPIs, Metrics & Reporting](#9-kpis-metrics--reporting)
10. [Organisation & Human Resources](#10-organisation--human-resources)
11. [Technology & Systems Considerations](#11-technology--systems-considerations)
12. [Appendix: Consolidated List of Outdated Items](#12-appendix-consolidated-list-of-outdated-items)

---

## 1. Key Terms & Glossary

| Term | Definition |
|------|-----------|
| **DPD** | Days Past Due — number of days since a payment was missed |
| **TPD** | Technical Past Due — total days since client first entered collections, regardless of partial payments |
| **Bucket** | A 30-day band of delinquency (Bucket 1 = 1–30 DPD, Bucket 2 = 31–60 DPD, etc.) |
| **EC** | Early Collections (1–90 DPD) |
| **LC** | Late Collections (90–180 DPD) |
| **WO** | Workout (180+ DPD, post-termination) |
| **PTP** | Promise-to-Pay — agreed commitment from the client to pay a defined amount by a defined date |
| **RPC** | Right Party Contact — the person legally entitled to make commitments on the debt (debtor, co-debtor, guarantor) |
| **CCPE** | Collections Clients Per Employee — benchmark for how many unique clients one collector handles per month |
| **Spin Rate** | Total call attempts divided by unique eligible clients — how often each client is dialled on average |
| **Contact Rate** | Total contacts / total attempts |
| **RPC Rate** | Right party contacts / total contacts |
| **Promise Rate** | PTPs taken / RPCs reached |
| **Kept Rate** | Kept PTPs / taken PTPs |
| **Conversion Rate** | Kept PTPs / total attempts (product of all pyramid rates) |
| **GINI coefficient** | Measure of how well a segmentation model separates good from bad clients (higher = better discrimination) |
| **VaR (Collections)** | Value at Risk = Probability of reaching next stage × Exposure |
| **FPD / SPD / TPD** | First / Second / Third Payment Default |
| **Lazy Payer** | Client who has entered collections 3+ times in last 6 months but max DPD is always <20 |
| **EXA** | External Collections Agency |
| **VAS** | Voluntary Asset Sale — client voluntarily sells collateral with bank supervision |
| **OTI** | Obligations to Income = all income minus all expenses; shows monthly cash flow balance |
| **DTI** | Debt-to-Income = all debt installments / total household income |
| **NPL** | Non-Performing Loan (typically 90+ DPD) |
| **CBS** | Core Banking System |
| **LLP** | Loan Loss Provisions |
| **FIFO** | First-In-First-Out (preferred DPD methodology) |
| **LIFO** | Last-In-First-Out (alternative DPD methodology, requires approximation strategy) |
| **Champion vs. Challenger** | Testing a newly proposed process (challenger) against the existing one (champion) |
| **Vintage** | Group of accounts entering the same delinquency status in the same time period |

---

## 2. Collections Lifecycle Overview

### 2.1 The Four Stages

```
 0 DPD ──────── 1 DPD ─────────────── 90 DPD ──────────── 180 DPD ──────────────►
│                │                    │                    │
│  Pre-Collections│  Early Collections │  Late Collections  │  Workout
│  (0 to -5 DPD) │  (1–90 DPD)        │  (90–180 DPD)      │  (180+ DPD)
│                │                    │                    │
```

**Pre-Collections (0 to −5 DPD)**
- Identify clients at risk before they miss a payment
- Sole tool: pre-collections SMS reminder
- Goal: reduce inflow into Bucket 1

**Early Collections (1–90 DPD)**
- Buckets 1–3 (each 30 days)
- Goal: recover arrears, return client to 0 DPD
- Tools: Intense Communication, Repayment Plan, Salary Pledge, Insurance, EXA

**Late Collections (90–180 DPD)**
- Buckets 4–6
- Goal: stabilise the client, maximise recoveries
- Tools: Credit Counseling, Restructuring, Voluntary Asset Sale + Residual Settlement, EXA

**Workout (180+ DPD)**
- Post-termination
- Goal: recover maximum of the total outstanding balance
- Tools: Termination, Pre-Legal, Legal Prosecution, Debt Settlement, Debt Sale, Write-Off

### 2.2 Client Flow Logic

Client progression is driven by two variables: **Ability to pay** and **Willingness to pay**.

| Ability | Willingness | Recommended Tools |
|---------|-------------|-------------------|
| No | No | Insurance, Termination, Pre-Legal, Legal, Debt Sale |
| No | Yes | Insurance, Credit Counseling, Restructuring, VAS, Debt Settlement, Debt Sale |
| Yes | No | Salary Pledge, Insurance, EXA, Termination, Pre-Legal, Legal, Debt Sale |
| Yes | Yes | Intense Communication, Repayment Plan, EXA, Credit Counseling |

### 2.3 Acceleration (Early Escalation)

Clients can be accelerated to a later stage before their DPD normally warrants it. Justified reasons include:

| Trigger | Acceleration Tool |
|---------|------------------|
| Non-contactable >30 days | EXA, Field Visits |
| Client requests different treatment | Credit Counseling, Restructuring, VAS |
| Reduced income (salary cut, job loss) | Credit Counseling, Restructuring, VAS, Pre-Legal |
| Non-cooperative | EXA, Field Visits, Legal, Termination |
| Confirmed fraud | Legal Prosecution |
| 3 broken PTPs in a row | EXA, Field Visits |
| 3rd-party execution in place | Pre-Legal, Legal, Debt Settlement, Debt Sale |

---

## 3. Portfolio Scope and Segmentation

### 3.1 Target Portfolio

Collections covers **two retail client groups**:
1. **Private individuals** — standard retail
2. **Micro clients** — enterprises or individuals with <10 employees and <€2M annual turnover

All clients are handled at **client level** (not account level) to reduce cost and avoid fragmented communication.

Product types in scope: current accounts & overdrafts, credit cards, consumer/cash loans, car loans, mortgages, housing loans.

### 3.2 Special Portfolio Categories

**Special cases** (VIP, deceased, employees, fraud suspects) are handled separately and typically accelerated to later stages or handed to fraud teams directly.

**Co-debtors and guarantors** bear equal responsibility; they enter collections if the primary debtor fails to cooperate. The client should be warned before contacting co-debtors/guarantors.

**Clients below threshold** (€10 for individuals; €20 for micro clients): minimum-touch treatment (typically 2 SMS), then early write-off.

**Micro clients**: Must be transferred to specialist collectors no later than 31 DPD. Analysis focuses on expected cash flows and balance sheet liquidity rather than personal finance.

### 3.3 Segmentation in Early Collections

The goal of segmentation is to predict which clients will reach the next DPD milestone, so collection intensity can be calibrated efficiently.

**Segmentation timing:** At minimum at entry (1–5 DPD). Best practice: re-segment at the start of each bucket.

**Risk classes:** At minimum High and Low; ideally also Medium.

**Two approaches:**

**A. Statistical (Model-Based) — Preferred**
- Uses Logistic Regression or Classification & Regression Trees (C&RT)
- Requires: DWH with 20,000+ historical cases across 3+ consecutive months, statistical tooling, daily flag-carrying capability in the collections system

> ⚠️ **OUTDATED — Technology:** The document cites SAS Enterprise Miner and Microsoft SQL Analytical Services as representative tools. These were standard in 2013 but the industry has largely shifted to Python (scikit-learn, XGBoost, LightGBM), R, and cloud ML platforms (Databricks, Azure ML, AWS SageMaker). The minimum case count (20,000) is also conservative by modern standards — gradient boosting models often outperform logistic regression with fewer cases, and transfer learning approaches can bootstrap new portfolios.

> ⚠️ **OUTDATED — Model types:** Only Logistic Regression and C&RT are mentioned. Current best practice includes gradient boosting (XGBoost, LightGBM), Random Forests, and increasingly neural networks / deep learning for collections propensity scoring. Real-time, API-served models replacing batch monthly runs are now standard in well-equipped banks.

**B. Expert-Based — Acceptable as Interim**
- Segmentation by observable attributes: DPD, product type, collateral, outstanding volume, reachability, past delinquencies, insurance status, etc.
- Done by pivot-table analysis of historical roll rates
- Acceptable temporarily while statistical capability is being built

**Segmentation variables in scope:**
- Ticket size (micro tickets <€50, high tickets = top 10% by balance)
- Lazy payer flag (3+ collections episodes in 6 months, max DPD <20)
- Current DPD / historical max DPD
- Collateral status (secured vs. unsecured)
- FPD / SPD / TPD (1st, 2nd, 3rd payment default)
- Time on book (<12 months)
- Recent restructuring (<12 months ago)

**Call list prioritisation** (mandatory parameters, in order):
1. DPD
2. Exposure
3. (Optional) Value at Risk = P(reaching next stage) × Exposure

### 3.4 Segmentation Monitoring

Three reports required to re-validate models:

| Report | Purpose |
|--------|---------|
| **Segment Size Report** | Monitors that segment proportions remain stable vs. original model |
| **Segment Performance Report** | Measures whether High/Medium/Low risk clients behave as predicted |
| **GINI Report** | Tracks predictive power over time; decline signals need to recalibrate |

All models must be re-validated at least **annually**.

---

## 4. Communication Channels & Templates

### 4.1 Core Channels (Mandatory for All Banks)

| Channel | Role | Key Rules |
|---------|------|-----------|
| **Telephone (outbound)** | Primary PTP capture tool; most effective | Every call must be logged with: officer ID, client ID, result, date, next action. RPC must be verified before any data shared. |
| **SMS** | Low-cost first touch; reminders; PTP follow-up | Automated send with delivery receipt required. Inbound-reply PTP possible via gateways. |
| **Letter** | Escalation; formal notification; reach non-contactable clients | Use registered mail with delivery receipt when all other channels fail. Automate generation to avoid distracting call officers. Fee may be charged to client (check local regulation). |

### 4.2 Additional Channels (Use Where Applicable)

| Channel | Notes |
|---------|-------|
| **IVR** (Interactive Voice Response) | Allows clients to self-serve; reduces call centre load. Callback option should be available. |
| **AVM** (Automated Voice Messaging) | Efficient for mass outreach; leaves a recorded message when client does not answer |
| **E-banking / Internet Banking** | Pop-up or inbox message when client logs in |
| **ATM** | Pop-up screen message when client uses ATM |
| **Bank statements** | Delinquency notice on monthly statement |
| **E-mail** | Used in LC for Credit Counseling and VAS document exchange; limited use in EC due to skip-tracing impossibility |
| **Field Visit / Meeting** | Most effective but most expensive; always conducted by two employees; good for non-contactable and high-ticket clients |

> ⚠️ **OUTDATED — Missing channels:** The document was written before the mainstream adoption of mobile banking apps, WhatsApp for Business, AI chatbots, push notifications, and in-app messaging. These are now primary channels in many collections operations, particularly for early-stage contacts and self-service repayment. Any modern collections strategy design must include a digital-first channel layer.

> ⚠️ **OUTDATED — IVR and AVM:** While IVR is still used, it is being rapidly replaced or augmented by AI-powered voice bots (conversational AI) that handle full collections dialogue without human agents. These can take authenticated PTPs, offer restructuring, and transfer to live agents for complex cases.

> ⚠️ **OUTDATED — ATM messages:** ATM-initiated collections messaging is largely obsolete. Mobile app push notifications are more effective, less intrusive, and have far higher open rates.

### 4.3 Communication Strategy by Segment and Bucket

- Low-risk clients: start calls later (up to 10 DPD); exhaust SMS/letter before calling
- High-risk clients: first call no later than Day 5 of delinquency
- Intensity and tonality must escalate bucket by bucket:

| Bucket | Tone | Approach |
|--------|------|---------|
| 1 (1–30 DPD) | Polite, friendly | Treat as accidental; explain remedy |
| 2 (31–60 DPD) | Official | Describe consequences; soft warning |
| 3 (61–90 DPD) | Formal, direct | Explicit threat of next steps; short sentences |

### 4.4 Communication Templates

- Personalised templates for written communication (name, contract number, due amount, due date, bank contact)
- Call scripts standardised by bucket and product type to ensure consistency, reduce wrap-up time, and lower operator stress
- All templates must be internally approved and version-controlled
- Templates for: SMS, letter, AVM, email, call scripts, field visit checklists

### 4.5 Call Recording and Data Logging

- Record outcome of every call: inbound/outbound, phone type (mobile/landline), respondent type (debtor/guarantor/other), result (PTP amount+date, new contact info, refusal reason)
- Standardised "Reason for Delinquency" codes must be maintained (see Section 9 for full list)

### 4.6 Prime Time Analysis

Identifying peak contact hours increases contactability significantly. Method:
1. Extract call time-of-day data from collections tool or manually track for ≥1 month
2. Group by time slot; identify slots with highest connect rate
3. Shift calling activity and FTE schedules to align with peak hours
4. Consider Saturday shifts if connect rates are higher on weekends

### 4.7 Skip Tracing

Skip tracing is the process of finding missing or invalid contact details.

**Triggers for skip tracing:**
- Client has no contact data in system
- Phone number is technically invalid (wrong digit count, invalid prefix)
- Client is registered but unreachable for a predefined period

**Sources for contact discovery:**
1. Internal bank systems and files
2. Web, search engines, open databases, social networks
3. Relatives and neighbours (with care — GDPR implications)
4. Employers
5. Yellow pages
6. Mobile network operators
7. Population registers
8. Loan registers / credit bureaux
9. Health insurances
10. Motor vehicle registers

> ⚠️ **OUTDATED — GDPR:** The document predates GDPR (2018). Several skip tracing methods listed (social networks, contacting relatives, population registers) are subject to strict data minimisation, purpose limitation, and lawful basis requirements under GDPR. Before implementing any skip tracing process in the EU/EEA, legal review against GDPR Articles 5, 6, and 9 is mandatory. The document's language around data sharing with EXAs also requires GDPR Article 28 compliant Data Processing Agreements.

---

## 5. Collection Tools — Pre-Collections Stage

### Pre-Collections Reminder (Optional Tool)

**Purpose:** Identify current clients (0 DPD) who are at risk of missing their next payment, and send a timely service-style reminder before the due date.

**Key characteristics:**
- Triggered 3–5 days before due date
- Communication is a service message, not a collections message — the client must not feel they are being "collected"
- Fully automated — no manual intervention; SMS is the standard channel
- Requires a predictive model (statistical or expert-based) re-validated annually

**Typical segmentation predictors:**
| Predictor | Signal |
|-----------|--------|
| New loans | 1st, 2nd, or 3rd payment since disbursement |
| Restructured loans | Recent change in payment conditions |
| Previous delinquencies | >30 DPD episode in last 6 months |
| Account balance vs. average | End-of-month balance 30% below 6-month average |
| Account balance vs. upcoming payment | Insufficient funds 3 days before due date |
| Credit turnover change | 50%+ drop in monthly inflow |
| Employer type / NACE code | Industry with known difficulties |
| Employer name | Specific employer known to be in financial distress |
| External negative data | Credit bureau flags |

**Exclusions:** Clients with active Salary Pledge; clients whose salary date is after their payment due date.

**Success measurement:**
- Compare inflow rate of treated group vs. untreated test group
- Net benefit must exceed SMS campaign costs to justify continuation

---

## 6. Collection Tools — Early Collections (1–90 DPD)

### 6.1 Intense Communication

**Purpose:** Core early-stage tool to obtain PTPs and bring clients back to 0 DPD through escalating outbound contact.

**Key parameters:**
- PTP minimum amount: 1/3 of original installment (or 1/3 of past due if installment not set)
- Maximum PTP window: 5 working days
- Reminder SMS sent 2 days before PTP due date
- If PTP not kept (below 90% paid): follow up within 2 days after due date
- 3 broken PTPs in a row → escalate client
- "On Hold" status used when client cannot pay within 5 days but commits to a future date

**Call centre operations:**
- Centralised call centre; inbound + outbound handled by same team
- Auto-dialler strongly recommended (progressive or predictive — see Section 11)
- High-risk: first call no later than Day 5. Low-risk: Day 10 acceptable.

### 6.2 Salary Pledge (Mandatory Where Legally Possible)

**Purpose:** Bind the employer to deduct and transfer part of the client's salary directly to the bank, on a regular basis.

**When activated:**
- Early collections (if law/contract allows): typically Bucket 2–3
- Late/Workout (via court execution order) if not contractually enabled earlier

**Process flow:**
1. Verify employment status (public register, pension fund, or employer call — optional)
2. Send formal letter to employer with Salary Pledge claim and legal basis
3. Follow up by phone if no response after normal postal delivery window
4. Monitor ongoing payments; terminate pledge when debt is cleared

**Applies equally to co-debtors and guarantors.**

**Note on limits:** Maximum pledge amount is set by local law (typically the salary portion above living expenses minimum).

### 6.3 Insurance Claim

**Purpose:** Transfer the overdue account to the insurance company when minimum collections conditions (as specified in the bank-insurer contract) have been met. Insurance company repays the outstanding; client becomes the insurer's account.

**Key rules:**
- Minimum collections activities defined in bank-insurer SLA must be fulfilled before claim
- Claim submission: batch monthly; prepare within 3 days, send within 2 days
- Claim deadline: typically by 300 DPD
- Bank must monitor payments from former insured clients in case funds come to bank account instead of insurer's account

**Strategic note:** Consider whether additional collections steps (beyond minimum requirements) are economically worthwhile before transferring. Factor in premium cost, administrative cost of claim, and recovery potential of each incremental call.

### 6.4 External Collection Agency (EXA)

**Purpose:** Outsource collection to a specialised agency for cases where the agency has a structural advantage (field access, skip tracing databases, cost efficiency, or psychological impact of an external collector).

**Three valid reasons to use EXA:**
1. EXA can do something the bank cannot (field visits at scale, large contact databases)
2. EXA does what the bank does, but cheaper/better
3. Bank lacks capacity and needs to offload volume

**Target cases for EXA:**
- Early collections: primarily non-contactable cases
- Late collections: cases resistant to internal process, typically lower-ticket unsecured debt

**Best practice — multiple EXA competition model:**
- Maintain 3 active EXAs simultaneously + 1 in backup ("3+1 rule")
- Allocate more volume to best-performing EXA
- Replace weakest performer with backup agency after each evaluation period
- Compare EXA results at least annually against internal performance or a competing EXA

> ⚠️ **OUTDATED — Governance reference:** The document ties the 3+1 rule decision to Sberbank Europe approval. This governance layer no longer exists. The operational principle (structured competition between EXAs) remains sound best practice.

**Key contract requirements with EXA:**
- Scope of services, data protection (GDPR-compliant DPA post-2018), communication standards, SLA, escalation process, commission structure, jurisdiction
- Weekly data exchange: updated outstanding, new contact data, activity logs, collections results
- Feedback report to EXA within 2 weeks of portfolio return
- Cases monitored for 1 week post-return to capture delayed payments

### 6.5 Repayment Plan

**Purpose:** Allow a cooperative client to repay accumulated arrears in installments added on top of their regular payment, without modifying the original contract (unlike Restructuring).

**Key characteristics:**
- Original contract terms remain unchanged
- Overdue amount is divided into additional periodic payments
- Multiple PTPs per month may be used
- Confirmation letter sent to client upon agreement
- Does **not** result in a "restructured" classification on the client record

**When to use:** Clients who are cooperative and have sufficient income to service both the regular installment and an extra repayment amount.

---

## 7. Collection Tools — Late Collections (90–180 DPD)

### 7.1 Credit Counseling (CC)

**Purpose:** Personal, analysis-driven engagement with the client to identify the best financial solution given their actual household situation.

**Core analysis dimensions:**
- **OTI (Obligations to Income):** total income minus total expenses — reveals monthly cash flow surplus/deficit
- **DTI (Debt-to-Income):** total debt installments / total household income — shows debt servicing burden

**Output decision tree:**

| Client Situation | Tool |
|------------------|------|
| Can service all debts independently | Promise to Pay (for full past-due amount) |
| Needs slight adjustment | Repayment Plan or Restructuring |
| Cannot service debt even with adjustment | Voluntary Asset Sale, Successor, Any Asset Sale, Termination |

**Delivery options:**
- Field visit (most effective but most expensive; allows property inspection)
- Bank branch meeting
- Phone call (cheapest; lower contact rate)

**Staffing requirement:** Skilled counselors assigned personally to each client for the full CC engagement.

### 7.2 Restructuring

**Purpose:** Modify the client's loan contract to restore regular payment capability by reorganising the repayment schedule.

**Six restructuring mechanisms (can be combined):**
1. Tenure extension — longer repayment period lowers monthly installment
2. Grace period — temporary payment holiday (principal or full installment)
3. Interest rate reduction — temporary or permanent
4. Bullet payment deferral — principal deferred to end of term
5. Debt consolidation — multiple loans merged into one
6. Combination of the above

**Additional securitisation often required as a condition:**
- New collateral pledge
- Salary Pledge (if not already in place)
- Adding a guarantor or co-debtor
- Creating a salary account at the bank
- Arbitration clause

**Process:**
1. Financial analysis (thorough via CC, or brief if CC not done)
2. Offer pre-calculated solution options to client
3. Require first "testing installment" payment before drawing up new contract — confirms client's willingness
4. Execute contract amendment only after testing payment received

**KPI:** Successfully closed cases; quality = 30+DPD at 3 months post-restructuring.

### 7.3 Voluntary Asset Sale (VAS) + Residual Settlement

**Purpose:** Supervised voluntary sale of collateral by the client, typically for mortgage/property-secured loans, to recover debt without litigation.

**Three stages:**
1. **Persuasion** — Contact client, explain alternatives, build relationship, overcome psychological barrier of selling property
2. **Remarketing** — Price setting via contracted real estate agency; promotion; client prepares property; agency conducts viewings
3. **Sales management** — Monitor sale progress; apply price decrease mechanism if necessary; after-sale settlement

**Price decrease mechanism:** Property price may not be decreased more frequently than every 3 months. Maximum per-decrease: up to 7% of market value.

**Appraisal:** New professional appraisal required (not older than 6 months). Liquidation price (minimum acceptable) must also be defined. Appraisal cost is charged to client only if client becomes uncooperative; otherwise the bank bears the cost.

**Residual Settlement:** When sale proceeds do not fully cover the outstanding debt, the bank may forgive part of the unsecured residual balance in exchange for the client repaying the remainder. Discount level is typically the highest offered in the entire collections process (clients with sold collateral rarely have resources for residual repayment). Requires Management Board approval.

---

## 8. Collection Tools — Workout Stage (180+ DPD)

### 8.1 Termination

**Purpose:** Formally declare the entire outstanding balance (not just arrears) immediately due and payable by ending the contract.

**Key parameters:**
- Selection for termination begins at approximately **160 DPD** (pre-selection and warning)
- Formal termination at approximately **180 DPD**
- Clients are sent a formal warning letter before termination
- Phone follow-up for above-threshold balances if letter receives no response
- Termination is **irreversible** — from this point, focus shifts entirely to recovery

**Important:** Turning a terminated loan back into a new loan to "restructure" is explicitly not acceptable. Small unsecured, low-ticket clients may be selected for termination directly after Early Collections.

> ⚠️ **NOTE — Regulatory variation:** Termination procedures are governed by local Central Bank regulations and vary significantly by country. The specific triggers and notification requirements described here are indicative minimums; local legal review is always required.

### 8.2 Pre-Legal

**Purpose:** One final escalation step after termination, before committing to full legal proceedings. Aim is to reduce the volume of cases entering court.

**Eligible cases:**
- **Group 1:** Exposure clearly justifies legal costs (secured loans, high-value unsecured)
- **Group 2:** High exposure but legal proceedings not planned; serious communication to extract payment
- **Group 3:** Below materiality threshold → not eligible for pre-legal treatment; skip directly to lower-cost resolution

**Process:**
1. Pre-legal letter (different layout from regular collections letters; may carry external law firm branding)
2. Deadline: client must pay full outstanding within 14 working days
3. If client proposes extended repayment and pays ≥10% of outstanding upfront → accelerate to Settlement (but no discount at this stage)

### 8.3 Legal Stage and Court Rulings Enforcement

**When to use:** After exhausting all pre-court options AND economic cost-benefit analysis confirms it is worthwhile to litigate.

**Cost-benefit analysis required before filing:**
- Expected court costs + lawyer's fees vs. expected recovery
- Asset check: does client have attachable assets?
- If exposure < threshold → do not litigate

**Handover to Legal / external law firm:**
- All documents transferred within defined time window
- Form and content must match local court requirements to minimise delay
- Reaction time SLA with Legal Department mandatory

**Post-title (execution) phase:**
- Contact client immediately after judgment to attempt voluntary settlement
- If no deal: proceed to enforcement via court or bailiff
- Prioritise bailiff case files by expected recovery from auctions
- Monitor bailiff performance (cash collected in first 6 months / total assigned)
- Allocate more cases to best-performing bailiffs
- Good relationship management with court officials and bailiffs is a competitive advantage

> ⚠️ **OUTDATED — Bailiff rules:** In some jurisdictions, the choice of bailiff is not discretionary. In countries where assignment is mandatory, the 3-bailiff competition model described is not applicable.

### 8.4 Debt Settlement

**Purpose:** Offer a partial debt forgiveness to motivate the client to make a fast final repayment, rather than proceeding to debt sale.

**Typical discount structure:**
- Post-legal: 50–80% discount possible
- Pre-legal (skipped legal): 20–40% discount
- Always offer at least 2–3 options (two similar, one different) — research shows clients pick more often from a similar pair, making the offer feel like a choice, not a take-it-or-leave-it

**Discount calculation floor:**
- Maximum forgiven amount = Provisioned balance − process costs − tax implications
- Never offer a discount that creates a negative P&L impact unless explicitly approved

**Repayment period:** Maximum 6 months for standard cases; negotiable for very large exposures. Initial down payment (typically 20%) recommended for high balances to demonstrate commitment.

**Note on reputational risk:** Debt settlement carries reputational and fraud risk. Use only after legal process or as an alternative to litigation, not as an early-stage tool.

**Required:** Management Board approval of discount parameters; clear separation of duties (one officer negotiates, another approves and books).

### 8.5 Debt Sale

**Purpose:** Transfer unrecoverable debt to a specialised debt purchaser as a last resort before write-off.

**Pre-conditions for sale:**
1. All previous tools exhausted or assessed as uneconomic
2. Legal prosecution not viable or cost-inefficient
3. Pre-sale warning letter sent to client (19 working days to pay before sale)
4. Cost-benefit analysis confirms sale proceeds > expected in-house recovery

**Portfolio preparation:**
- Data quality is critical — poor-quality files reduce sale price
- Clean data signals control and lower risk to buyer → higher price

**Buyer selection criteria:**
- No proven client abuse
- No criminal convictions in top management
- Adequate track record and financial stability
- Not eligible: short track record, doubtful financial background

**Sale types:** The document describes periodic portfolio sales. Other models (roll-forward, outsource + buy, forward flow) exist but were not detailed in the source.

**Pricing:** Fixed percentage of outstanding, or fixed + variable (variable tied to buyer's recovery). Do not fund buyers through a bank loan (this does not transfer risk).

**Post-sale obligations:** Bank retains copies; handles complaints; accepts back defective cases (fraud, deceased); communicates with buyer on exceptions.

### 8.6 Write-Off

**Purpose:** Remove uncollectable debt from the balance sheet as an accounting expense (Loan Loss Provision consumption).

**When applicable:**
- After all tools exhausted or assessed as uneconomic
- Early write-off possible around 90 DPD for very small tickets (below €10) where collections cost exceeds expected recovery
- Typical examples: residual fees on current accounts; loans repaid at 99%

**Reporting requirements (internal governance):**
- Requires Management Board approval for all write-offs above materiality threshold
- Exceptions: write-offs resulting from Settlement, Residual Settlement, Debt Sale tools; below-threshold amounts
- Report must include: total exposure, amount written off, P&L impact, selection criteria, tools used, tax implications

---

## 9. KPIs, Metrics & Reporting

### 9.1 The Collection Pyramid

The Collection Pyramid is the core operational reporting framework. It tracks the funnel from total eligible clients to cash collected.

**Operation-view pyramid (attempts as base):**

```
Total Eligible Clients
       ▼  [Penetration Rate = unique attempts / eligible]
Total Attempted Clients
       ▼  [Contact Rate = contacts / attempts]
Total Contacted
       ▼  [RPC Rate = RPCs / contacts]
Total Right Party Contacts (RPCs)
       ▼  [Promise Rate = PTPs taken / RPCs]
Total Promises Taken (PTPs)
       ▼  [Kept Rate = kept PTPs / taken PTPs]
Total Kept Promises → CASH COLLECTED
```

**Conversion Rate** = Contact Rate × RPC Rate × Promise Rate × Kept Rate  
(or: Kept PTPs / Total Attempts)

**PTP categories:**
| Category | Definition |
|----------|-----------|
| Kept PTP | 100% of promised amount paid on time |
| Kept PTP 90% | At least 90% paid on time |
| Partially paid PTP | 30–90% paid on time |
| Broken PTP | <30% paid on time |
| Grace period | Up to 2 extra days allowed before classification |

### 9.2 Stage-Level KPIs

**Early Collections — Manager KPI:**

Monthly Efficiency = Cash Collected on overdue (1–90 DPD) during the month / (Opening overdue stock + New overdue entering EC in the month)

Formula: `MIN(1, SUM(MIN(overdue+due, cash collected)) / SUM(overdue+due))` (portfolio level)

**Early Collections — Collector KPIs:**
1. PTP-Taken per man-hour = PTPs taken since BoM / Hours worked since BoM
2. Monthly PTP-Kept ratio = Cash collected within PTP period (+ 2 grace days) / Expiring PTP amount

**Late Collections — Manager KPI:**
- Volume of successfully closed cases per month (0 DPD OR restructured)
- Quality metric: 30+ DPD at 3 months after successful closure

**Workout — Legal Support KPIs:**
1. Time to First Auction (target defined locally)
2. Backlog: % of cases with no action for >31 days (error level: 5%)
3. Recovery bonus: cash recovered above expected recovery rate × agreed %

### 9.3 Additional Performance Indicators

| Metric | What it measures |
|--------|-----------------|
| **Efficiency Rate** | % of total past-due collected per month (includes both arrears and due installments) |
| **Recovery Rate** | Vintage-based: cumulative cash recovered / original terminated balance (12, 24, 36-month curves) |
| **Successfully Closed Cases Rate** | % of vintage balance that returned to 0 DPD |
| **CCPE** | Unique clients in collections / number of EC employees — capacity benchmark |
| **Costs per Action/Tool** | Administrative + operational cost per unit of tool used (used for cost-benefit decisions) |
| **Status Monitoring** | Snapshot of clients/volumes in each process step — reveals bottlenecks |
| **Time to Action** | Average duration of each process step — identifies inefficiencies |
| **Price Monitoring** | Used in VAS and Debt Sale to track achieved prices vs. appraisal/benchmark |
| **Drop-Off / Refusal Reasons** | Frequency of client refusals — tunes offer parameters and scripts |
| **Offer Popularity** | Which tools/offers clients accept most — reveals mis-calibrated offers |

### 9.4 Compensation and Incentive Design

| Role | Fixed:Variable Ratio | Primary KPI Drivers |
|------|---------------------|---------------------|
| Early Collector | ~60% fix / 40% variable | PTPs per hour, PTP-Kept ratio |
| Late Collections Specialist | ~70–80% fix | Successful closures, quality at 3M |
| Legal Support | ~90% fix / 10% variable | Time to First Auction, backlog rate, recovery above expected |
| Administrative | Fixed / timeliness-based | Error rate, on-time completion |

**Calibration period:** Allow 1–3 months to calibrate KPI targets with actual collector performance before making them bonus-eligible.

**Quarterly bonuses for LC:** Recommended because LC actions have mostly delayed impact on provisions; monthly incentives create perverse pressure.

### 9.5 Common Reasons for Insufficient KPI Performance

- Unclear ownership / shared responsibility
- Wrong prioritisation assumptions
- Auto-dialler misconfiguration or absence
- Unplanned system downtime
- Insufficient FTE capacity
- Data quality problems
- Wrong calling hours (not aligned with prime time)
- Over-focus on low-risk clients who would self-cure
- No contact update / skip tracing policy
- Poor underwriting quality (fraud entering collections)
- Clients recognising the bank's number and not answering
- Artificial RPC inflation (multiple contacts logged for one client)
- Collector skill gaps, poor system support, or weak incentive design
- High attrition rate (knowledge loss)
- Unemployment spike (verify via salary inflow monitoring)

### 9.6 Delinquency Reasons Classification

| Code | Description |
|------|-------------|
| Reduced salary | Pay cut, lost commissions, fewer hours |
| Late salary | Employer delayed payroll |
| Technical delinquency | Payday vs. installment date mismatch |
| Job loss / unemployment | No longer employed |
| Excessive obligations | Over-indebtedness across multiple creditors |
| Other priorities | Discretionary spending displacing payment |
| Other person is paying | Nominee loan situation |
| Sickness — client | Prolonged illness preventing income |
| Sickness — family member | Extraordinary medical expenses |
| Imprisonment | Client serving sentence |
| Death — client | Loan obligation transfers to estate |
| Death — family member | Extraordinary bereavement expenses |
| Marital difficulties | Separation/divorce dispute |
| Dispute / Complaint | Active disagreement about debt terms |
| Other | Catch-all |

---

## 10. Organisation & Human Resources

### 10.1 Centralisation Principle

All collections activities must be centralised in a dedicated department. Reasons:
- Faster decisions
- Easier monitoring and bottleneck detection
- Avoids front-office conflict of interest (selling vs. collecting)
- Enables specialisation

Branches retain a **supporting** role: collecting documents, getting signatures. They should not make collections decisions.

> ⚠️ **OUTDATED — Remote/hybrid work:** The document assumes a physical, centralised call centre model. Post-COVID (2020+), remote and hybrid collections team models are operationally viable and widespread. Centralisation of process governance remains important; physical centralisation of staff is now optional. Tooling (cloud-based collections platforms, VoIP, softphones) must support distributed teams.

### 10.2 Minimum Required Roles

| Role | Key Responsibilities |
|------|---------------------|
| **Head of Collections** | Strategy, efficiency ownership, KPI oversight, incentive scheme design |
| **Team Leader EC / LC** | Workload allocation, performance monitoring, team management |
| **EC Call Officer** | Outbound calling, PTP capture, system logging |
| **EC Administrative Officer** | Back-office tasks in EC (letter generation, data entry) |
| **Field Visitor** | On-site visits; always two employees together |
| **Skip Tracing Specialist** | Contact data recovery and validation |
| **LC Agent** | All LC tools: CC, Restructuring, VAS, Settlement |
| **Legal Support** | Pre-court preparation; execution management; external law firm liaison |

### 10.3 Team Sizing and Structure

- Optimal team size: **10–15 people** (mix of junior and senior)
- Junior collectors reach full productivity in approximately **3 months**
- Senior collectors typically show productivity decline after approximately **9 months** (burnout risk) — plan hiring to offset attrition
- Specialisation (outbound vs. inbound, EC vs. skip tracing vs. back-office) improves productivity significantly over generalist models

**Employment types:**
| Type | Trade-offs |
|------|-----------|
| Full-time | Most stable and productive; most expensive; full data access |
| Part-time | Cheaper, more flexible; lower reliability; may have data access restrictions |
| External/agency | Most flexible; highest compliance and data protection risk |

### 10.4 Capacity Planning

**Three time dimensions:**
1. **Contracted time** — hours in employment contract
2. **Productive time** — contracted time minus absences, holidays, training, breaks
3. **Net working time** — time actually spent on collections activity (the correct capacity measure)

**Capacity calculation steps:**
1. Forecast unique clients entering collections by segment and bucket
2. Apply self-cure rate (clients who pay without contact) and connect rate to get "clients needing service"
3. Calculate net collector hours per day × working days per month
4. Divide demand by supply to test sufficiency

**Capacity optimisation levers:**
| Tool | How it helps |
|------|-------------|
| Prime time shift planning | Move part-time staff to peak contact hours |
| Call blending | Combine inbound + outbound capacity to smooth peaks |
| Grace amount | Exclude below-threshold accounts from early-stage collecting |
| Idle period | Delay first action to allow self-cure (saves FTE without reducing collection) |
| Pre-collections activity | Reduce EC inflow by contacting clients before they lapse |
| Predictive auto-dialler | Eliminate manual dialling time |
| Downtime prevention | Protect business-critical systems (any downtime = lost collections and FTE waste) |
| SMS/letter waves | Reduce outbound call volume but create predictable inbound surges — plan accordingly |

---

## 11. Technology & Systems Considerations

### 11.1 Collections System (Core Requirement)

Every bank must have a system capable of:
- Storing complete communication history per client
- Carrying segment flags daily per client
- Generating daily calling lists and assignments
- Supporting automated template generation and dispatch (SMS, letter)
- Recording call outcomes in structured format (not free text)
- Enabling daily update of prioritisation lists

### 11.2 Auto-Dialler Types

| Type | How it works | Best for |
|------|-------------|---------|
| **Preview dialler** | Collector reviews case before dialling | LC and complex cases |
| **Progressive dialler** | System dials when operator becomes available | Standard EC outbound |
| **Predictive dialler** | System predicts when a line will be free; dials ahead | High-volume, simple EC |

Predictive diallers require compliance with local regulations (abandoned call rates, calling hours).

> ⚠️ **OUTDATED — Dialler technology:** Modern platforms combine outbound dialling with omni-channel orchestration (SMS, email, WhatsApp, in-app) from a single interface. Standalone predictive diallers are increasingly replaced by cloud-based contact centre platforms (Genesys, NICE, Amazon Connect, Five9) which integrate all channels, AI routing, real-time analytics, and compliance management.

### 11.3 Statistical Tooling

> ⚠️ **OUTDATED — Analytics tooling:** The document recommends SAS Enterprise Miner and Microsoft SQL Server Analysis Services for segmentation modelling. Current industry standard includes: **Python** (scikit-learn, XGBoost, LightGBM, TensorFlow/PyTorch), **R**, and managed cloud ML services (Azure ML, AWS SageMaker, Databricks). These are generally faster, cheaper, and more capable than the 2013 tooling references.

> ⚠️ **OUTDATED — Batch vs. real-time scoring:** The document describes monthly (or at best daily) batch segmentation. Modern collections operations score clients in real time or near-real time as each event occurs (payment received, call made, login detected), enabling dynamic next-best-action recommendations.

### 11.4 Data Warehouse and Data Quality

- DWH or equivalent data store required for historical analysis and model training
- Minimum 20,000 cases across 3+ consecutive months for statistical models
- Phone number format validation should be embedded in CBS (correct digit count, valid prefix)
- Verified contact rules should be reviewed bi-annually (or on event: new operator, number format change)

### 11.5 System Downtime Management

Business-critical systems (collections tool, CBS, dialler, data feeds) require:
- Formal business continuity / disaster recovery plans
- Downtime = direct loss of collections productivity and FTE waste
- Every major downtime must be logged and trended

---

## 12. Appendix: Consolidated List of Outdated Items

This appendix consolidates all items flagged `⚠️ OUTDATED` in the document above, for quick reference during training design or advisory work.

| # | Topic | What the document says | What is outdated / what has changed |
|---|-------|----------------------|--------------------------------------|
| 1 | **Governing entity** | All approvals and escalations flow through Sberbank Europe AG | Sberbank Europe was divested/dissolved following 2022 sanctions. Governance references are obsolete. The operational framework is independent of this. |
| 2 | **Document date** | Version 2.0, July 2013 | 12+ years old. While core processes remain valid, all regulatory references pre-date GDPR (2018), PSD2 (2018), EBA NPL guidelines (2017+), and Basel IV phasing. |
| 3 | **Statistical tooling** | SAS Enterprise Miner, MS SQL Analysis Services | Industry has moved to Python (XGBoost, LightGBM, scikit-learn), R, and cloud ML platforms. SAS is still used in some banks but is no longer the standard. |
| 4 | **ML model types** | Only Logistic Regression and C&RT mentioned | Modern collections use gradient boosting, random forests, neural networks, and increasingly LLM-based systems for call scripting and next-best-action. |
| 5 | **Scoring cadence** | Monthly batch segmentation | Real-time and event-triggered scoring is now standard in digitally mature banks. |
| 6 | **Digital channels — missing** | No mention of mobile app, push notifications, WhatsApp, chatbots, in-app messaging | These are primary channels in 2025 collections strategy, particularly for early-stage and self-service repayment. Any modern channel strategy must include a digital-first layer. |
| 7 | **IVR and AVM** | Presented as modern interactive tools | IVR remains in use but is declining. AI-powered voice bots (conversational AI) handle full collections dialogues without human agents and are rapidly displacing IVR in leading banks. |
| 8 | **ATM pop-ups** | Listed as a communication channel | Largely obsolete. Mobile app push notifications achieve better reach, targeting, and personalisation. |
| 9 | **GDPR compliance** | Generic data protection language | GDPR (2018) imposes strict requirements on: lawful basis for data processing, purpose limitation, data minimisation, explicit consent for some skip tracing methods, Article 28 DPAs with EXAs. All processes must be GDPR-reviewed before implementation in EU/EEA. |
| 10 | **Skip tracing — social networks and relatives** | Listed as standard sources | Under GDPR, using social networks and contacting relatives for skip tracing requires careful legal basis analysis (legitimate interest test, proportionality). This is not a blanket right. |
| 11 | **PSD2 / Open Banking** | Not mentioned | PSD2 (2018) enables (with consent) access to account transaction data that can dramatically improve pre-collections propensity models and early warning detection. This is a major capability gap vs. what a 2013 document could describe. |
| 12 | **EBA NPL guidelines** | Not mentioned | EBA's NPL Guidelines (2017) and subsequent regulations significantly standardised NPL definitions, provisioning, and reporting. Any collections strategy in an EU bank must align with these. |
| 13 | **Vulnerable client handling** | Not mentioned | Regulatory requirements for identifying and accommodating financially vulnerable clients are now mandatory in many EU jurisdictions and strongly recommended under EBA guidelines. This includes adapted communication, forbearance measures, and staff training. |
| 14 | **Remote / hybrid work** | Assumes physical call centre centralisation | Post-COVID, remote and hybrid models are standard. Physical centralisation is still a valid model but not the only viable one. |
| 15 | **Auto-dialler platforms** | Standalone predictive/progressive diallers | Modern contact centre platforms (Genesys, NICE, Amazon Connect) integrate all channels, AI routing, compliance recording, and analytics into a single cloud platform. |
| 16 | **Debt sale models** | Only periodic portfolio sale described | Forward flow agreements (continuous sale of aged debt) are now common, especially for unsecured consumer portfolios. This offers more predictable P&L and cleaner portfolio management than periodic auctions. |
| 17 | **Bailiff assignment** | Suggests bank can choose bailiff and run competition model | In some jurisdictions bailiff assignment is mandatory and non-discretionary. The competition model is not universally applicable. |
| 18 | **Salary pledge terminology** | "Salary pledge" with employer letter as core mechanism | Wage garnishment via court order is more common post-termination. Digital employer verification services now exist in some markets, reducing administrative burden. |
| 19 | **Letter as escalation** | Physical mail treated as a primary escalation channel | Email, e-statements, and app notifications are more cost-effective and faster escalation channels. Physical mail remains important for legal notices where local law requires it. |
| 20 | **ESG / Responsible lending** | Not mentioned | ESG considerations increasingly affect collections strategy: ethical debt recovery codes, sustainability reporting, impact on client financial wellbeing. Some jurisdictions have introduced mandatory forbearance requirements. |

---

*Knowledge base compiled from: ABC_Collections_Guideline.docx (Sberbank Europe, v2.0, 2013)*  
*Outdated item assessment based on European banking standards and regulatory developments through 2025.*
