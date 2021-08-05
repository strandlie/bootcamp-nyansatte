# First things first
Enkle oppgaver som oppvarming.

Del 1:
1. Fork repo (kun 1 person)
    * Gjøres i github/gitlab
1. Klon den nye forken
    * `git clone <url-fra-github/gitlab>`
1. Lag en ny branch med ditt navn
    * `git checkout -b <navn>` eller `git branch <navn>`
    * Sjekk hvilken branch du er på med `git branch` eller `git status`
1. Lag en ny fil med ditt navn
    * Skriv inn to (2) av dine favoritt-band, -serier, -filmer, -spill, -sporter, -bøker, -malerier, -land å reise til, eller -språk.
    <!-- Denne delen kan kanskje flyttes til senere, siden den skal lage merge conflicts -->
1. Lag en ny fil med navnet "greatest.txt"
    * Skriv inn enten: "The greatest thinkers of all time", "The greatest type of rock of all time", "The greatest ice creams of all time", eller en annen tittel for de beste av noe slag. Du kan også skrive overskriften på norsk
    * Fyll inn med minst en (1) person/ting
    <!-- Slutt på flyttes til senere -->
1. Legg til og commit filene
    * `git add <filnavn>`
    * `git status` for å se hvordan det ligger an
    * `git commit` -> den vil åpne editoren som er konfigurert til å brukes, når du lukker vil det commites
1. Merge tilbake til master
    * `git merge --help`
    * `git checkout master`
    * `git merge <branchnavn>`

Del 2:






# Oppgaver

## Intro

Du jobber i en organisasjon som har bestemt at det ikke er lov til å pushe commits til master som feiler tester. På en feature-branch kjører testene grønt nå, men du merker at det er mer enn en commit.

Den allvitende tech leaden har bestemt at man skal aldri squashe commits når man merger, fordi da klumper man (potensielt) sammen for mange endringer.

Du får vite av en litt mer senior utvikler at det kan være lurt å kjøre denne før man lager en merge request:
```
git rebase main --exec pytest
```
Pass på at alle commits i feature-branch1 passerer testene ved å kjøre pytest etter hver commit.


Relevante kommandoer (å lese om):
* squash
* rebase --interactive
* rebase --exec
* push --force
## Del 1




# Ressurser å bruke som start
* https://missing.csail.mit.edu/2020/version-control/
MIT sin "The Missing Semester of your CS education" - Inneholder en del forklaring, en forelesning, lenker til andre ressurser og noen oppgaver.

* https://github.com/neuralsandwich/git-workshop

Gammel (2014), men ser ut som den har mye i seg. Viste seg å ikke være så bra. Men den gir en grei introduksjon.
Vi bør nok fokusere mer på branching og merge conflicts.
Kanskje rebasing med kjøring av kommandoer for å sjekke at alle commits kompilerer.

* https://learngitbranching.js.org/

Helt basic git visualisering, tror det er for lett og lite håndfast.

