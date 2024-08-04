# Personal Development Roadmap
This repository contains a Mermaid-based diagram visualizing a personal development roadmap. The roadmap is designed to help track progress in acquiring new skills and achieving professional objectives.


```mermaid
%%{init: { "theme": "dark", "flowchart": { "htmlLabels": true, "curve": "linear" } } }%%

graph TD;

    %% Current State
    A[Personal Development Roadmap]:::current

    %% Software Development Block
    subgraph B1[Improve Coding Skills]
        direction TB;
        B1_1[Review Data Structures & Algorithms, Design Patterns]:::sd --> B1_2[Leetcode & Kattis]:::sd
        B1_1 --> B1_3[Resources: 
        Hello-algo, 
        NeetCode.io, 
        Mastering Python Design Patterns Third Edition]:::sd
        B1_1 --> B1_4[Rewrite Existing Personal Repositories]:::sd
        
        B1_5[Front End Dev Projects]:::sd --> B1_6[Explore Angular / React]:::sd
    end

    %% Machine Learning Engineering Block
    subgraph B2[ML Engineering]
        direction TB;
        B2_1[Build and Deploy ML Models]:::ml --> B2_2[Examples: RecSys, Timeseries, etc.]:::ml
        B2_3[ML System Design]:::ml --> B2_4[Resources: 
        Designing Machine Learning Systems, 
        Machine Learning Solutions Architect Handbook, 
        Machine Learning Design Patterns, 
        ML System Design Interview]:::ml
        B2_3 --> B2_5[Hands-on Deployment on GCP, AWS]:::ml
        B2_1 --> B2_3
    end

    %% Deep Learning & AI Block
    subgraph B3[Brush Up on Deep Learning & AI]
        direction TB;
        B3_1[Review PyTorch and 
        Deep Learning Concepts]:::dl
        B3_2[Build LLM Projects]:::dl
        
        B3_2 --> B3_3[Productionize & Evaluation]:::dl
    end

    %% Linking Current State to Each Block
    A --> B1
    A --> B2
    A --> B3

    %% Style Definitions
    classDef current fill:#333333,stroke:#ffffff,stroke-width:2px,color:#ffffff;
    classDef sd fill:#555555,stroke:#61dafb,stroke-width:2px,color:#ffffff;
    classDef ml fill:#444444,stroke:#f39c12,stroke-width:2px,color:#ffffff;
    classDef dl fill:#2f4f4f,stroke:#2ecc71,stroke-width:2px,color:#ffffff;


```

