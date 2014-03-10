# Deadline 1

## Luo itsellesi Github-repositorio, jonka nimi vastaa projektiasi.
* Esimerkiksi jos harjoitusty�si aihe on Monopoli ylim��r�isell� blingill� niin repositoriosi voit nimet� vaikkapa Swagopoliksi.
* [Git-ohje](Git-ohje.md)

## Luo uusi Netbeans-projekti repositoriokansioosi
* Luo projekti ja konfiguroi Maven, Cobertura ja PIT [n�iden ohjeiden](Maven-Cobertura-ja-PIT.md) mukaisesti.
* Samalla kansioon pit�isi ilmesty� .gitignore -tiedosto

## Kirjoita aihem��rittely

Lyhyt kuvaus toteutettavasta ohjelmasta. Kuvauksen ei tarvitse olla kovin pitk� eik� kattava. Kuvaus tarkentuu my�hemmin, aluksi dokumentoidaan vain ideat, joiden pohjalta ty�t� l�hdet��n tekem��n. Kuvaus sis�lt�� muutaman tekstikappaleen pituisen yleiskuvauksen.

Tee aihem��rittelyst� md-tiedosto. N�m� tiedostot ovat siis GitHubin tukemia Markdown-tiedostoja, joihin on mahdollisuus lis�t� omia muotoiluja. Kannattaa tutustua  [Markdownin perusteisiin](https://help.github.com/articles/markdown-basics) ja [GitHub Flavored Markdowniin](https://help.github.com/articles/github-flavored-markdown). Tyylitietoisimmat voivat etsi� lis�� kikkoja [t�st� kattavasta oppaasta](http://guides.github.com/overviews/mastering-markdown/). Kaikki kurssilla kirjoitettava dokumentaatio tulee olemaan md-tiedostoissa. Md-tiedostoja voi editoida my�s suoraan GitHubissa.

Aihem��rittelylle hyv� muoto on seuraava:

**Aihe:** ilmoittautumisj�rjestelm�
Toteutetaan j�rjestelm�, jonka avulla yll�pidet��n tietojenk�sittelylaitoksen kurssitietoja sek� tietoja kursseille ilmoittautuneista opiskelijoista... [lis�� teksti� 1-2 tekstikappaleen verran]

**K�ytt�j�t:** Opiskelija ja Opetushallinto

**Kaikkien k�ytt�jien toiminnot:**
* j�rjestelm��n kirjautuminen
  * onnistuu jos salasana ja k�ytt�j�tunnus oikein
* kaikkien kurssien listaus
* ...

**Opiskelijan toiminnot:**
* ilmoittautuminen
  * onnistuu jos kurssi ei ole t�ynn� ja opiskelija ei ole jo kurssilla
* omien ilmoittautumisten listaus
* ...

**Opetushallinnon toiminnot:**
* uusien kurssien lis�ys
* tietyn kurssin ilmoittautujien listaaminen
* ...

## Aloita tuntikirjanpito

* Muoto: md-tiedosto
* Pid� kirjaa harjoitusty�h�n k�ytt�m�st�si ty�m��r�st�
* K�ytt�m�si ty�m��r� ei vaikuta arvosanaan, joten ole rehellinen
* Merkitse aina v�hint��n p�iv�m��r�, k�ytt�m�si aika ja ajank�yt�n kohde

## Noudata kansiorakennetta

Kansiorakenne n�ytt�� sen, milt� projektikansion pit�isi n�ytt�� kurssin lopulla. Esimerkiksi Javadoc-kansiota tai k�ytt�ohjeita ei tarvitse kuin kurssin lopussa. Noudata selke�� kansiorakennetta kuitenkin heti alussa. 

Kansiorakenne:
* Harjoitusty�si juurikansio (Repositoriokansio)
  * Ohjelma.jar (Vaaditaan vasta palautuksessa)
  * ohjelmasinimit�h�n (Netbeansin projektihakemisto)
  * javadoc (Generoitu dokumentaatio, vaaditaan vasta loppupalautuksessa)
  * dokumentointi
    * aiheenKuvausJaRakenne.md
    * testausdokumentti.md
    * k�ytt�ohjeet.md
    * tuntikirjanpito.md
    * luokka- ja sekvenssikaaviot.png tai .jpg

## Palauta Githubiin ja rekister�i itsesi kurssin labtooliin

Puske (push) kaikki edell� tehdyt muutokset ja lis�ykset Githubiin Git-ohjeiden mukaisesti.
Rekister�i itsesi kurssin labtooliin osoitteessa: http://tktl-labtool.herokuapp.com/register. Rekister�itymiseen tarvitset nimesi, s�hk�postiosoitteesi, opiskelijanumerosi, harjoitusty�aiheesi ja Github-repositoriosi http-osoitteen.

**Palautuksia ei l�hetet� s�hk�postilla. Jos t�rm��t ongelmiin, niin �l� j�� murhehtimaan yksin�si, vaan l�het� s�hk�postia ohjaajille. Palautukseksi katsotaan viimeisin ennen deadlinea tehty Github pushaus. Ohjaajat siis seuraavat edistymist� suoraan Github-repositoriosi kautta ja antavat palautetta ty�st�si pajassa sek� labtoolin v�lityksell�** http://tktl-labtool.herokuapp.com/mypage