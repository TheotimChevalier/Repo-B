introduction 

add submodul: 
git submodule add https://github.com/TheotimChevalier/Repo-A.git apps/web






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

    SRCwebsite-->>  WorkflowA: 1) push
     WorkflowA->>  WorkflowB: 3) activation workflow B 
     WorkflowB-->>  SRCwebsite: 4) update submodul
     WorkflowB-->>Submodul (Repo A): 5)  Build
    WorkflowB-->>infra : 5)  Deployed
```



