# Crear un repositorio

| Comando                     | Descripción                                    |
| --------------------------- | ---------------------------------------------- |
| `$ git init [project name]` | Desde cero -- Crear un nuevo repositorio local |
| `$ git clone my_url`        | Descargar desde un repositorio existente       |

---

# Observar un repositorio

| Comando                         | Descripción                                                                                    |
| ------------------------------- | ---------------------------------------------------------------------------------------------- |
| `$ git status`                  | Listar ficheros nuevos o modificados aún no confirmados                                        |
| `$ git dif`                     | Mostrar los cambios en los ficheros que aún no se han preparado                                |
| `$ git diff --cached`           | Mostrar los cambios en los archivos organizados                                                |
| `$ git diff HEAD`               | Mostrar todos los cambios en los ficheros, tanto los que ya están como los que aún no lo están |
| `$ git diff commit1 commit2`    | Mostrar los cambios entre dos identificadores de confirmación                                  |
| `$ git blame [file]`            | Mostrar las fechas de modificación y los autores de un archivo                                 |
| `$ git show [commit]:[file]`    | Mostrar los cambios de un archivo para un identificador de confirmación y/o archivo            |
| `$ git log`                     | Mostrar el historial completo de cambios                                                       |
| `$ git log -p [file/directory]` | Mostrar el historial de cambios de un archivo/directorio incluyendo los diffs                  |

---

# Trabajar con ramas

| Comando                                          | Descripción                                                        |
| ------------------------------------------------ | ------------------------------------------------------------------ |
| `$ git branch`                                   | Lista de todas las sucursales locales                              |
| `$ git branch -av`                               | Lista de todas las ramas, locales y remotas                        |
| `$ git checkout my_branch`                       | Cambiar a una rama, mi_rama, y actualizar el directorio de trabajo |
| `$ git branch new_branch`                        | Crear una nueva rama llamada nueva_rama                            |
| `$ git branch -d my_branch`                      | Eliminar la rama llamada mi_rama                                   |
| `$ git checkout branch_b & $ git merge branch_a` | Fusionar rama_a en rama_b                                          |
| `$ git tag my_tag`                               | Etiquetar la confirmación actual                                   |

---

# Cambia

| Comando                             | Descripción                                                         |
| ----------------------------------- | ------------------------------------------------------------------- |
| `$ git add [file]`                  | Prepara el archivo para la confirmación                             |
| `$ git add .`                       | Prepara todos los archivos modificados, listos para la confirmación |
| `$ git commit -m 'commit message'`  | Confirmar todos los archivos en el historial de versiones           |
| `$ git commit -am 'commit message'` | Consignar todos los archivos rastreados al historial versionado     |
| `$ git reset [file]`                | Desescalar el archivo, manteniendo los cambios                      |
| `$ git reset --hard`                | Revertir todo a la última confirmación                              |

---

# Sincronice

| Comando               | Descripción                                         |
| --------------------- | --------------------------------------------------- |
| `$ git fetch`         | Obtener los últimos cambios del origen (sin fusión) |
| `$ git pull`          | Obtener los últimos cambios del origen y fusionar   |
| `$ git pull --rebase` | Obtener los últimos cambios del origen y fusionar   |
| `$ git push`          | Empujar los cambios locales al origen               |
