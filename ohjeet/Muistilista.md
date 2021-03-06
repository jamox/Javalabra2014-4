﻿# Muistilista

Ohessa tarkistuslista lopullisen työn tavoitteisiin. Vajavainen toteutus vähentää pisteitä, puuttuva osat voi miinustaa pisteitä. Kurssin yhden osa-alueen (aikataulun noudattaminen, toteutus, dokumentaatio, testaus) laiminlyöminen voi olla yksin syy hylättyyn kurssisuoritukseen.

Täyteen arvosanaan ei vaadita virheetöntä suoritusta, mutta ohjeita kannattaa noudattaa mahdollisimman hyvin - niin opit itsekin parhaiten.

### Ohjelma

**Ohjelmakoodi**
Ohjelma on riittävän laaja. Yksinkertaista aihetta on laajennettu esimerkiksi tallentamisella, pistetilastoilla, kirjautumisella tai erityisominaisuuksilla. Koodi on selkeää luettavaa, jaoteltu selkeisiin paketteihin ja luokkiin, joilla on yksi vastuu. Koodi on ylläpidettävää ja laajennettavaa.
* [Koodin laatuvaatimukset](Koodin-laatuvaatimukset.md)

**Jar-tiedosto**
Auttaa arvostelussa, jos tarkastajat eivät saa muuten käännettyä ohjelmakoodia. Huomioi erityisesti ohjelmasi tarvitsemat resurssit, kuten kuva- tai tekstitiedostot. Niiden sijainnit ilmoitetaan koodissa usein suhteellisina sijainteina, jolloin joudut ottamaan tiedostojen sijainnin huomioon myös jar-tiedoston kanssa. Testaa Jar-tiedostoa usealla koneella.
* Yleisin syy toimimattomuuteen on Javan versiossa tai tiedostopolussa

**Ohjelman toimivuus**
Ohjelma ottaa huomioon esimerkiksi vääränmuotoisen syötteen, vääränmuotoiset tekstitiedostot tai ohjelman kannalta oleellisten tiedostojen puuttumisen kaatumatta. Pelien säännöt toimivat oikein.

### Testit

Ohjelman kaikkia järkeviä loogisia luokkia on testattu kattavasti: mahdollisimman montaa metodia, virhetilanteet ja syötteet huomioiden. Testeissä on tärkeää myös testien laatu. Testien tulisi testata järkeviä asioita, hyvin nimettyinä sekä järkevästi rakennettuina. Testiluokkien muuttujien, setUp() -metodin sekä apumetodien käyttö, asserttien virheilmoitusten sekä useiden erilaisten asserttien käyttö auttavat testien selkeyteen.
* Käyttöliittymä, mahdolliset grafiikat, äänet ja ulkopuolisten kirjastojen toiminta testataan käsin, sillä yksikkötestausta näitä varten ei ole opetettu

### Dokumentaatio

Käytä kaikessa dokumentoinnissa omaa harkintakykyäsi pituuden ja laajuuden kannalta. 

**Javadoc**
* Muista erityisesti seuraavat:
  * Luokat kuvattu
  * Attribuutit kuvattu
  * Metodit ja metodien parametrit/palautusarvot kuvattu
* Testejä **ei** tarvitse kuvata
* @Override -metodeja **ei** tarvitse usein kuvata
* Set/Get -metodeja **ei** tarvitse kuvata, jos metodit eivät tee laskentaa tai tarkastuksia
* Käyttöliittymäluokkien koodia **ei** tarvitse kuvata kovin tarkasti

**Luokkakaavio**
* Merkitty kaikki oleelliset luokat, osallistumisrajoitteet ja yhteyksien suunnat
* Käyttöliittymän voi kuitata yhdellä luokalla, tärkeintä on käyttöliittyymän suhde muuhun koodiin
* **Ei** tarvitse merkitä attribuutteja tai metodeja - ne löytyvät JavaDocista
* .jpg, .png tai .pdf

**Sekvenssikaaviot**
* 3-5 sekvenssikaaviota tärkeimmistä toiminnallisuuksista
* Tärkeää sekvenssikaavioiden oikeellisuus ja selkeys
* .jpg, .png tai .pdf

**Aihemäärittely**
* Selkeä parin kappaleen selitys ohjelman sisällöstä
* Lueteltu ohjelman käyttäjät
* ...sekä käyttäjien toiminnat
* Kelpaa myös käyttötapauskaaviona
* .txt tai .pdf

**Ohjelman rakenteen kuvaus**
* Luokkakaaviota selitetty sanallisesti hieman auki
* Vapaamuotoinen muutaman tekstikappaleen kuvaus
* .txt tai .pdf

**Käyttöohjeet**
* Ajattele ihmistä, joka ei ole koskaan käyttänyt ohjelmaasi
* Jos ohjelma selittää itse itsensä, riittää suppeat käyttöohjeet tai toisinaan pelkkä käynnistysohje
* .txt tai .pdf

**Tuntikirjanpito**
* Merkitse aina vähintään päivä, käyttämäsi aika ja ajankäytön kohde
* .txt tai .pdf

**Testausdokumentaatio**
* (VAPAAEHTOINEN)
* Vapaamuotoinen selitys siitä, miten ohjelmaansa on testannut automaattisella testauksella ja käsin
* Hyvä muoto voi olla esimerkiksi taulukko tai muutama tekstikappale
* Testausdokumentaatio on luonnollisin sijainti bugihavainnoille
* .txt tai .pdf

### Kansiorakenne:

* Harjoitustyösi juurikansio (Repositoriokansio)
  * Ohjelma.jar
  * projekti (Netbeansin projektihakemisto)
  * javadoc (Generoitu dokumentaatio)
  * dokumentointi
    * aiheenKuvausJaRakenne.pdf
    * testausdokumentti.pdf
    * käyttöohjeet.pdf
    * tuntikirjanpito.txt
    * luokka- ja sekvenssikaaviot

### Lopputulos:

![viiskauttaviis](https://raw.github.com/kxkyllon/Javalabra/master/kuvat/viiskauttaviis.gif)!