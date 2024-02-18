# Hướng dẫn nâng cao - Sử dụng tính năng tư vấn

## A. Giới thiệu

Tính năng tư vấn là tính năng cho phép chatbot Mindmaid có thể chủ động giới thiệu sản phẩm phù hợp cho khách hàng. Ví dụ:Kịch bản 1:

* Khách: shop có bán sản phẩm X không?
* Chatbot: có ạ, đây là thông tin về sản phẩm X
* Khách: cho xin giá của sản phẩm này
* Chatbot: giá của sản phẩm này là YYY đồng

\
Kịch bản 2:

* Khách: tư vấn cho tôi rượu vang ngọt có giá dưới 2 triệu đồng
* Chatbot: dưới đây là một số dòng sản phẩm có giá dưới 2 triệu đồng
* Khách: cho xin giá của chai Bordeaux
* Chatbot: giá của sản phẩm này là YYY đồng

## B. Động lực

* Tính năng này cho phép chatbot Mindmaid không chỉ dùng để CSKH mà còn để tư vấn sản phẩm, một bước quan trọng trong hành trình bán hàng --> Giá trị của Mindmaid tăng lên. Khách cũng dễ chi tiền hơn vì đây là đầu tư cho bán hàng.

<figure><img src="https://aivgroupworking.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=OTVlNzhhMzU3Y2M0NTA3YzgzMWQwZmE5ZDdlODBiNTlfQ25sY2dsYmVlNWtteWlZNWdaUUxQbGFXOFIxaFdpRklfVG9rZW46WklmTWJQb3l4b054SDN4SUtCVWxlR1p3Z3poXzE3MDgyNjA3OTU6MTcwODI2NDM5NV9WNA" alt=""><figcaption></figcaption></figure>

* Các đơn vị bán lẻ có số lượng sản phẩm rất lớn (vd: xe máy, hàng tạp hóa, sách truyện...), do đó nhân sự con người khó có thể tư vấn hiệu quả. Chatbot có thể tư vấn được + gửi hình ảnh & video sẽ mang lại hiệu quả rất lớn



## C. Cách cài đặt

1. <mark style="color:blue;">**Chuẩn bị dữ liệu database để huấn luyện**</mark>

Vui lòng xem chi tiết tại sheet **4. Danh sách sản phẩm** của file sau: [https://docs.google.com/spreadsheets/d/1336NI827chjFkU1-C-p7luALIYwdonOAvEP3HXT76vQ/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1336NI827chjFkU1-C-p7luALIYwdonOAvEP3HXT76vQ/edit?usp=sharing)

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>



4. Danh sách sản phẩm
5. Tạo hoặc chọn vào bot mindmaid
6. Chọn vào "Huấn luyện trợ lý ảo"
7. Chọn vào data cần huấn luyện
8. Chọn vào tab "Tài liệu mẫu" (Dữ liệu mẫu có thể lấy ở đây)
9. Tải lên file xlsx hoặc đường dẫn đến file để huấn luyện
10. Huấn luyện
11. Dùng thử
