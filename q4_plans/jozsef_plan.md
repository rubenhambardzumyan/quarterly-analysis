Central Engineering Budget Plan Q4
2025

Business Unit Plan

Prior quarter review
Highlights
● Khoros Import Done
○ We imported 5 Khoros products in 90 days using our structured playbook.
Released 72 builds with no outages.
○ Legacy teams exited (124 engineers); engineering picked up ops and stabilized
the stack fast.
○ The Twitter/X deletion project—usually outside the scope of import—was also
completed during this phase due to its urgency and impact.

● AI Code as Default
○ 99% of code was AI-generated. Cascade usage jumped to 95% (up from 75% in
Q2). AI-first delivery is now the norm.

● Agent Platform Live
○ Rolled out the first version of our Claude/Docker agent platform. Engineers
started defining agent flows—this sets us up to ship real Tier-1 agents in Q4.

● Team Upgrade
○ Topgraded 16% of low performers.
○ Used our new coaching loop to raise the bar and improve consistency.

Outcomes
● Kanban Hit Rate: 90%
○ Up from 83% in Q2. More frequent AI check-ins helped. Still aiming for 100%.
○ To close the gap, we’ll need our progress review agent live—something that flags
misalignment early and goes deep into recovery mode.
○ Check out the Central Product - Q4'25 Plan for a detailed goal delivery table.
● Cost Optimization via AI + CloudFix
○ AI-assisted cost reduction efforts contributed to ~$4.3M in realized annualized
AWS savings across the org. These savings didn’t shift Khoros into PP
compliance, but they did materially move the needle.

○ In Q3, we delivered savings across Khoros ($3.8M) and the broader SaaS
portfolio ($500K).

● Agentic Engineering Foundation
○ Every engineer started defining agent flows on the new platform. Not production
yet, but the data will fuel great agent launches in Q4.

● P&L Visibility
○ Built BU-level engineering P&Ls using a 40% overhead model.
○ Highlighted where we’re overspending—and where we’re too lean.

Issues
● Kanban Misses
○ CloudSense: Bulk Order dropped.
○ Khoros Communities: Custom features descoped to unblock migrations.
○ Khoros Care: AI-PI stretch goal skipped to finish legacy work.
○ Jive: Patch Management didn’t land—limited bandwidth.
○ GFI: Spam filter deferred (EULA priorities).
● Khoros Backlog Dump
○ 400+ tickets dropped into SE7. Made SLA performance tank.
○ We held the line on new tickets (~30/week), but legacy load needs agent help in
Q4.
● Ticket SLA Slip
○ Ticket age breached SLA due to the backlog surge. Q4 plan is to use agents
more.
● $250K Overspend
○ Topgrading had an overlap cost.
○ Hiring pace stayed high despite no new product imports planned for Q4.
○ Kayako work started earlier than planned.
○ GitHub Budget Hole - $240K/year for 100 seats. Engineering appears to be
paying for everyone. Reviewing with IT.

● IDE Workflow Chaos
○ 100 Engineers = 100 workflows. Introduced a master workflow (80% compliance
target). WorkSmart AI review + monthly updates will keep us aligned and
adaptable.
● Unbalanced P&Ls
○ Khoros: High cost from a more senior team and an extra QA team.
○ Totogi: High cost from more senior team to build telco/foundations.

Goals
● Achieve 100% Kanban Goal Delivery Through AI Check-Ins:
○ Specific: Reach 100% Kanban goal delivery in Q4 by building an AI-based
check-in system that analyzes progress trends and recommends specific
adjustments in scope, sequencing, or resourcing.

■ We currently review goal scope and progress monthly. Measurement is
done manually. It's inaccurate and has significant lag, leaving us little time
to address issues.
■ We will use AI agents to monitor TPM/ENG weekly checkpoint meetings.
We will use this to track scope changes and known risks. Our AI agents
will escalate if there is insufficient insight coming from the checkpoint
meetings.

○ Measurable: Move from 90% delivery in Q3 to 100% in Q4 across all engineering
Kanbans.
○ Achievable: Use historical delivery patterns to train agent prompts; deploy weekly
AI reviews that suggest corrective actions to DRIs.
○ Relevant: Consistent goal delivery is critical to velocity, trust, and predictability —
AI guidance helps close the final 10% execution gap.
○ Time-bound: AI check-in system live by end of October; 100% goal delivery by
end of Q4 2025.

● Eliminate Khoros Maintenance Backlog:
○ Specific: Use our new agentic platform to triage and resolve the 400+ legacy
maintenance tickets in Khoros, with AI agents escalating decisions to TPMs and
a named owner driving execution.
■ Fix backlog quality - we will have agents to identify misaligned work - e.g.
features; duplicates; operations; non-customers.
■ AI wins - Taro (our maintenance ai agent) will attempt to fix every code
level ticket. We will get the low-hanging fruit. We will learn from the rest
and improve Taro.
■ Human + AI - we will use our AI-KB and Engineering AI-IDE workflow to
streamline our resolution of the rest.

○ Measurable: Achieve average ticket age under 7 days by clearing pre-acquisition
backlog.
○ Achievable: Leverage AI agent + TPM loop, with dedicated ownership outside the
main maintenance team.
○ Relevant: Improves customer experience, resets standards from prior ownership,
and enables SLA recovery.
○ Time-bound: By the end of Q4 2025.
○ This will also enable us to have less HC on SE7 and meet our budget plan.
● Standardize AI IDE Workflows Across Engineering:
○ Specific: Replace fragmented engineering practices by rolling out a unified,
AI-first IDE workflow for defect and feature work. Engineers are expected to
follow the standard workflow at least 80% of the time, with 20% left open for
experimentation and innovation.
■ AI-IDEs are the most powerful agentic AI tools on the market today. We
are making the AI-powered IDE the centre of the developer experience.
■ 1 - we bring all context into the IDE - done

■ 2 - we leverage our AI experience from the last 3 years to roll out
standard workflow and prompts - ensuring even our newest staff benefit
from our AI capability
■ 3 - we measure and reinforce, using WorkSmart AI to provide insight into
our compliance, and coaching guidance for managers

○ Measurable: Worksmart screen recording and AI-first review will track workflow
compliance and identify emerging best practices. We will update the master
workflow monthly based on these insights.
○ Achievable: Delivered through repo-based templates, multi-agent workflows,
long-running validation agents, and AI-first review loops, with coaching and
usage dashboards supporting adoption.
○ Relevant: Ensures consistent, high-leverage use of AI agents across the full
SDLC, improves quality, and institutionalizes learnings from bottom-up
innovation.
○ Time-bound: By end of Q4 2025.
● Maintain Budget Discipline on People Cost:
○ Specific: Stay within the approved Q4 HC budget of $2.98M by enforcing tighter
topgrading and disciplined hiring. All new or replacement hires must be backed
by a written plan tied to roadmap outcomes.
○ Measurable: Monitor monthly HC spend via finance reports; maintain cumulative
HC spend within $2.98M and eliminate Q3-style overspend from overlapping
transitions.
○ Achievable: Require documented justification before every hire, accelerate
topgrading handoffs to minimize cost overlap, and review HC forecasts monthly
against actuals.
○ Relevant: Protects Q4 net margin (currently projected at 16%) and avoids
unnecessary cash burn while preserving execution capacity.
○ Time-bound: Enforced continuously through Q4 2025, tracked monthly.
● Increase Autonomous AI Code Contribution to 25%:
○ Specific: Scale adoption of our Claude Code + Docker-based autonomous agent
platform to reach 25% of total code output. Each engineer must define at least 3
agents aligned to their workflows to seed data for Tier 1 agent development.
■ We will engage on feature. Every task breakdown will be required to
contain a task that can be done completely by AI working off a GitHub
ticket. We will introduce this requirement, starting with one 100% AI ticket
per mini spec, and increase it as we learn, aiming for 25% of 100% AI
tickets by EOQ.

○ Measurable: Reach 25% of total code output in Q4 delivered by autonomous
agents, measured via repo commit analysis and Workspace metrics.
○ Achievable: Platform is already deployed; success depends on team compliance
with agent definition, and centralized tracking of agent activity and code output.
○ Relevant: Reduces manual effort, accelerates delivery, and enables Tier 1
reusable agents through data aggregation and refinement.

○ Time-bound: Agent definition by end of October; 25% autonomous code target by
end of Q4 2025.
● Restore Gross Margin to 95%+:
○ Specific: Reduce CF COGS to reverse the Q4 gross-margin compression.
○ Measurable: Cut CF COGS from $233K to ≤$133K (−$100K) and raise Gross
Margin from 93% to 95%+.
○ Achievable: Reprice and rationalize CF services; shift/park non-prod compute to
lower-cost tiers
○ Relevant: Protects margin and supports the Code Arbitrage model’s economics.
○ Time-bound: By Dec 31, 2025.
● Achieve Q4 Net Margin 8%+:
○ Specific: Improve overall profitability to deliver Net Margin of 8%+ in Q4.
○ Measurable: Lift Net Margin from the current 3% plan to 8%+; align Net Profit to
~$280K+ on ~$3.53M revenue.
○ Achievable: Combine ≥$100K CF COGS reduction with HC spend adherence
and incremental revenue lift
○ Relevant: Restores Q4 profitability trajectory and supports FY’25 EBITDA
recovery.
○ Time-bound: By Dec 31, 2025.

Most Important Problems
● Maintenance Backlog Dragging SLA:
○ Problem: The SE7 backlog grew by 400+ tickets after the Khoros import,
breaching age SLAs and overwhelming current team capacity. Most of these are
legacy bugs that now block maintenance velocity.
○ Why Critical: The backlog inflates perceived instability and slows roadmap
delivery. Manual bug triage and fixes won’t scale—without automation, we won’t
catch up or stay current.
○ Initial Plan:
■ Deploy a triage agent by 30 Oct to deduplicate, group, or discard
non-priority issues.
■ Deploy a fix-agent for grouped legacy issues and reduce backlog age to
<7 days by EOQ4.

○ In parallel, we launched weekend AI mini-hackathons—opt-in sessions where
Khoros Kanban engineers join the maintenance squads to burn down the
backlog.
● AI Agent Output Gap:
○ Problem: We’ve laid the groundwork for autonomous agents, but engineering
output still relies heavily on only AI supported workflows. No Tier-1 agents are
live, and agent output isn’t contributing meaningfully to delivery yet.
○ Why Critical: Autonomous delivery is key to our 25% AI-generated code goal in
Q4. Without real agent output, we can’t scale efficiency, close skill gaps, or
unlock compounding leverage from our Claude-based platform.

○ Initial Plan:
■ Require all engineers to define and ship 3 functional agents by 15 Nov,
with working examples of use in their IDE or test environments.
■ Select top-performing flows and begin Tier-1 agent production by 1 Dec,
targeting 25% of total code output via agents by EOQ4.

● Budget Discipline Drift:
○ Problem: Q3 overspend exceeded ~$250K due to topgrading overlap and
late-stage hiring momentum not tied to active plans. Replacement cycles also
caused parallel cost periods that weren’t managed tightly.
○ Why Critical: Headcount is our biggest cost driver. Without tighter control, we risk
blowing the Q4 budget, weakening margin, and losing financial credibility.
○ Initial Plan:
■ Require all hiring decisions to be backed by a written plan approved by
Jozsef, linked to BU goals or efficiency gains.
■ Track monthly spend vs. plan using Finance reports, with a zero-tolerance
policy for off-plan additions by EOQ4.

Financial Performance & Forecasts

FY25 - Current Plan vs Previous Plan
Key Highlights:
● Q4'25 plan lifts Total Revenue to $3,967,250 (+$439,125 vs prior plan), driving Gross
Profit to $3,822,661 (+$427,311) and Net Profit to $745,880 (+$207,780); Q4 Net Margin
improves to 19% from 15%.
● FY'25 Net Profit decreases by $91,515 to $167,361 despite revenue +$439,125 and
Gross Profit +$418,450, as Total Expenses rise by $509,965 (HC Spend +$515,134); FY
Net Margin slips to 1% from 2%.
● Q3'25 deteriorates plan-on-plan: Net Profit down $240,336 to $(168,000) and margin to
-5% from 2%, driven by HC Expenses +$226,346 and NHC +$13,990 with revenue
unchanged.
● Gross Margin remains strong and stable at 96% in Q4 and 95% for FY'25; COGS
change is minimal (FY +$20,675).
● EBITDA Test - FY'25: FAIL.
Strategic Implications:
● Shows expense growth outpacing profit; tighten HC ramp and discretionary spend in
Q3-Q4 or offset with additional high-margin revenue to recover at least $91,515 FY profit
and address the EBITDA test failure.
● Indicates heightened dependence on Q4 performance (Net Profit $745,880); de-risk
revenue attainment at $3,967,250 and protect the 96% Gross Margin to safeguard FY
results.

● Reflects a Q3 profitability gap ($(240,336)); implement immediate cost containment or
rephase investments to prevent FY Net Margin from compressing below 1%.
● Highlights a fully non-recurring revenue mix; pursue recurring components to stabilize
earnings and reduce end-of-year concentration risk.
Reference table

Current Plan vs. Previous Plan - FY'25 Current Plan Previous Plan Current Plan vs Previous Plan
EBITDA Test - FY'25 ---------- >>>>>> FAIL
4 Rolling Quarters Q1'25 Act. Q2'25 Act. Q3'25 Fcst. Q4'25 Bdt. FY'25 Q1'25 Act. Q2'25 Fcst. Q3'25 Bdt. Q4'25 FY'25 Q1'25 Q2'25 Q3'25 Q4'25 FY'25
Non Recurring Revenue $ 2,860,000 $ 3,020,375 $ 3,528,375 $ 3,967,250 $ 13,376,000 $ 2,860,000 $ 3,020,375 $ 3,528,375 $ 3,528,125 $ 12,936,875 $ - $ (0) $ - $ 439,125 $ 439,125
Total Revenue $ 2,860,000 $ 3,020,375 $ 3,528,375 $ 3,967,250 $ 13,376,000 $ 2,860,000 $ 3,020,375 $ 3,528,375 $ 3,528,125 $ 12,936,875 $ - $ (0) $ - $ 439,125 $ 439,125
HC COGS $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ -
NHC COGS $ - $ 8,861 $ - $ - $ 8,861 $ - $ - $ - $ - $ - $ - $ 8,861 $ - $ - $ 8,861
CF COGS $ 214,032 $ 153,484 $ 132,775 $ 144,589 $ 644,879 $ 214,032 $ 153,484 $ 132,775 $ 132,775 $ 633,065 $ - $ 0 $ (0) $ 11,814 $ 11,814
Total COGS $ 214,032 $ 162,345 $ 132,775 $ 144,589 $ 653,740 $ 214,032 $ 153,484 $ 132,775 $ 132,775 $ 633,065 $ - $ 8,861 $ (0) $ 11,814 $ 20,675
Gross Profit $ 2,645,968 $ 2,858,030 $ 3,395,600 $ 3,822,661 $ 12,722,259 $ 2,645,968 $ 2,866,891 $ 3,395,600 $ 3,395,350 $ 12,303,810 $ - $ (8,861) $ 0 $ 427,311 $ 418,450
Gross Margin 93% 95% 96% 96% 95% 93% 95% 96% 96% 95% 0% 0% 0% 0% 0%
HC Expenses $ 2,520,803 $ 3,066,665 $ 3,413,494 $ 2,961,290 $ 11,962,252 $ 2,520,803 $ 3,018,034 $ 3,187,148 $ 2,721,134 $ 11,447,119 $ - $ 48,631 $ 226,346 $ 240,156 $ 515,134
NHC Expenses $ 114,553 $ 156,246 $ 121,981 $ 102,991 $ 495,771 $ 114,553 $ 154,780 $ 107,991 $ 107,991 $ 485,315 $ - $ 1,466 $ 13,990 $ (5,000) $ 10,456
Total Revenue Write Off $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ -
CF Expenses $ 28,125 $ 28,125 $ 28,125 $ 12,500 $ 96,875 $ 28,125 $ 28,125 $ 28,125 $ 28,125 $ 112,500 $ - $ - $ - $ (15,625) $ (15,625)
Core Allocation $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ - $ -
Total Expenses $ 2,663,482 $ 3,251,036 $ 3,563,600 $ 3,076,781 $ 12,554,899 $ 2,663,482 $ 3,200,939 $ 3,323,264 $ 2,857,250 $ 12,044,934 $ - $ 50,097 $ 240,336 $ 219,531 $ 509,965
Net Profit $ (17,514) $ (393,006) $ (168,000) $ 745,880 $ 167,361 $ (17,514) $ (334,047) $ 72,337 $ 538,101 $ 258,876 $ - $ (58,959) $ (240,336) $ 207,780 $ (91,515)
Net Margin -1% -13% -5% 19% 1% -1% -11% 2% 15% 2% 0% -2% -7% 4% -1%
Total HC Spend $ 2,520,803 $ 3,066,665 $ 3,413,494 $ 2,961,290 $ 11,962,252 $ 2,520,803 $ 3,018,034 $ 3,187,148 $ 2,721,134 $ 11,447,119 $ - $ 48,631 $ 226,346 $ 240,156 $ 515,134
Total NHC Spend $ 114,553 $ 165,107 $ 121,981 $ 102,991 $ 504,633 $ 114,553 $ 154,780 $ 107,991 $ 107,991 $ 485,315 $ - $ 10,327 $ 13,990 $ (5,000) $ 19,317
Total CF Spend $ 242,157 $ 181,609 $ 160,900 $ 157,089 $ 741,754 $ 242,157 $ 181,609 $ 160,900 $ 160,900 $ 745,565 $ - $ 0 $ (0) $ (3,811) $ (3,811)

Current Quarter Plan
Key Highlights:
● Q4'25 Current Plan increases Total Revenue by $ 439,125 to $ 3,967,250 (entirely Non Recurring Revenue); CF COGS rises $ 11,814 to $ 144,589; Gross Profit up $ 427,311
to $ 3,822,661 with Gross Margin steady at 96%.

● Expense mix shifts: HC Expenses increase $ 240,156 to $ 2,961,290; NHC Expenses
decrease $ (5,000) to $ 102,991; CF Expenses decrease $ (15,625) to $ 12,500; Total
Expenses rise $ 219,531 to $ 3,076,781.
● Profitability strengthens: Net Profit increases $ 207,780 to $ 745,880; Net Margin
expands to 19% from 15% (+4 pts).
● Total CF Spend declines $ 3,811 to $ 157,089 despite higher CF COGS, reflecting lower
CF Expenses.
Strategic Implications:
● Shows accretive revenue growth with unchanged 96% gross margin, supporting further
margin expansion; sustain delivery cost discipline as revenue scales.
● Revenue is 100% non-recurring; prioritize converting project wins to recurring/renewal
streams and secure Q4 backlog to mitigate volatility risk.
● HC ramp (+$ 240,156) raises the fixed cost base; ensure utilization and pipeline
coverage to protect margins into FY26 while maintaining NHC/CF spend discipline.
Reference table

Central Engineering

Q4'25 Current
Plan
Q4'25 Previous
Plan
Current Plan vs.
previous Plan
Non Recurring Revenue $ 3,967,250 $ 3,528,125 $ 439,125
Total Revenue $ 3,967,250 $ 3,528,125 $ 439,125
HC COGS $ - $ - $ -
NHC COGS $ - $ - $ -
CF COGS $ 144,589 $ 132,775 $ 11,814
Total COGS $ 144,589 $ 132,775 $ 11,814
Gross Profit $ 3,822,661 $ 3,395,350 $ 427,311
Gross Margin 96% 96% 0%
HC Expenses $ 2,961,290 $ 2,721,134 $ 240,156
NHC Expenses $ 102,991 $ 107,991 $ (5,000)
Total Revenue Write Off $ - $ - $ -
CF Expenses $ 12,500 $ 28,125 $ (15,625)
Core Allocation $ - $ - $ -
Total Expenses $ 3,076,781 $ 2,857,250 $ 219,531
Net Profit $ 745,880 $ 538,101 $ 207,780
Net Margin 19% 15% 4%

Total HC Spend $ 2,961,290 $ 2,721,134 $ 240,156
Total NHC Spend $ 102,991 $ 107,991 $ (5,000)

Total CF Spend $ 157,089 $ 160,900 $ (3,811)

Prior Quarter Review
Key Highlights:
● Shows Q3'25 revenue met plan at $3,528,375; gross margin sustained at 96% with
COGS on plan at $132,775 and gross profit at $3,395,600.
● Indicates Opex overspend: total expenses forecast $3,563,600 vs budget $3,323,264
(+$240,336, +7%); HC +$226,346 (+7%), NHC +$13,990 (+13%).
● Reflects profitability shortfall: net profit $(168,000) vs $72,337 budget (−$240,336; net
margin −5% vs 2%, −7 pt).
Strategic Implications:
● Requires immediate expense discipline to close the $240,336 gap; align HC and NHC
run-rate to the budget envelope to restore margin.
● At 96% gross margin, closing the gap demands $240,336 in expense reductions or
$250,350 in incremental revenue in Q4.
● Concentration in non-recurring revenue ($3,528,375) heightens volatility; prioritize
high-confidence bookings/backlog conversion to protect net margin targets.
Reference table

Q3'25 Fcst Q3'25 Bdt Delta % Delta $
Non Recurring Revenue $ 3,528,375 $ 3,528,375 0% $ -
Total Revenue $ 3,528,375 $ 3,528,375 0% $ -
HC COGS $ - $ - $ -
NHC COGS $ - $ - $ -
CF COGS $ 132,775 $ 132,775 0% $ (0)
Total COGS $ 132,775 $ 132,775 0% $ (0)
Gross Profit $ 3,395,600 $ 3,395,600 0% $ 0
Gross Margin 96% 96% 0 pt 0%
HC Expenses $ 3,413,494 $ 3,187,148 7% $ 226,346
NHC Expenses $ 121,981 $ 107,991 13% $ 13,990
Total Revenue Write Off $ - $ - $ -
CF Expenses $ 28,125 $ 28,125 0% $ -
Core Allocation $ - $ - $ -
Total Expenses $ 3,563,600 $ 3,323,264 7% $ 240,336
Net Profit $ (168,000) $ 72,337 -332% $ (240,336)

Net Margin -5% 2% -7 pt $ (0)

Total HC Spend $ 3,413,494 $ 3,187,148 7% $ 226,346
Total NHC Spend $ 121,981 $ 107,991 13% $ 13,990
Total CF Spend $ 160,900 $ 160,900 0% $ (0)