# [Python_Guide_001] Cài Đặt Virtual Environment (Môi Trường Ảo) Trong VSCode
Cài đặt môi trường ảo trong VSCode.

# TÊN của thư mục ảo nên có dấu chấm '.' phía trước
Ví dụ: .env, .venv, .Python3_Env, ...

## Tạo thư mục ảo với Visual Studio Code (VSCode)
Tại thư mục dự án có tên **Project_X** > Nhấn chuột phải và chọn "**Open in Integrated Terminal**"

![image](https://github.com/user-attachments/assets/79cc8b73-6edb-45c6-bc24-ff64df4b6b16)

> **Bước 1:** Tạo môi trường ảo **.venv** bên trong thư mục **Project_X**:
```bash
python -m venv .venv --prompt="Python3_Env"
```

![image](https://github.com/user-attachments/assets/bc98525a-4941-4878-9638-0fcbb15be13d)

- Chọn "**Yes**"

![image](https://github.com/user-attachments/assets/b2ba48a2-8450-4562-be6f-a777ba6b03fc)

- Tại thư mục **Project_X** sẽ có thêm thư mục **.venv** (Môi trường ảo được đặt tên ở trên)

![image](https://github.com/user-attachments/assets/a8416fd0-894d-49b9-a42c-01183a6573c6)

> **Bước 2:** Kích hoạt môi trường ảo:

_1. Khởi chạy VSCode bằng quyền **Administrator**_

![image](https://github.com/user-attachments/assets/e75f643f-0128-4c57-b1d7-8f8f134eb328)

- Tại thư mục dự án có tên **Project_X** > Nhấn chuột phải và chọn "**Open in Integrated Terminal**"

![image](https://github.com/user-attachments/assets/79cc8b73-6edb-45c6-bc24-ff64df4b6b16)

- Khởi chạy môi trường ảo **.venv**
```bash
.venv\Scripts\activate
```

![image](https://github.com/user-attachments/assets/522d06ac-5bf4-4e65-b750-b19e8c8ad979)

> **=> Thành công** (Hiện tên môi trường phía trước đường dẫn của thư mục).

_2. **KHÔNG** khởi chạy VSCode bằng quyền **Administrator**, thì khi chạy lệnh **.venv\Scripts\activate** => **Lỗi (Error)**_

_Phải chạy trước lệnh bên dưới để thiết lập **Execution Policy**_
```bash
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned -Force
```
> **=> Tiếp tục chạy lại từ mục 1.**
