# GDPR – Artikla 2 – Aineellinen soveltamisala

(14) Tämän asetuksen tarjoaman suojelun olisi koskettava luonnollisia henkilöitä heidän henkilötietojensa käsittelyssä.  

**Tämä asetus ei koske oikeushenkilöiden henkilötietojen käsittelyä, kuten yritysten nimiä tai yhteystietoja.**  
**Teknisen asiantuntijan näkökulmasta tämä tarkoittaa, että järjestelmät ja datavirrat on suunniteltava siten, että suojauksella ei ole vaikutusta juridisten henkilöiden tietoihin, vaan keskitytään luonnollisten henkilöiden dataan.**

1.Tätä asetusta sovelletaan henkilötietojen käsittelyyn, joka on osittain tai kokonaan automaattista, sekä sellaisten henkilötietojen käsittelyyn muussa kuin automaattisessa muodossa, jotka muodostavat rekisterin osan tai joiden on tarkoitus muodostaa rekisterin osa.  
**Teknisen asiantuntijan kannalta tämä tarkoittaa, että automaattiset järjestelmät ja rekisterit on suunniteltava tietosuojaa noudattaen alusta alkaen.**

(15) Vakavan väärinkäytösten riskin välttämiseksi luonnollisten henkilöiden suojelun olisi oltava **teknologianeutraalia** eli se ei saisi riippua käytetystä tekniikasta.  
**Tietosuoja koskee sekä automaattista että manuaalista käsittelyä, jos tiedot kuuluvat rekisteriin.**

2.Tätä asetusta ei sovelleta henkilötietojen käsittelyyn:

- a) jota suoritetaan sellaisen toiminnan yhteydessä, joka ei kuulu unionin lainsäädännön soveltamisalaan;  

(16) Tämä ei koske kansallista turvallisuutta tai unionin yhteiseen ulko‑ ja turvallisuuspolitiikkaan liittyviä toimia.  
**Teknisesti tämä tarkoittaa, että nämä poikkeukset on huomioitava järjestelmien suunnittelussa siten, että GDPR‑kontrollit eivät estä kyseisiä toimintoja tarpeettomasti.**

- b) jota suorittavat jäsenvaltiot toteuttaessaan SEU V osaston 2 luvun soveltamisalaan kuuluvaa toimintaa;

- c) jonka luonnollinen henkilö suorittaa yksinomaan henkilökohtaisessa tai kotitalouttaan koskevassa toiminnassa;  

(18) Esimerkiksi kirjeenvaihto ja sosiaalinen verkostoituminen ilman ammatillista tai kaupallista yhteyttä eivät kuulu soveltamisalaan.  
**Teknisesti tämä tarkoittaa, että tietosuoja‑arkkitehtuurin ei tarvitse kohdistua puhtaasti henkilökohtaiseen dataan, mutta palveluntarjoajien järjestelmien tulee olla yhteensopivia GDPR:n kanssa.**

- d) jota toimivaltaiset viranomaiset suorittavat rikosten ennalta estämistä, tutkintaa, paljastamista tai rikosoikeudellisten seuraamusten täytäntöönpanoa varten (mukaan lukien julkisen turvallisuuden uhkien käsittely);  

(19) Tällainen data‑käsittely on säädetty erillisellä unionin oikeudella.  
**Teknisesti tämä tarkoittaa, että viranomaisjärjestelmät voivat käyttää omia sääntöjään, mutta niiden täytyy integroida turvallisuus ja suojaukset asianmukaisesti, jos data siirtyy GDPR:n soveltamisalaan.**

3. Unionin toimielinten, elinten ja laitosten suorittamaan henkilötietojen käsittelyyn sovelletaan asetusta (EY) N:o 45/2001.  

(17) Tämä tulee mukauttaa tämän asetuksen periaatteiden mukaisesti.  
**Teknisesti tämä edellyttää yhdenmukaistettuja valvontamekanismeja ja auditointia koko järjestelmässä.**

4. Tällä asetuksella ei rajoiteta direktiivin 2000/31/EY soveltamista, erityisesti välittäjinä toimivien palveluntarjoajien vastuuta koskevia säännöksiä.  

(21) Direktiivin tarkoituksena on varmistaa sisämarkkinoiden moitteeton toiminta.  
**Teknisesti tämä vaikuttaa siihen, miten välittäjäpalvelut toteutetaan, mutta ei poista tarvetta tietosuojan perustekijöille.**

---

## Ydinviesti teknisestä asiantuntijakulmasta

Artikla 2 asettaa **ainesoveltamisalan reunaehdot teknisille toteutuksille**:

- **GDPR koskee luonnollisten henkilöiden dataa — ei oikeushenkilöiden.**
- **Automaattinen ja manuaalinen käsittely on teknisesti hallittava rekistereissä ja datavirroissa.**
- **Poikkeukset (esim. viranomaiskäyttö, henkilökohtainen data) vaikuttavat siihen, miten tietosuojapolitiikka ja järjestelmät on konfiguroitava.**

- ---

## Aineellisen soveltamisalan visuaalinen flowchart

```mermaid
flowchart TD
    A["Automatisoitu käsittely?"] -->|Kyllä| B["Henkilökohtaiset tai kotitaloutta koskevat toiminnot?"]
    A -->|Ei| C["Rekisterijärjestelmät"]

    C -->|Kyllä| B
    C -->|Ei| D["Ei GDPR:n aineellisen soveltamisalan piirissä"]

    B -->|Ei| E["Rikosoikeudellinen käsittely, kansallinen turvallisuus, ulkopolitiikka tai soveltamisalueen ulkopuolella?"]
    B -->|Kyllä| D

    E -->|Ei| F["GDPR:n aineellisen soveltamisalan piirissä"]
    E -->|Kyllä| D
markdown
Copy code


