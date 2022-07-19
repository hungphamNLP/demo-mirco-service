mô hình micro service 

1. Mỗi microservice nên có một database riêng biệt
Cơ sở dữ liệu cho mỗi dịch vụ
Để giải quyết các vấn đề trên, một cơ sở dữ liệu cho mỗi microservice phải được thiết kế; nó phải là riêng tư đối với dịch vụ đó. Nó chỉ được truy cập bằng API microservice. Nó không thể được truy cập trực tiếp bởi các dịch vụ khác. Ví dụ, đối với cơ sở dữ liệu quan hệ, chúng ta có thể sử dụng private-table-per-service, schema-per-service hoặc database-server-per-service.

Cơ sở dữ liệu được chia sẻ trên mỗi dịch vụ
Chúng tôi đã nói về một cơ sở dữ liệu cho mỗi dịch vụ là lý tưởng cho các dịch vụ nhỏ. Nó là một mô hình chống cho microservices. Nếu ứng dụng là một khối nguyên khối và cố gắng xâm nhập vào các microservices, việc chuẩn hóa không phải là điều dễ dàng. Cơ sở dữ liệu dùng chung cho mỗi dịch vụ không phải là lý tưởng, nhưng đó là giải pháp hiệu quả. Hầu hết mọi người coi đây là một mô hình chống đối với microservices, nhưng đối với các ứng dụng brownfield, đây là một khởi đầu tốt để chia ứng dụng thành các phần nhỏ hợp lý hơn. Điều này không nên được áp dụng cho các ứng dụng greenfield.

2. Cách thức giao tiếp giữa các micro-service


*Mỗi service phải đăng ký 
*discover service là phần 

    
    
    
   
   
# demo-mirco-service
