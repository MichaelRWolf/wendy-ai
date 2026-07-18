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
    
    style C fill:#ffcccc
    style E fill:#ffcccc
    style G fill:#ffcccc
    style I fill:#ffcccc
    style L fill:#ffcccc
    style J fill:#ccffcc
    style C1 fill:#ffe6e6
    style E1 fill:#ffe6e6
    style G1 fill:#ffe6e6
    style I1 fill:#ffe6e6
    style L1 fill:#ffe6e6
```

---

## Reading the Flowchart

**Red boxes** = Problem diagnosis
**Light red boxes** = Fix/action to take
**Green box** = Success (message works, move to Phase 2)

**The path depends on your data:**

- High clicks but low page views? → Link/load problem
- High page views but low registrations? → Form/offer problem  
- High registrations but low attendance? → Reminder/timing problem
- Low at every stage? → Message isn't resonating with this audience
