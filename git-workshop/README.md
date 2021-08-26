# First things first
Dere skal jobbe i grupper, men alle skal gjøre disse oppgavene på egen maskin.
Når det oppstår et problem skal dere hjelpe hverandre til å løse det.

## Del 1:
1. Klon repoet
    * `git clone <url-fra-github>`
1. Lag en ny fil med ditt navn
    * Skriv inn to (2) av dine favoritt-band, -serier, -filmer, -spill, -sporter, -bøker, -malerier, -land å reise til, eller -språk.
1. Legg til og commit filen
    * `git add <filnavn>`
    * `git commit -m <commit-melding>`
1. Lag en ny fil med navnet "greatest.txt"
    * Skriv inn enten: "The greatest thinkers of all time", "The greatest type of rock of all time", "The greatest ice creams of all time", eller en annen tittel for de beste av noe slag. Du kan også skrive overskriften på norsk
    * Fyll inn med minst en (1) person/ting
1. Legg til og commit filene
    * `git add <filnavn>`
    * `git status` for å se hvordan det ligger an
    * `git commit` -> den vil åpne teksteditoren som er konfigurert til å brukes, når du lukker vil det commites (hvis dere har problemer, ta kontakt med Peter)
1. **Stopp! Nå skal dere jobbe sammen**. Dere skal løse de neste delene sekvensielt. Altså skal kun en person sitt tastatur være aktivt om gangen. Gjør stegene til det er ferdig for første person; gå deretter til neste person.
1. Push endringene dine til remote repository
    * `git push`
1. Om det er endringer i remote må dere pulle ned endringene
    * `git pull`
1. Nå kan det være merge conflict og det må håndteres. Noen kommandoer som kan være hjelpsomme:
    * `git status` viser hvordan man ligger an, om det er en merge conflict og hvilken fil det gjelder
    * `git diff`
    * `git log --merge`
    * `git merge --abort` vil stoppe mergingen og putte deg tilbake der du var før sammenslåingskonflikten oppsto, dette kan brukes for å begynne på nytt hvis man har rotet seg vekk



[Litt informasjon om merge conflicts om man vil](https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts)


# Oppgaver

## Intro
I denne delen skal dere få trening i å jobbe med forskjellige strategier for konflikthåndtering i Git. Hver del kommer fra en gitt måte å arbeide på.

Hver del vil lenke til et eget repository som dere skal forke og jobbe på.

## Utfordring (skip hvis du ikke har gjort resten)
Du jobber i en organisasjon som har bestemt at det ikke er lov til å pushe commits til master som feiler tester. På en feature-branch kjører testene grønt nå, men du merker at det er mer enn en commit.

Den allvitende tech leaden har bestemt at man skal aldri squashe commits når man merger, fordi da klumper man (potensielt) sammen for mange endringer.

Du får vite av en litt mer senior utvikler at det kan være lurt å kjøre denne før man lager en merge request:
```
git rebase main --exec pytest
```
Pass på at alle commits i `feature-branch1` passerer testene ved å kjøre `pytest` etter hver commit.


Relevante kommandoer (å lese om):
* squash
* rebase --interactive
* rebase --exec
* push --force



# Ressurser å bruke som start
* https://missing.csail.mit.edu/2020/version-control/

MIT sin "The Missing Semester of your CS education" - Inneholder en del forklaring, en forelesning, lenker til andre ressurser og noen oppgaver.

* https://github.com/neuralsandwich/git-workshop

Gammel (2014), men ser ut som den har mye i seg. Viste seg å ikke være så bra. Men den gir en grei introduksjon.
Vi bør nok fokusere mer på branching og merge conflicts.
Kanskje rebasing med kjøring av kommandoer for å sjekke at alle commits kompilerer.

* https://learngitbranching.js.org/

Helt basic git visualisering, tror det er for lett og lite håndfast.

