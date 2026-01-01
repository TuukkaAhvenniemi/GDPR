# GDPR – ISO/IEC 27701 – DPIA – PII-prosessoreiden hallinta

ISO/IEC 27701 (adopted 2019) täydentää ISO/IEC 27002 ohjeita erityisesti henkilötietojen käsittelyn (PII) hallintaan ja tukee GDPR:n Art. 29 soveltamista käytännössä. Tämä standardi tarjoaa konkreettisen viitekehyksen teknisten ja organisatoristen toimenpiteiden (TOMs) suunnitteluun ja dokumentointiin.

---

## Keskeiset periaatteet asiantuntijan näkökulmasta

- **Tarkoituksenmukainen käsittely:** Kaikki PII:t on käsiteltävä vain asiakkaan dokumentoitujen ohjeiden mukaisesti.
- **Sopimusvelvoitteet:** Sopimuksessa määritellään selkeästi objektit, aikakehys ja prosessin rajat.
- **Tekninen toteutus:** Organisaatio voi valita prosessointimenetelmät, jotka optimoivat suorituskykyä ja resursseja, mutta eivät poikkea asiakkaan ohjeista.
- **Auditointi ja todentaminen:** Asiakkaalla tulee olla mahdollisuus tarkistaa, että PII:tä ei käytetä muihin tarkoituksiin.

---

## Implementointipallurat

- **Organisaation sisäiset prosessit:**  
  - Dokumentoi kaikki PII-prosessit ja ohjeistukset.
  - Määritä vastuut käsittelijöille ja alihankkijoille.
  - Luo hallintamalli, jossa Poikkeamien hallinta, RoPA ja DPIA ovat linkitettynä.
 
---

- **Sopimus- ja ohjeistusketju:**  
  - Sisällytä asiakkaan ohjeet palvelusopimukseen.  
    - Objektit: mitä tietoja käsitellään  
    - Aikakehys: milloin ja kuinka kauan käsittely tapahtuu  
    - Prosessin rajat: sallitut toimenpiteet ja tekniset rajoitteet  
  - Alihankkijoiden sitouttaminen:  
    - Ala-ala pallura: varmista, että alihankkijat noudattavat samoja ohjeita  
    - Ala-ala pallura: tarkista auditointiraportit ja sopimuspoikkeamat
   
---

- **Tekninen ja organisatorinen valvonta:**  
  - Pääsynhallinta (RBAC, MFA) ja rooliperusteinen valtuutus  
  - Jatkuva lokitus ja auditointilokit  
  - Salaus ja pseudonymisointi / anonymisointi tarvittaessa  
  - Riskienhallinnan integrointi DPIA-prosessiin  
    - Ala-ala pallura: tunnista ja arvioi ketjun jokaisen vaiheen riskit  
    - Ala-ala pallura: dokumentoi lieventävät toimenpiteet ja residual riskit
   
---

- **Todentaminen ja raportointi:**  
  - Asiakkaan tarkistusmahdollisuus prosessointien mukaisuudesta  
  - KPI:t ja mittarit riskienhallinnan tehokkuuden seuraamiseen  
  - Raportit auditointeihin ja viranomaisviestintään  
    - Ala-ala pallura: RoPA-linkitys käsittelytoimiin  
    - Ala-ala pallura: TOMs-dokumentaatio teknisistä ja organisatorisista toimista

---

## Asiantuntijan näkökulma

### Perustietäjä
- Ymmärtää, että ISO/IEC 27701 antaa ohjeita PII-prosessoreille ja Art. 29 noudattamiselle.
- Osaa dokumentoida ohjeiden mukaisen käsittelyn muodollisesti.
- Tietää, että auditointi- ja tarkastusketju liittyy sopimuksiin ja ohjeisiin.

### Asiantuntija
- Riskien tunnistaminen ja hallinta koko ketjussa:  
  - Luvaton pääsy ja tietovuodot  
  - Alihankkijoiden epäasianmukainen toiminta  
  - Epäselvät ohjeistukset ja poikkeamat
- Arviointi ja lieventäminen:  
  - Riskien todennäköisyyden ja vaikutuksen analyysi  
  - Lieventävät tekniset toimet (salaus, RBAC, MFA, auditointilokit)  
  - Lieventävät organisatoriset toimet (koulutus, ohjeistus, sopimukset)  
- Todentaminen ja raportointi:  
  - KPI:t, auditointiraportit ja RoPA-linkitys  
  - Dokumentoi jäännösriskit ja hyväksynnät  
  - Mahdollisuus esittää todentaminen viranomaiselle

---

## Viranomais- ja auditointinäkökulma
- Kyky osoittaa, että kaikki PII käsitellään asiakkaan ohjeiden mukaisesti.  
- Tarkastukset voivat kohdistua:  
  - EU:n valvontaviranomainen (DPA)  
    - Auditointi ja dokumentaation tarkistus  
    - Riskienhallinnan tehokkuuden arviointi  
  - Kansalliset tietosuojaviranomaiset  
    - Lainsäädännön vaatimusten täyttymisen tarkastus  
    - Ohjeistus ja huomautukset  
  - Sisäiset auditointiryhmät  
    - Ketjun kaikkien vaiheiden läpikäynti  
    - Poikkeamien dokumentointi  
  - Ulkoiset auditoijat ja sertifiointielimet (ISO 27701 / ISO 27001)  
    - Standardien mukaisuuden arviointi  
    - Suositukset prosessien ja kontrollien kehittämiseksi
