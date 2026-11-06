# Fishing Jam - demo prototype

Bản chơi thử trên trình duyệt (Unity WebGL), dùng nội bộ để trình bày ý tưởng.
Chơi tại: https://dylananatole.github.io/demofishingjam/

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

## Ghi chú

Hình ảnh trong bản demo chỉ để trình bày nội bộ, sẽ thay bằng art riêng trước khi phát hành.
