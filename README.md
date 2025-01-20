# Git ja GitHub


**Mitä on versiohallinta?**

Versiohallinta on tekniikka, jolla pidetään kirjaa tiedostoihin tehdyistä muutoksista ja niistä säilötään vanhemmat versiot.

![alt text](git.png)

**Mikä on Git?**

Git on ilmainen vapaan lähdekoodin ohjelma, jota käytetään versiohallintaan. Ohjelma säilyttää tietoa kaikista tiedostoihin tehdyistä muutoksista, ja mahdollistaa projektissa versiohallinnan.

![alt text](github.png)

**Mikä on GitHub?**

GitHub on vuonna 2008 avattu verkkosivusto, joka tarjoaa paikan Git-versionhallintaa käyttäville ohjelmistokehitysprojekteille.

**Miten Git:ä käytetään?**

Git:ä voidaan käyttää komentoriviltä, tai suoraan esimerkiksi Visual Studio Coden kautta. 

*Git järjestelmänä koostuu kolmesta osasta*
  1. Työkansio tietoineen (working directory)
  2. Git indeksi (staging area)
  3. Paikallinen versionhallinta repositorio .git hakemistossa (local .git)

*Git tietojen määrittäminen:*
  - Git versiohallinnan ottaminen käyttöön työkansiossa: `git init`
  - Git käyttäjänimen määrittäminen: `git config user.name "etunimi sukunimi"`
  - Sähköpostiosoitteen määrittäminen: `git config --global user.email "erkki.esimerkki@example.com"`
  - Git tietojen näyttäminen: `git config --list --global`
    
*Git työskentelyn peruskomentoja:*
  - Tiedon tuottaminen ja muokkaaminen Git työkansiossa
  - Tiedon lisääminen Git indeksiin: `git add b.txt tai git add .`
  - Commit:n luominen indeksissä olevista tiedoista: `git commit -m "Commit viesti"`
  - Git commit:n listaaminen: `git log tai git log --oneline`
  - Git tilan tarkastminen: `git status`


![alt text](buny.jpg)

**Miten Git ja GitHub toimivat keskenään?**
*Työhakemiston synkronoiminen GitHub:n:*
  - Paikallisen työkansion kytkeminen GitHub repositorioon:
    `git remote add origin https://github.com/GitHubTunnus/GitHubRepositorio.git`
  - Etärepositorio kytköksen tarkistaminen: `git remote -v`
  - Paikallisen työkansion tietojen puskeminen GitHub:n: `git push -u origin master`

*GitHub:a olevien tietojen synkronoiminen paikalliseen työkansioon:*

  - GitHub repositorion ja paikallisen työkansion tilenteen erojen päivittäminen: `git fetch`
  - Tietojen lataaminen GitHub repositoriosta paikalliseen työkansioon: `git pull`

*GitHub fork:*
  - Ns. Fork on GitHub repositorio joka syntynyt fork toiminnon takia kopiona jonkun toisen GitHub repositorista. Fork sisältää kaikki samat tiedot kuin alkuperäinen repositorio. Fork:n     omistaa kopion luonut henkilö joten tietojen lisääminen Fork repositorioon on mahdollista.

*Git fork:n liittyviä Git komentoja*

  - Upstream remoten lisääminen paikalliseen Git työhakemistoon:
  `git remote add upstream <git://github.com/GitHubTunnus>/GitHubRepositorio.git>`
  - Upstream remoten tietojen synkronoiminen Giot työhakemistoon: `git fetch upstream`
    
**Haarat eli branch:t**

Git haara (branch) on toiminallisuus joka mahdollistaa haarassa olevien tietojen muuttamisen ilman että muutoksilla on vaikutusta työkansion muihin tietoihin. Haaraa voitaisiin käyttää sovelluksen erilaisten toiminnallisuuksien kehittämiseen ilman että kehitystyöllä on vaikutusta sovelluksen muun lähdekoodin toimintaan. Haarassa olevat tiedot yhdistetään lopulta sovelluksen päähaaran (master tai main) sisältämään lähdekoodiin.

Git haaroihin liittyvä työskentely:
  - Git haarojen listaaminen: `git branch`
  - Uuden haaran lisääminen: `git branch haaran_nimi tai git checkout haaran_nimi`
  - Haaran tietojen yhdistäminen master päähaaraan: `git merge haaran_nimi`
  - Haaran poistaminen: `git branch -d uusibranch`


##Linkkejä##
[Git](https://git-scm.com/)
[Github]((https://github.com/)
