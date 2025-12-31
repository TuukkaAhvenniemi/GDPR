# GDPR (DPIA) – Riskimatriisi

Tämä matriisi havainnollistaa riskien vakavuuden ja todennäköisyyden arviointia DPIA:ssa.

```mermaid
%% Mermaid riskimatriisi, 5x5
%% Vaakasuora: Todennäköisyys (Low->High)
%% Pystysuora: Vaikutus (Low->High)
%% Värit: Low=tummanvihreä, Medium=tummankeltainen, High=tummanoranssi, Critical=tumma punainen
%% Teksti mustana

graph LR
    A1[Low x Low]:::low --> A2[Low x Medium]:::low
    A2 --> A3[Low x High]:::medium
    A3 --> A4[Low x Very High]:::medium
    A4 --> A5[Low x Critical]:::high

    B1[Medium x Low]:::low --> B2[Medium x Medium]:::medium
    B2 --> B3[Medium x High]:::medium
    B3 --> B4[Medium x Very High]:::high
    B4 --> B5[Medium x Critical]:::critical

    C1[High x Low]:::medium --> C2[High x Medium]:::medium
    C2 --> C3[High x High]:::high
    C3 --> C4[High x Very High]:::critical
    C4 --> C5[High x Critical]:::critical

    D1[Very High x Low]:::medium --> D2[Very High x Medium]:::high
    D2 --> D3[Very High x High]:::critical
    D3 --> D4[Very High x Very High]:::critical
    D4 --> D5[Very High x Critical]:::critical

    classDef low fill:#006400,stroke:#333,stroke-width:1px,color:#000
    classDef medium fill:#DAA520,stroke:#333,stroke-width:1px,color:#000
    classDef high fill:#FF8C00,stroke:#333,stroke-width:1px,color:#000
    classDef critical fill:#8B0000,stroke:#333,stroke-width:1px,color:#000
