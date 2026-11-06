# Fishing Jam - demo prototype

Bản chơi thử trên trình duyệt (Unity WebGL), dùng nội bộ để trình bày ý tưởng.
Mở trang GitHub Pages của repo này để chơi.

## Ý tưởng game

Fishing Jam là game câu cá kết hợp ghép 3, chơi dọc trên điện thoại. Người chơi chạm nước để thả câu và lái lưỡi câu tới con cá cần bắt, mồi giúp hút cá lại gần cho dễ câu. Khi cá cắn câu, người chơi đổi ô để ghép 3. Mỗi lần ghép vừa kéo cá lại gần vừa phải giữ cho dây không đứt, ghép 4–5 ô sẽ tạo ra ô đặc biệt mạnh hơn. Mục tiêu là bắt đủ số cá trước khi hết giờ, câu nhầm cá hoặc để đứt dây sẽ bị trừ thời gian.

## Ghi chú: những gì đã làm

- Luồng chơi: trang chủ → chèo thuyền (loading) → chọn hồ → chèo thuyền → vào màn.
- Thả câu: chạm nước để thả, giữ ngón tay lái lưỡi câu; chọn mồi đầu màn, đổi được giữa các lần thả.
- Kéo cá: bàn ghép 3 kiểu 7×7, vuốt hoặc chạm để đổi ô; hai thanh GIỮ và CÂU đặt cạnh nhau.
- 5 ô hành động (Giật cần, Thu dây, Nới dây, Ghìm cần, Vợt) và ô đặc biệt: sọc (ghép 4), bom (L/T), ngôi sao (ghép 5).
- Combo dây chuyền, gợi ý nước đi khi đứng yên 5 giây, hiệu ứng trượt/rơi/nổ ô.
- 7 loài cá với nhịp giằng/đuối; cá khỏe lao giật dây; chiêu riêng: mực phun mực, nóc xù gai, cá mập ném rong.
- 10 màn chơi kèm mẹo, nhiệm vụ phụ, 3 sao, xu và mua thêm 20 giây.
- Cân bằng độ khó bằng công cụ mô phỏng trong Unity.
- Bản HTML (WebGL) tự co theo tỉ lệ 9:16, chơi được trên máy tính và điện thoại.

Đã làm trong Unity, chưa có trên bản web:
- Mồi chỉ giúp hút cá, cá nào chạm lưỡi câu cũng cắn.
- Hình cá mới.
- Giao diện màn kéo cá mới: ô bóng, bàn cờ xanh, thanh dạng ống, màu ô tươi hơn.

Hình ảnh trong bản demo chỉ để trình bày nội bộ, sẽ thay bằng art riêng trước khi phát hành.
