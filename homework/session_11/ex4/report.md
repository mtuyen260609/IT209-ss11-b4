# Báo cáo Bài 4: GitHub Secrets và GHCR

## 1. Mục tiêu
Lưu Personal Access Token trong GitHub Repository Secrets và cấu hình đăng nhập GHCR tự động.

## 2. Cấu hình
- Repository Secret: REGISTRY_TOKEN
- Registry: ghcr.io
- Action: docker/login-action@v3
- Token được tham chiếu qua secrets.REGISTRY_TOKEN.

## 3. Kiểm tra
Cập nhật kết quả sau khi chạy GitHub Actions và xác nhận bước đăng nhập thành công.

## 4. Minh chứng
- Ảnh Repository Secret REGISTRY_TOKEN.
- Ảnh log bước đăng nhập GHCR hiển thị Login Succeeded.
