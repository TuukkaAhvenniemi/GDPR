# GDPR DPIA – Prosessikaavio

Tämä kaavio havainnollistaa tietosuojavaikutusten arvioinnin (DPIA) keskeiset vaiheet, riskienhallinnan ja dokumentoinnin.

```mermaid
flowchart TD
    A[Henkilötietojen käsittelyprojekti] --> B{DPIA pakollinen?}
    B -- Kyllä --> C[Käsittelytoimien kuvaus]
    C --> D[Riskien tunnistaminen]
    D --> E[Riskien arviointi]
    E --> F[Tekniset ja organisatoriset lieventävät toimet]
    F --> G[Jäännösriskin arviointi]
    G --> H[DPIA-dokumentointi]
    H --> I{Tarvitaanko ennakkokuuleminen?}
    I -- Kyllä --> J[Yhteys valvontaviranomaiseen]
    I -- Ei --> K[Hyväksyntä ja hallintomalli]
    J --> K
    K --> L[RoPA- ja TOMs-linkitys]
    L --> M[Auditointi & näyttö viranomaiselle]

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#ff9,stroke:#333,stroke-width:2px
    style D fill:#9ff,stroke:#333,stroke-width:2px
    style F fill:#9f9,stroke:#333,stroke-width:2px
    style G fill:#fc9,stroke:#333,stroke-width:2px
    style H fill:#ccf,stroke:#333,stroke-width:2px
    style I fill:#f99,stroke:#333,stroke-width:2px
    style J fill:#fcf,stroke:#333,stroke-width:2px
    style K fill:#cff,stroke:#333,stroke-width:2px
    style L fill:#ffcc99,stroke:#333,stroke-width:2px
    style M fill:#99ccff,stroke:#333,stroke-width:2px
