# GDPR – Kokonaiskuva ja perusperiaatteet

## Keskeiset artiklat

### Artikla 1 – Tarkoitus
- Määrittelee GDPR:n tavoitteen: suojata yksilöiden henkilötietoja ja varmistaa tietosuoja EU:ssa.
- Korostaa rekisteröidyn oikeuksien suojaa ja organisaatioiden vastuita.

### Artikla 2 – Soveltamisala
- Määrittelee, millä organisaatioilla ja tilanteissa GDPR koskee.
- Kattaa EU:ssa toimivat rekisterinpitäjät ja käsittelijät sekä EU:n ulkopuoliset palvelut, jotka käsittelevät EU-kansalaisten tietoja.
- Perusta juridiselle ja tekniselle soveltamisrajaukselle.

### Artikla 3 – Maantieteellinen soveltamisala
- Selventää, että GDPR koskee myös EU:n ulkopuolisia organisaatioita, jos ne tarjoavat palveluita EU:n kansalaisille tai seuraavat heidän käyttäytymistään.
- Vaikuttaa ulkomaisten palveluntarjoajien sopimuksiin ja tietoturvakäytäntöihin.

### Artikla 4 – Määritelmät
- Selventää keskeiset käsitteet: rekisteröity, henkilötiedot, käsittely, rekisterinpitäjä ja käsittelijä.
- Perusta kaikelle jatkokäsittelylle ja sopimustulkinnalle.

---
### GDPR:n perusta ja soveltamislogiikka – Tekninen kokonaiskuva

```mermaid

flowchart TD

A["GDPR Artikla 1<br/>Tarkoitus ja tavoitteet"] --> B["GDPR Artikla 2<br/>Soveltamisala"]
B --> C["Kuuluuko toiminta soveltamisalaan?"]
C -->|Kyllä| D["GDPR Artikla 3<br/>Alueellinen soveltaminen"]
C -->|Ei| X["Ei GDPR-vaatimuksia<br/>Perustason tietoturva"]
D --> E["EU:ssa tai EU-kohdistus"]
E --> F["GDPR Artikla 4<br/>Keskeiset määritelmät"]
F --> G["Rekisterinpitäjä ja käsittelijä<br/>tunnistettu"]
F --> H["Henkilötiedot ja käsittely<br/>tunnistettu"]
G --> I["Vastuut ja velvoitteet<br/>kohdistettavissa"]
H --> J["Tekniset ja organisatoriset<br/>toimenpiteet määriteltävissä"]
I --> K["Siirtymä operatiivisiin kokonaisuuksiin"]
J --> K
K --> L["DPIA"]
K --> M["TOMs"]
K --> N["RoPA"]
K --> O["DPA"]
