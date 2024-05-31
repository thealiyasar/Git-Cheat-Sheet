# Bir Repositor Oluşturun

| Komut                       | Açıklama                                  |
| --------------------------- | ----------------------------------------- |
| `$ git init [project name]` | Sıfırdan -- Yeni bir yerel depo oluşturun |
| `$ git clone my_url`        | Mevcut bir depodan indirme                |

---

# Bir Depoyu Gözlemleyin

| Komut                           | Açıklama                                                              |
| ------------------------------- | --------------------------------------------------------------------- |
| `$ git status`                  | Henüz işlenmemiş yeni veya değiştirilmiş dosyaları listeleme          |
| `$ git dif`                     | Henüz aşamalandırılmamış dosyalardaki değişiklikleri göster           |
| `$ git diff --cached`           | Hazırlanan dosyalardaki değişiklikleri göster                         |
| `$ git diff HEAD`               | Tüm aşamalı ve aşamasız dosya değişikliklerini göster                 |
| `$ git diff commit1 commit2`    | İki commit kimliği arasındaki değişiklikleri göster                   |
| `$ git blame [file]`            | Bir dosya için değişiklik tarihlerini ve yazarları listeleme          |
| `$ git show [commit]:[file]`    | Bir commit kimliği ve/veya dosya için dosya değişikliklerini gösterme |
| `$ git log`                     | Tüm değişiklik geçmişini göster                                       |
| `$ git log -p [file/directory]` | Farklar dahil dosya/dizin için değişiklik geçmişini göster            |

---

# Working With Branches

| Komut                                                | Açıklama                                                    |
| ---------------------------------------------------- | ----------------------------------------------------------- |
| `$ git branch`                                       | Tüm yerel şubeleri listeleyin                               |
| `$ git branch -av`                                   | Yerel ve uzak tüm şubeleri listeleyin                       |
| `$ git checkout my_branch`                           | Bir dala, my_branch'a geçin ve çalışma dizinini güncelleyin |
| `$ git branch new_branch`                            | new_branch adında yeni bir şube oluşturun                   |
| `$ git branch -d my_branch`                          | my_branch adlı dalı sil                                     |
| `$ git checkout branch_b ----  $ git merge branch_a` | branch_a'yı branch_b ile birleştir                          |
| `$ git tag my_tag`                                   | Geçerli commit'i etiketleyin                                |

---

# Şubelerle Çalışma

| Komut                               | Açıklama                                                       |
| ----------------------------------- | -------------------------------------------------------------- |
| `$ git add [file]`                  | Dosyayı commit için hazır hale getirir                         |
| `$ git add .`                       | Değiştirilen tüm dosyaları işleme hazır hale getirin           |
| `$ git commit -m 'commit message'`  | Tüm aşamalı dosyaları sürümlü geçmişe işleyin                  |
| `$ git commit -am 'commit message'` | İzlediğiniz tüm dosyaları sürümlü geçmişe işleyin              |
| `$ git reset [file]`                | Dosya değişikliklerini koruyarak dosyanın aşamalarını kaldırır |
| `$ git reset --hard`                | Her şeyi son işleme geri döndür                                |

---

# Senkronize et

| Komut                 | Açıklama                                                       |
| --------------------- | -------------------------------------------------------------- |
| `$ git fetch`         | Origin'den en son değişiklikleri al (birleştirme yok)          |
| `$ git pull`          | Origin'den en son değişiklikleri getir ve birleştir            |
| `$ git pull --rebase` | Origin'den en son değişiklikleri getirin ve yeniden tabanlayın |
| `$ git push`          | Yerel değişiklikleri orijine gönderme                          |
