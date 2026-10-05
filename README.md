# Bài 3 - Xử lý xung đột khi Rebase

## Conflict lần 1

Commit `feat: change API port` xung đột với thay đổi port trên
nhánh main. Tôi giữ port 9000 của feature, đồng thời giữ cấu hình
debug và env production của main.

Sau khi sửa marker conflict, tôi chạy:

```bash
git add config.json
git rebase --continue
