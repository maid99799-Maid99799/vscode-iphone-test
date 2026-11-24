# vscode-iphone-test

Môi trường lập trình VS Code trên iPhone, chi phí 0 đồng — dùng GitHub Codespaces (gói Free).

## Máy đã kiểm chứng (25/11/2026)

- Codespace: probable trout, máy 2-core • 8 GB RAM • 32 GB, region Southeast Asia.
- Python 3.12.1, Node.js v22.15.0, npm 9.8.1, Git 2.49.0.
- Lần chạy thử 12 phút tốn 0,3 giờ máy 2-core = $0,05, được trừ hết bằng hạn mức miễn phí nên billable $0.
- Hạn mức Free: 120 core-hours/tháng và 15 GB-month lưu trữ/tháng.

## 1. Mở codespace trên Safari (iPhone)

1. Mở Safari, vào https://github.com/codespaces
2. Nhấn vào codespace probable trout để mở VS Code trên trình duyệt.
3. Lần đầu mở sau khi tạo mới có thể mất khoảng 10 phút để build; các lần mở lại sau đó nhanh hơn.
4. Nếu VS Code hỏi, nhấn "Tin tưởng thư mục và tiếp tục".

## 2. Dùng bàn phím ảo

- Nhấn vào vùng soạn thảo hoặc Terminal để hiện bàn phím.
- Mở Terminal: nhấn biểu tượng menu, chọn Terminal > New Terminal.
- Xoay ngang iPhone để có màn hình rộng hơn khi gõ code.
- Các ký tự đặc biệt (`, $, ", ', ;, |) nằm ở bàn phím số/ký hiệu: nhấn phím 123 rồi #+= trên bàn phím iPhone.

## 3. Chạy Python / Node

Trong Terminal (thư mục /workspaces/vscode-iphone-test):

```
python3 --version
node --version
python3 hello.py
node hello.js
```

## 4. Xong việc: commit + push + stop

```
git status
git add .
git commit -m "Mo ta ngan gon ve thay doi"
git push
```

Sau đó STOP codespace ngay, không để chạy: vào https://github.com/codespaces, nhấn "..." ở codespace rồi chọn Stop codespace.

## 5. Quy tắc tiết kiệm quota (quan trọng)

- Chỉ giữ đúng 1 codespace duy nhất (probable trout), không tạo thêm.
- Luôn chọn máy 2-core, loại rẻ nhất ($0,18/giờ).
- Luôn stop codespace sau khi xong việc — đừng chỉ đóng Safari.
- Idle timeout mặc định là 240 phút (4 giờ), nên đừng trông chờ máy tự tắt.
- Codespace đã dừng sẽ tự bị xóa sau 30 ngày không dùng; code đã push lên repo thì vẫn còn.
- Kiểm tra mức dùng tại https://github.com/settings/billing (mục Codespaces).
