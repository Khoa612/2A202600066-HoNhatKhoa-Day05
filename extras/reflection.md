# Góc nhìn: Từ Tư duy Định chuẩn (Deterministic) đến Thất bại Thanh lịch (Graceful Failure)

Bài học lớn nhất tôi rút ra từ Day 5 không nằm ở một framework mới, mà là sự thay đổi hoàn toàn về tư duy phát triển sản phẩm: **"AI không phải là phần mềm thường"**.

Làm quen với việc xây dựng các kiến trúc hệ thống backend và thao tác với cơ sở dữ liệu chặt chẽ, tư duy mặc định của tôi luôn mang tính định chuẩn (deterministic). Một API, một hàm xử lý logic hay một truy vấn database luôn tuân theo quy tắc: 1 là đúng, 0 là sai. Nếu hệ thống trả về sai, đó là một "bug" kỹ thuật cần phải được fix triệt để.

Tuy nhiên, bài học về "Thiết kế cho sự không chắc chắn" (Uncertainty) đã bẻ gãy tư duy đó. AI hoạt động dựa trên xác suất (probabilistic). Việc cố gắng "tối ưu model để đúng 100%" trong mọi trường hợp là một cái bẫy viển vông. AI chắc chắn sẽ sai, vấn đề chỉ là khi nào và sai như thế nào.

Khi thực hành mổ xẻ 4 Paths của MoMo Moni, tôi nhận ra sự thiếu sót lớn nhất của sản phẩm không nằm ở thuật toán phân loại chưa đủ thông minh, mà nằm ở việc thiếu vắng một "lưới an toàn" UX khi thuật toán đó thất bại. Việc hệ thống AI không có một lối thoát hiểm (fallback) về con người, cho thấy một khuyết điểm cần khắc phục của chatbox.

Qua buổi thực hành, tôi nhận ra giá trị thực sự của một AI Product Manager / Engineer không chỉ là làm ra một AI giỏi, mà là thiết kế được sự "Thất bại thanh lịch" (Graceful Failure). Thay vì che giấu điểm yếu của hệ thống, ta cần chủ động thiết kế UI/UX để AI biết cách xin lỗi, biết cách hỏi lại ngữ cảnh, và quan trọng nhất: biến những lần sửa sai của người dùng (Correction Path) thành dữ liệu huấn luyện (Feedback loop) để hệ thống ngày một thông minh hơn.

Thiết kế AI là thiết kế cho những lúc hệ thống không hoàn hảo.