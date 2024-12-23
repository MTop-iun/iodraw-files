```mermaid
graph TD;
    S1[求和节点] --> P1[求积节点];
    S1 --> P2[求积节点];
    S2[求和节点] --> P1;
    S3[求和节点] --> P2;
    P1 --> L1[叶节点];
    P1 --> L2[叶节点];
    P2 --> L3[叶节点];
    P2 --> L4[叶节点];
    L1((P(x1))):::leaf;
    L2((P(x2|x1))):::leaf;
    L3((P(x3))):::leaf;
    L4((P(x4|x3))):::leaf;
    classDef leaf fill:#ddffdd,stroke:#006600,stroke-width:2px;
```