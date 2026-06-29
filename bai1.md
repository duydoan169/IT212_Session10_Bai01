## Bài 1: Phân Tích & Lựa Chọn Chiến Lược Tài Liệu Hóa

### Đáp án: Phương án B


### Lý do chọn Phương án B

- Antigravity cho phép index toàn bộ thư mục dự án, giúp AI hiểu toàn bộ ngữ cảnh codebase thay vì từng file rời rạc.
- Prompt được thiết kế đúng chuẩn: giao vai trò rõ ràng (System Analyst), chỉ định endpoint cụ thể, yêu cầu output đúng format SRS (Pre-conditions, Main flow, Exceptions).
- Logic nghiệp vụ trải dài qua Controller, Service, Repository và JWT Filter được AI tự động truy vết liên kết, không cần người dùng tổng hợp thủ công.
- Kết quả đầu ra trực tiếp là tài liệu SRS có cấu trúc, tiết kiệm thời gian và giảm sai sót do diễn giải sai.


### Lý do loại trừ Phương án A

- Copilot Chat chỉ đọc đoạn code được bôi đen tại thời điểm đó, không có khả năng nhìn toàn luồng xử lý xuyên suốt nhiều file.
- Người dùng phải tự tổng hợp kết quả từ nhiều lần giải thích riêng lẻ, dễ bỏ sót mối liên hệ giữa các tầng (ví dụ: logic xác thực JWT ảnh hưởng thế nào đến checkout flow).
- Rủi ro context loss cao: mỗi lần hỏi là một ngữ cảnh độc lập, AI không biết đoạn code trước liên quan gì đến đoạn code sau.


### Lý do loại trừ Phương án C

- Giới hạn cửa sổ ngữ cảnh của ChatGPT/Gemini có thể không đủ để chứa toàn bộ 5 file Java cùng lúc, dẫn đến thông tin bị cắt bớt.
- Copy-paste thủ công dễ bỏ sót file, sai thứ tự, hoặc thiếu các đoạn code quan trọng (ví dụ: filter bảo mật).
- Không có workspace hay index, AI chỉ phân tích đoạn văn bản được dán vào mà không hiểu cấu trúc tổng thể của dự án.
- Phụ thuộc vào kỹ năng chọn lọc file của người dùng, nếu thiếu file nào thì tài liệu SRS sẽ không chính xác.