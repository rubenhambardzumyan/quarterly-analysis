# Crossover Problems Decomposition

### Intro

The goal of this document is to break down the Q4/2025 plan of Crossover into problems to analyze BrainLift opportunities for each problem and present either a purpose statement or questions to clarify before a BrainLift with a purpose statement can be presented.

### Thought Process

- **The Priority**
  - Identify good goals, and use those good goals to articulate a good purpose statement in cases a BrainLift can be suggested
  - Using questions to understand the goals deeper and improve the goals, thus being able to suggest a BrainLift with a good purpose statement
- **Goal Extraction & Validation**
  - Extract all stated goals from the document
  - For each goal, assess whether it is actionable as-is or requires decomposition:
    - Can specific problems or decisions be identified from the document context?
    - Is the goal describing a problem to solve, or merely a desired outcome?
    - Does the document provide sufficient context about current state, challenges, or approach?
    - Are there enough context and understanding to decompose it into complete, actionable work sub goals?
- **Problem Identification**
  - Extract underlying problems from:
    - Explicit problem statements in the document.
    - Challenges mentioned in context.
    - Gaps between current state and goal.
  - Avoid inventing problems not present in the document.
- **Problem Analysis**
  - For each identified problem, assess clarity:
    - If clearly defined:
      - Determine whether solving it requires developing expertise (not just executing tasks).
        - If expertise development is needed, then propose a BrainLift with clear purpose statement and use the context to articulate a clear, high quality purpose. In case of gaps, list the curious questions that need to be answered and prepare to clarify them with the user
        - If execution only, then note that it is an execution task, not a BrainLift candidate.
    - If not clearly defined:
      - List specific curious questions needed to clarify:
        - What is the current state?
        - What are the actual challenges?
        - What has been tried?
        - What decisions need to be made?
        - What expertise is lacking?
- **Quality Standards**
  - Never propose a BrainLift without a clear, specific purpose statement.
  - If the purpose statement merely restates the goal, insufficient context exists.
  - When in doubt, ask clarifying questions rather than make assumptions

### Crossover Q4 Goals

- **Goal 1 (as stated): Improve Hiring Operations**
  - Target as specified in the document:
    - 80% fill rate at the 45 days mark for in-model roles, with LinkedIn sourcing
    - 100% of pipelines "in-model" (this goal is not full control of Crossover, but measuring it and working to push it higher is the the right thing to do)
  - Identified problems:
    - Unclear organizational structure leads to hiring inefficiencies
      - Possible BrainLift: Organization discovery & alignment framework for new BUs
      - Purpose: Unclear organizational structure leads to duplicate orders, missing orders, over/under hiring, and hiring for wrong locations. The Q3 review shows Education had challenges with "unclear org structure, work unit plan, pay rates, mapping to industry roles & expertise, orders, DRIs." This BrainLift captures the expertise that OrgBuilders developed through defining work units and supporting Education's growth, turning it into a set of applicable SPOVs and a standard process that can be reused for future business units.
        - In scope:
          - Discovery session methodology for extracting org structure from stakeholders
          - Framework for mapping work units to industry roles and expertise levels
          - Process for identifying Accountable Business Executives (ABEs) for each BU/CF
          - Methodology for translating business goals into clear hiring orders with defined pay rates and locations
        - Out of scope:
          - General organizational design theory
          - Business unit strategy or product roadmaps
          - Existing, well-defined org structures that just need execution
          - Post-hire onboarding or organizational change management
    - Plagiarism and fraud waste interviewer time
      - No BrainLift needed, since this has clear requirements and is more like an engineering task than a problem that requires expertise building. The document specifies concrete technical solutions: detecting plagiarism using AI for CodeSignal, proprietary AI-assisted coding assessments, and GDoc-based RWAs, plus extending AI-led screening to detect misrepresentation.
    - Grading backlogs occur when waiting for SME feedback blocks AI grading rollout
      - No BrainLift needed, since this is more of a process issue that requires SMEs to commit to provide feedback on time rather than an opportunity to develop expertise. The document already has a solution: "independently move to AI grading after a batch of 15-20 submissions, without being blocked on SME feedback."
    - Interview feedback delays persist despite escalation emails
      - No BrainLift needed, since the document outlines clear execution tasks: present HMs with relevant information, consolidate information across interviewers, provide GChat prep notes, and add their own bot to replace Read.ai. This is behavioral/process issue with defined technical solutions.

- **Goal 2 (as stated): Improve Education Hiring**
  - Target as specified in the document:
    - Reduce time-to-offer, cut mishires, raise screen→interview pass quality, and sustain interviews per week (T4W) above plan
  - EDU's top issues: attention, mishires, vague requirements, and niche roles
  - Identified problems:
    - Vague or subjective requirements cause hiring bottlenecks
      - Possible BrainLift: Standardized education role filters and quality bars
      - Purpose: Education hiring faces a critical efficiency problem: vague or subjective requirements create bottlenecks that extend time-to-offer and contribute to mishires. Hiring managers often apply implicit quality standards that aren't documented anywhere, forcing recruiters to guess what makes a candidate suitable. Additionally, niche education roles lack standardized filters, meaning each role gets reinvented from scratch. The Q3 review highlights specific challenging cases: "persona-based screening for 2HL & Core Edu roles (personal, lived experience + mission alignment)" and "hyper-specific Ops spec (MBB alum)."

        This BrainLift captures the expertise needed to solve this problem by:
        - Defining clear, standardized role filters for education positions that can be reused and adapted
        - Extracting and documenting the implicit quality bars that experienced hiring managers use but haven't articulated

        - In scope:
          - Framework for translating vague education role requirements into clear, actionable filters
          - Decision criteria for when requirements are "clear enough" vs need more specificity
          - Methodology for documenting implicit quality bars from experienced education hiring managers
          - Approach to handling persona-based requirements (mission alignment, lived experience) systematically
        - Out of scope:
          - General job description writing or copywriting techniques
          - Requirements standardization for non-education roles (engineering, sales, etc.)
          - Candidate sourcing strategies
          - Interview design or assessment creation
    - Unclear how proposed activities solve defined problems
      - Questions to clarify:
        - On problem:
          - What's the definition of success for each of the problem patterns (attention, mishires, vague requirements, niche roles)?
          - How exactly will hiring a VP OrgBuilder address the mishires problem?
          - How exactly will the Outbound Recruiting Engine reduce time-to-offer or improve requirement clarity?
        - On assumptions:
          - Is the assumption that mishires are primarily caused by vague requirements, or are there other root causes?
          - What evidence exists that the current OrgBuilder capacity is the bottleneck vs. other factors?

- **Goal 3 (as stated): Align on relying primarily on LinkedIn; Stop Searching for Alternatives**
  - Target as specified in the document:
    - Secure executive buy-in for a (multi)yearly contract with LinkedIn
  - Identified problems:
    - Expired hiring slots limit capacity to 200 for EDU only
      - No BrainLift needed, since this is about securing executive buy-in and creating a purchase request document, not about developing expertise. The goal is about alignment and negotiation.
    - Short-term Q4 strategy contradicts long-term LinkedIn-only strategy
      - Questions to clarify:
        - On problem:
          - What is the actual challenge of getting the executive buy-in?
          - What are other actions to secure the executive buy-in than creating the purchase request document?
        - On assumptions:
          - How solid is the acknowledgement that LinkedIn should be the only source of hiring?
          - What specific evidence demonstrates that "alternative channels are low quality, higher cost and leave important talent segments not covered"?
          - How does focusing on short-term Q4 fulfillment with Indeed and Google Ads help move the needle in getting the executive buy-in to use LinkedIn only?

- **Goal 4 (as stated): Scale BrainLift Coach**
  - Target as specified in the document:
    - Increase adoption inside Trilogy - 80% of all Trilogy users spending time on BrainLifts find value in the product
  - Identified problems:
    - Target is an outcome without clarity on what's missing
      - Questions to clarify:
        - On target:
          - What does "spending time on BrainLifts" mean? Is it creating, reading, or using them with AI?
          - How is "find value" measured? Is it self-reported or based on behavioral data?
          - What does success look like? What happens when 80% adoption is achieved?
        - On assumptions:
          - Is self-reported evidence of success enough to measure the success?
          - What is the current adoption rate and why is 80% the target?
        - On BrainLift Coach:
          - What works now? The document shows 141 registered users, 383 BrainLifts created, 35 weekly active users - is this considered success or failure?
          - What doesn't work based on data and/or user research? The document mentions "at times overwhelming or unaware of the limitations of scope" - what specific problems does this cause?
          - What user research or data exists about why people don't use BrainLifts or don't find value?
          - What is the relationship between the proposed improvements (WorkSmart AI recommendations, meeting context leverage, IDE integration) and the adoption/value problem?

- **Goal 5 (as stated): Make WorkSmart Vision AI Valuable**
  - Target as specified in the document:
    - 2 core functions using it to make decisions or generate insights
  - Current Reality:
    - Most customers only use basic time tracking
    - Full behavioral tracking exists but isn't activated
    - Strategy has been making WorkSmart AI ontology available via AIPIs but "we do not have clear value proposition that makes customers say 'I need this'"
  - Identified problems:
    - This is a solution in search of a problem
      - Questions to clarify:
        - On target:
          - Why is "2 core functions using it" the success metric? Why not 1 or 5?
          - Is the real problem lack of customer demand, unclear value prop, or something else?
          - What happens if you achieve this target? How does it benefit Crossover or the core functions?
        - On AI vision:
          - Why do most of the customers use only time tracking?
          - Why isn't full behavioral tracking activated - is it because it's not ready, not tested, or customers don't want it?
          - What research was done with users to understand the value proposition?
          - What problems do Central Eng and Central SaaS currently have that WorkSmart Vision AI would solve?
        - On use cases:
          - For "Explain the HOW behind the WHAT" - what specific decisions would this enable that can't be made today?
          - For hiring process support - what specific information about hires would be valuable and why?

- **Goal 6 (as stated): Make WorkSmart the People Source of Truth**
  - Target as specified in the document:
    - Support the COO and SaaS group by making XO Manage the source of truth of all contractors working with Trilogy businesses
  - Identified problems:
    - Goal doesn't articulate the problem being solved
      - Questions to clarify:
        - On target:
          - What is the problem of not having this? Why is it worth investing in this in Q4 specifically?
          - What's the definition of success?
          - What does "people source of truth" mean? What specific data/decisions would this enable?
        - On product:
          - What data cleaning challenges are expected? Are these technical challenges or data quality challenges?
          - What's the COO group's role - subject matter expertise or coordination?
          - What actions or decisions would the COO and SaaS group take with this information that they can't do today?

- **Goal 7 (as stated): Connect Brand investment to business value**
  - Target as specified in the document:
    - Prove brand impact on hiring metrics and optimize spend for maximum ROI
  - Investment outcomes listed:
    - Glassdoor: 4.1/5.0 (up from 1.8 in 2021)
    - Radically Remote newsletter: 2.5M subscribers (#11 newsletter on LinkedIn)
    - 50% increase in non-branded search, 41% increase in AI search traffic
    - Content Champions: 4.2x engagement improvement
  - Identified problems:
    - Goal doesn't specify what problem it solves
      - Questions to clarify:
        - On target:
          - What does success look like? What happens when the brand impact is proven?
          - What's the impact of this on Crossover in general?
          - Is this about getting more budget, defending existing budget, or redirecting budget?
        - On problem:
          - What is the actual challenge - lack of funds? Not enough impressions? Poor conversion despite good brand metrics?
          - The document says "pragmatically focus our investment on quantifiable business value" - what was the focus before, and why is it changing now?
          - What decisions will be made differently based on proving brand impact?
        - On activities:
          - Why specifically these activities (baseline impact, target problem segments, optimize spend) and no others?
          - What hypothesis exists about which problem segments need brand content vs. other interventions?
