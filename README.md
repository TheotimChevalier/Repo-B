sequenceDiagram :

```mermaid

    sequenceDiagram
    box Purple Repo A
    participant website
    participant yamlA
    end
    box blue Repo B
    participant infra
    participant interne page 
    participant Submodul
    participant yamlB
    end
    yamlA->>website: What's new ?
    website-->>yamlA: give all the news!
    yamlA->>yamlB: we have some update!
    yamlB-->>Submodul: Do the update
```
