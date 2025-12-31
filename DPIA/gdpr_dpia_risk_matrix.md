# GDPR (DPIA) – Riskimatriisi

Tämä matriisi havainnollistaa riskien vakavuuden ja todennäköisyyden arviointia DPIA:ssa.

```mermaid
%% Mermaid riskimatriisi, 5x5
%% Vaakasuora: Todennäköisyys (Low->High)
%% Pystysuora: Vaikutus (Low->High)
%% Värit: Low=tummanvihreä, Medium=tummankeltainen, High=tummanoranssi, Critical=tumma punainen
%% Teksti mustana

graph LR
    A1[Low x Low –> Satunnainen anonymisoitu data-analyysi]:::low --> A2[Low x Medium –> Vähäinen henkilötietojen käsittely sisäisessä raportissa]:::low
    A2 --> A3[Low x High –> Vanha asiakastietokanta testikäytössä]:::medium
    A3 --> A4[Low x Very High –> Arkistoidut henkilötiedot projektiarkistossa]:::medium
    A4 --> A5[Low x Critical –> Poikkeuksellinen manuaalinen tietojen käsittely]:::high

    B1[Medium x Low –> Sisäinen henkilöstöraportti ei arkaluontoista dataa]:::low --> B2[Medium x Medium – Sähköpostitse lähetettävä asiakastieto]:::medium
    B2 --> B3[Medium x High –> Asiakastietojen yhdistäminen analytiikkaan]:::medium
    B3 --> B4[Medium x Very High –> Terveystietojen käsittely ilman salattua kanavaa]:::high
    B4 --> B5[Medium x Critical –> Henkilötietojen laajamittainen siirto EU:n ulkopuolelle]:::critical

    C1[High x Low –> Henkilötietojen käsittely pienessä tiimissä, rajoitettu pääsy]:::medium --> C2[High x Medium –> Henkilöstön suoritustietojen käsittely]:::medium
    C2 --> C3[High x High –> Finanssidata yhdistettynä henkilötietoihin]:::high
    C3 --> C4[High x Very High –> Arkaluonteisten tietojen jakaminen ulkopuoliselle alihankkijalle]:::critical
    C4 --> C5[High x Critical –> Henkilötietojen rikolliseen käyttöön altistava järjestelmävirhe]:::critical

    D1[Very High x Low –> Testidata sisältää suppeasti arkaluontoisia tietoja]:::medium --> D2[Very High x Medium –> Sisäinen HR-järjestelmä, riskinä henkilötietojen väärinkäyttö]:::high
    D2 --> D3[Very High x High –> Terveystietojen yhdistäminen muiden tietojoukkojen kanssa ilman suostumusta]:::critical
    D3 --> D4[Very High x Very High –> Kriittiset asiakas- tai potilastiedot päässeet ulkopuolisille]:::critical
    D4 --> D5[Very High x Critical –> Koko järjestelmän tietovuoto, miljoonien henkilötietojen paljastuminen]:::critical

    classDef low fill:#006400,stroke:#333,stroke-width:1px,color:#000
    classDef medium fill:#DAA520,stroke:#333,stroke-width:1px,color:#000
    classDef high fill:#FF8C00,stroke:#333,stroke-width:1px,color:#000
    classDef critical fill:#8B0000,stroke:#333,stroke-width:1px,color:#000
