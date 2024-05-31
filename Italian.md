# Creare un repository

| Comando                     | Descrizione                                  |
| --------------------------- | -------------------------------------------- |
| `$ git init [project name]` | Da zero -- Creare un nuovo repository locale |
| `$ git clone my_url`        | Scaricare da un repository esistente         |

---

# Osservare un archivio

| Comando                         | Descrizione                                                                    |
| ------------------------------- | ------------------------------------------------------------------------------ |
| `$ git status`                  | Elencare i file nuovi o modificati non ancora impegnati                        |
| `$ git dif`                     | Mostrare le modifiche ai file non ancora in scena                              |
| `$ git diff --cached`           | Mostra le modifiche ai file staged                                             |
| `$ git diff HEAD`               | Mostra tutte le modifiche ai file staged e unstaged                            |
| `$ git diff commit1 commit2`    | Mostrare le modifiche tra due ID di commit                                     |
| `$ git blame [file]`            | Elencare le date di modifica e gli autori per un file                          |
| `$ git show [commit]:[file]`    | Mostrare le modifiche ai file per un id di commit e/o un file                  |
| `$ git log`                     | Mostra la cronologia completa delle modifiche                                  |
| `$ git log -p [file/directory]` | Mostra la cronologia delle modifiche per file/directory, incluse le differenze |

---

# Lavorare con i rami

| Comando                                          | Descrizione                                                       |
| ------------------------------------------------ | ----------------------------------------------------------------- |
| `$ git branch`                                   | Elenco di tutte le filiali locali                                 |
| `$ git branch -av`                               | Elencare tutti i rami, locali e remoti                            |
| `$ git checkout my_branch`                       | Passare a un ramo, my_branch, e aggiornare la directory di lavoro |
| `$ git branch new_branch`                        | Creare un nuovo ramo chiamato nuovo_ramo                          |
| `$ git branch -d my_branch`                      | Eliminare il ramo chiamato mio_ramo                               |
| `$ git checkout branch_b & $ git merge branch_a` | Unire il ramo_a al ramo_b                                         |
| `$ git tag my_tag`                               | Taggare il commit corrente                                        |

---

# Cambiamento

| Comando                             | Descrizione                                                      |
| ----------------------------------- | ---------------------------------------------------------------- |
| `$ git add [file]`                  | Mette in scena il file, pronto per il commit                     |
| `$ git add .`                       | Mette in scena tutti i file modificati, pronti per il commit     |
| `$ git commit -m 'commit message'`  | Impegnare tutti i file in fase nella cronologia delle versioni   |
| `$ git commit -am 'commit message'` | Impegnare tutti i file tracciati nella cronologia delle versioni |
| `$ git reset [file]`                | Disallestimento del file, mantenendo le modifiche al file        |
| `$ git reset --hard`                | Riporta tutto all'ultimo commit                                  |

---

# Sincronizzare

| Comando               | Descrizione                                                  |
| --------------------- | ------------------------------------------------------------ |
| `$ git fetch`         | Ottenere le ultime modifiche dall'origine (senza fusione)    |
| `$ git pull`          | Recuperare le ultime modifiche dall'origine e fare il merge  |
| `$ git pull --rebase` | Recuperare le ultime modifiche dall'origine e fare il rebase |
| `$ git push`          | Spingere le modifiche locali all'origine                     |
