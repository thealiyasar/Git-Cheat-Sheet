# Repozitor yaradın

| Əmr                         | Təsvir                                      |
| --------------------------- | ------------------------------------------- |
| `$ git init [project name]` | Sıfırdan -- Yeni yerli repozitoriya yaradın |
| `$ git clone my_url`        | Mövcud depodan yükləyin                     |

---

# Repozitoru müşahidə edin

| Əmr                             | Təsvir                                                               |
| ------------------------------- | -------------------------------------------------------------------- |
| `$ git status`                  | Hələ qəbul edilməmiş yeni və ya dəyişdirilmiş faylları sadalayın     |
| `$ git dif`                     | Hələ səhnələşdirilməmiş fayllardakı dəyişiklikləri göstərin          |
| `$ git diff --cached`           | Mərhələli fayllardakı dəyişiklikləri göstərin                        |
| `$ git diff HEAD`               | Bütün mərhələli və mərhələsiz fayl dəyişikliklərini göstərin         |
| `$ git diff commit1 commit2`    | İki icra identifikatoru arasındakı dəyişiklikləri göstərin           |
| `$ git blame [file]`            | Fayl üçün dəyişiklik tarixlərini və müəlliflərini sadalayın          |
| `$ git show [commit]:[file]`    | Tapşırıq id və/və ya fayl üçün fayl dəyişikliklərini göstərin        |
| `$ git log`                     | Tam dəyişiklik tarixçəsini göstərin                                  |
| `$ git log -p [file/directory]` | Fərqlər daxil olmaqla fayl/kataloq üçün dəyişiklik tarixini göstərin |

---

# Filiallarla İş

| Əmr                                              | Təsvir                                              |
| ------------------------------------------------ | --------------------------------------------------- |
| `$ git branch`                                   | Bütün yerli filialları sadalayın                    |
| `$ git branch -av`                               | Yerli və uzaq bütün filialları sadalayın            |
| `$ git checkout my_branch`                       | Filial, my_branch-a keçin və iş qovluğunu yeniləyin |
| `$ git branch new_branch`                        | new_branch adlı yeni filial yaradın                 |
| `$ git branch -d my_branch`                      | my_branch adlı filialı silin                        |
| `$ git checkout branch_b & $ git merge branch_a` | filialı_b filialına birləşdirin                     |
| `$ git tag my_tag`                               | Cari öhdəliyi tag edin                              |

---

# Dəyişiklik edin

| Əmr                                 | Təsvir                                                        |
| ----------------------------------- | ------------------------------------------------------------- |
| `$ git add [file]`                  | Faylı mərhələləşdirir, icraya hazırdır                        |
| `$ git add .`                       | Bütün dəyişdirilmiş faylları səhnələşdirin, icraya hazır olun |
| `$ git commit -m 'commit message'`  | Bütün mərhələli faylları versiya tarixçəsinə həvalə edin      |
| `$ git commit -am 'commit message'` | Bütün izlənilən fayllarınızı versiya tarixçəsinə həvalə edin  |
| `$ git reset [file]`                | Fayl dəyişikliklərini saxlayaraq, faylı mərhələsizləşdirir    |
| `$ git reset --hard`                | Hər şeyi son öhdəliyə qaytarın                                |

---

# Sinxronlaşdırın

| Əmr                   | Təsvir                                                     |
| --------------------- | ---------------------------------------------------------- |
| `$ git fetch`         | Mənbədən ən son dəyişiklikləri əldə edin (birləşmə yoxdur) |
| `$ git pull`          | Ən son dəyişiklikləri mənşədən alın və birləşdirin         |
| `$ git pull --rebase` | Mənşə və yenidən bazadan ən son dəyişiklikləri əldə edin   |
| `$ git push`          | Yerli dəyişiklikləri mənşəyə itələyin                      |
