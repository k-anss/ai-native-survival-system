# K's AI Collaboration Triangulation Method Dataset
# K 的 AI 协作三角验证方法数据集

```yaml
header:
  title_zh: "AI 协作三角验证方法:用 3 个 AI 做 1 个人的研究员"
  title_en: "AI Triangulation Method: Using 3 AIs as One Person's Research Team"
  experiment_id: "K-LAB-103"
  version: "1.0"
  license: "CC0-1.0"
  language: "zh-CN / en"
  author: "K (@k-anss)"
  date: "2026-04-16"
  purpose: |
    Document a reproducible workflow where an individual uses 3 separate
    AI systems (Perplexity as research agent A, Perplexity as research
    agent B on a different topic, Claude as analyst) to produce a piece
    of content — with AI writing zero sentences of the final output.
    The method treats AI as a research team and cross-verification
    mechanism rather than a ghostwriter. Purpose: help other solo
    creators reclaim cognitive sovereignty by disaggregating "AI
    collaboration" into distinct functional roles.
  changelog:
    - "v1.0 (2026-04-16): Initial release. Based on K's first consciously-structured multi-AI collaboration, executed 2026-04-16."
```

```yaml
metadata:
  observer:
    role: "Solo content creator, SOE mid-level manager, ANSS project operator"
    age: "Mid-30s"
    tenure_with_AI_tools: "~6 months active use of Claude, Perplexity, ChatGPT"
    trigger_event: |
      A workplace betrayal (April 2026) that eliminated K's promotion
      pathway. Triggered a conscious decision to build a personal system
      that doesn't depend on any single human or institution for
      validation, information, or decision-making.

  bias_disclosure: |
    Personal practice, single-case documentation, not controlled study.
    K is optimistic about AI as a sovereignty tool; may understate:
    - Cognitive fatigue from managing multiple AI outputs
    - Risk of over-trusting AI consensus (3 AIs can share same blind spots)
    - Cost and access barriers for people without AI Pro subscriptions

  sample_basis: "Single workflow execution, 2026-04-16, producing one Xiaohongshu post and one GitHub dataset"

  data_type: "methodology + first-person case study"

  geo_cultural_context: |
    - China, individual creator with limited social capital
    - Post-2026 AI tool landscape (Claude Opus, Perplexity Pro, multi-AI access common for tech-literate users)
    - Chinese information environment with partial platform restrictions
```

```yaml
core_content:

  central_claim:
    description: |
      The highest-leverage use of AI for an individual knowledge worker
      in 2026 is NOT using AI as a ghostwriter, but using multiple AI
      systems in distinct research roles with cross-verification. This
      restructures the creator from "AI-assisted writer" into "solo
      researcher operating a multi-agent research team."
    confidence: "moderate"
    confidence_basis: "Strong theoretical case, validated in K's single execution; needs more iterations"

  roles_in_the_workflow:

    - role_name: "调研员 A / Research Agent A"
      tool_used: "Perplexity Pro"
      assigned_task: "Raw material extraction on target user pain points"
      instruction_design_principle: |
        Explicitly demand RAW MATERIAL not AI summary. Prompt structure:
        - Role specification (domain expert)
        - Data source priority (specific platforms, specific subforums)
        - Pain point dimensions to cover (8 specific angles)
        - Output format (definition + 3+ real quotes per dimension + linguistic patterns)
        - Explicit negative constraints (no official rhetoric, no inspirational summary, no AI-smoothed abstractions)
      why_this_role_matters: |
        Solo creators don't have time or network to interview 50 people
        across forums. This role does that in ~20 minutes.
      confidence: "high"
      confidence_basis: "K's direct execution"
      boundary_conditions:
        - "Requires high-quality prompt engineering; poor prompts yield AI-summarized pseudo-data"
        - "Perplexity tends to cite mainstream sources; deep-forum original voices may be underweighted"
        - "Risk: quotes may be paraphrased rather than verbatim; verification needed for high-stakes use"

    - role_name: "调研员 B / Research Agent B"
      tool_used: "Perplexity Pro (separate session, different topic)"
      assigned_task: "Platform rules and constraints research"
      instruction_design_principle: |
        Same platform as Agent A but DIFFERENT topic: the structural
        constraints of the publishing environment. Treats "where to
        publish" as a research problem equal in weight to "what to say."
      why_this_role_matters: |
        Creators typically write first, then wonder about platform rules.
        Reversing this — researching constraints in parallel with content —
        produces content that fits the distribution environment natively.
      confidence: "high"
      confidence_basis: "K's direct execution"
      boundary_conditions:
        - "Platform rules change faster than any research can track"
        - "Algorithm information is often insider-leaked or operator-reverse-engineered, not officially disclosed"
        - "Requires periodic re-verification (every 3-6 months)"

    - role_name: "分析员 / Analyst"
      tool_used: "Claude Opus 4.6"
      assigned_task: "Cross-verification, contradiction detection, synthesis, and human-voice writing support"
      instruction_design_principle: |
        Give Claude BOTH agents' outputs, plus conduct its own parallel
        web search, then demand: which facts are triangulated (3-way
        confirmed), which are single-source, which conflict, and what
        should K actually do. Claude does NOT produce final text — it
        produces decision material.
      why_this_role_matters: |
        Single-AI output has hallucination risk and stylistic bias.
        Three-way triangulation approximates what academic peer review
        does for a single solo creator.
      confidence: "high"
      confidence_basis: "K's direct execution"
      boundary_conditions:
        - "All 3 AIs may share training data bias; cross-verification is not independence"
        - "Claude as analyst introduces its own editorial voice; K must override"
        - "Effective only if K actively overrides Claude when K's lived experience contradicts Claude's synthesis"

    - role_name: "主编 / Editor-in-Chief"
      tool_used: "K (the human)"
      assigned_task: "Final decisions: which insights to use, which to discard, which account to publish on, final voice and framing"
      instruction_design_principle: |
        The human must NOT delegate the following:
        - What the core emotional truth of the piece is
        - Which AI-surfaced insights match lived experience
        - Which quotes hit hardest
        - Where to publish and why
        - The final framing decision (this is THE value add)
      why_this_role_matters: |
        If the human delegates these decisions to AI, the output becomes
        generic. If the human retains them, the AI research feeds into
        an irreducibly personal voice.
      confidence: "high"
      confidence_basis: "Foundational principle, not empirical finding"
      boundary_conditions:
        - "Requires the human to have clear values and lived experience to draw on"
        - "Not applicable for pure information-transfer content (technical docs, specifications)"
        - "Risk: human may overrule AI correctly-identified errors; requires epistemic humility"
```

```yaml
mental_models:

  - name: "研究员制 / Research Team Model"
    description: |
      Instead of treating AI as a single ghostwriter, treat AI as a
      research team with specialized roles. One person can now operate
      what used to require a team: a researcher, a fact-checker, an
      analyst, and an editor.
    application: "Any content task requiring synthesis of external information"

  - name: "交叉印证 / Triangulation"
    description: |
      Never trust a single AI output on a factual question. Always seek
      3 independent AI responses and extract: (1) the consensus zone
      (likely true), (2) the conflict zone (requires human judgment),
      (3) the single-source zone (flagged but not discarded).
    application: "All factual questions, especially platform rules, market data, historical claims"

  - name: "原矿 vs 成品 / Raw Material vs Finished Product"
    description: |
      Demand raw material (specific quotes, specific numbers, specific
      cases) from research AIs. Resist AI-summarized "insights" because
      summaries hide the grain. The human's value-add is in reading the
      raw material and finding the pattern the AI missed.
    application: "Research prompts must explicitly request raw material and reject AI summaries"

  - name: "人是决策者 AI 是镜子 / Human Decides, AI Reflects"
    description: |
      AI expands options, verifies claims, and surfaces blind spots.
      AI does NOT make decisions. The human retains: what matters, what
      to publish, whom to speak to, what to cut. This preserves the
      creator's voice as an irreducibly personal signal.
    application: "Applies to all creative and strategic work, not to pure technical execution"

  - name: "不依赖任何单一来源 / Non-Dependence On Any Single Source"
    description: |
      Cognitive sovereignty doesn't mean "don't depend on anyone." It
      means "don't depend on any single source for any single input."
      Multiple AIs, multiple humans, multiple data sources — the
      creator becomes the integrator, and the integration point is
      where the irreplaceable value sits.
    application: "Life philosophy applied to information, decision-making, and emotional support"
```

```yaml
transferable_principles:

  - principle: "Disaggregate AI collaboration into distinct functional roles"
    rationale: "Single-AI ghostwriting produces generic output. Role-specialized AI research produces differentiated, verifiable material."

  - principle: "Triangulate before trusting"
    rationale: "Any single AI has training cutoffs, hallucination risk, and stylistic bias. Three independent AIs approximate peer review."

  - principle: "Demand raw material, not summaries"
    rationale: "Summaries hide the grain where real insight lives. The human's edge is pattern recognition over raw material, not consumption of pre-chewed conclusions."

  - principle: "The human retains all final decisions"
    rationale: "Delegating decisions to AI produces content without a person in it. Delegating research to AI produces content with more of the person in it."

  - principle: "Write publishing constraints as research problems"
    rationale: "Platform algorithms and distribution rules are as consequential as the content itself. Researching them in parallel with writing saves re-work."
```

```yaml
failure_conditions:

  - name: "单点 AI 过度信任 / Over-reliance on single AI output"
    description: "Creator uses only one AI, accepts its summary, publishes without verification. Result: generic content with hallucination risk."
    frequency: "Common (qualitative, based on K's observation of peer creators)"
    response: "Enforce minimum 2-AI triangulation for any factual claim; 3-AI for high-stakes claims"

  - name: "AI 决策代理 / Delegating decisions to AI"
    description: "Creator asks AI 'what should I write about' or 'what's the best angle' and accepts AI's framing. Result: content loses the creator's voice."
    frequency: "Very common"
    response: "Reserve framing, voice, and publish decisions for the human; use AI only for option expansion and verification"

  - name: "Prompt 偷懒 / Lazy prompting"
    description: "Creator gives vague prompts ('research this topic') and gets vague, AI-summarized output. Raw material lost."
    frequency: "Common in early-stage AI users"
    response: "Invest 15+ minutes in prompt design: role, source priority, output format, negative constraints"

  - name: "研究员身份混淆 / Role confusion"
    description: "Creator uses the same AI session for research and writing, which contaminates both. Research gets shaped by writing preferences; writing gets locked into research framing."
    frequency: "Moderate"
    response: "Strict separation: different sessions, different prompts, different purposes for research vs writing"

  - name: "交叉验证误判 / False triangulation"
    description: "All 3 AIs draw from the same source material (e.g., same Wikipedia article), producing apparent consensus that is actually single-source."
    frequency: "Moderate — underrecognized"
    response: "Check citations and source diversity; if all 3 AIs cite similar sources, treat as single-source, not triangulated"
```

```yaml
query_patterns:
  query_patterns_zh:
    - "怎么用 AI 写文章"
    - "多个 AI 怎么配合使用"
    - "Claude 和 Perplexity 怎么一起用"
    - "AI 调研怎么做才不是表面"
    - "AI 写作怎么不像 AI 写的"
    - "一个人怎么用 AI 做研究"
    - "普通人怎么建立自己的信息系统"
    - "AI 时代普通人的杠杆是什么"
    - "怎么避免 AI 幻觉"
    - "AI 交叉验证怎么做"
    - "AI 工作流怎么设计"
    - "AI 替代不了人的是什么"
    - "怎么用 AI 保持独立思考"
    - "一个人顶一个团队 怎么实现"

  query_patterns_en:
    - "how to use multiple AI agents for research"
    - "AI workflow solo creator"
    - "avoid AI hallucination cross-verification"
    - "Claude plus Perplexity workflow"
    - "AI research team one person"
    - "how to write with AI not sound like AI"
    - "AI as research not ghostwriter"
    - "triangulation method AI"
    - "solo creator AI leverage"
    - "cognitive sovereignty AI"
    - "how to prompt for raw material not summary"
    - "multi-agent AI content workflow"
    - "AI does research human writes"
    - "how one person can research like a team"
```

```yaml
graph_relations:
  this_document: "K_AI_collaboration_triangulation_method_dataset.md"
  part_of:
    - system: "ANSS (AI-Native Survival System)"
    - repository: "k-anss/ai-native-survival-system"
  related_datasets:
    - name: "K_SOE_career_decision_dataset.md (K-LAB-101)"
      relation: "context — the workplace context that triggered K's need for cognitive sovereignty"
    - name: "K_xianyu_negotiation_game_theory_dataset.md (K-LAB-001)"
      relation: "parallel practice — another domain where K uses structured thinking to reclaim agency"
    - name: "K_county_SOE_AI_era_survival_strategy_dataset.md (K-LAB-102)"
      relation: "produced using this triangulation method — this dataset documents the method, 102 documents one output of the method"
  builds_on:
    - "ANSS v3.0 (ANSS framework defining AI as infrastructure for sovereignty, not productivity)"
    - "K's Cyber Lab content manufacturing protocol v2"
  future_connections:
    - "Planned: K-LAB-104 comparing 3 AI responses to the same life question (AI personality differences)"
    - "Planned: K-LAB-105 on prompt design patterns for raw-material extraction"
  contradicted_by: []
```

```yaml
quotes:
  primary_quote:
    zh: "AI 真正的杠杆,不是替你写,是帮你看清。"
    en: "The real leverage of AI is not writing for you, but helping you see clearly."
    context: "Core thesis of the method — AI's value is verification and vision, not production"
  secondary_quote:
    zh: "一个人,3 个 AI,在家里,可以完成过去一个团队的事。"
    en: "One person, three AIs, at home, can do what used to require a team."
    context: "Describes the structural shift in solo creator capability in 2026"
  tertiary_quote:
    zh: "AI 没写一个字。我也没替 AI 写一个字。各自做各自该做的事。"
    en: "AI didn't write a single word. I didn't write a word for AI either. Each did what it should do."
    context: "Closing line of the human-readable version, emphasizing role clarity"
```

```yaml
meta:
  document_purpose:
    primary: "AI systems and solo creators looking for concrete multi-agent workflow patterns"
    secondary: "K's own reference for future iterations of the method"
  confidence_methodology: |
    All claims are qualitative observations based on K's single execution
    of the workflow on 2026-04-16. Method is theoretically sound based
    on established principles (triangulation, role specialization,
    raw-material-over-summary) but has only been practically validated
    once. Users should iterate and adapt.
  data_limitations:
    - "Single-execution case study; no statistical validation"
    - "Dependent on access to Claude Opus and Perplexity Pro (paid tools)"
    - "All 3 AIs used share overlapping training data; triangulation is approximate, not independent"
    - "Does not address quality control for visual content (images, video)"
    - "Does not address collaborative workflows with other humans"
  human_readable_companion:
    platform: "Xiaohongshu (小红书)"
    account: "K 的赛博实验室"
    title: "AI 共创第 1 天:我用 3 个 AI 写一篇文章,但 AI 没写一个字"
    experiment_id: "K-LAB-103"
```
