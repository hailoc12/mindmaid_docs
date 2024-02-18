# Hướng dẫn nâng cao - Sử dụng tính năng Luồng kịch bản

## A. Giới thiệu

Tính năng chạy theo kịch bản là tính năng tạo kịch bản cho bot. Tính năng này cho phép chatbot Mindmaid trả lời các câu hỏi theo flow định nghĩa sẵn từ user.

## B. Nguyên lý hoạt động

Tính năng kịch bản sẽ có 2 thành phần chính:

* Flow: Là định nghĩa kịch bản chính cho chatbot
* State Flow: Là định nghĩa trạng thái hoạt động cho kịch bản

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

## C. Cách cài đặt

1. Truy cập Mindmaid
2. Chọn một "Bot Mindmaid" bất kỳ và chọn vào menu "Luồng kịch bản"
3. Chọn nút "Thêm mới" và nhập các thông tin: Tên luồng kịch bản
4. Chọn vào "Kịch bản" đã tạo phần "Danh sách trạng thái" chọn vào nút "Thêm mới" để thêm mới trạng thái và nhập các thông tin yêu cầu:
   1. Từ khóa: Từ khóa cần xuất hiện ở mỗi câu hỏi đầu vào của người dùng sẽ kích hoạt trạng thái của "Kịch bản".
   2. Phản hồi: Là phản hồi của trạng thái "Kịch bản" mỗi khi kịch bản được kích hoạt thông qua "Trạng thái"
5. Dùng thử với các "Kịch bản" đã thêm vào.

<figure><img src="https://aivgroupworking.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=ZmFkYTg1NDlhOWY4ZjI4ZTFiNzgwODkzYjAxZmJjODJfeXV0SWRFcHVrUjUzMUdRdDVQMVFzVDNvN0FnQzI2QmZfVG9rZW46UjI1OGJDWVFKb2RWVXJ4RUpmUWxQRUg3Z3BmXzE3MDgyNjE5MDc6MTcwODI2NTUwN19WNA" alt=""><figcaption></figcaption></figure>

## D. Lưu ý

* Mỗi bot chứa được nhiều "Kịch bản", mỗi "Kịch bản" có thể chứa nhiều "Trạng thái"
* Có thể nhập được nhiều "Từ khóa" của "Trạng thái" với mỗi từ khóa cách nhau bằng dấu ";"
