
# Digital Yrkesvägledning

Research proof-of-concepts within a Swedish [research project](https://www.vinnova.se/p/pilot-digital-infrastruktur-kll/), funded by Sweden's innovation agency, looking at existing and future needs for data and service surrounding digital career counseling.

This repo is managed by RISE Reseatch Insititutes of Sweden, area of Lifelong Learning, contact [@ollenyman].

## First scenario iteration
Starts with a job ad and identifies a persons competence gap. Tabled because of Arbetsförmedlingen's analysis.

## Second scenario iteration
Starts with a CV, extracts keywords and lets the user guide towards job ad or education. As work progresses, more inputs into the process are expected - using AF Atlas taxonomy's relationship graph, using ChatGPT-style queries for widening the search for keywords, etc.
Initial implementation using the [competence-hub repo](https://github.com/LearningArena/competence-hub) (vagledning branch) as testbed.  
Current data sources usage:

```mermaid

flowchart TD
    classDef taxonomy color:#ff0
    classDef userselect fill:#555,stroke:#555
    subgraph CV Start
        B[CV] --> C{JobAd<br>enrichtextdocument}
        C --> E[Occupation terms]
        C --> D[Competence terms]
        C --> F[Trait terms]
    end
    B[CV] -.-> N{AI/LLM}
    N -.-> D
    subgraph Insight
        D --> V[user selection]:::userselect
        V --> G{JobEd<br>match-by-text}
        G --> H[Occupations]:::taxonomy
        G --> I[Occupation Groups]:::taxonomy
        H --> U{Taxonomy<br>related}
        I --> R{Taxonomy<br>related}
        R --> S[Occupation Fields]:::taxonomy
        U --> S
        I --> J{Taxonomy<br>related}
        J --> K[Skills]:::taxonomy
        K -->|user repeat| V
    end
    Q{Yrkesprognoser dataset<br>- bristvärde} -.-> H
    Q{Yrkesprognoser dataset<br>- bristvärde} -.-> I
    subgraph Outlook
        K --> X[user selection]:::userselect
        S --> Y[user selection]:::userselect
        I --> Z[user selection]:::userselect
    end
    subgraph Future
        H --> AB[user adjustments]:::userselect
        V --> AB
        X --> AB
        Y --> AB
        Z --> AB
        AB -->|user selection| L{JobSearch<br>- skills<br>- occupation<br>- occupation-groups<br>- occupation-field}
        L --> M[Ads<br>]
        M -->|user repeat| AB
    end
    O{Yrkesprognoser dataset<br>- bristvärde} -.-> M
    T{JobAd<br>enrichtextdocument<br>- competencies} -.-> M
    subgraph MyPath
        M -.-> AC[Din resa, jobed utbildningar etc ...]
    end

```
<!-- Last mermaid letter: AC -->

## Glossary
- Sveriges referensram för kvalifikationer (SeQF)
- Standard för svensk yrkesklassificering (SSYK2012)
- Svensk utbildningsnomenklatur (SUN)
- Standard för svensk näringsgrensindelning (SNI)
- Europeiska klassificering av färdigheter, kvalifikationer och yrken (ESCO)
