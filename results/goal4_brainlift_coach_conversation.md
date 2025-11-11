# Goal 4: Scale BrainLift Coach - Clarification Conversation

## Goal Statement
Increase adoption inside Trilogy - 80% of all Trilogy users spending time on BrainLifts find value in the product

## Current Context from Document
- 141 registered users
- 383 BrainLifts created in 3 months
- 35 weekly active users on average for Chrome extension
- User feedback: "at times overwhelming or unaware of the limitations of scope"
- Proposed improvements: WorkSmart AI recommendations, meeting context leverage, IDE integration

## Conversation Log

### Session 1: Understanding Current State & Metrics

**Q1: Is current state (141 users, 383 BrainLifts, 35 WAU) success or failure?**

A: **Success!** Updated metrics are even stronger:
- 500+ BrainLifts created (vs 383)
- 70 weekly active users (vs 35)
- 300+ registered users (vs 141)
- 100% growth over last quarter

**Q2: How is "find value" measured?**

A: Combination of qualitative + quantitative:
- Personally reaching out to users and asking their opinion
- PostHog and QuickSight dashboards for quantitative data
- Mix of self-reported and behavioral data

**Q3: What does "spending time on BrainLifts" mean?**

A: **Creating BrainLifts specifically**
- Working 1hr/day → 3-5 days to create a BrainLift
- Minimum 3+ hours needed (using extension in Workflowy)
- About 1 hour using web app for insights and feedback
- Total: ~4+ hours to create a BrainLift that passes QC
- Target users = BrainLift creators (for now)

---

### Session 2: Understanding the Adoption Gap

**Q4: Current adoption rate?**

A:
- 183 users have created BrainLifts (out of 300+ registered = ~60% conversion)
- Unknown: How many of those who invested 4+ hours "find value" → **needs research**
- Unknown: Current % finding value and distance to 80% target → **needs research**

**Q5: What does "overwhelming" and "unaware of limitations" mean?**

A: Three main problems for new users:
1. **Without completing curriculum, users have no idea how to create a BrainLift**
2. **Feedback from extension and web app is sometimes confusing**
3. **Newbies don't understand what a good BrainLift is**

**Q6: Dropout patterns?**

A:
- **Most users drop mid-curriculum** (only few passed all 27 lessons)
- 183 users with BrainLifts (117+ users registered but never created one)
- Typical dropout journey not analyzed yet

---

### Session 3: Understanding the Curriculum Bottleneck

**Q7: Where do users drop in the curriculum?**

A:
- **No specific lesson** - dropout is **gradual starting from lesson 1**
- Full curriculum takes **~2 weeks to complete**
- Time per lesson: **5-30 minutes** (varies by lesson)

**Q8: Correlation between curriculum completion and BrainLift success?**

A:
- Need to research: How many of 183 BrainLift creators completed curriculum
- **Yes**: BrainLifts from curriculum completers pass QC more often
- **Yes**: Users CAN create good BrainLifts without completing curriculum

**Q9: Why do users drop out of curriculum?**

A:
- Primary reason: **Too time consuming**
- Various reasons: from not having time to not wanting advanced tracks
- Dropout is gradual (not concentrated at specific lesson)

**Q10: What feedback is confusing?**

A: **Discrepancy between two feedback channels:**
- **Chrome extension**: Real-time feedback (proactive, as you work)
- **Web app**: Static feedback/scoring (user must check manually)
- Problem: Different types of feedback can be **inconsistent or contradictory**

---

### Session 4: Identifying the Real Barrier

**Q11: Is curriculum mandatory?**

A: **No, curriculum is optional** - it's for users who don't know how to create BrainLifts

**Q12: What actually prevents users from finding value?**

A: **Option B + Behavioral/Habitual Issues**
- They create BrainLifts but **don't actually use them in their work**
- They **don't invest enough time to create BrainLifts** (behavioral/habitual problem)

**Q13: What's different about success cases (70 WAU)?**

A: Need to research - did they complete curriculum or skip it? What's their pattern?

---

### Session 5: Understanding the Value Realization Gap

**Q14: Where/how are BrainLifts supposed to be used?**

A: **In daily work with AI to get expert opinions**
- When someone needs the BrainLift creator's expert opinion on same/similar problem
- When solving the same problem in a different context
- **Primary use case**: Better align with AI so it doesn't answer in defaults (generic responses)
- Users attach BrainLifts to AI conversations to get expert-calibrated responses

**Q15: How do proposed solutions address "create but don't use"?**

A: **IDE integration**
- Provides MCP (Model Context Protocol) to query and use BrainLifts in daily work
- Makes BrainLifts accessible directly in development environment

**Q16: What motivates users to invest 4+ hours creating BrainLifts?**

A: **Two primary motivations:**
1. **Personal need**: They need to create that BrainLift for their own work
2. **Manager request**: Manager asks them to create that BrainLift

These two motivations drive the 70 WAU who are actively creating BrainLifts.

---

## Problem Synthesis

### What I Clearly Understand:

**The Goal:**
- 80% of users creating BrainLifts should find value in the product
- Currently: 100% QoQ growth, 183/300+ users created BrainLifts (~60%)
- Motivation to create: Personal need OR manager request

**The Core Problem:**
Users invest 4+ hours creating BrainLifts but **don't use them in daily work**, so they:
1. Don't experience the intended value (expert-calibrated AI responses vs generic defaults)
2. Therefore don't "find value" in BrainLift Coach
3. Secondary: Don't invest enough time creating BrainLifts (behavioral/habitual)

**Intended Value:**
- BrainLifts should be attached to AI conversations (Claude, ChatGPT, etc.)
- Get expert opinions on similar problems in different contexts
- Prevent AI from giving generic default answers

**Proposed Solution:**
- IDE integration via MCP to make BrainLifts queryable in daily work
- Hypothesis: Make BrainLifts accessible where users actually work

**What I Don't Know (but won't block BrainLift proposal):**
- Exact usage metrics (created vs actually used with AI)
- Success case patterns (what do the 70 WAU do differently?)
- Whether users are in AI-assisted workflows daily

---

## BrainLift Proposal

### Problem Confirmed:
**Creation-to-Usage Gap in BrainLift Coach**

Users invest 4+ hours creating BrainLifts but don't use them in daily AI-assisted work. This prevents them from experiencing the intended value (expert-calibrated AI responses vs generic defaults), so they don't "find value" in the product. The challenge isn't teaching users to create BrainLifts - it's making BrainLifts actually get used after creation.

---

### Possible BrainLift: **Product Adoption Pattern for Knowledge Tool Integration**

**Purpose:**
BrainLift Coach faces a critical adoption gap: users create high-quality BrainLifts (500+ created, 183 active creators) but don't integrate them into daily AI-assisted workflows. This means they never experience the core value proposition—getting expert-calibrated AI responses instead of generic defaults. The result is that users invest 4+ hours creating BrainLifts that sit unused, preventing the product from reaching 80% "find value" adoption.

Solving this requires developing expertise in:
- **Workflow integration patterns**: How to surface the right BrainLift at the right moment in users' daily work
- **Context-aware discovery**: Determining when a user's current problem matches an existing BrainLift
- **Friction reduction**: Making it effortless to go from "I have a BrainLift" to "I'm using it with AI right now"
- **Usage measurement**: Tracking creation vs actual usage to understand what drives value realization
- **Multi-environment integration**: Designing patterns that work across IDEs (via MCP), chat interfaces, and other tools

This BrainLift captures the expertise needed to bridge the creation-to-usage gap in knowledge tools, turning created artifacts into actively-used resources.

**In scope:**
- Framework for identifying moments when existing BrainLifts should be surfaced in workflows
- Methodology for measuring actual usage (not just creation) of knowledge artifacts
- Integration pattern design for different work environments (IDEs, AI chat, web apps)
- Decision criteria for when to proactively suggest vs passively make available BrainLifts
- Approach to reducing friction between knowledge creation and knowledge application
- Techniques for context-aware matching between current problems and existing BrainLifts

**Out of scope:**
- BrainLift content quality or creation process improvements
- Curriculum design or educational content development
- General product onboarding or user acquisition strategies
- Technical implementation details of MCP or specific integrations
- Motivation/behavioral psychology for initial BrainLift creation
- Use cases outside of AI-assisted knowledge work

