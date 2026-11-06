# Fishing Jam - demo prototype

Bản chơi thử trên trình duyệt (Unity WebGL), dùng nội bộ để trình bày ý tưởng.
Mở trang GitHub Pages của repo này để chơi.

## Ý tưởng game

Game mobile dọc, casual + puzzle: **thả câu để chọn cá, rồi ghép 3 để kéo cá lên.**
Nguyên tắc: đơn giản, ít chữ, người chơi tự hiểu khi chơi.

**1. Thả câu (~25% thời gian chơi)**
- Chạm nước để thả lưỡi, giữ ngón tay để lái lưỡi câu tới con cá cần bắt.
- Mồi chọn đầu màn và đổi được giữa các lần thả: mỗi mồi hút vài loài cá bơi lại gần lưỡi, dễ câu hơn.
- Câu nhầm cá không cần thì bị trừ thời gian.

**2. Kéo cá (~75%)**: bàn ghép 3 kiểu 7×7, vuốt hoặc chạm để đổi ô
- Hai thanh đứng cạnh nhau: **GIỮ** (dây, tụt dần, hết thì đứt dây) và **CÂU** (đầy thì bắt được cá).
- 5 ô hành động: Giật cần, Thu dây, Nới dây, Ghìm cần, Vợt (chỉ dùng được khi CÂU ≥ 70%).
- Ghép 4 ra ô sọc, ghép chữ L/T ra bom, ghép 5 ra ngôi sao. Ăn dây chuyền thì nhân điểm CÂU.
- Cá có nhịp giằng/đuối, cá khỏe thì lao giật dây. Một số loài có chiêu: mực phun mực, nóc xù gai, cá mập ném rong.
- Cả màn dùng chung một bàn ghép, ô đặc biệt để dành được sang con cá sau.

**Thắng/thua**
- Mỗi màn bắt đủ số cá yêu cầu trước khi hết giờ. Hết giờ là thua duy nhất.
- Câu nhầm cá hoặc đứt dây: trừ 10 giây.
- 3 sao: 2 sao theo thời gian còn lại, 1 sao cho nhiệm vụ phụ (không trượt / tạo ô đặc biệt / dây chuyền).

**Luồng chơi:** Trang chủ (thuyền cạnh nhà sàn) → chèo thuyền (loading) → chọn hồ → chèo thuyền → vào màn.

## Ghi chú: những gì đã làm

- Luồng chơi: trang chủ → chèo thuyền (loading) → chọn hồ → chèo thuyền → vào màn.
- Thả câu: chạm nước để thả, giữ ngón tay lái lưỡi câu; chọn mồi đầu màn, đổi được giữa các lần thả.
- Kéo cá: bàn ghép 3 kiểu 7×7, vuốt hoặc chạm để đổi ô; hai thanh GIỮ và CÂU đặt cạnh nhau.
- 5 ô hành động (Giật cần, Thu dây, Nới dây, Ghìm cần, Vợt) và ô đặc biệt: sọc (ghép 4), bom (L/T), ngôi sao (ghép 5).
- Mồi chỉ giúp hút cá lại gần, cá nào chạm lưỡi câu cũng cắn.
- Combo dây chuyền, gợi ý nước đi khi đứng yên (3 giây ở màn 1–2, 5 giây các màn sau), hiệu ứng trượt/rơi/nổ ô.
- 7 loài cá với nhịp giằng/đuối; cá khỏe lao giật dây; chiêu riêng: mực phun mực, nóc xù gai, cá mập ném rong.
- Bản demo mở sẵn cả 10 màn để trình bày (chọn thẳng màn boss được).
- 10 màn chơi kèm mẹo, nhiệm vụ phụ, 3 sao, xu và mua thêm 20 giây.
- Hướng dẫn lần đầu: bàn tay chỉ con cá cần bắt khi thả câu, và kéo mẫu hai ô cần đổi ở lần ghép đầu.
- Giao diện: HUD xanh navy, nút bóng, bảng thông báo bật nảy, ô ghép bóng, bàn cờ xanh, thanh dạng ống, bảng thắng có sao nảy.
- Âm thanh tự tạo cho thả câu, cắn câu, đổi ô, nổ ô (cao dần theo combo), ô đặc biệt, bắt cá, đứt dây, thắng/thua.
- Khoảnh khắc bắt cá: cá nhảy vọt lên, xoay vòng, chữ "BẮT ĐƯỢC!".
- Cân bằng độ khó bằng công cụ mô phỏng trong Unity (tính cả việc câu nhầm khi hồ nhiều cá không cần bắt).
- Bản HTML (WebGL) tự co theo tỉ lệ 9:16, chơi được trên máy tính và điện thoại.

Hình ảnh trong bản demo chỉ để trình bày nội bộ, sẽ thay bằng art riêng trước khi phát hành.
