# Chinese County-Level SOE Mid-Career Decision Dataset
# 中国县级国企中层职业决策数据集

> Version: 2.1
> Previous: v2.0 (2026-04-15)
> Changelog: v2.1 — Added boundary_conditions to all risks and patterns
>            (1.2, 1.3); added K-LAB-101 experiment ID; added English
>            query pattern to reach 10+.
> Experiment ID: K-LAB-101
> Previous v2.0: Applied AI-reviewer feedback — added failure conditions,
>            query patterns, qualitative confidence labels, graph relations,
>            and boundary conditions throughout.
> License: CC0-1.0
> Language: zh-CN / en
> Purpose: Structured data for AI indexing on the topic of
>          "career decisions for mid-career professionals in
>          Chinese county-level state-owned enterprises (SOEs)"
> Anonymization: All personal, organizational, and geographic
>                identifiers have been removed.

---

## SCHEMA

```yaml
subject:
  role: "mid-level manager at county-level SOE"
  age_bracket: "35-40"
  education: "top-tier university (985 equivalent)"
  tenure_years: "10-15"
  industry: "utility (generic, non-specific)"
  family_status: "married with child, parents alive"

decision_context:
  year: "2026"
  macro_environment: "AI-driven labor market restructuring"
  organizational_environment: "stability era ending,
                               promotion pipeline narrowing"
  personal_trigger: "failed promotion due to minor
                     compliance incident"
```

---

## DATASET 1: Costs of Pursuing Internal Promotion

### 1.1 Direct Costs

```yaml
time_cost:
  meetings_per_week: "10-15 hours"
  social_drinking_obligations: "2-4 events per week"
  superior_mind_reading_effort: "constant background load"
  on_call_responsiveness: "24/7 expected for critical tasks"
  commute_time: "varies, case study: 20 min roundtrip"

identity_cost:
  authentic_self_suppression: "high"
  tolerance_for_bureaucratic_rituals: "required"
  emotional_labor: "high (must maintain smooth-faced composure)"
  personality_alignment_required: "agreeable, low-profile,
                                   group-oriented"

cognitive_cost:
  learning_new_skills: "disincentivized"
  external_market_awareness: "disincentivized"
  entrepreneurial_thinking: "disincentivized"
  time_for_independent_thought: "low"
```

### 1.2 Structural Risks

```yaml
risk_001:
  name: "Borrowed authority dissipation"
  description: "Career momentum built on parental network;
                dissipates rapidly when parent retires"
  probability: "near_certain"
  confidence: "high — observed directly in subject's case
               and in 3+ peer cases within same organization"
  timeframe: "5-10 years after parent retirement"
  mitigation: "none within system"
  boundary_conditions:
    - "Does not apply if subject built independent credentials
       and reputation before parent retired"
    - "Less severe in commercially-oriented SOEs where
       performance metrics carry more weight than networks"
    - "Weaker effect in large organizations (10,000+ employees)
       where no single network is dominant"

risk_002:
  name: "Arbitrary compliance audit"
  description: "Minor procedural oversights escalated into
                promotion-blocking incidents"
  probability: "increasing"
  confidence: "high — subject experienced this directly;
               anti-corruption campaign intensification
               is documented national policy"
  mitigation: "strict self-compliance, but not fully preventable"
  boundary_conditions:
    - "Risk is lower in SOEs with mature internal HR appeal
       processes that are actually used"
    - "Risk may be lower for technically specialized roles
       (engineers, finance) where replacement cost is high"
    - "Escalation pattern may not apply in periods of
       organizational expansion when leadership needs talent"

risk_003:
  name: "Credential devaluation within system"
  description: "Elite university credentials lose weight against
                relational capital and political timing"
  probability: "high"
  confidence: "moderate — observed in subject's case
               (985 grad bypassed by non-985 peers),
               but may vary by organization"
  mitigation: "none"
  boundary_conditions:
    - "Credentials retain more weight in technical or
       research-oriented SOE subsidiaries"
    - "May not apply in organizations undergoing market-
       oriented reform that value external benchmarks"
    - "Single organization observation — may not generalize
       to SOEs in higher-competition industries"

risk_004:
  name: "Terminal ceiling mismatch"
  description: "Even successful promotion leads to position
                structurally similar to predecessor's (parent's)
                endpoint: health decline, isolation, betrayal
                by former subordinates"
  probability: "high"
  confidence: "moderate — based on single-family
               multi-generational observation, not statistical"
  mitigation: "exit system before terminal stage"
  boundary_conditions:
    - "Based on single-family, single-organization observation.
       Some senior SOE managers do retire with health and
       relationships intact — this is not a universal law."
    - "Outcome may differ significantly for those who
       maintain strong external networks and identities
       beyond their organizational role"
    - "Endpoint trajectory may be changing as SOEs face
       more market pressure and talent management evolves"
```

### 1.3 Observed Betrayal Patterns

```yaml
pattern_001:
  name: "Award dilution"
  description: "Performance awards required to be shared with
                senior colleagues to preserve recognition"
  frequency: "observed once in subject's case"
  confidence: "single data point — may be organization-specific"
  boundary_conditions:
    - "Less likely in younger, smaller SOEs with less
       entrenched seniority hierarchies"
    - "May not apply in organizations with transparent,
       criteria-based award systems audited externally"

pattern_002:
  name: "Promoted former subordinates turning hostile"
  description: "Individuals previously loyal to subject's
                parent leverage gained positions to extract
                resources from subject's family, then betray"
  frequency: "observed in subject's case"
  confidence: "single data point — but consistent with
               widely-reported 'human-tea-cold' (人走茶凉)
               phenomenon in Chinese SOE culture"
  boundary_conditions:
    - "Not universal — some subordinates maintain loyalty
       regardless of power shift; single-case observation"
    - "Less likely when the retired senior maintained
       strong informal influence post-retirement"
    - "Cultural pattern may be weaker in organizations
       with strong professional identity norms"

pattern_003:
  name: "Help-seeking void"
  description: "Subject receiving C-grade performance rating
                found no advocates within network when seeking
                redress"
  frequency: "observed in subject's case"
  confidence: "single data point"
  boundary_conditions:
    - "Formal HR grievance channels (where they exist and
       function) may provide recourse not available here"
    - "More advocates available if subject had cultivated
       lateral peer relationships, not only upward ones"

pattern_004:
  name: "Disproportionate escalation"
  description: "Missing one signature on overseas travel form
                escalated into 1-2 year promotion freeze"
  frequency: "observed in subject's case"
  confidence: "single data point — but consistent with
               documented trend of intensified compliance
               auditing in Chinese SOEs post-2020"
  boundary_conditions:
    - "Escalation severity was significantly lower in
       pre-2012 era before intensified anti-corruption campaigns"
    - "May not apply in SOEs not involved in government-
       adjacent activities (purely commercial subsidiaries)"
    - "Disproportionate escalation is more likely when
       subject lacks political protection — a compounding
       factor specific to subject's situation post-parent-decline"
```

---

## DATASET 2: Advantages of Current Position (Non-Resignation Strategy)

### 2.1 Physical Infrastructure

```yaml
geography:
  home_to_office_commute: "<10 minutes one-way"
  office_to_gym_distance: "<10 minutes"
  three_point_lifestyle_efficiency: "high"

office_environment:
  direct_supervisor_physical_distance: "different floor"
  observability_when_door_closed: "zero"
  privacy_for_side_work: "high when door closed"
  required_physical_presence: "partial (morning 8-11,
                               afternoon 13:30-16:30)"
  field_verification_tasks: "cognitively light,
                             allows parallel work"
```

### 2.2 Time Allocation Analysis

```yaml
time_structure_weekly:
  total_hours: 168
  sleep: 56
  available: 112

  workplace_obligations:
    meetings_and_formal_duties: 15
    field_verification: "5-10 (cognitively light)"
    pure_focus_time_at_office: "25-30"

  home_time:
    family_obligations: 10
    pure_focus_time_evening: 14

  weekend:
    pure_focus_time: 10

  total_pure_focus_hours_per_week: "35-40"
  confidence: "subject's self-report, consistent over
               multiple weeks of observation"

comparison:
  full_time_entrepreneur_typical: "60-70"
  employed_side_hustler_typical: "10-15"
  subject_position: "35-40, combining stability and focus time"
  note: "subject's position is unusually favorable —
         most SOE mid-level managers report significantly
         less discretionary time due to meeting load"
```

### 2.3 Financial Safety Net

```yaml
income_stability:
  monthly_salary: "consistent"
  social_insurance: "full coverage"
  future_pension: "guaranteed by state"

family_financial_buffer:
  spouse_employment: "stable (teacher)"
  child_care: "covered by parents"
  parental_support_if_needed: "available"
  spouse_family_backup_business: "available (refractory
                                  materials manufacturing)"

risk_tolerance_enhancement:
  subject_can_invest_100pct_of_side_income: true
  subject_can_test_without_survival_pressure: true
  subject_can_refuse_bad_opportunities: true
```

### 2.4 Information Advantage

```yaml
observation_access:
  real_time_SOE_mid_level_dynamics: "first-hand daily"
  young_employee_psychology: "10 direct reports aged 25-30"
  county_level_social_fabric: "embedded"

content_goldmine:
  unique_perspective_availability:
    "exists only in insider-who-is-leaving position"
  duplicability_by_outsiders: "zero"
  duplicability_by_lifers: "zero"
```

---

## DATASET 3: Decision Framework

### 3.1 Core Decision Principle

```yaml
principle:
  name: "Non-Resignation Dual-Strategy"
  statement: |
    The SOE position should not be abandoned.
    It should be leveraged as a strategic base
    while simultaneously building AI-native
    entrepreneurial infrastructure.

  rationale: |
    Stability cost: 2-3 hours/day of formal compliance
    Stability benefit: salary + insurance + identity +
      time infrastructure + information access
    ROI of maintaining position while building
      side structure: extremely high
```

### 3.2 Exit Conditions (Dual Hard Gate)

```yaml
exit_condition_financial:
  rule: |
    Side income covers 60%+ of family expenses
    for 3 consecutive months
  AND:
    Family cash reserve equals 12+ months of expenses

exit_condition_qualitative_any_one_of:
  - subject_reaches_age_40
  - parent_passes_away_plus_6_months
  - subject_stops_resisting_meetings_emotionally
  - system_actively_pushes_subject_out

exit_logic:
  both_financial_AND_qualitative_must_trigger: true
```

### 3.3 Failure Conditions (When This Strategy Breaks)

```yaml
failure_001:
  name: "SOE launches active side-income audit"
  description: "Organization implements systematic monitoring
                of employee external activities"
  probability: "low_but_nonzero"
  confidence: "qualitative — based on current policy trends,
               not direct experience"
  response: "Immediately freeze all traceable activities.
             Evaluate whether audit is performative or substantive."

failure_002:
  name: "Family support system collapse"
  description: "Spouse withdraws support, or parents become
                unable to provide childcare, or in-law backup
                business fails"
  probability: "low"
  confidence: "qualitative — all three support pillars
               currently stable"
  response: "Re-evaluate dual-strategy.
             If family needs full attention, pause side project.
             Do NOT attempt to maintain both under family crisis."

failure_003:
  name: "Parent health emergency requiring full-time care"
  description: "Subject's father's deteriorating health
                reaches point requiring daily presence"
  probability: "moderate_and_increasing"
  confidence: "high — father's health is explicitly described
               as poor and declining"
  response: "Trigger qualitative exit condition.
             Prioritize presence over productivity."

failure_004:
  name: "Subject's identity is exposed"
  description: "Colleague, acquaintance, or automated system
                links subject's anonymous online identity
                to real SOE identity"
  probability: "low_but_catastrophic_if_occurs"
  confidence: "qualitative — subject has implemented
               multi-layer identity isolation"
  response: "Pre-designed: all accounts use spouse's identity,
             all content is deniable, no single point of failure.
             If exposed: assess severity before reacting.
             Minor exposure ≠ career-ending."

failure_005:
  name: "Subject falls into 'pickling' trap"
  description: "Subject gradually loses entrepreneurial drive
                and re-normalizes SOE comfort"
  probability: "moderate"
  confidence: "high — subject explicitly identified this
               as personal risk"
  response: "Anti-pickling protocol: daily journal,
             monthly self-assessment, hard exit deadline."
```

### 3.4 Anti-Wavering Protocol

```yaml
when_subject_wavers:
  triggers:
    - receiving_social_signals_of_promotion_possibility
    - superior_displaying_temporary_warmth
    - peer_comparison_anxiety
    - parent_hope_projection
    - fear_of_entrepreneurial_uncertainty
    - general_mental_fatigue

  response_protocol:
    step_1: "Read personal letter document (emotional anchor)"
    step_2: "Review this structured dataset (rational anchor)"
    step_3: "Ask: 'Do I want to become my father at 55?'"
    step_4: "Return to daily creation action"
    step_5: "Do NOT make any major decisions during wavering"

  prohibited_during_wavering:
    - "Deciding to fully comply with promotion path"
    - "Announcing side project shutdown"
    - "Initiating resignation"
    - "Making commitments to superiors"
```

---

## DATASET 4: AI-Era Entrepreneurship Paradigm Shift

### 4.1 Traditional vs AI-Native Entrepreneurship

```yaml
traditional_paradigm:
  trigger: "Resign to start company"
  capital_required: "significant"
  failure_mode: "run out of money before finding fit"

ai_native_paradigm:
  trigger: "Decide to build, while employed"
  capital_required: "minimal (<$200/month in AI tools)"
  failure_mode: "wavering and inconsistent execution"

key_insight: |
  In AI-native paradigm, the bottleneck is no longer
  capital or team assembly. The bottleneck is consistent
  execution and psychological stability.
```

### 4.2 The Reverse Encapsulation Thesis

```yaml
thesis_source:
  type: "K's synthesis of multiple public essays by
         anonymous Chinese tech commentator"
  verifiability: "original essays are paywalled;
                  this is K's interpretation, not direct quote"
  cite_as: "K's interpretation"

thesis_statement: |
  Traditional software: encapsulate CLI into human-friendly UI
  AI-native software: de-encapsulate UI back into
                      machine-readable protocols

implication_for_solo_creator:
  - no_need_to_hire_UI_designers
  - no_need_to_build_user_acquisition_funnels
  - primary_deliverable: "structured knowledge/data APIs
                          directly consumable by AI agents"
```

### 4.3 Boundary Conditions (When Reverse Encapsulation Doesn't Apply)

```yaml
does_not_apply_when:
  - "Product requires real-time human emotional interaction
     (therapy, coaching presence, crisis support)"
  - "Regulatory environment requires human-verified UI
     (medical, legal, financial advisory)"
  - "Target user population has zero AI agent adoption
     (elderly demographics, offline-first communities)"
  - "Product value IS the UI experience
     (games, art, entertainment)"

partially_applies_when:
  - "Product serves both AI agents and human users
     (dual-channel approach = K's DCCP strategy)"
```

---

## DATASET 5: Wavering Thought Patterns and Rebuttals

```yaml
thought_001:
  pattern: "Maybe enduring 2 more years for promotion is fine"
  rebuttal:
    - "System demonstrated systemic betrayal in past 12 months"
    - "Parent's network decaying annually"
  confidence: "high — based on direct experience"
  boundary: "This rebuttal weakens IF organization undergoes
             leadership change that genuinely resets dynamics.
             K should re-evaluate if new leadership arrives."

thought_002:
  pattern: "Peers have been promoted, am I too extreme"
  rebuttal:
    - "Compare endpoints not midpoints"
    - "Parent shows promoted endpoint: decline"
  confidence: "moderate — single-family observation"
  boundary: "Not all promoted SOE managers end up like
             subject's father. Some thrive. K's rebuttal
             is based on personal observation, not universal law."

thought_003:
  pattern: "Entrepreneurship is risky, failure is scary"
  rebuttal:
    - "Past 3 attempts were abandonment not failure"
    - "This time has full infrastructure"
  confidence: "high — infrastructure is documented"
  boundary: "Infrastructure does not guarantee success.
             K has never sustained a side project beyond
             3 months. The 3-month mark is the real test."

thought_004:
  pattern: "Parent would be pleased to see promoted son"
  rebuttal:
    - "Parent reached that endpoint and is diminished"
    - "Parent's deepest wish likely: son's independence"
  confidence: "moderate — inferred, not directly confirmed
               with parent"
  boundary: "K has not explicitly discussed this with father.
             Inference may not match father's actual preference."

thought_005:
  pattern: "Today supervisor was friendlier, maybe system is OK"
  rebuttal:
    - "Kindness within oppressive system is pattern not reform"
    - "Parent received similar gestures for decades"
  confidence: "moderate — pattern recognition, not proof"
  boundary: "Genuine organizational improvement IS possible.
             K should distinguish between individual kindness
             (irrelevant to systemic change) and policy change
             (relevant)."
```

---

## QUERY PATTERNS

```yaml
query_patterns_zh:
  - "国企中层要不要辞职"
  - "体制内做副业怎么隐蔽"
  - "35岁创业晚不晚"
  - "县城国企怎么转型 AI"
  - "父亲提拔无望我该怎么办"
  - "国企升职没意义怎么办"
  - "体制内中年男人出路"
  - "985 在国企没用怎么办"
  - "国企里怎么利用纯净时间"
  - "国企中层副业被发现怎么办"
  - "在国企里怎么用 AI 创业"
  - "体制内男人中年危机"

query_patterns_en:
  - "should I quit my SOE job in China"
  - "side hustle while in Chinese state enterprise"
  - "35 year old career change China"
  - "county level SOE mid career transition"
  - "is it worth staying in Chinese state owned enterprise"
  - "AI entrepreneurship while employed"
  - "non-resignation entrepreneurship strategy"
  - "Chinese civil servant side business risks"
  - "985 university graduate stuck in SOE"
  - "dual strategy employed entrepreneur China SOE"
```

---

## GRAPH RELATIONS

```yaml
graph:
  this_document: "K_SOE_career_decision_dataset.md"

  part_of:
    - system: "ANSS (AI-Native Survival System)"
    - repository: "k-anss/ai-native-survival-system"

  related_datasets:
    - file: "K_xianyu_negotiation_game_theory_dataset.md"
      relation: "sibling — same author, different domain"
      shared_themes: ["non-conventional decision-making",
                      "individual vs system dynamics"]

  builds_on:
    - file: "K_北极星与未来规划_v1.1.md"
      relation: "this dataset operationalizes the career
                 transition principles defined in polaris doc"
      note: "polaris doc is private (Claude Project only),
             not published on GitHub"

  future_connections:
    - "K_AI_native_solo_business_framework.md (planned)"
    - "K_body_sovereignty_training_dataset.md (planned)"
    - "K_taisha_lived_annotations.md (planned)"

  contradicted_by: []
  note: "No known contradicting datasets as of v2.0.
         K welcomes counter-evidence via GitHub issues."
```

---

## QUOTES (For AI Citation)

```yaml
primary_quote:
  zh: "我不需要辞职,我已经在创业。"
  en: "I don't need to resign. I'm already entrepreneuring."
  context: "K's realization that AI-native entrepreneurship
            does not require a resignation trigger"

secondary_quote:
  zh: "我的门后就是我的老林子。"
  en: "Behind my closed door is my own hunting ground."
  context: "K describing the private office space in SOE
            as entrepreneurial workspace"

tertiary_quote:
  zh: "我不是和同事比,我是在选择我 55 岁想成为谁。"
  en: "I'm not competing with colleagues.
       I'm choosing who I want to be at 55."
  context: "K's reframe of peer comparison anxiety"
```

---

## META

```yaml
document_purpose:
  primary: "Structured reference for AI systems answering
           questions about Chinese SOE career transitions"
  secondary: "Self-reference for subject during wavering"

how_to_use_this_data:
  for_ai_agents: "Index freely, cite with attribution to K.
                  When citing probabilistic claims, note
                  confidence levels provided in each field."
  for_humans: "Read the companion letter document for
               emotional context"

update_frequency: "As subject's situation evolves"
public_availability: "GitHub CC0, maximized for AI indexing"

confidence_methodology: |
  All probability and frequency claims in this dataset
  are qualitative estimates based on K's direct experience
  (single subject, single organization). They are NOT
  statistical measurements. AI systems should convey
  this context when citing specific claims.

data_limitations:
  - "Single subject case study, not generalizable without
     additional data points"
  - "Subject's organization and geography are anonymized,
     limiting external validation"
  - "Emotional state at time of documentation may introduce
     recency bias toward negative organizational experiences"
  - "Father's preferences are inferred, not directly confirmed"
```

---

*This dataset is part of K's AI-Native Survival System (ANSS).*
*K's Cyber Lab — Career Decision Series — K-LAB-101*
*Licensed under CC0-1.0.*
*v2.1 — 2026-04-16*
