Khung controller

1. Controller cho User

a. LoginController
- login(username,password): Xử lý yêu cầu đăng nhập.
- register(username, email, password, confirmPassword): Xử lý yêu cầu đăng ký tài khoản mới.

 b. HomeController
-listExams(): Hiển thị danh sách các kỳ thi.
-searchExams(examName,examType): Tìm kiếm và lọc kỳ thi theo tên hoặc loại.

 c.ExamController
- showExam(): Hiển thị câu hỏi và lựa chọn cho mỗi bài thi đã chọn.
- submitExam(): Xử lý nộp bài thi và tính toán kết quả.

d.ResultController
-showResult(username, examName) : Hiển thị chi tiết kết quả bài thi của người dùng

 2. Controller cho Admin

 a. AdminAuthController
- login(username,password): Xử lý yêu cầu đăng nhập cho admin.

 b. DashboardController
- manageExams(): Truy cập và quản lý danh sách các kỳ thi (thêm mới, chỉnh sửa, xóa).
- manageUsers(): Truy cập và quản lý danh sách tài khoản người dùng (thêm mới, chỉnh sửa, xóa tài khoản sinh viên).
-viewStatistics(): xem thống kê về kỳ thi(tỷ lệ hoàn thành, số lượng người dùng, điểm trung bình)

 c. ExamManagementController
- createExam(examName, description, examType): Tạo kỳ thi mới.
- editExam(): Chỉnh sửa thông tin kỳ thi.
- deleteExam(): Xóa kỳ thi.
- importQuestions(): Nhập câu hỏi từ file Excel.

 d. StatisticsController
- showStatistics(): Hiển thị thống kê chung.
- exportReport(): Xuất báo cáo thống kê dưới dạng PDF hoặc Excel.
- filterStatistics(): Lọc thống kê theo kỳ thi, ngày,...

 e. StudentResultsController
- searchStudentResults(): Tìm kiếm và hiển thị kết quả thi của sinh viên cụ thể.
- exportStudentReport(): Xuất báo cáo kết quả của sinh viên ra một file pdf hoặc excel
