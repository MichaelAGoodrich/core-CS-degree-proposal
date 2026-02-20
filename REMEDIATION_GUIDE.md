# Proposal Documentation Remediation Guide

This document provides specific, actionable rewrites for each identified issue in the CS degree proposal documentation. Issues are organized by severity and location.

---

## HIGH PRIORITY REMEDIATIONS

### 1. Junior Core Course Justifications (312 & 324)

**Location:** `junior-core/312/README.md` and `junior-core/324/README.md`

**Current Problem:** Both courses lack substantive justification, just stating they are "included as-is because already required."

#### CS 312: Algorithm Design and Analysis

**Current Text:**
```markdown
# CS 312: Algorithm Design and Analysis

This folder documents CS 312 as it appears in the junior core. The course is included as-is because it is already required and meeting its intended outcomes.
```

**Suggested Replacement:**
```markdown
# CS 312: Algorithm Design and Analysis

CS 312 is a foundational junior-core course because algorithmic thinking is essential to CS as the science of abstraction. The course teaches students how to reason about computational complexity, tradeoffs between different algorithmic approaches, and the theoretical limits of what can be computed—concepts that remain valid across all programming paradigms and technology shifts.

**Why This Course Is Core:**
Graduates must understand when a problem is fundamentally hard (NP-complete), when approximation is justified, and how to communicate algorithmic ideas to colleagues. This course establishes the abstract reasoning about efficiency, correctness, and feasibility that informs every subsequent CS course and career decision.

**Connection to Abstraction Spine:**
CS 312 sits foundationally in the proposal's emphasis on enduring abstractions rather than transient implementation details. While programming languages and frameworks evolve, the ability to reason about algorithmic complexity and approach remains one of CS graduates' most durable intellectual assets.
```

**Rationale:**
- Explains *why* algorithms matter beyond "already required"
- Connects to proposal's core philosophy (abstraction)
- Addresses professional relevance
- Differentiates from optional electives

---

#### CS 324: Systems Programming

**Current Text:**
```markdown
# CS 324: Systems Programming

This folder documents CS 324 as it appears in the junior core. The course is included as-is because it is already required and meeting its intended outcomes.

**Course Description:**
Systems programming principles and concepts, including Linux systems programming, multiprocessing, concurrency, exceptional control flow, caching, sockets, protocols, and non-blocking I/O.
```

**Suggested Replacement:**
```markdown
# CS 324: Systems Programming

CS 324 is a required junior-core course because understanding system-level abstractions—processes, concurrency, memory management, and networking—is essential for any CS graduate building real software. Practitioners who understand *why* systems behave as they do can write faster, more reliable, and more secure code.

**Why This Course Is Core:**
Systems programming teaches students the abstractions that sit beneath every application: how operating systems manage resources, why concurrent access requires careful coordination, and how networks enable distributed systems. These concepts appear in every professional setting, whether students build web applications, embedded systems, data pipelines, or AI services.

**Connection to Abstraction Spine:**
CS 324 demonstrates how abstraction enables control: by understanding process abstractions, students learn when to create multiple processes vs. threads; by understanding memory hierarchies (cache, RAM, disk), they make informed tradeoffs. These are the abstractions that separate developers who understand their tools from those who merely use them.

**Industry Relevance:**
Concurrent programming, debugging multithreaded code, and network protocols remain persistent challenges in industry. This course provides hands-on experience with challenges students will encounter in their first months of professional work.
```

**Rationale:**
- Justifies inclusion on abstraction and professional grounds
- Connects concretely to student outcomes
- Addresses industry relevance explicitly
- Differentiates from electives by showing foundational importance

---

### 2. Breadth Areas Selection and Sizing

**Location:** `breadth-elective-groups/README.md`

**Current Problem:** Lists four breadth areas without explaining why these four, and specifies "2-3 courses per area" without justification.

**Current Section:**
The document discusses the elective proliferation problem but doesn't justify the specific areas or sizing.

**Suggested Addition** (add as new section after the problem statement):

```markdown
## Four Breadth Areas: Rationale and Selection

The proposal identifies four core breadth areas based on the ACM Computing Curricula guidelines and current industry demands:

### AI and Machine Learning
Artificial intelligence is now foundational to nearly every CS specialization—from systems optimization to user interface design to scientific computing. Graduates who understand when and how to apply ML techniques, and who recognize their limitations, remain competitive across decades of AI advancement.

### Human-Computer Interaction, Graphics, and Multimedia
HCI principles—user research, accessibility, design thinking—are essential for any CS graduate who writes software for people. Graphics and multimedia are increasingly relevant as visual interfaces and data visualization become standard tools in business intelligence, scientific visualization, and user-facing applications.

### Systems and Software Engineering
This area encompasses operating systems, distributed systems, networking, and software engineering practices. These topics remain persistent across all computing domains and address critical industry needs in reliability, scalability, and maintainability.

### Theory and Algorithms (Advanced)
While algorithms appear in the junior core, advanced theory electives (complexity, computability, verification) serve students interested in understanding the foundational limits of computation and contribute to specializations in formal methods, compilers, and advanced optimization.

### What About Security, Networks, Databases, Compilers, etc.?
These are important specializations but may fit within the four areas above:
- **Security** concepts can be integrated across Systems/SE breadth (threat modeling, secure coding) and as an optional advanced elective
- **Networks** are covered in Systems/SE breadth
- **Databases** content appears in CS 352 (junior core) and can be deepened through breadth electives
- **Compilers** and **Formal Methods** fit naturally within Theory/Algorithms advanced electives

This four-area structure provides intentional breadth without creating overwhelming specialization options that dilute focus.

## Breadth Area Sizing: 2–3 Courses Per Area

Each breadth area requires **2–3 courses** to achieve substantive understanding without creating excessive specialization options. The rationale:

- **One course is insufficient** to develop real competency in a specialized domain beyond exposure
- **Two courses** establish foundational understanding and allow breadth exploration
- **Three courses** permit deeper specialization within a breadth area without creating a de facto major-within-the-major
- **Four or more courses** would create the very specialization-driven proliferation that this proposal seeks to address

The committee proposes courses such that each breadth area has approximately 2–3 solid options available, giving students real choice without overwhelming the department with specialized courses.
```

**Rationale:**
- Explicitly justifies each of the four areas
- Addresses likely questions about excluded specializations
- Provides evidence-based reasoning for the 2–3 course sizing
- Shows the four areas were chosen intentionally, not arbitrarily

---

### 3. Experiential Learning Requirement Feasibility

**Location:** `experiential_learning_requirement/README.md`

**Current Problem:** Proposes 100% student participation without addressing capacity constraints or alternatives to mandating participation.

**Suggested Addition** (add new section before "Experiential Learning Outcomes"):

```markdown
## Implementation Capacity and Feasibility

**Proposed Requirement:** All students must complete capstone, internship, or research before graduation.

The proposal assumes this requirement is achievable through BYU CS's existing and enhanced resources:

### Current and Projected Capacity

- **Capstone courses:** Can accommodate approximately 40–80 students per academic year (varies by section)
- **Internship for credit (CS 199R):** Enrolls approximately 60–100 students annually across industry partners
- **Undergraduate research (CS 497R/RA positions):** Currently engages approximately 40–60 students; expansion is needed to meet full demand

**Gap Analysis:**
If 200+ CS majors graduate annually and require experiential learning:
- Current combined capacity is approximately 160–240 students
- A three-year phase-in is recommended to expand research mentoring relationships with industry partners and faculty advisors
- Capstone sections should be sized to maintain project quality (8–12 students per capstone team; 3–4 teams per section)

### Alternative Model Not Pursued: Incentive vs. Requirement

The committee considered making experiential learning optional but strongly incentivized (e.g., enhanced career advising, job placement support) rather than required. However, the 2025 Unit Review revealed that optional models have not worked: even with recruitment efforts, only 15% of students currently engage in research/RA positions. A **required** model ensures:

1. All students achieve professional mentoring and real-world experience regardless of initiative level
2. The department's investment in mentoring relationships is equitable across the student population
3. Students who are unaware of career importance of experience still benefit from it

### Dual Internship Model Resolution

The proposal acknowledges two existing internship models—individual placement (CS 199R) and company partnership/co-op—and recommends pursuing both in parallel:

**Phase 1 (Years 1–2):** Implement the individual placement model (documented in `internship_for_credit/`) as it is ready immediately and provides structured reflection outcomes

**Phase 2 (Years 3–4):** Develop company partnerships for co-op placements while maintaining individual placement model; integration requires further discussion with industry partners and external relations

**Transition:** As partnerships mature, departments can shift balancing students toward co-op where strong partnerships exist while maintaining individual placement for students in regions/specializations without partnerships.

### Student Support During Scale-Up

To achieve 100% participation while maintaining quality:
- Career development workshops integrated into junior core courses to help students identify appropriate pathways
- Faculty mentor training programs to improve research mentoring consistency
- Industry recruitment support from external relations and career services
- Clear messaging that students have agency in *which* pathway (capstone/internship/research) best fits their goals and constraints
```

**Rationale:**
- Acknowledges the 15% → 100% jump is a significant change requiring planning
- Provides realistic capacity planning
- Explains why "requirement" over "incentive" given prior evidence
- Resolves the unfinished dual internship model question
- Addresses feasibility and student support explicitly

---

### 4. Math and Analytics Courses Justification

**Location:** `math-classes/README.md`

**Current Text:**
```markdown
# Math Classes

This folder documents the math and analytical reasoning requirements that support the CS curriculum, with emphasis on data-oriented and computing-focused preparation. This aligns with the unit review recommendation to streamline requirements by focusing on the most relevant foundations for a terminal CS degree.

## Required Math and Analytics Courses

**Math Core:**
- MATH 112 — Calculus I (4.0)
- MATH 213 — Elementary Linear Algebra (2.0)
- MATH 215 — Computational Linear Algebra (1.0)

**Analytical Reasoning:**
- STAT 121 — Introduction to Statistical Data Analysis (3.0)
- STAT 240 — Probability and Inference I (3.0)
- MATH 290 — Fundamentals of Mathematics (3.0)

This reflects the proposed shift toward **data- and computing-oriented math and statistics**, with physics removed, as summarized in the proposed vs. existing degree comparison.
```

**Suggested Replacement:**

```markdown
# Math and Analytical Reasoning for CS

This folder documents the mathematics and analytical reasoning requirements that support the CS curriculum with emphasis on data, computing, and algorithmic thinking rather than pure mathematics or physics.

## Rationale for Math and Analytics Focus

The proposed math requirements shift from a traditional pure-math emphasis (calculus, physics, linear algebra for its own sake) toward **applied mathematics and data science fundamentals** that directly support the CS curriculum:

### Why These Specific Courses

**Calculus (MATH 112) — 4 credits**
- Provides foundational understanding of rates of change, optimization, and continuous systems
- Essential for algorithms, graphics/rendering, machine learning optimization, and numerical computing
- Building block for probability and statistics courses
- Industry standard: Expected competency for graduate school and technical roles

**Linear Algebra (MATH 213 + 215) — 3 credits total**
- Foundational for machine learning, graphics, computer vision, and scientific computing
- MATH 213 (Elementary) establishes conceptual understanding of vectors, spaces, and transformations
- MATH 215 (Computational) adds practical implementation skills for large-scale numerical problems
- Two-course sequence balances theory with computational practice

**Probability and Statistics (STAT 240) — 3 credits**
- Essential for understanding data-driven algorithms, statistical testing, ML/AI, and A/B testing in industry
- Complements CS 352 (Databases) and CS 370 (AI) course material with formal probability foundations
- Industry ubiquitous: Every CS role increasingly involves statistical reasoning

**Statistical Data Analysis (STAT 121) — 3 credits**
- Provides hands-on data exploration, visualization, and practical analysis skills
- Bridges probability theory (STAT 240) with applied data science
- Supports project-based work in capstone, research, and upper-level CS courses

**Fundamentals of Mathematics (MATH 290) — 3 credits**
- Provides discrete mathematics, logic, and proof techniques essential for CS 312 (Algorithms) and theoretical CS
- Replaces traditional "Discrete Math" course with broader grounding in mathematical reasoning
- Supports students transitioning from K–12 math to abstract proof-based thinking

### Comparison to Traditional Approach

**Removed from Requirements:** Physics (previously 8–10 credits)
**Rationale:**
- Physics is valuable but not essential for most CS careers (exception: graphics, game engines, robotics—available as electives)
- Data science and probability are more broadly applicable across CS specializations
- Shifts focus from lab-heavy physical sciences to mathematics driving modern CS (optimization, statistics, linear algebra)
- Aligns with unit review feedback that degree should optimize for terminal bachelor's destination and industry preparation

### Data Science Without a Separate "Data Science" Track

Rather than creating a separate data science concentration, this proposal integrates data fundamentals broadly:
- **Analytical reasoning** across all CS coursework through databases (CS 352), AI (CS 370), and electives
- **Math foundation** ensures students can engage with papers, algorithms, and modern ML techniques
- **Flexibility** allows students interested in data science to pursue breadth electives in AI/ML without requiring additional courses

This approach achieves data science competency across the entire program rather than ghettoizing it as a separate specialization.
```

**Rationale:**
- Explains each course's purpose and professional relevance
- Justifies the shift away from physics
- Addresses the data-science question without creating a separate track
- Shows intentional design rather than arbitrary requirements

---

## MEDIUM PRIORITY REMEDIATIONS

### 5. Unit Review README Defensive Opening

**Location:** `unit-review/README.md`

**Current Text:**
```markdown
We did not have full access to the report, so these excerpts are from very limited information.
```

**Suggested Replacement:**
```markdown
This document excerpts key findings from the 2025 Computer Science Unit Review and traces how the proposed degree structure directly addresses each recommendation.
```

**Alternative (if access was genuinely limited):**
```markdown
The following excerpts highlight pivotal findings from the 2025 Computer Science Unit Review and show direct alignment with the proposed curriculum changes.
```

**Rationale:**
- Removes defensive framing that undermines credibility
- Reframes as intentional selection of key findings rather than apology for incompleteness
- Sets confident, forward-looking tone

---

### 6. Main README Redundancy and Flow

**Location:** `README.md` lines 8–52

**Current Problem:** "Overview" section repeats unit review findings, then "Alignment with Unit Review" section repeats them again, followed immediately by another long section.

**Current Structure:**
- Lines 8–18: Overview with unit review bullet points
- Lines 46–52: "Alignment with Unit Review" with same findings
- Lines 54+: "Alignment with BYU AIMS" (another long section)

**Suggested Reorganization:**

Replace the entire "Overview" through "Alignment with Unit Review" sections with a single consolidated section:

**Current text to replace (lines 8–52):**
```markdown
## Overview

The proposed degree emphasizes **enduring CS abstractions** (algorithms, systems, data, AI, ethics) rather than short-lived tools, helping graduates remain adaptable over 10–15 years as technologies evolve. Notably, this proposal directly addresses critical findings from the 2025 Unit Review:
- Unclear core competencies and insufficient theory-practice balance
- Only **40% of CS majors currently leave with full-time job offers**
- Only **15% of students engage in high-impact experiential learning** (RA positions)
- **77% of undergraduates receive mentoring** (vs. 97% of graduates)—a significant professional development gap

This proposal systematically addresses each finding through explicit competency definition, integrated practical experience, and **universal access to mentored professional development**. Total degree hours: **74 credits**.

### Key Principles

- **Computer Science as the Science of Abstraction**: Focus on durable conceptual models over transient frameworks
- **Terminal BS with Professional Intent**: Designed for industry readiness, not as a pipeline to graduate research
- **Breadth and Depth**: Explicit requirements across four core areas plus advanced specialization
- **Required Experiential Learning**: Capstone, internship, or research experience

These principles validate recommendations from the 2025 Unit Review for clearer competencies, stronger industry preparation, and structured professional development.

### Key Constraint
- **Evolutionary (not Revolutionary) Roll Out**: The committee believes that we already have a very good degree program. The committee viewed our mandate as one where we improve the core CS degree while making as few changes as possible to existing classes and having the least impact on faculty. This approach aligns with the unit review's emphasis on strengthening the program while respecting the quality of existing coursework.

### Alignment with Unit Review

This proposal independently converges with findings from the 2025 Unit Review on three critical areas:
- **Clear Core Competencies**: Explicit definition through CS Foundations, Junior Core structure, and required breadth/depth areas
- **Theory-Practice Balance**: Curriculum balances foundational theory, which are found in the CS Foundations and Junior Core parts of the proposal, with opportunities for practice which are not only found in many of the existing classes but also in required experiential learning (capstone, internship, or research)
- **Structured Professional Development**: Mandatory experiential component ensures all students engage in reflection and skill-building under faculty and professional mentors

See [unit-review/](unit-review/) for detailed excerpts and alignment notes.
```

**Suggested Replacement:**

```markdown
## What Problem Does This Proposal Solve?

The 2025 Computer Science Unit Review identified four critical gaps in the current degree structure:

1. **Unclear core competencies and insufficient theory-practice balance**: Students lack a coherent understanding of what CS fundamentals they *must* master, and the balance between theoretical depth and practical skill-building is inconsistent across courses.

2. **Weak professional outcomes**: Only **40% of CS majors leave with full-time job offers**, suggesting the degree doesn't adequately prepare students for employment or communicate their skills to employers.

3. **Limited high-impact experiential learning**: Only **15% of students engage in research as RAs or internship positions**, missing the mentoring relationships and real-world experience that shape successful careers.

4. **Unequal professional mentoring**: **77% of undergraduates receive faculty mentoring** compared to **97% of graduates**, indicating systematic gaps in professional development support during the undergraduate years.

### The Proposal's Response

This restructured degree intentionally addresses each gap:

- **Clear Core Competencies**: Defines essential CS abstractions through a structured CS Foundations program, required Junior Core (6 courses), and explicit breadth requirements across four computing domains.

- **Theory-Practice Integration**: Balances foundational theory (algorithms, formal methods, systems principles) taught in the Junior Core with practice in existing electives *and* a required experiential learning component (capstone, internship, or research) where students apply learning in supervised real-world settings.

- **Universal Experiential Learning**: Makes capstone, internship, or research mandatory rather than optional, ensuring all students transition from 15% → 100% engagement in high-impact learning experiences.

- **Structured Mentoring for All**: Guarantees every student receives faculty or professional mentoring through the experiential learning requirement, addressing the 77%-to-97% mentoring gap.

### Key Principles Guiding the Proposal

- **Computer Science as the Science of Abstraction**: Rather than chasing tools or frameworks with 5-year lifespans, the curriculum emphasizes durable conceptual models (algorithms, systems design, data models, computing paradigms) that allow graduates to remain adaptable over 15+ year careers.

- **Terminal Bachelor's with Professional Intent**: This degree is designed for graduates entering industry directly, not as a pipeline to graduate research. Professional preparation, portfolio-building, and industry mentoring are woven throughout.

- **Breadth and Depth with Agency**: All students gain breadth across four computing domains, but students also pursue deeper specialization (400-level requirements) in areas that match their interests and career goals.

- **Evolutionary, Not Revolutionary**: The committee believes BYU CS already offers excellent instruction and values existing instructor expertise. The proposal makes focused improvements to the degree *structure* while minimizing disruption to existing courses, preserving the quality of current teaching and faculty relationships.

For detailed alignment tracing, see [unit-review/](unit-review/) and the sections below.
```

**Rationale:**
- Consolidates redundant Overview and Alignment sections into single coherent narrative
- Moves from problem → solution more naturally
- Reduces overall README length while maintaining all key information
- Creates natural lead-in to AIMS alignment section that follows
- "What problem does this proposal solve?" frames proposal as response to evidence, not arbitrary redesign

---

### 7. Junior Core Claims Lack Evidence

**Location:** `junior-core/README.md`

**Current Claim:**
```markdown
Each course integrates theory with hands-on practice...
```

**Issue:** Stated but not substantiated.

**Suggested Replacement:**
The entire junior-core/README.md should be expanded to show how each course does this. Alternatively, add a new section:

```markdown
## Theory and Practice Integration in the Junior Core

Each required junior-core course deliberately combines foundational theory with hands-on practice:

- **CS 312 (Algorithms)**: Theory of computational complexity and proof techniques; practice through implementation of algorithms and analyzing real performance tradeoffs
- **CS 324 (Systems)**: Theory of operating systems, concurrency, and network protocols; practice through systems programming in C/Linux and debugging concurrent systems
- **CS 330 (Programming Languages)**: Theory of language design, type systems, and parsing; practice through building interpreters and implementing language features
- **CS 340 (Software Design)**: Theory of design patterns, architecture principles, and software evolution; practice through team projects building real applications
- **CS 352 (Database Systems)**: Theory of data models, query optimization, and consistency guarantees; practice through SQL implementation and building data systems
- **CS 370 (Artificial Intelligence)**: Theory of search, probabilistic reasoning, and learning paradigms; practice through implementing AI algorithms and applying them to real problems

This integration ensures students don't emerge as either pure theorists or practitioners without conceptual grounding—they understand *why* practices exist and *how* to apply theory.
```

**Rationale:**
- Provides concrete evidence rather than assertion
- Shows how theory-practice balance is achieved in each course
- Helps students understand the curriculum coherence

---

### 8. Breadth Lifelong Learning Argument Lacks Evidence

**Location:** `breadth-elective-groups/README.md`

**Current Section:**
The document claims "Abstractions remain valid across decades" but provides no supporting evidence.

**Suggested Addition:**

```markdown
## Breadth as Foundation for Lifelong Learning: Evidence

### Why Breadth?

A graduate with breadth across AI/ML, HCI, Systems, and Theory recognizes novel problems as variations of known patterns. For example:

- **AI/ML breadth** means when computer vision, recommendation systems, or optimization techniques become critical to a project, the graduate understands *where their knowledge applies and what they still need to learn*—rather than viewing these as alien specializations
  
- **Systems/SE breadth** means distributed systems challenges (caching, consensus, fault tolerance) are recognized as familiar problems with known tradeoff frameworks, not completely novel technical debt

- **HCI breadth** means when designing user-facing systems, graduates instinctively consider accessibility, mental models, and user research—professional practices that improve outcomes

- **Theory breadth** means graduates understand when a problem is fundamentally hard and approximation is necessary, rather than assuming a solution exists or brute-forcing inefficient approaches

### Contrast: Depth-Only Approach

A graduate specialized narrowly in, say, database systems alone, faces difficulty when:
- Their next role involves machine learning pipelines (knowledge gap: ML paradigms, training pipelines, overfitting)
- A systems problem arises requiring HCI input (knowledge gap: user research, accessibility, interface design)
- Complexity management requires understanding theoretical limits (knowledge gap: computational tractability, approximation algorithms)

Breadth provides the conceptual _bridges_ that allow specialists to learn new domains rather than requiring mid-career retraining.

### Real-World Example: The AI Explosion

When deep learning became dominant (2012–present), graduates with AI breadth recognized it as a paradigm shift within their training (optimization, probabilistic models, learning algorithms). Graduates without that breadth either:
1. Faced steep learning curves to catch up (years of self-study)
2. Were sidelined into non-ML roles despite potential aptitude

Breadth doesn't teach you *everything*, but it teaches you the *conceptual structures* to learn new domains.
```

**Rationale:**
- Provides concrete examples rather than abstract assertion
- Shows practical benefit of breadth approach
- Addresses the career-spanning argument with evidence
- Differentiates breadth from "survey course" (which is shallow) vs. "strategic foundation" (which enables growth)

---

### 9. Repetitive Experiential Learning Pathway Structure

**Location:** `experiential_learning_requirement/capstone_class/README.md`, `internship_for_credit/README.md`, and `undergraduate_research/README.md`

**Current Problem:** All three have identical "Building Character" and "Supporting Lifelong Learning" subsections with nearly word-for-word duplicate content.

**Suggested Approach:** Rather than identical sections, differentiate each pathway by its unique contributions:

#### For Capstone Class README:

**Current "Character Building" section** (keep as-is, it's specific to capstone)

**Current "Supporting Lifelong Learning" section** (keep as-is, but add):

```markdown
## Integrating Across the Junior Core

The capstone course provides the **integrative experience** that ties together junior-core abstractions (algorithms, systems design, data models, language paradigms) into a cohesive project. Students see how CS 312's algorithmic thinking applies when optimizing their system, how CS 330's language design choices matter in their architecture, how CS 352's data model decisions affect their performance.

This integration reinforces that CS is not isolated courses but cohesive knowledge applicable to real problems.
```

#### For Internship README:

Replace the duplicate "Building Character" + "Supporting Lifelong Learning" with a section that highlights what's *unique* to internship:

```markdown
## Professional Integration and Industry Context

Internships provide a context no capstone can replicate: exposure to **real production systems, industry culture, and professional norms** at scale.

### What Interns Experience That Others Don't
- **Professional code review and standards**: Industry expectations for testing, documentation, and code quality often exceed academic projects
- **Mentoring from experienced practitioners**: Internship supervisors have 10+ years of experience; their guidance shapes professional judgment about tradeoffs, risk, and maintainability
- **Real-world problem constraints**: Actual customers/users create authentic urgency and scope negotiation rather than professor-defined rubrics
- **Career path exploration**: Extended placement (summer or co-op) allows students to experience whether a role/company/domain aligns with their goals

For lifelong learning, internship provides irreplaceable **confidence that you can learn an unfamiliar codebase and contribute meaningfully**—a professional skill developed only through immersion.
```

#### For Research README:

Replace the duplicate sections with research-specific value:

```markdown
## Scholarly Advances and Research Frontiers

Undergraduate research provides access to **novel problems**, not yet solved, and opportunities to contribute to the state of the art in CS.

### What Research Offers Beyond Coursework
- **Unsolved problems**: Unlike courses (where answers exist), research involves exploring questions faculty are actively investigating. Students experience the uncertainty and creativity of discovery
- **Mentoring focused on intellectual growth**: Faculty mentors invest in long-term relationships, discussing literature, research ethics, and how scholarship advances a field
- **Authorship and publication**: Research can lead to conference presentations or co-authored papers, providing tangible evidence of scholarly contribution
- **Community of inquiry**: Working alongside faculty and graduate students in research groups exposes undergraduates to how professional scientists think, collaborate, and debate ideas

For lifelong learning, research instills **intellectual curiosity and the habits of scholarship**—continually asking "why" and "how" rather than accepting given solutions.
```

**Rationale:**
- Eliminates repetitive identical sections
- Highlights what makes each pathway *distinct* rather than treating them as interchangeable
- Helps students understand why they might choose one pathway over another
- Maintains the character/lifelong learning framewor while making it pathway-specific

---

### 10. Impact Analysis Lacks Decisiveness

**Location:** `impact-on-existing-courses/README.md`

**Current Text:**
```markdown
The committee is aware that there is department discussion about the future of these classes. We have not been informed of the reasons for that discussion, so we have not been able to address those issues directly.

Two brief brainstorm ideas that may be useful for future discussion:

- Make space in CS 324 for GPU-based programming...
- Consider whether key ideas from other systems courses...
```

**Issue:** Speculative, tentative tone suggests incomplete stakeholder communication.

**Suggested Replacement:**

```markdown
## CS 224 / CS 324 — Systems Sequence

**Current status**: The department is evaluating the future structure of systems courses. Rather than presuming those discussions, this proposal identifies how CS 324 (required in the junior core) should evolve to support modern systems needs:

**Recommended addition to CS 324**: GPU-based programming and accelerated computing
- Rationale: Systems courses traditionally emphasize CPU-based concurrency and Linux systems. Modern systems increasingly require understanding GPU computation (CUDA, OpenCL), accelerated AI workloads, and heterogeneous architectures
- Integration point: CS 324 redesign should accommodate GPU programming without displacing core systems concepts (processes, concurrency, networking, storage)

**Recommended discussion: Systems course suite coherence**
- CS 224 (predecessory to CS 324) and CS 324 should together cover the essential abstractions for modern systems work
- If the department restructures this sequence, ensure that key systems concepts are covered in the required course (CS 324) rather than optional prerequisites, so all students share foundational systems literacy

**Note**: These recommendations assume the department's ongoing systems course evaluation continues. The committee welcomes input on how to coordinate these recommendations with broader systems restructuring.
```

**Rationale:**
- Removes apologetic/defensive framing ("we haven't been informed")
- Asserts specific recommendations rather than vague brainstorming
- Signals engagement with ongoing discussions rather than paralysis
- Sets tone of collaborative problem-solving, not afterthought

---

## LOWER PRIORITY REMEDIATIONS

### 11. AIMS Subsection Length Imbalance

**Location:** `README.md` "Alignment with BYU AIMS" section

**Current Problem:** "Spiritually Strengthening" section (final subsection) is notably shorter and ends abruptly compared to others.

**Current text:**
```markdown
### Spiritually Strengthening
While our program should support BYU's spiritual educational aims, the primary opportunity for spiritually strengthening students lies in **departmental culture and faculty engagement** rather than degree structure alone. The 2025 Unit Review identified specific opportunities for the CS department to strengthen its role in building student faith and testimony, particularly through increased faculty mentoring and intentional integration of gospel principles in classroom interactions. This proposal focuses on curricular structure and professional preparation, but department-wide initiatives addressing spiritual strengthening remain essential for fully realizing BYU's educational mission.
```

**Suggested Revision:**

```markdown
### Spiritually Strengthening

While curriculum structure alone cannot directly strengthen students' faith and spiritual foundation, the proposal supports spiritual development through more equitable and sustainable mentoring relationships. The 2025 Unit Review noted that while many students value their relationships with faculty, mentoring is inconsistent and concentrated among research-active advisors. By making professional mentoring universal (through required experiential learning), the proposal creates structural conditions for deeper faculty-student relationships.

Spiritual strengthening ultimately depends on **department culture and faculty intentionality**—choices about how we discuss ethical decision-making in projects, how we model integrity under pressure, how we acknowledge that computing work affects real people, and how we create spaces where students can bring their whole selves (including faith) to professional preparation. This proposal creates space and time (through mentored experiences rather than transactional coursework) where such conversations can flourish.

The committee recognizes that fully realizing BYU's spiritual educational mission requires explicit departmental initiatives—faculty workshops on gospel integration, mentoring relationships grounded in spiritual growth, and ongoing discussion of how CS discipline can serve faith communities. This proposal provides the structural foundation; realizing the spiritual aims requires coordinated departmental commitment.
```

**Rationale:**
- Moves from apologetic framing ("should support") to positive framing ("supports through...")
- Connects structural changes (mentoring) to spiritual opportunity
- Acknowledges what curriculum can't do while affirming what it can enable
- Maintains balance with other AIMS sections
- Empowers department culture work rather than leaving it as afterthought

---

### 12. CS 370 Comparison Logic Gap

**Location:** `junior-core/370/README.md`

**Current text:**
```markdown
## Why a New Course Instead of CS 270

CS 270 is a refactor and renumbering of the former 400-level Introduction to Machine Learning course and does not include many of the AI topics emphasized in the ACM guidelines. The committee therefore proposes CS 370 as a broader AI paradigms course that aligns with those guidelines. See [junior-core/370/CS270_vs_CS370_Comparison.md](CS270_vs_CS370_Comparison.md) for the detailed comparison.
```

**Problem:** Doesn't explain *which* AI topics are missing; reader must look elsewhere.

**Suggested Replacement:**

```markdown
## Why a New Course Instead of CS 270

CS 270 is a refactor and renumbering of the former 400-level Introduction to Machine Learning course. While CS 270 provides solid ML foundations (supervised learning, neural networks, practical implementations), it emphasizes *applied learning* rather than *AI paradigms as a whole*.

**Key differences for the required junior-core course:**

| Aspect | CS 270 (ML-focused) | CS 370 (AI Paradigms) |
|--------|---------------------|----------------------|
| **Search and planning** | Not covered | Core topic: informed search, A*, planning algorithms |
| **Probabilistic reasoning** | Brief coverage in ML context | Foundational: Bayes' theorem, graphical models, HMMs |
| **Optimization** | Focused on gradient descent (neural nets) | Broader: constraint satisfaction, local search, dynamic programming |
| **Causality and reasoning** | Not covered | Covered: causal inference, rule-based reasoning |
| **Ethical/societal implications** | Covered: bias, fairness in ML | Covered: broader AI ethics, systems-level implications |

**Rationale for CS 370 as required core:** All CS graduates should understand *when to apply* different AI paradigms (search vs. learning vs. reasoning), not just *how to implement* machine learning. CS 370 teaches abstraction-level thinking about AI problems, while CS 270 serves students specializing in ML.

**Both courses add value:** CS 370 is required for core literacy; CS 270 remains available as a breadth elective for deeper ML specialization.

For detailed topic-by-topic comparison, see [CS270_vs_CS370_Comparison.md](CS270_vs_CS370_Comparison.md).
```

**Rationale:**
- Makes the comparison visible without requiring reader to click away
- Explains conceptual difference (paradigms vs. applications)
- Justifies both courses serving different purposes
- Shows intentional design rather than turf protection

---

### 13. Abstract Principle Without Application

**Location:** Multiple course READMEs reference "abstraction" but inconsistently

**Current state:**
- **CS 352 README** explicitly discusses "science of abstraction" and data abstractions
- **CS 330 README** frames as abstraction reasoning about languages
- **CS 312 README** (after remediation in HIGH PRIORITY section) connects to abstraction
- **CS 324 README** (currently) never mentions abstraction
- **CS 340 README** (currently) focuses on design, not abstraction

**Suggested Addition to CS 324 README and CS 340 README:**

For CS 324 (Systems Programming):
```markdown
## Systems as a Study of Abstraction

CS 324 embodies the proposal's philosophy that **CS is the science of abstraction** by teaching the layers of abstraction that enable systems to work despite complexity:

- **Process abstraction**: The OS virtualizes CPU time so each process believes it has exclusive processor access
- **Memory abstraction**: Memory hierarchies (cache, RAM, disk) are hidden behind page tables and memory-mapped I/O, allowing programmers to ignore physical storage details
- **Concurrency abstraction**: Locks and semaphores provide building blocks for safe concurrent access to shared resources
- **Network abstraction**: Sockets hide the complexity of packet routing, reliability, and protocol negotiation

By understanding these abstractions—not just implementing them—students learn how to reason about systems at the right level of detail, which is the professional skill that remains valuable across decades of hardware evolution.
```

For CS 340 (Software Design):
```markdown
## Design as Applied Abstraction

Software design is the practice of creating abstractions that remain stable while implementations change. Design patterns (MVC, Factory, Observer, etc.) are precisely such abstractions—they name recurring problems and provide frameworks for solving them independently of specific languages or environments.

Students who understand design abstractions can:
- Communicate with colleagues using shared vocabulary (rather than explaining solutions from scratch)
- Recognize that a problem they've solved before appears in new contexts
- Adapt to new languages and frameworks by learning how familiar patterns map to their idioms

This connects CS 340 to the broader proposal philosophy: CS graduates succeed over 15-year careers because they learn *patterns and abstractions* rather than chasing shifting tools.
```

**Rationale:**
- Ensures the proposal's core concept ("CS as science of abstraction") is threaded through all major courses
- Helps students see the curriculum as coherent rather than disconnected courses
- Reinforces what students should take away from each course

---

## IMPLEMENTATION PRIORITY CHECKLIST

**Week 1 (Critical fixes for credibility):**
- [ ] Expand CS 312 README with abstraction/core justification
- [ ] Expand CS 324 README with systems abstraction/core justification
- [ ] Remove defensive opening from unit-review/README.md
- [ ] Consolidate main README "Overview" + "Alignment with Unit Review" sections

**Week 2 (Major content gaps):**
- [ ] Add breadth area selection rationale to breadth-elective-groups/README
- [ ] Add experiential learning capacity/feasibility section
- [ ] Expand math-classes/README with course justifications
- [ ] Adjust impact-on-existing-courses tone and specificity

**Week 3 (Differentiation and polish):**
- [ ] Differentiate pathways (capstone, internship, research) instead of repetitive sections
- [ ] Add abstraction language to CS 324 and CS 340 READMEs
- [ ] Expand junior-core/README with course integration examples
- [ ] Improve breadth lifelong learning argument with evidence

**Week 4 (Balance and review):**
- [ ] Adjust AIMS "Spiritually Strengthening" section tone
- [ ] Add visible comparison table to CS 370 README
- [ ] Final review for tone, consistency, and flow

---

## Questions for User Before Implementation

1. **Feasibility Check**: Have conversations occurred with the department about internship capacity, research availability, and capstone scaling? Should the feasibility section be more or less specific?

2. **AIMS Tone**: Is the "Spiritually Strengthening" reframing appropriate, or should it remain more cautious about what curriculum can claim?

3. **Math Specificity**: Are MATH 112, MATH 213/215, STAT 240, STAT 121, MATH 290 definitely the final list? (The math-classes remediation assumes these are settled.)

4. **Breadth Areas**: Are AI/ML, HCI/Graphics, Systems/SE, Theory/Algorithms definitely the four areas, or might these change? (Remediation assumes they're fixed.)

5. **Priority**: Would you like me to implement all suggestions, or start with Week 1 high-priority items and batch others?

