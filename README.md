# JR Companion cho Anki Vector

**JR Automation** · Triển khai bởi **Tuan Cong Jr**

JR Companion là bản nâng cấp phần mềm cho robot **Anki Vector 1.0** chạy WireOS: nói chuyện tiếng Việt với AI, làm bạn đồng hành trong nhà, bật tắt đèn bằng giọng nói và quản lý robot qua trang web ngay trong mạng nhà.

> Repo này chỉ chứa **giới thiệu chức năng** và **bản cập nhật nhanh** (mục Releases). Mã nguồn không công khai.

## Chức năng chính

| Nhóm | Robot làm được |
|---|---|
| Trợ lý giọng nói | Gọi "Hey Vector" rồi nói chuyện tiếng Việt / tiếng Anh. Chọn trợ lý: Xiaozhi, Gemini Live, OpenAI Realtime, Grok Voice, AI tự chọn, hoặc Vosk chạy offline. |
| Hành vi gốc bằng tiếng Việt | Xem giờ, thời tiết, hẹn giờ, báo thức, lại đây, về sạc, nhảy, hát, chơi với khối lập phương, nhận ra người quen. |
| Bạn đồng hành | Chào theo giờ khi thấy người quen, đoán cảm xúc qua camera để hỏi han, nhắc đứng dậy khi ngồi lâu, chúc mừng sinh nhật. |
| Trí nhớ từng người | Nhớ điều mỗi người kể (sở thích, lịch hẹn, ngày sinh) và nhắc lại khi được hỏi. |
| Làm việc (Pomodoro) | Mặt robot thành đồng hồ đếm ngược 25/5 phút, nhắc nghỉ, nghỉ dài sau 4 phiên. |
| Trông nhà | Thấy người lạ hoặc chuyển động thì chụp ảnh gửi về Gmail. |
| Nhà thông minh | Bật tắt đèn, ổ cắm, quạt bằng giọng nói hoặc trên web; chạy cảnh ("chế độ đi ngủ"). Hỗ trợ Tasmota, Shelly, ESPHome, Sonoff DIY, Home Assistant, MQTT, link HTTP tự nhập. |
| Hoạt cảnh vui | Xe cứu hỏa, xe cảnh sát, xe cứu thương, máy bay, tàu hoả, tàu siêu tốc, màn sinh nhật có bánh kem, pháo hoa năm mới. |
| Trò chơi | 14 trò bằng giọng nói trên mặt robot (đoán số, đố vui, caro, sudoku, 2048, wordle…) và cờ vua, cờ tướng, caro, cờ vây, uno, xì dách trên web. |
| Trang web robot | Cài Wi‑Fi, âm lượng, màu mắt, từ đánh thức; lái robot và xem camera; điều khiển từ 4G qua link bảo mật; xem nhật ký. |
| Cập nhật nhanh | Dán link bản mới vào web robot là cập nhật, khoảng 1 phút, không mất cài đặt, lỗi thì tự quay về bản cũ. |

## Lệnh giọng nói cơ bản

Nói **"Hey Vector"** trước, rồi nói một trong các câu sau.

| Muốn | Ví dụ câu nói |
|---|---|
| Giờ, thời tiết | "mấy giờ rồi", "thời tiết thế nào", "ngày mai có mưa không" |
| Hẹn giờ, báo thức | "hẹn giờ 5 phút", "tắt hẹn giờ", "đặt báo thức 6 giờ sáng", "tắt chuông" |
| Di chuyển | "lại đây", "về sạc", "nhìn tôi", "quay vòng", "đi ngủ", "im lặng", "đập tay" |
| Nhảy, hát | "nhảy đi", "hát cho tôi nghe" |
| Khối lập phương | "lấy khối lập phương", "lăn khối", "mang khối lại đây" |
| Hoạt cảnh | "làm xe cứu hỏa đi", "làm máy bay cho xem", "làm tàu hoả đi", "làm tàu siêu tốc" |
| Sinh nhật | "hôm nay là sinh nhật của tôi", "chúc mừng sinh nhật của bạn" |
| Nhìn, nhận người | "đây là cái gì", "tôi là ai", "nhớ mặt tôi, tôi tên là …" |
| Trí nhớ | "nhớ giúp tôi …", "sinh nhật tôi ngày 20/11", "bạn nhớ gì về tôi?", "quên … đi" |
| Làm việc | "bắt đầu làm việc", "tập trung 45 phút", "dừng làm việc" |
| Trông nhà | "trông nhà giúp tôi", "tắt trông nhà" |
| Nhà thông minh | "bật đèn phòng ngủ", "tắt đèn học", "tắt hết đèn", "bật chế độ đi ngủ" |
| Trò chơi | "chơi đoán số", "chơi đố vui", "chơi cờ caro", "chơi lại", "dừng chơi" |
| Năm mới | "chúc mừng năm mới", "bắn pháo hoa" |

Câu nói chuyện bình thường (hỏi đáp, kể chuyện, dịch, học bài…) thì trợ lý AI trả lời.

## Cập nhật nhanh

Dành cho robot đã cài JR Companion bản OTA tương ứng (gói 27.x cần OTA v27).

1. Mở mục **Releases** của repo này, chuột phải vào file `jr-companion-<phiên bản>.jrup` › **Sao chép địa chỉ liên kết**.
2. Mở trang web robot › tab **Cập nhật OS** › thẻ **⚡ Cập nhật nhanh JR** › dán link › **⚡ Cập nhật nhanh**.
3. Chờ khoảng 1 phút, trang tự tải lại. Hoặc bấm **🔍 Kiểm tra bản mới** để robot tự tìm bản mới nhất.

Bản mới bị lỗi thì robot tự quay về bản trước; cũng có nút **↩️ Quay lại bản trước** trong cùng thẻ.

## Liên hệ

Cài đặt JR Companion, sửa chữa robot Vector, hỗ trợ kỹ thuật: **JR Automation – Tuan Cong Jr** (GitHub [@tuancongjr10](https://github.com/tuancongjr10)).
