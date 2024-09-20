sequenceDiagram :

```mermaid

    sequenceDiagram
    box Purple Repo A
    participant Create
    participant other things
    participant yamlA
    end
    box Repo B
    participant infra 
    participant Submodul
    participant yamlB
    end
    yamlA->>Create: What's new ?
    Create->>yamlA: give all the news!
    yamlA->>yamlB: we have some update!
    yamlB->>Submodul: Do the update
```
