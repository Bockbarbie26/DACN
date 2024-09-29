# DACN
Đồ án chuyên ngành - HK 241 
Plan:
# Kế hoạch 15 tuần cho dự án quản lý phương tiện giao thông vận tải
## Tuần 1: Lên ý tưởng và phân tích yêu cầu
- Thu thập yêu cầu từ người dùng.
- Phân tích quy trình đăng ký xe và các workflow liên quan.
- Lập danh sách chức năng chính: đăng ký xe, duyệt hồ sơ, quản lý phương tiện, báo cáo, quản lý người dùng.

## Tuần 2: Thiết kế kiến trúc hệ thống
- Chọn công nghệ: .NET Core cho backend, Angular cho frontend, SQL Server/MongoDB cho cơ sở dữ liệu.
- Thiết kế sơ đồ kiến trúc hệ thống.
- Thiết kế sơ đồ cơ sở dữ liệu.

## Tuần 3: Thiết kế UI/UX
- Thiết kế wireframe và prototype cho các màn hình chính.
- Xác định trải nghiệm người dùng.
- Sử dụng Figma hoặc Adobe XD để thiết kế giao diện.

## Tuần 4: Thiết kế workflow động
- Thiết kế cơ chế workflow động cho quy trình duyệt phiếu trong .NET.
- Xác định các trạng thái và hành động trong quy trình.
- Lập kế hoạch tích hợp workflow với hệ thống đăng ký xe.

## Tuần 5: Cài đặt môi trường phát triển
- Cài đặt môi trường phát triển backend (.NET Core, Entity Framework).
- Cài đặt môi trường phát triển frontend (Angular, Angular Material).
- Thiết lập kết nối cơ sở dữ liệu (SQL Server hoặc MongoDB).

## Tuần 6: Xây dựng cơ sở dữ liệu
- Thiết kế và triển khai cơ sở dữ liệu cho các thực thể (phương tiện, người dùng, quy trình).
- Tạo API RESTful trong .NET để xử lý CRUD.

## Tuần 7: Phát triển tính năng đăng ký xe
- Xây dựng form đăng ký xe bằng Angular.
- Kết nối form với API .NET để lưu trữ và quản lý dữ liệu đăng ký xe.

## Tuần 8: Phát triển tính năng duyệt phiếu
- Xây dựng danh sách phiếu chờ duyệt bằng Angular.
- Tạo các API duyệt, từ chối hoặc yêu cầu bổ sung thông tin.

## Tuần 9: Tích hợp workflow động
- Tích hợp workflow động vào quy trình duyệt phiếu với .NET.
- Thiết lập khả năng cấu hình quy trình dựa trên trạng thái và vai trò người dùng.

## Tuần 10: Quản lý người dùng và phân quyền
- Tạo hệ thống đăng nhập, xác thực và phân quyền với Identity Framework của .NET.
- Quy định quyền truy cập (admin, nhân viên, khách hàng).

## Tuần 11: Phát triển tính năng báo cáo và thông báo
- Xây dựng tính năng báo cáo trạng thái phương tiện, hồ sơ đăng ký.
- Tích hợp hệ thống thông báo (email hoặc notifications).

## Tuần 12: Tối ưu hóa hiệu suất
- Tối ưu hóa các truy vấn cơ sở dữ liệu.
- Cải thiện tốc độ tải trang trong Angular và giảm thiểu độ trễ khi giao tiếp với API.

## Tuần 13: Kiểm thử hệ thống
- Thực hiện kiểm thử đơn vị (unit test) và kiểm thử tích hợp (integration test).
- Kiểm thử giao diện người dùng và sửa lỗi phát sinh.

## Tuần 14: Hoàn thiện và chuẩn bị triển khai
- Đảm bảo toàn bộ tính năng hoạt động mượt mà.
- Viết tài liệu hướng dẫn sử dụng và tài liệu kỹ thuật.
- Cài đặt môi trường production.

## Tuần 15: Triển khai và đánh giá
- Triển khai hệ thống lên server (Azure hoặc AWS).
- Thu thập phản hồi từ người dùng.
- Điều chỉnh hệ thống và lên kế hoạch bảo trì.
