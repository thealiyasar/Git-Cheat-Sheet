# Criar um Repositor

| Comando                     | Descrição                                  |
| --------------------------- | ------------------------------------------ |
| `$ git init [project name]` | Do zero -- Criar um novo repositório local |
| `$ git clone my_url`        | Descarregar de um repositório existente    |

---

# Observar um repositório

| Comando                         | Descrição                                                                   |
| ------------------------------- | --------------------------------------------------------------------------- |
| `$ git status`                  | Listar ficheiros novos ou modificados ainda não confirmados                 |
| `$ git dif`                     | Mostrar as alterações aos ficheiros ainda não preparados                    |
| `$ git diff --cached`           | Mostrar as alterações aos ficheiros preparados                              |
| `$ git diff HEAD`               | Mostrar todas as alterações de ficheiros preparadas e não preparadas        |
| `$ git diff commit1 commit2`    | Mostrar as alterações entre dois IDs de commit                              |
| `$ git blame [file]`            | Listar as datas de alteração e os autores de um ficheiro                    |
| `$ git show [commit]:[file]`    | Mostrar as alterações de um arquivo para um ID de commit e/ou arquivo       |
| `$ git log`                     | Mostrar todo o histórico de alterações                                      |
| `$ git log -p [file/directory]` | Mostrar o histórico de alterações de um ficheiro/diretório, incluindo diffs |

---

# Trabalhar com ramificações

| Comando                                          | Descrição                                                                  |
| ------------------------------------------------ | -------------------------------------------------------------------------- |
| `$ git branch`                                   | Listar todas as sucursais locais                                           |
| `$ git branch -av`                               | Listar todas as ramificações, locais e remotas                             |
| `$ git checkout my_branch`                       | Mudar para uma ramificação, my_branch, e atualizar o diretório de trabalho |
| `$ git branch new_branch`                        | Criar uma nova ramificação chamada new_branch                              |
| `$ git branch -d my_branch`                      | Excluir a ramificação chamada minha_ramificação                            |
| `$ git checkout branch_b & $ git merge branch_a` | Mesclar branch_a em branch_b                                               |
| `$ git tag my_tag`                               | Marcar o commit atual                                                      |

---

# Fazer uma mudança

| Comando                             | Descrição                                                             |
| ----------------------------------- | --------------------------------------------------------------------- |
| `$ git add [file]`                  | Prepara o ficheiro, pronto para submissão                             |
| `$ git add .`                       | Prepara todos os ficheiros alterados, prontos para submissão          |
| `$ git commit -m 'commit message'`  | Comprometer todos os ficheiros preparados para o histórico de versões |
| `$ git commit -am 'commit message'` | Submete todos os seus ficheiros controlados ao histórico de versões   |
| `$ git reset [file]`                | Desfaz o stage do ficheiro, mantendo as alterações do ficheiro        |
| `$ git reset --hard`                | Reverter tudo para o último commit                                    |

---

# Sincronizar

| Comando               | Descrição                                                   |
| --------------------- | ----------------------------------------------------------- |
| `$ git fetch`         | Obter as alterações mais recentes da origem (sem mesclagem) |
| `$ git pull`          | Obter as últimas alterações da origem e fazer merge         |
| `$ git pull --rebase` | Obter as últimas alterações da origem e fazer rebase        |
| `$ git push`          | Enviar as alterações locais para a origem                   |
