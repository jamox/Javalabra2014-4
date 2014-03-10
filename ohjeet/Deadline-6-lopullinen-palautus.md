# Deadline 6, lopullinen palautus

### JavaDoc
* Kaikki luokat, attribuutit, julkiset ja privaatit metodit on dokumentoitu
* Javadocia **ei** tarvitse kirjoittaa...
  * Testeille
  * @Override -metodeille
  * Gettereille ja Settereille, jotka eiv�t tee mit��n ylim��r�ist�
  * Aivan kaikille k�ytt�liittym�luokkien metodeille

### Kirjoita rakennekuvaus
* Kirjoita lyhyt, esimerkiksi muutaman tekstikappaleen kuvaus ohjelmasi rakenteesta
* Toisin sanoen: Avaa luokkakaaviotasi sanallisesti
* Tallenna kuvaus omaan tiedostoonsa tai aihem��rittelyn jatkoksi

### Tarkista projektisi valmius
* Ohjelma toimii ja on valmis
* JUnit-testej� mahdollisimman kattavasti
* Kaaviot, Javadoc ja muu dokumentointi ajantasalla 

### Clean-code
* Ohjelmasi tulisi noudattaa [koodin laatuvaatimuksia](Koodin-laatuvaatimukset.md) mahdollisimman hyvin

### Luo ajettava jar-tiedosto
* Shade-pluginin pit�isi paketoida mukaan ohjelmasi tarvitsemat riippuvuudet, jos sellaisia on.
* Lis�� pom.xml-tiedostoosi uusi plugin:

```
<build>
    <plugins> 
        <!-- ... -->
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-shade-plugin</artifactId>
            <version>2.2</version>
            <executions>
                <execution>
                    <phase>package</phase>
                    <goals>
                        <goal>shade</goal>
                    </goals>
                    <configuration>
                        <transformers>
                            <transformer implementation="org.apache.maven.plugins.shade.resource.ManifestResourceTransformer">
                                <mainClass>javalabra.Main</mainClass>
                            </transformer>
                        </transformers>
                    </configuration>
                </execution>
            </executions>
        </plugin>
    </plugins>
</build>
```

* Korvaa javalabra.Main omalla p��luokallasi (siis haluamallasi `main`-metodin toteuttavalla luokalla).
* Valitse Netbeansista "Clean & Build". Komentorivilt� paketin saa luotua komennolla `mvn package`. Jar-tiedosto luodaan projektikansiosi `target`-kansion sis��n.
* Kokeile .jar -tiedoston toimivuus. Komentorivilt� jar-tiedosto voidaan ajaa komennolla `java -jar paketti.jar`.
   * Jos ohjelma ei toimi, tarkista erityisesti ohjelmasi k�ytt�m�t tiedostopolut - ne ovat suhteellisia .jar-tiedoston sijaintiin
* Kokeile ajaa ohjelmaasi my�s jollain muulla kuin omalla koneellasi. Esimerkiksi natiivikirjastojen kanssa paketointi saattaa vaatia ylim��r�ist� s��t�� - n�iss� tapauksissa esimerkiksi kirjaston dokumentaatio saattaa kertoa sopivimman paketointitavan.

### Kirjoita k�ytt�ohjeet
* Ajattele k�ytt�j��, joka ei ole k�ytt�nyt ohjelmaasi
* Jos ohjelmasi on yksinkertainen k�ytt��, ei k�ytt�ohjeidenkaan tarvitse olla pitk�t

###  Kirjoita testausdokumentaatio
* **Vapaaehtoinen**
* Testausdokumentaatio korvaa yksikk�testauksen puutteita maksimissaan +2 pistett�
* Kirjoita esimerkiksi seuraavista
** Mit� et testannut automaattisesti?
** Miten n�it� on testattu k�sin?
** Raportoi my�s mahdolliset bugit

### Varmista kaikki viel� kerran
* Tarkista, ett� kaikki dokumentaatio on .md, .png tai .jpg -tiedostomuodoissa
* Puske kaikki vaadittava repositorioon ennen deadlinea, viimeisin ennen deadlinea tehty commit arvostellaan
* Tarkista selaimesta, ett� kaikki on varmasti Githubissa
* Tarkista, ett� ohjelma toimii varmasti laitoksen koneilla
* Muistilistana toimii [arvosteluperusteet](Arvosteluperusteet.md)