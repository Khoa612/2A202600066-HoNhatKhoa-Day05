# UX exercise — MoMo Moni AI

**Họ và tên:** Hồ Nhất Khoa  
**MSSV:** 2A 2026 00066  

## Sản phẩm: MoMo — Moni AI Assistant (phân loại chi tiêu)

## Khám phá (Marketing vs. Thực tế)
- **Marketing:** MoMo định vị Moni là một "trợ lý tài chính cá nhân" với khả năng phân tích dòng tiền, phân loại chi tiêu thông minh bằng AI, và cá nhân hóa như một người bạn thực thụ.
- **Thực tế:** Trải nghiệm cho thấy sản phẩm thực tế cơ bản làm được như những gì PR/Marketing đã hứa hẹn.

## Phân tích 4 paths

### 1. Khi AI đúng
- User thấy AI phản hồi chính xác.
- UI/Hệ thống: Có thêm các minh chứng thành công như hiển thị dấu tick xác nhận và đưa ra những câu trả lời/đánh giá chung mượt mà.

### 2. Khi AI không chắc
- Hệ thống sẽ đưa ra các câu hỏi thêm để thu thập thông tin.
- AI chủ động hỏi user muốn làm gì tiếp theo và cần hỗ trợ chỉnh sửa gì không.

### 3. Khi AI sai
- Hệ thống biết cách xin lỗi.
- AI chủ động hỏi người dùng có muốn hệ thống kiểm tra lại thông tin hay không.

### 4. Khi user mất niềm tin
- Khi người dùng không tin AI và báo AI đã sai, AI sẽ không ngừng kiểm tra lại và lặp lại câu trả lời cũ.
- Khi người dùng liên tục báo sai, AI cứ tiếp tục kiểm tra lại một cách máy móc.
- **Vấn đề:** Không có cơ chế fallback (chuyển tiếp) về người thật để giải quyết triệt để.

## Đánh giá Path tốt nhất & yếu nhất

- **Path xử lý tốt nhất: Path 2 (Khi AI không chắc).**
  - Khi dữ liệu đầu vào thiếu, AI vẫn có thể trả lời tổng quát, đồng thời hỏi thêm thông tin xem người dùng có cần giúp đỡ gì không. UX ở điểm này rất tốt, mang lại cảm giác đây là một trợ lý thông minh thực sự.

- **Path yếu nhất: Path 4 (Khi user mất niềm tin).**
  - AI không biết làm gì ngoài việc tự đọc lại thông tin và trả lời lặp lại lần nữa, cho dù người dùng đã trực tiếp nói là AI sai.
  - Ngoài ra, không có tính năng fallback chuyển sang người thật. Khi người dùng yêu cầu được nói chuyện với nhân viên hỗ trợ (con người), AI chỉ trả lời là không thể hỗ trợ.

## Sketch 
Kham khảo file sketch.pdf