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
  - Git versiohallinnan ottaminen käyttöön työkansiossa: git init
  - Git käyttäjänimen määrittäminen: git config user.name "etunimi sukunimi"
  - Sähköpostiosoitteen määrittäminen: git config --global user.email "erkki.esimerkki@example.com"
  - Git tietojen näyttäminen: git config --list --global
    
*Git työskentelyn peruskomentoja:*
  - Tiedon tuottaminen ja muokkaaminen Git työkansiossa
  - Tiedon lisääminen Git indeksiin: git add b.txt tai git add .
  - Commit:n luominen indeksissä olevista tiedoista: git commit -m "Commit viesti"
  - Git commit:n listaaminen: git log tai git log --oneline
  - Git tilan tarkastminen: git status


![alt text](buny.jpg)

**Miten Git ja GitHub toimivat keskenään?**
Työhakemiston synkronoiminen GitHub:n:
  - Paikallisen työkansion kytkeminen GitHub repositorioon:
  ´git remote add origin https://github.com/GitHubTunnus/GitHubRepositorio.git´
  - Etärepositorio kytköksen tarkistaminen: git remote -v
  - Paikallisen työkansion tietojen puskeminen GitHub:n: git push -u origin master
