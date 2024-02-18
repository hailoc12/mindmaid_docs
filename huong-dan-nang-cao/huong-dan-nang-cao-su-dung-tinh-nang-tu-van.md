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

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

2. <mark style="color:blue;">Vào phần Huấn luyện Trợ lý ảo, chọn Tab Tài liệu mẫu > Danh sách sản phẩm</mark>

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

3. <mark style="color:blue;">Tải lên file xlxs hoặc link đến file ở bước 1 để huấn luyện</mark>

<figure><img src="../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

4. <mark style="color:blue;">Mô tả nghiệp vụ dữ liệu</mark>

Phần này mô tả ý nghĩa của các cột.&#x20;

Ví dụ:

product\_name: tên của sản phẩm mà công ty ABC đang kinh doanh

selling\_price: giá bán hiện hành của sản phẩm&#x20;

quantity: số lượng sản phẩm còn lại trong kho&#x20;

<figure><img src="../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

5. <mark style="color:blue;">Chọn</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Đào tạo**</mark>
