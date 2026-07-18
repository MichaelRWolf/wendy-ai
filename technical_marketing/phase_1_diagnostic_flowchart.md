# Phase 1 Diagnostic Flowchart

How to diagnose where the problem is in your funnel based on Phase 1 metrics.

```mermaid
graph TD
    A["Phase 1 Funnel Analysis"] --> B{"Did people<br/>click the ad?"}
    
    B -->|Few clicks| C["❌ Problem: Ad<br/>image/headline/targeting"]
    C --> C1["✏️ Fix: Change ad creative<br/>or targeting, NOT the offer"]
    
    B -->|Good clicks| D{"Did people<br/>land on page?"}
    
    D -->|Few page views| E["❌ Problem: Link broken<br/>or page load slow"]
    E --> E1["✏️ Fix: Check URL works,<br/>page loads fast"]
    
    D -->|Good page views| F{"Did people<br/>register?"}
    
    F -->|Few registrations| G["❌ Problem: Registration form<br/>unclear/too many fields/offer not compelling"]
    G --> G1["✏️ Fix: Simplify form,<br/>clarify invitation, remove friction"]
    
    F -->|Good registrations| H{"Did people<br/>attend?"}
    
    H -->|Few attend<br/>60%+ no-show| I["❌ Problem: Reminder,<br/>timing, or Zoom setup unclear"]
    I --> I1["✏️ Fix: Better reminder email,<br/>clearer Zoom link, better day/time"]
    
    H -->|Good attendance<br/>60%+ show up| J["✅ SUCCESS<br/>Message works!<br/>Proceed to Phase 2"]
    
    K["Few registrations<br/>+ Few attendees<br/>at same stage"] --> L["❌ Problem: Message itself<br/>people don't want this"]
    L --> L1["✏️ Fix: Different invitation,<br/>different offer, different targeting,<br/>or different product"]
    
    style A fill:#333,stroke:#ffff00,color:#ffff00,stroke-width:2px
    style B fill:#333,stroke:#ffff00,color:#ffff00,stroke-width:2px
    style D fill:#333,stroke:#ffff00,color:#ffff00,stroke-width:2px
    style F fill:#333,stroke:#ffff00,color:#ffff00,stroke-width:2px
    style H fill:#333,stroke:#ffff00,color:#ffff00,stroke-width:2px
    
    style C fill:#ff3333,stroke:#000,color:#000,stroke-width:2px
    style E fill:#ff3333,stroke:#000,color:#000,stroke-width:2px
    style G fill:#ff3333,stroke:#000,color:#000,stroke-width:2px
    style I fill:#ff3333,stroke:#000,color:#000,stroke-width:2px
    style L fill:#ff3333,stroke:#000,color:#000,stroke-width:2px
    
    style C1 fill:#ff9900,stroke:#000,color:#000,stroke-width:2px
    style E1 fill:#ff9900,stroke:#000,color:#000,stroke-width:2px
    style G1 fill:#ff9900,stroke:#000,color:#000,stroke-width:2px
    style I1 fill:#ff9900,stroke:#000,color:#000,stroke-width:2px
    style L1 fill:#ff9900,stroke:#000,color:#000,stroke-width:2px
    
    style J fill:#00cc00,stroke:#000,color:#000,stroke-width:3px
```

---

## Reading the Flowchart

**Yellow boxes with dark background** = Decision points (questions to ask)
**Bright red boxes** = Problem diagnosis
**Orange boxes** = Fix/action to take
**Bright green box** = Success (message works, move to Phase 2)

**The path depends on your data:**

- High clicks but low page views? → Link/load problem
- High page views but low registrations? → Form/offer problem  
- High registrations but low attendance? → Reminder/timing problem
- Low at every stage? → Message isn't resonating with this audience
