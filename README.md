workflow explication :

```mermaid

    sequenceDiagram
    box Purple Repo A
    participant SRCwebsite
    participant WorkflowA
    end
    box blue Repo B
    participant infra
    participant Submodul (Repo A)
    participant  WorkflowB
    end
     WorkflowA->>SRCwebsite: What's new ?
    SRCwebsite-->> WorkflowA: give all the news!
     WorkflowA->> WorkflowB: give some update!
     WorkflowB-->> SRCwebsite: look update 
     WorkflowB-->>Submodul (Repo A): Do the update
```
