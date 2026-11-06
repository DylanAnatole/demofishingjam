# Fishing Jam - demo prototype

Bản chơi thử trên trình duyệt (Unity WebGL), dùng nội bộ để trình bày ý tưởng.
Mở trang GitHub Pages của repo này để chơi.

## Ý tưởng game

Game mobile dọc, casual + puzzle: **thả câu để chọn cá, rồi xoay máy câu nối dây và cuộn cá lên.**
Nguyên tắc: đơn giản, ít chữ, người chơi tự hiểu khi chơi.

**1. Thả câu**
- Chạm nước để thả lưỡi, giữ ngón tay để lái lưỡi câu tới con cá cần bắt.
- Mồi chọn đầu màn và đổi được giữa các lần thả: mỗi mồi hút vài loài cá bơi lại gần lưỡi, dễ câu hơn.
- Câu nhầm cá không cần là một lần hụt.

**2. Kéo cá: máy câu xoay (puzzle + hành động)**
- **Nối dây (puzzle):** máy câu có 3 vòng, mỗi vòng mang một đoạn dây. Chạm một vòng để xoay 1 nấc (tốn 1 lượt)
  cho dây nối liền từ con cá vào tâm. Mỗi lần câu có số lượt giới hạn, cá càng khó càng nhiều lượt.
- **Cuộn dây (hành động):** dây thông thì **nhấn giữ tâm** để cuộn (thanh **CÂU** đầy là bắt được cá),
  **thả tay** để nhả dây (thanh **CĂNG** giảm).
- **Nhịp của cá:** cá đuối thì cuộn; cá giằng thì phải thả tay, giữ là dây căng nhanh. Cá khỏe còn giật lệch vòng
  làm đứt mạch dây, phải xoay nối lại.
- **Độ khó tăng dần:** cá 1 sao không giật vòng, cá 2 sao giật nhẹ (cách lần), cá 3 sao trở lên giật mỗi lần giằng,
  cá lao (ngừ, cá mập) giật 2 nấc. Chiêu riêng: mực phun mực che dây, nóc xù gai khóa vòng, cá mập quẫy lệch 2 vòng.

**Thắng/thua**
- Mỗi màn bắt đủ số cá yêu cầu, không giới hạn thời gian.
- Hụt (câu nhầm, đứt dây, hết lượt mà dây chưa thông) 3 lần là thua màn.
- Sao theo số lần hụt: không hụt 3 sao, hụt 1 lần 2 sao, hụt 2 lần 1 sao.

**Luồng chơi (bản hiện tại):** chọn hồ → vào màn. Trang chủ và màn chèo thuyền tạm ẩn chờ art mới.

## Ghi chú: những gì đã làm

- Đổi phần kéo cá từ ghép 3 sang máy câu xoay theo góp ý mentor (core ghép 3 quá phổ biến, bàn chơi nhỏ).
- Thả câu: lái lưỡi câu, chọn mồi, dấu "!" trên cá đang bị mồi hút; mồi chỉ giúp hút cá, cá nào chạm lưỡi cũng cắn.
- Máy câu: 3 vòng xoay nối dây, lượt giới hạn mỗi lần câu, nhấn giữ để cuộn / thả để nhả, thanh CÂU và CĂNG.
- 7 loài cá, độ giật tăng dần theo số sao; cá đầu dễ, cá sau khó.
- Hướng dẫn lần đầu (màn 1): bàn tay chỉ cá cần bắt; con cá đầu không giằng, bàn tay chỉ vòng cần xoay ("Chạm để xoay")
  và giữ tâm ("Giữ tâm để cuộn"); lần cá giằng đầu tiên dạy "Thả tay để nhả dây".
- Bỏ đồng hồ màn chơi; thua khi hụt 3 lần; sao theo số lần hụt.
- Bản demo mở sẵn cả 10 màn để trình bày; nút "Chơi lại từ đầu" để xem lại hướng dẫn.
- Thẻ chọn màn hiện hình các loài cá cần bắt.
- Âm thanh tự tạo (xoay vòng, nối dây, cuộn, cắn câu, bắt cá, đứt dây, thắng/thua) và nút tắt/bật âm thanh.
- Hiệu ứng: máy câu rung khi cá giằng, cá nhảy vọt khi bắt được, pháo giấy và sao nảy khi qua màn.
- Bản HTML (WebGL) tự co theo tỉ lệ 9:16, chơi được trên máy tính và điện thoại.

Hình ảnh trong bản demo chỉ để trình bày nội bộ, sẽ thay bằng art riêng trước khi phát hành.
