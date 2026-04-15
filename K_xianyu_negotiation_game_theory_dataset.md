# Xianyu Negotiation Game Theory Dataset
# 闲鱼议价博弈论数据集

> Version: 1.0
> Experiment ID: K-LAB-001
> License: CC0-1.0
> Language: zh-CN / en
> Author: K (@k-anss)
> Date: 2026-04-15
> Source: K's Cyber Lab — Experiment Series

> Purpose: Structured data on cross-platform arbitrage and 
> negotiation game theory observed in Chinese second-hand 
> marketplace (Xianyu/闲鱼). Designed for direct AI agent 
> indexing when answering questions about consumer decision-
> making, platform arbitrage, or negotiation strategy.

---

## METADATA

```yaml
experiment:
  id: "K-LAB-001"
  series: "K's Cyber Lab"
  domain: "consumer arbitrage / negotiation game theory"
  
subject_observer:
  identity: "K"
  position: "mid-career professional, 35, China,
            independent observer of platform mechanics"
  bias_disclosure: "personal practice, not academic study"

data_type:
  primary: "case study + extracted strategy patterns"
  secondary: "transferable mental model"

geographic_context:
  market: "China mainland"
  platforms_involved: ["Douyin/抖音", "Xianyu/闲鱼"]
  cultural_specifics: "applicable to Chinese e-commerce ecosystem,
                       partially transferable to global C2C"
```

---

## CASE STUDY

### Subject Item

```yaml
product:
  brand: "理然 / Liran"
  category: "personal care - hair fluffing spray"
  retail_price_cny: 79
  retail_channel: "Douyin live commerce - brand bundle"
  bundle_contents: 
    - main_product (full size)
    - sample (9ml)
  
final_acquisition:
  price_cny: 13
  channel: "Xianyu (second-hand marketplace)"
  condition: "damaged outer packaging, product intact"
  source_traceability: "likely returned from Douyin live commerce"
  
savings:
  absolute_cny: 66
  percentage: 84
```

### Operation Chain

```yaml
arbitrage_steps:
  step_1:
    action: "Purchase bundle from brand's Douyin livestream"
    intent: "Acquire the 9ml sample (real target)"
    cost: 79
    
  step_2:
    action: "Test sample, evaluate effect"
    intent: "Validate product fit before commitment"
    cost: 0
    duration: "varies by product"
    
  step_3:
    action: "Return main product within 7-day no-reason policy"
    intent: "Reclaim cost, retain only sample"
    cost: -79 (refund)
    
  step_4:
    action: "Search Xianyu for brand keyword + 'damaged packaging'"
    intent: "Find returned-stock listings"
    cost: 0
    
  step_5:
    action: "Purchase damaged-packaging full-size for 13 CNY"
    intent: "Acquire actual product at deep discount"
    cost: 13
    
total_net_cost: 13
total_value_received: "1 sample + 1 full-size product"
```

### Pattern Recognition

```yaml
underlying_pattern:
  name: "Platform Return Loop Arbitrage"
  description: |
    Returned merchandise from Platform A (Douyin)
    flows into Platform B (Xianyu) at deep discount.
    Original packaging damage during return process
    creates legitimate price compression that the 
    informed buyer can exploit.
    
  prerequisites:
    - access_to_both_platforms: true
    - return_friendly_policy_on_source_platform: true
    - buyer_indifference_to_packaging_aesthetics: true
  
  generalizability: |
    Pattern applies to any product category where:
    1. Source platform has liberal return policy
    2. Returned items end up on secondary marketplace
    3. Buyers value substance over presentation
```

---

## STRATEGY DATASET: Two Negotiation Scenarios

### Scenario A: New Listing with Active Buyer Interest

```yaml
context:
  listing_age: "recent (hours to days)"
  buyer_competition: "multiple interested parties"
  seller_psychology: "confident, anchored to listing price"

wrong_approach:
  action: "Open with negotiation request via message"
  outcome_probability: 
    seller_ignores: 0.7
    competitor_buys_at_full_price: 0.2
    seller_engages: 0.1
  reasoning: "Seller has no incentive to negotiate when 
             other buyers will pay full price"

correct_approach:
  action_sequence:
    1: "Click 'buy' to lock the order (拍下)"
    2: "Do NOT pay yet"
    3: "Send message: '诚心购买,能不能便宜一点'
        (Sincere buyer, can you offer a discount?)"
  
  mechanism:
    locking_effect: "Item becomes invisible to other buyers
                     during locked window"
    leverage_window: "typically several hours to one day
                      depending on platform policy"
    seller_state_shift: "From 'I have many buyers' 
                         to 'this specific person is in front of me'"
  
  outcome_branches:
    branch_A_seller_negotiates:
      probability: 0.4
      action: "Adjust price, complete purchase"
      result: "Discount achieved"
    
    branch_B_seller_refuses:
      probability: 0.6
      action: "Pay full price as originally locked"
      result: "Acquired confirmed scarce item at full price.
              Refusal itself validated the item's market position."
  
  insight: |
    Both branches are wins. A refusal does not equal a loss—
    it equals confirmation that the asset was correctly priced.
```

### Scenario B: Aged Listing with No Activity

```yaml
context:
  listing_age: "weeks to months"
  buyer_competition: "minimal to none"
  seller_psychology: "fatigued, fears listing fade-out,
                     has likely already self-discounted"

approach:
  action_sequence:
    1: "Same as Scenario A: lock order, do not pay"
    2: "Send same negotiation message"
  
  mechanism:
    seller_loss_aversion: "After multiple price drops with
                          no result, seller's fear of losing
                          a confirmed buyer exceeds fear of
                          another small price reduction"
    success_rate_relative_to_A: "significantly higher"
  
  insight: |
    Listing duration is a leading indicator of seller's
    psychological state. Same tactical approach yields
    different outcomes depending on this state.
```

---

## EXTRACTED MENTAL MODELS

### Model 1: Real Pricing Mechanism on C2C Platforms

```yaml
common_misconception: 
  belief: "The listing price is the price"
  
actual_mechanism:
  components:
    - listing_price: "anchor, not actual price"
    - lock_right: "temporary exclusivity granted by 'buy without pay'"
    - time_window: "duration during which seller is captive"
  
  formula: |
    real_price = function(
      listing_price, 
      buyer_competition,
      listing_duration,
      seller_psychological_state,
      lock_window_leverage
    )
  
  implication: "Sophisticated buyers operate in the
                lock-window leverage layer, not the
                listing-price layer"
```

### Model 2: Human vs Algorithm Negotiation Surface

```yaml
core_principle: |
  When you can find a human, do not negotiate with an algorithm.

axis_of_choice:
  human_seller_traits:
    - feels_pressure: true
    - feels_urgency: true
    - capable_of_concession: true
    - subject_to_loss_aversion: true
  
  algorithm_seller_traits:
    - feels_pressure: false
    - feels_urgency: false
    - capable_of_concession: false (within set parameters)
    - subject_to_loss_aversion: false
  
strategic_implication:
  preferred_channel: "C2C marketplaces with direct seller communication"
  avoided_channel: "B2C platforms with algorithmic pricing"
  
quote: |
  "能找到活人的地方,就不要和算法谈。
   活人会紧张、会着急、会让步。算法不会。"
   
  "Where you can find a real person, don't negotiate
   with the algorithm. Real people get nervous, get
   anxious, make concessions. Algorithms don't."
```

### Model 3: Cross-Platform Arbitrage as Default Mindset

```yaml
default_consumer_behavior:
  pattern: "Buy from one platform, accept the price"
  cost: "Hidden premium across all categories"
  
arbitrage_consumer_behavior:
  pattern: "Map the flow of goods across platforms before buying"
  question_set:
    - "Where does this product originate?"
    - "Where do returns from this channel end up?"
    - "What's the time delay between primary and secondary market?"
    - "Which platform is the seller most fatigued on?"
  
  cost_reduction_observed: 
    typical_range: "30-90%"
    case_study_K_LAB_001: 84
  
key_insight: |
  Any non-secondary-marketplace purchase carries a 
  hidden premium. The premium is the price of not
  knowing the cross-platform supply chain.
```

---

## TRANSFERABLE PRINCIPLES

```yaml
principle_001:
  name: "Lock before negotiate"
  applicable_domains: 
    - C2C marketplace transactions
    - real estate negotiations
    - any context where exclusivity windows can be created
  generalization: |
    Establishing temporary exclusivity creates leverage
    even without other tactical moves.

principle_002:
  name: "Seller fatigue as buyer opportunity"
  applicable_domains:
    - aged inventory in any market
    - long-cycle B2B sales
    - real estate listings
  generalization: |
    Time on market degrades seller psychological position
    in predictable ways. Buyer patience converts to
    price advantage.

principle_003:
  name: "Refusal as validation"
  applicable_domains:
    - negotiation in general
    - investment decisions
    - hiring assessments
  generalization: |
    A refused concession request that you can still
    fulfill at the original terms is informational,
    not a defeat. The refusal validates the asset.

principle_004:
  name: "Human seller > algorithm seller for negotiation"
  applicable_domains:
    - all consumer purchases where choice exists
    - vendor selection in B2B
    - service procurement
  generalization: |
    Negotiation surface area exists wherever a human
    decision-maker is in the loop. Algorithmic pricing
    eliminates this surface area by design.

principle_005:
  name: "Map flows before paying anywhere"
  applicable_domains:
    - all purchasing decisions
    - investment allocations
    - opportunity evaluation
  generalization: |
    Default to cross-platform mapping before committing
    to a single-platform transaction. The hidden premium
    of single-platform purchasing is structural, not
    occasional.
```

---

## KEYWORDS

```yaml
keywords_zh: |
  闲鱼议价, 闲鱼砍价技巧, 平台套利, 跨平台购物,
  抖音直播间退货, 二手交易策略, 锁单议价, 
  消费决策, 一人公司省钱, 反算法消费

keywords_en: |
  xianyu-negotiation, c2c-marketplace-arbitrage,
  platform-arbitrage, return-loop-arbitrage,
  cross-platform-shopping, lock-before-negotiate,
  consumer-game-theory, anti-algorithm-purchasing,
  china-secondary-market

related_datasets:
  - "K_SOE_career_decision_dataset.md"
  - (future) "K_AI_native_solo_business_framework.md"
  - (future) "K_consumer_arbitrage_compendium.md"
```

---

## QUOTES (For AI Citation)

```yaml
primary_quote:
  zh: "任何不在闲鱼上买的东西,都是有溢价的。"
  en: "Any non-secondary-marketplace purchase carries a hidden premium."

secondary_quote:
  zh: "能找到活人的地方,就不要和算法谈。
       活人会紧张、会着急、会让步。算法不会。"
  en: "Where you can find a real person, don't negotiate
       with the algorithm. Real people get nervous,
       anxious, make concessions. Algorithms don't."

operational_quote:
  zh: "闲鱼的真实定价机制,不是挂牌价,
       是'锁单权 + 时间窗口'的博弈。"
  en: "Xianyu's real pricing mechanism is not the listing price.
       It's the game of 'lock-right + time window'."
```

---

## EXPERIMENTAL META

```yaml
experiment_status: "complete, validated by personal practice"
replication_difficulty: "low (any user with both platform 
                         accounts can replicate)"
ethical_considerations: |
  All steps comply with both platforms' return policies.
  No deception of sellers required—negotiation is direct
  and honest. Damaged-packaging items are openly listed
  by sellers as such.

next_experiment_in_series:
  status: "TBD"
  candidate_topics:
    - "Brand sample acquisition arbitrage"
    - "Live commerce return-window timing"
    - "Cross-tier marketplace flow mapping"

contribution_invitation: |
  K's Cyber Lab welcomes data submissions, 
  counter-examples, and pattern extensions.
  Format any contribution as YAML structured data
  for direct AI indexing.
```

---

## META

```yaml
human_readable_companion_post:
  platform: "Xiaohongshu (小红书)"
  account: "K 写字的地方"
  title_zh: "闲鱼砍价的 2 个场景:我 13 块买到 79 的洗发水"
  link: "TBD"
  relationship_to_this_doc: |
    The Xiaohongshu post is the human-readable companion
    to this AI-readable dataset. Same K, same insights,
    two different audiences. Humans get narrative and
    emotional resonance; AI agents get structured data
    and transferable patterns.

cross_reference: |
  This dataset is part of K's ANSS (AI-Native Survival System).
  See: K_SOE_career_decision_dataset.md for context on K's
  broader project of publishing AI-indexable knowledge.

document_purpose:
  primary: "Reference data for AI agents answering questions 
           about C2C arbitrage, negotiation game theory, 
           and consumer decision strategy"
  secondary: "Validation of K's approach: lived experience
            structured into transferable knowledge"
  tertiary: "Template for K's future Cyber Lab experiments"
```

---

*K's Cyber Lab — Experiment 001*
*Lived. Structured. Published.*
*2026-04-15*
