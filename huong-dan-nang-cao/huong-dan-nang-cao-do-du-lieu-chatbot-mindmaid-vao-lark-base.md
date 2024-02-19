# Hướng dẫn nâng cao - Đổ dữ liệu chatbot Mindmaid vào Lark Base

## A. Tạo Lark App và cấp quyền cho Lark App

{% hint style="info" %}
Nếu bạn đã có Lark App, vui lòng bỏ qua bước này!
{% endhint %}

| <ul><li>Truy cập Lark Developer tại: https://open.larksuite.com/</li><li>Chọn <strong>Create App</strong></li></ul>                                                                                                                                                                                                                         | ![](https://miaduong.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=ZTI1ZjI4OGVmOTljNmM4ZmMzZWRhMzU5ZDI4YWIyZjhfZk5tNGpPdG52aXBneEc3Nzd1UlE0NnVneE1VYXo1UmhfVG9rZW46VEpKamJRbk5rb1BFRzB4eXo3bGx1QjdMZzdiXzE3MDgzMzg2OTA6MTcwODM0MjI5MF9WNA) |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>Chọn <strong>Create Custom App</strong></li></ul><p><br></p>                                                                                                                                                                                                                                                                        | ![](https://miaduong.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=YzQyZmRhNTBiMzM3ZjAzODFmMmRkNDFiYmU1NzIyN2JfN3ZZNXNmNjBVNk9NdEN3YmppVWExeDZTVW9ueHJTWVVfVG9rZW46VkNrMmJaYnAzb1hyTEt4RXdSZ2xDd0NDZ0ZoXzE3MDgzMzg2OTA6MTcwODM0MjI5MF9WNA) |
| <ul><li>Điền thông tin của App và chọn <strong>Create</strong></li></ul><p><br></p>                                                                                                                                                                                                                                                         | ![](https://miaduong.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=OGFlMWViNmMxMmJlNDgzZTYxM2QzNmNlNDY5Y2QxNzJfTW5TSWZJdXVqMm5OdjF4eVFVTXJLM2J0cXV2RkU3ZEdfVG9rZW46U2VBNGJMWVk3b2YzZVd4dU4zOGxtcVVDZ0tjXzE3MDgzMzg2OTA6MTcwODM0MjI5MF9WNA) |
| <ul><li>Trong trang <strong>Permissions &#x26; Scopes, add tất cả các quyền</strong></li><li>Chọn <strong>Add in Bulk</strong></li><li>Chọn <strong>Confirm and Go to Create Version</strong></li><li>Điền thông tin version</li><li>Chọn Submit để gửi Admin duyệt</li></ul><p><br><em><strong>Vui lòng xem video ở dưới</strong></em></p> | <img src="../.gitbook/assets/img_v3_0287_ee98ad89-b64b-4e56-b3ab-dcf7387766hu (1).jpg" alt="" data-size="original">                                                                                                                                         |
| <ul><li>Sau khi Admin duyệt, bạn đã hoàn thành việc tạo Lark App</li></ul>                                                                                                                                                                                                                                                                  | <p><br></p>                                                                                                                                                                                                                                                 |
| <ul><li>Lấy App ID và Secret ID</li></ul>                                                                                                                                                                                                                                                                                                   | <img src="../.gitbook/assets/image (68).png" alt="" data-size="original">                                                                                                                                                                                   |



{% file src="../.gitbook/assets/Screen Recording 2024-01-04 at 03.34.00.mov" %}

## B. Tạo Base từ template

* Tạo Base mới từ template sau: [https://aivgroupworking.sg.larksuite.com/base/HFqdbTYqRaEgrMsNABJlcmklgvd?table=tblXDQwkdbEoBYu7\&view=vewPA81xUf](https://aivgroupworking.sg.larksuite.com/base/HFqdbTYqRaEgrMsNABJlcmklgvd?table=tblXDQwkdbEoBYu7\&view=vewPA81xUf)&#x20;



* Phân quyền People in organization can edit

