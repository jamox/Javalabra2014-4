# Muistilista

Ohessa tarkistuslista lopullisen ty�n tavoitteisiin. Vajavainen toteutus v�hent�� pisteit�, puuttuva osat voi miinustaa pisteit�. Kurssin yhden osa-alueen (aikataulun noudattaminen, toteutus, dokumentaatio, testaus) laiminly�minen voi olla yksin syy hyl�ttyyn kurssisuoritukseen.

T�yteen arvosanaan ei vaadita virheet�nt� suoritusta, mutta ohjeita kannattaa noudattaa mahdollisimman hyvin - niin opit itsekin parhaiten.

### Ohjelma

**Ohjelmakoodi**
Ohjelma on riitt�v�n laaja. Yksinkertaista aihetta on laajennettu esimerkiksi tallentamisella, pistetilastoilla, kirjautumisella tai erityisominaisuuksilla. Koodi on selke�� luettavaa, jaoteltu selkeisiin paketteihin ja luokkiin, joilla on yksi vastuu. Koodi on yll�pidett�v�� ja laajennettavaa.
* [Koodin laatuvaatimukset](Koodin-laatuvaatimukset.md)

**Jar-tiedosto**
Auttaa arvostelussa, jos tarkastajat eiv�t saa muuten k��nnetty� ohjelmakoodia. Huomioi erityisesti ohjelmasi tarvitsemat resurssit, kuten kuva- tai tekstitiedostot. Niiden sijainnit ilmoitetaan koodissa usein suhteellisina sijainteina, jolloin joudut ottamaan tiedostojen sijainnin huomioon my�s jar-tiedoston kanssa. Testaa Jar-tiedostoa usealla koneella.
* Yleisin syy toimimattomuuteen on Javan versiossa tai tiedostopolussa

**Ohjelman toimivuus**
Ohjelma ottaa huomioon esimerkiksi v��r�nmuotoisen sy�tteen, v��r�nmuotoiset tekstitiedostot tai ohjelman kannalta oleellisten tiedostojen puuttumisen kaatumatta. Pelien s��nn�t toimivat oikein.

### Testit

Ohjelman kaikkia j�rkevi� loogisia luokkia on testattu kattavasti: mahdollisimman montaa metodia, virhetilanteet ja sy�tteet huomioiden. Testeiss� on t�rke�� my�s testien laatu. Testien tulisi testata j�rkevi� asioita, hyvin nimettyin� sek� j�rkev�sti rakennettuina. Testiluokkien muuttujien, setUp() -metodin sek� apumetodien k�ytt�, asserttien virheilmoitusten sek� useiden erilaisten asserttien k�ytt� auttavat testien selkeyteen.
* K�ytt�liittym�, mahdolliset grafiikat, ��net ja ulkopuolisten kirjastojen toiminta testataan k�sin, sill� yksikk�testausta n�it� varten ei ole opetettu

### Dokumentaatio

K�yt� kaikessa dokumentoinnissa omaa harkintakyky�si pituuden ja laajuuden kannalta. 

**Javadoc**
* Muista erityisesti seuraavat:
  * Luokat kuvattu
  * Attribuutit kuvattu
  * Metodit ja metodien parametrit/palautusarvot kuvattu
* Testej� **ei** tarvitse kuvata
* @Override -metodeja **ei** tarvitse usein kuvata
* Set/Get -metodeja **ei** tarvitse kuvata, jos metodit eiv�t tee laskentaa tai tarkastuksia
* K�ytt�liittym�luokkien koodia **ei** tarvitse kuvata kovin tarkasti

**Luokkakaavio**
* Merkitty kaikki oleelliset luokat, osallistumisrajoitteet ja yhteyksien suunnat
* K�ytt�liittym�n voi kuitata yhdell� luokalla, t�rkeint� on k�ytt�liittyym�n suhde muuhun koodiin
* **Ei** tarvitse merkit� attribuutteja tai metodeja - ne l�ytyv�t JavaDocista
* .jpg, .png tai .pdf

**Sekvenssikaaviot**
* 3-5 sekvenssikaaviota t�rkeimmist� toiminnallisuuksista
* T�rke�� sekvenssikaavioiden oikeellisuus ja selkeys
* .jpg, .png tai .pdf

**Aihem��rittely**
* Selke� parin kappaleen selitys ohjelman sis�ll�st�
* Lueteltu ohjelman k�ytt�j�t
* ...sek� k�ytt�jien toiminnat
* Kelpaa my�s k�ytt�tapauskaaviona
* .txt tai .pdf

**Ohjelman rakenteen kuvaus**
* Luokkakaaviota selitetty sanallisesti hieman auki
* Vapaamuotoinen muutaman tekstikappaleen kuvaus
* .txt tai .pdf

**K�ytt�ohjeet**
* Ajattele ihmist�, joka ei ole koskaan k�ytt�nyt ohjelmaasi
* Jos ohjelma selitt�� itse itsens�, riitt�� suppeat k�ytt�ohjeet tai toisinaan pelkk� k�ynnistysohje
* .txt tai .pdf

**Tuntikirjanpito**
* Merkitse aina v�hint��n p�iv�, k�ytt�m�si aika ja ajank�yt�n kohde
* .txt tai .pdf

**Testausdokumentaatio**
* (VAPAAEHTOINEN)
* Vapaamuotoinen selitys siit�, miten ohjelmaansa on testannut automaattisella testauksella ja k�sin
* Hyv� muoto voi olla esimerkiksi taulukko tai muutama tekstikappale
* Testausdokumentaatio on luonnollisin sijainti bugihavainnoille
* .txt tai .pdf

### Kansiorakenne:

* Harjoitusty�si juurikansio (Repositoriokansio)
  * Ohjelma.jar
  * projekti (Netbeansin projektihakemisto)
  * javadoc (Generoitu dokumentaatio)
  * dokumentointi
    * aiheenKuvausJaRakenne.pdf
    * testausdokumentti.pdf
    * k�ytt�ohjeet.pdf
    * tuntikirjanpito.txt
    * luokka- ja sekvenssikaaviot

### Lopputulos:

![viiskauttaviis](https://raw.github.com/kxkyllon/Javalabra/master/kuvat/viiskauttaviis.gif)!