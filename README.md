# bootcamp-nyansatte
Workshops og annet for bootcamp for nyansatte


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
