# Tạo một kho lưu trữ

| Yêu cầu                     | Sự miêu tả                              |
| --------------------------- | --------------------------------------- |
| `$ git init [project name]` | Từ đầu - Tạo một kho lưu trữ cục bộ mới |
| `$ git clone my_url`        | Tải xuống từ kho lưu trữ hiện có        |

---

# Quan sát một kho lưu trữ

| Yêu cầu                         | Sự miêu tả                                                              |
| ------------------------------- | ----------------------------------------------------------------------- |
| `$ git status`                  | Liệt kê các tập tin mới hoặc sửa đổi chưa được cam kết                  |
| `$ git dif`                     | Hiển thị các thay đổi đối với các tệp chưa được sắp xếp                 |
| `$ git diff --cached`           | Hiển thị các thay đổi đối với các tệp theo giai đoạn                    |
| `$ git diff HEAD`               | Hiển thị tất cả các thay đổi tệp theo giai đoạn và không theo giai đoạn |
| `$ git diff commit1 commit2`    | Hiển thị các thay đổi giữa hai id cam kết                               |
| `$ git blame [file]`            | Liệt kê ngày thay đổi và tác giả của một tập tin                        |
| `$ git show [commit]:[file]`    | Hiển thị các thay đổi tệp cho id và/hoặc tệp cam kết                    |
| `$ git log`                     | Hiển thị toàn bộ lịch sử thay đổi                                       |
| `$ git log -p [file/directory]` | Hiển thị lịch sử thay đổi cho tập tin/thư mục bao gồm các khác biệt     |

---

# Làm việc với các chi nhánh

| Yêu cầu                                          | Sự miêu tả                                               |
| ------------------------------------------------ | -------------------------------------------------------- |
| `$ git branch`                                   | Liệt kê tất cả các chi nhánh địa phương                  |
| `$ git branch -av`                               | Liệt kê tất cả các chi nhánh, địa phương và từ xa        |
| `$ git checkout my_branch`                       | Chuyển sang nhánh my_branch và cập nhật thư mục làm việc |
| `$ git branch new_branch`                        | Tạo một nhánh mới gọi là new_branch                      |
| `$ git branch -d my_branch`                      | Xóa nhánh có tên my_branch                               |
| `$ git checkout branch_b & $ git merge branch_a` | Hợp nhất nhánh_a vào nhánh_b                             |
| `$ git tag my_tag`                               | Gắn thẻ cam kết hiện tại                                 |

---

# Thực hiện thay đổi

| Yêu cầu                             | Sự miêu tả                                                              |
| ----------------------------------- | ----------------------------------------------------------------------- |
| `$ git add [file]`                  | Sắp xếp tập tin, sẵn sàng cho cam kết                                   |
| `$ git add .`                       | Giai đoạn tất cả các tập tin đã thay đổi, sẵn sàng cho cam kết          |
| `$ git commit -m 'commit message'`  | Cam kết tất cả các tệp được dàn dựng với lịch sử được phiên bản         |
| `$ git commit -am 'commit message'` | Cam kết tất cả các tệp được theo dõi của bạn với lịch sử được phiên bản |
| `$ git reset [file]`                | Bỏ tập tin, giữ các thay đổi của tập tin                                |
| `$ git reset --hard`                | Hoàn nguyên mọi thứ về lần xác nhận cuối cùng                           |

---

# Làm cho đồng bộ

| Yêu cầu               | Sự miêu tả                                                     |
| --------------------- | -------------------------------------------------------------- |
| `$ git fetch`         | Nhận những thay đổi mới nhất từ ​​​​nguồn gốc (không hợp nhất) |
| `$ git pull`          | Tìm nạp những thay đổi mới nhất từ ​​​​nguồn gốc và hợp nhất   |
| `$ git pull --rebase` | Tìm nạp những thay đổi mới nhất từ ​​nguồn gốc và rebase       |
| `$ git push`          | Đẩy các thay đổi cục bộ về nguồn gốc                           |
