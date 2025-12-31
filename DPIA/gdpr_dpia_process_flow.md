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
