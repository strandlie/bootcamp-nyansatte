## Utfordring (skip hvis du ikke har gjort resten)
Du jobber i en organisasjon som har bestemt at det ikke er lov til å pushe commits til master som feiler tester. På en feature-branch kjører testene grønt nå, men du merker at det er mer enn en commit.

Den allvitende tech leaden har bestemt at man skal aldri squashe commits når man merger, fordi da klumper man (potensielt) sammen for mange endringer.

Du får vite av en litt mer senior utvikler at det kan være lurt å kjøre denne før man lager en merge request:
```
git rebase main --exec pytest
```
Pass på at alle commits i `feature-branch` passerer testene ved å kjøre `pytest` etter hver commit.
Hvis noen tester feiler må du fikse koden og så committe tilbake.

Bonus: Det er en fil som ikke bør være med i en av committene.

Relevante kommandoer (å lese om):
* squash
* rebase --interactive
* rebase --exec
* push --force

