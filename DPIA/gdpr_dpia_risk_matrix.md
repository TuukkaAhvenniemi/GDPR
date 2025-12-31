# GDPR (DPIA) – Riskimatriisi

Tämä matriisi havainnollistaa riskien vakavuuden ja todennäköisyyden arviointia DPIA:ssa.

```mermaid
%% Mermaid riskimatriisi, 5x5
%% Vaakasuora: Todennäköisyys (Low->High)
%% Pystysuora: Vaikutus (Low->High)
%% Värit: Low=tummanvihreä, Medium=tummankeltainen, High=tummanoranssi, Critical=tumma punainen
%% Teksti mustana

graph LR
    A1[Low x Low\nEsim: satunnainen anonymisoitu data-analyysi]:::low --> A2[Low x Medium\ Vähäinen henkilötietojen käsittely sisäisessä raportissa]:::low
    A2 --> A3[Low x High\ Vanha asiakastietokanta testikäytössä]:::medium
    A3 --> A4[Low x Very High\ Arkistoidut henkilötiedot projektiarkistossa]:::medium
    A4 --> A5[Low x Critical\ Poikkeuksellinen manuaalinen tietojen käsittely]:::high

    B1[Medium x Low\nEsim: sisäinen henkilöstöraportti ei arkaluontoista dataa]:::low --> B2[Medium x Medium\nEsim: sähköpostitse lähetettävä asiakastieto]:::medium
    B2 --> B3[Medium x High\nEsim: asiakastietojen yhdistäminen analytiikkaan]:::medium
    B3 --> B4[Medium x Very High\nEsim: terveystietojen käsittely ilman salattua kanavaa]:::high
    B4 --> B5[Medium x Critical\nEsim: henkilötietojen laajamittainen siirto EU:n ulkopuolelle]:::critical

    C1[High x Low\nEsim: henkilötietojen käsittely pienessä tiimissä, rajoitettu pääsy]:::medium --> C2[High x Medium\nEsim: henkilöstön suoritustietojen käsittely]:::medium
    C2 --> C3[High x High\nEsim: finanssidata yhdistettynä henkilötietoihin]:::high
    C3 --> C4[High x Very High\nEsim: arkaluonteisten tietojen jakaminen ulkopuoliselle alihankkijalle]:::critical
    C4 --> C5[High x Critical\nEsim: henkilötietojen rikolliseen käyttöön altistava järjestelmävirhe]:::critical

    D1[Very High x Low\nEsim: testidata sisältää suppeasti arkaluontoisia tietoja]:::medium --> D2[Very High x Medium\nEsim: sisäinen HR-järjestelmä, riskinä henkilötietojen väärinkäyttö]:::high
    D2 --> D3[Very High x High\nEsim: terveystietojen yhdistäminen muiden tietojoukkojen kanssa ilman suostumusta]:::critical
    D3 --> D4[Very High x Very High\nEsim: kriittiset asiakas- tai potilastiedot päässeet ulkopuolisille]:::critical
    D4 --> D5[Very High x Critical\nEsim: koko järjestelmän tietovuoto, miljoonien henkilötietojen paljastuminen]:::critical

    classDef low fill:#006400,stroke:#333,stroke-width:1px,color:#000
    classDef medium fill:#DAA520,stroke:#333,stroke-width:1px,color:#000
    classDef high fill:#FF8C00,stroke:#333,stroke-width:1px,color:#000
    classDef critical fill:#8B0000,stroke:#333,stroke-width:1px,color:#000
