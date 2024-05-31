# Utwórz repozytorium

| Polecenie                   | Opis                                        |
| --------------------------- | ------------------------------------------- |
| `$ git init [project name]` | Od zera -- Utwórz nowe repozytorium lokalne |
| `$ git clone my_url`        | Pobierz z istniejącego repozytorium         |

---

# Obserwowanie repozytorium

| Polecenie                       | Opis                                                                            |
| ------------------------------- | ------------------------------------------------------------------------------- |
| `$ git status`                  | Lista nowych lub zmodyfikowanych plików, które nie zostały jeszcze zatwierdzone |
| `$ git dif`                     | Pokaż zmiany w plikach, które nie zostały jeszcze zatwierdzone                  |
| `$ git diff --cached`           | Pokaż zmiany w zainscenizowanych plikach                                        |
| `$ git diff HEAD`               | Pokaż wszystkie etapowe i nieetapowe zmiany plików                              |
| `$ git diff commit1 commit2`    | Pokaż zmiany między dwoma identyfikatorami zatwierdzenia                        |
| `$ git blame [file]`            | Lista dat zmian i autorów dla pliku                                             |
| `$ git show [commit]:[file]`    | Pokaż zmiany pliku dla identyfikatora zatwierdzenia i/lub pliku                 |
| `$ git log`                     | Pokaż pełną historię zmian                                                      |
| `$ git log -p [file/directory]` | Pokaż historię zmian dla pliku/katalogu, w tym różnice                          |

---

# Praca z oddziałami

| Polecenie                                        | Opis                                                            |
| ------------------------------------------------ | --------------------------------------------------------------- |
| `$ git branch`                                   | Lista wszystkich oddziałów lokalnych                            |
| `$ git branch -av`                               | Lista wszystkich oddziałów, lokalnych i zdalnych                |
| `$ git checkout my_branch`                       | Przejście do gałęzi my_branch i aktualizacja katalogu roboczego |
| `$ git branch new_branch`                        | Utworzenie nowej gałęzi o nazwie new_branch                     |
| `$ git branch -d my_branch`                      | Usunięcie gałęzi o nazwie my_branch                             |
| `$ git checkout branch_b & $ git merge branch_a` | Scalenie gałęzi_a z gałęzią_b                                   |
| `$ git tag my_tag`                               | Oznaczenie bieżącego zatwierdzenia                              |

---

# Dokonaj zmiany

| Polecenie                           | Opis                                                       |
| ----------------------------------- | ---------------------------------------------------------- |
| `$ git add [file]`                  | Przygotowuje plik do zatwierdzenia                         |
| `$ git add .`                       | Etapuje wszystkie zmienione pliki, gotowe do zatwierdzenia |
| `$ git commit -m 'commit message'`  | Zatwierdź wszystkie etapowe pliki do historii wersji       |
| `$ git commit -am 'commit message'` | Zatwierdź wszystkie śledzone pliki do historii wersji      |
| `$ git reset [file]`                | Unstages plik, zachowując zmiany w pliku                   |
| `$ git reset --hard`                | Przywrócenie wszystkiego do ostatniego zatwierdzenia       |

---

# Synchronizacja

| Polecenie             | Opis                                             |
| --------------------- | ------------------------------------------------ |
| `$ git fetch`         | Pobierz najnowsze zmiany z źródła (bez scalania) |
| `$ git pull`          | Pobierz najnowsze zmiany z źródła i scal         |
| `$ git pull --rebase` | Pobranie najnowszych zmian z źródła i rebase     |
| `$ git push`          | Przesłanie lokalnych zmian do źródła             |
