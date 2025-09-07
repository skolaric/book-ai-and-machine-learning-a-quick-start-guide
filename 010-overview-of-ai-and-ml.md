
# Overview of AI and ML

Artificial Intelligence (AI) is the broadest field, encompassing Machine Learning (ML), which focuses on learning from data. Deep Learning (DL) is a specialized ML branch using neural networks to analyze complex patterns. Generative AI, including large language models (LLMs), is a subset of DL centered on creating new content. The following figure shows how these disciplines are nested within each other.

```mermaid
graph LR
    subgraph AI ["AI"]
        subgraph ML ["ML"]
            subgraph DL ["Deep Learning"]
                subgraph GenAI ["Gen AI (LLMs)"]
                end
            end
        end
    end
    
    %% Styling
    classDef level1 fill:#e3f2fd,stroke:#777777,stroke-width:4px,rx:15,ry:15,color:#000000
    classDef level2 fill:#f3e5f5,stroke:#777777,stroke-width:3px,rx:15,ry:15,color:#000000
    classDef level3 fill:#e8f5e8,stroke:#777777,stroke-width:3px,rx:15,ry:15,color:#000000
    classDef level4 fill:#fff3e0,stroke:#777777,stroke-width:3px,rx:15,ry:15,color:#000000
    
    class AI level1
    class ML level2
    class DL level3
    class GenAI level4
```

In conventional computing, a human-written program accepts input data and processes it to generate output data:

```mermaid
graph LR
    A[Input Data] --> B[Program] --> C[Output Data]
    
    %% Styling
    classDef inputStyle fill:#e3f2fd,stroke:#1976d2,stroke-width:3px,rx:10,ry:10,color:#000000
    classDef programStyle fill:#f3e5f5,stroke:#7b1fa2,stroke-width:3px,rx:10,ry:10,color:#000000
    classDef outputStyle fill:#e8f5e8,stroke:#388e3c,stroke-width:3px,rx:10,ry:10,color:#000000
    
    class A inputStyle
    class B programStyle
    class C outputStyle
```

In ML however, we use input data AND output data to generate the program:
