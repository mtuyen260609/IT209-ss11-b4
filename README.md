# IT209 - Session 11: CI/CD Pipeline & GitHub Container Registry

## Bài 4: Khai báo GitHub Secrets và cấu hình Đăng nhập Container Registry

Bài nộp được đặt tại: [homework/session_11/ex4/](homework/session_11/ex4/)

### Danh mục nộp bài:
- Tệp kịch bản GitHub Actions: [`.github/workflows/ci.yml`](.github/workflows/ci.yml) (và bản sao [`homework/session_11/ex4/ci.yml`](homework/session_11/ex4/ci.yml))
- Ảnh minh chứng Repository Secrets `REGISTRY_TOKEN`: [`homework/session_11/ex4/screenshot_secret.png`](homework/session_11/ex4/screenshot_secret.png)
- Báo cáo kỹ thuật chi tiết: [`homework/session_11/ex4/README.md`](homework/session_11/ex4/README.md)

### Tóm tắt các bước thực hiện:
1. Tạo Personal Access Token (classic) với quyền `write:packages` trên GitHub.
2. Thêm Repository Secret mang tên `REGISTRY_TOKEN` trong **Settings -> Secrets and variables -> Actions**.
3. Cấu hình bước đăng nhập `docker/login-action@v3` trong `.github/workflows/ci.yml` sử dụng `${{ secrets.REGISTRY_TOKEN }}`.
4. Kiểm tra tab **Actions** trên GitHub xác nhận log `Login Succeeded`.
