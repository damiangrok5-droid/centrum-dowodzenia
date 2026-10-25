# Centrum dowodzenia

Strona: https://damiangrok5-droid.github.io/centrum-dowodzenia/

Jedna strona HTML, która pokazuje wszystkie moje projekty z GitHuba. Lista wczytuje się na żywo z API GitHuba,
a co godzinę workflow `refresh.yml` zapisuje kopię zapasową w `repos.json`. Ładniejsze nazwy i opisy można dopisać w `meta.json`.

## Automatyczna kopia `repos.json`
Plik workflow czeka w `workflow-do-dodania/refresh.yml`. Token, którym wgrano repozytorium, nie ma uprawnienia `workflow`,
więc trzeba go dodać ręcznie: na GitHubie *Add file → Create new file*, ścieżka `.github/workflows/refresh.yml`, wklej zawartość i zatwierdź.
Strona działa i tak — lista wczytuje się na żywo z API GitHuba.
