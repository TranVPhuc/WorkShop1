---
title : "Cấu trúc Web Server"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2.2.</b> "
---

### Cấu trúc Web Server
Trong Amazon Web Services (AWS), bạn có thể triển khai một cấu trúc web server bằng nhiều cách, tùy thuộc vào nhu cầu cụ thể của bạn và các dịch vụ AWS mà bạn muốn sử dụng. Dưới đây là  một cấu trúc web server cơ bản trên AWS:
![ws-structure](/images/2.2-ws-structure/simplewsstructure.png?featherlight=false&width=55pc)
Cấu trúc của một web server có thể được phân thành các thành phần cơ bản sau:
1. **EC2 (Elastic Compute Cloud)**:
> * Là thành phần cốt lõi, chịu trách nhiệm xử lý yêu cầu và gửi trả kết quả cho người dùng.
> * Có thể lựa chọn cấu hình phù hợp với nhu cầu về CPU, RAM, dung lượng lưu trữ,...
> * Hệ điều hành phổ biến: Amazon Linux 2, Ubuntu Server, Windows Server.
> * Cấu hình tường lửa để cho phép kết nối HTTP (port 80) và HTTPS (port 443) vào instance.

2. **RDS (Relational Database Service)**:
> * Nếu ứng dụng web của bạn cần cơ sở dữ liệu, bạn có thể sử dụng RDS để triển khai cơ sở dữ liệu quan hệ như MySQL, PostgreSQL, hoặc SQL Server.
> * RDS cung cấp các tính năng như sao lưu tự động, mở rộng dựa trên nhu cầu, và bảo mật dữ liệu.

3. **IAM (Identity and Access Management**):

> * Quản lý quyền truy cập vào các tài nguyên AWS bằng cách sử dụng IAM để đảm bảo rằng chỉ có người dùng được ủy quyền mới có thể truy cập vào các tài nguyên của bạn.

4. **Auto Scaling và Elastic Load Balancing**:

> * Sử dụng Auto Scaling để tự động điều chỉnh số lượng các instance EC2 dựa trên yêu cầu của ứng dụng.
> * Sử dụng Elastic Load Balancing để phân phối lưu lượng truy cập giữa các instance EC2 và tăng khả năng chịu tải của ứng dụng.
