# DACN
Đồ án chuyên ngành - HK 241 
Hệ thống quản lý phương tiện giao thông vận tải
Plan:

## Tuần 1: Lên ý tưởng và phân tích yêu cầu
- **Thu thập yêu cầu** từ các đối tượng liên quan (người quản lý, nhân viên, khách hàng) để hiểu rõ mong muốn và quy trình làm việc.
- **Phân tích quy trình đăng ký xe** và các bước duyệt phiếu hiện tại.
- **Lập danh sách chức năng chính**:
  - Đăng ký phương tiện.
  - Duyệt hồ sơ đăng ký.
  - Quản lý trạng thái phương tiện.
  - Báo cáo và thống kê.
  - Quản lý người dùng (quản trị viên, nhân viên, khách hàng).
- **Định nghĩa các workflow** liên quan đến duyệt phiếu đăng ký xe, trạng thái hồ sơ và quy trình xử lý.

## Tuần 2: Thiết kế kiến trúc hệ thống
- **Xác định kiến trúc công nghệ**:
  - **Backend**: Sử dụng .NET Core (ASP.NET).
  - **Frontend**: Sử dụng Angular.
  - **Cơ sở dữ liệu**: SQL Server hoặc MongoDB.
- **Thiết kế sơ đồ kiến trúc** tổng quan của hệ thống, gồm các thành phần chính: API, giao diện người dùng (UI), cơ sở dữ liệu (DB).
- **Thiết kế sơ đồ cơ sở dữ liệu**:
  - Bảng thông tin phương tiện.
  - Bảng người dùng (quản trị viên, nhân viên, khách hàng).
  - Bảng quy trình duyệt hồ sơ, trạng thái duyệt.

## Tuần 3: Thiết kế giao diện người dùng (UI/UX)
- **Thiết kế wireframe** cho các màn hình chính:
  - Trang chủ.
  - Trang đăng ký phương tiện.
  - Trang duyệt phiếu đăng ký.
  - Trang quản lý người dùng.
- **Tạo prototype** bằng Figma hoặc Adobe XD để mô phỏng trải nghiệm người dùng (UX) và hình dung cách giao diện hoạt động.
- **Xác định trải nghiệm người dùng** cho quy trình đăng ký và duyệt phiếu sao cho dễ sử dụng và trực quan.

## Tuần 4: Thiết kế workflow động
- **Thiết kế hệ thống workflow động** trong .NET cho quy trình duyệt phiếu, bao gồm các trạng thái như:
  - Tạo mới phiếu.
  - Gửi phiếu chờ duyệt.
  - Duyệt hoặc từ chối phiếu.
  - Hoàn tất quy trình.
- **Xác định các trạng thái** và hành động có thể xảy ra trong mỗi bước của workflow.
- **Lập kế hoạch tích hợp workflow** với hệ thống đăng ký xe và hệ thống người dùng.

## Tuần 5: Cài đặt môi trường phát triển
- **Cài đặt .NET Core** cho backend và các thư viện như Entity Framework cho cơ sở dữ liệu.
- **Cài đặt Angular** và các công cụ frontend cần thiết (Angular CLI, Angular Material).
- **Thiết lập cơ sở dữ liệu** (SQL Server hoặc MongoDB).
- **Thiết lập môi trường phát triển** tích hợp giữa .NET API và Angular frontend.

## Tuần 6: Xây dựng cơ sở dữ liệu
- **Thiết kế bảng dữ liệu** cho các thực thể:
  - Thông tin phương tiện (biển số, loại xe, chủ sở hữu, trạng thái).
  - Thông tin người dùng (quản trị viên, nhân viên, khách hàng).
  - Bảng lưu trữ quy trình duyệt hồ sơ (trạng thái, thời gian, người duyệt).
- **Tạo API RESTful trong .NET** để thực hiện các thao tác CRUD:
  - Tạo mới phương tiện.
  - Cập nhật thông tin phương tiện.
  - Xóa phương tiện.
  - Lấy danh sách phương tiện.

## Tuần 7: Phát triển tính năng đăng ký xe
- **Xây dựng form đăng ký phương tiện** trong Angular với các trường thông tin như: biển số, loại xe, chủ sở hữu.
- **Kết nối form Angular với API .NET** để gửi và lưu trữ dữ liệu đăng ký xe.
- **Xử lý các lỗi người dùng** khi nhập dữ liệu sai và hiển thị thông báo lỗi.

## Tuần 8: Phát triển tính năng duyệt phiếu
- **Xây dựng danh sách phiếu chờ duyệt** trong Angular, hiển thị thông tin cơ bản của từng phiếu đăng ký xe.
- **Tạo các API duyệt, từ chối phiếu** và cập nhật trạng thái phiếu đăng ký.
- **Hiển thị chi tiết phiếu** cho người duyệt xem trước khi phê duyệt hoặc từ chối.

## Tuần 9: Tích hợp workflow động
- **Tích hợp hệ thống workflow động** vào quy trình duyệt phiếu trong .NET.
- **Thiết lập quy trình workflow tùy biến** để cho phép thay đổi hành động dựa trên trạng thái và vai trò người dùng.
- **Cấu hình khả năng linh động** cho các quy trình duyệt, giúp quy trình có thể thay đổi dễ dàng dựa trên yêu cầu thực tế.

## Tuần 10: Quản lý người dùng và phân quyền
- **Tạo hệ thống đăng nhập và xác thực** với .NET Identity Framework.
- **Phân quyền người dùng**: Quản trị viên, nhân viên, khách hàng.
- **Xác định quyền truy cập** cho từng vai trò:
  - Quản trị viên: Quản lý toàn bộ hệ thống.
  - Nhân viên: Duyệt phiếu đăng ký, quản lý thông tin phương tiện.
  - Khách hàng: Đăng ký phương tiện.

## Tuần 11: Phát triển tính năng báo cáo và thông báo
- **Xây dựng trang báo cáo** thống kê trạng thái phương tiện, số lượng phiếu duyệt, tình trạng hồ sơ.
- **Tạo API báo cáo** trong .NET để trích xuất dữ liệu từ cơ sở dữ liệu.
- **Tích hợp hệ thống thông báo** cho người dùng:
  - Thông báo email khi có phiếu mới hoặc khi phiếu được duyệt.
  - Hiển thị thông báo trên giao diện người dùng.

## Tuần 12: Tối ưu hóa hiệu suất
- **Tối ưu hóa truy vấn cơ sở dữ liệu** để giảm thiểu thời gian phản hồi từ server.
- **Tối ưu hóa frontend**:
  - Giảm thiểu kích thước các file JavaScript và CSS trong Angular.
  - Tăng tốc độ tải trang và trải nghiệm người dùng.
- **Giảm độ trễ giao tiếp giữa frontend và backend** qua việc tối ưu hóa API và kết nối.

## Tuần 13: Kiểm thử hệ thống
- **Thực hiện kiểm thử đơn vị (unit test)** cho các API backend .NET và các thành phần frontend Angular.
- **Kiểm thử tích hợp (integration test)** để đảm bảo sự tương tác giữa các thành phần hệ thống hoạt động mượt mà.
- **Kiểm thử giao diện người dùng (UI test)** để đảm bảo trải nghiệm người dùng không có lỗi và mượt mà.

## Tuần 14: Hoàn thiện và chuẩn bị triển khai
- **Kiểm tra toàn bộ hệ thống**, sửa lỗi và hoàn thiện các tính năng.
- **Viết tài liệu hướng dẫn** sử dụng cho người dùng cuối và tài liệu kỹ thuật cho nhà phát triển.
- **Thiết lập môi trường production** trên server (Azure hoặc AWS).
- **Kiểm tra khả năng mở rộng** và bảo mật của hệ thống trước khi triển khai.

## Tuần 15: Triển khai và đánh giá
- **Triển khai hệ thống lên server** thực tế.
- **Theo dõi hoạt động của hệ thống** và thu thập phản hồi từ người dùng.
- **Điều chỉnh hệ thống** nếu cần thiết dựa trên phản hồi.
- **Lập kế hoạch bảo trì** và phát triển thêm tính năng mới trong tương lai.

