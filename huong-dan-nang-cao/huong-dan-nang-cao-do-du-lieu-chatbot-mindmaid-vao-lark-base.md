# Hướng dẫn nâng cao - Đổ dữ liệu chatbot Mindmaid vào Lark Base

## A. Tạo Lark App và cấp quyền cho Lark App

{% hint style="info" %}
Nếu bạn đã có Lark App, vui lòng bỏ qua bước này!
{% endhint %}

| <ul><li>Truy cập Lark Developer tại: https://open.larksuite.com/</li><li>Chọn <strong>Create App</strong></li></ul>                                                                                                                                                                                                                         | <img src="../.gitbook/assets/image (1).png" alt="" data-size="original">                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| <ul><li>Chọn <strong>Create Custom App</strong></li></ul><p><br></p>                                                                                                                                                                                                                                                                        | <img src="../.gitbook/assets/image (1) (1).png" alt="" data-size="original">                                        |
| <ul><li>Điền thông tin của App và chọn <strong>Create</strong></li></ul><p><br></p>                                                                                                                                                                                                                                                         | <img src="../.gitbook/assets/image (2).png" alt="" data-size="original">                                            |
| <ul><li>Trong trang <strong>Permissions &#x26; Scopes, add tất cả các quyền</strong></li><li>Chọn <strong>Add in Bulk</strong></li><li>Chọn <strong>Confirm and Go to Create Version</strong></li><li>Điền thông tin version</li><li>Chọn Submit để gửi Admin duyệt</li></ul><p><br><em><strong>Vui lòng xem video ở dưới</strong></em></p> | <img src="../.gitbook/assets/img_v3_0287_ee98ad89-b64b-4e56-b3ab-dcf7387766hu (1).jpg" alt="" data-size="original"> |
| <ul><li>Sau khi Admin duyệt, bạn đã hoàn thành việc tạo Lark App</li></ul>                                                                                                                                                                                                                                                                  | <p><br></p>                                                                                                         |
| <ul><li>Lấy App ID và Secret ID</li></ul>                                                                                                                                                                                                                                                                                                   | <img src="../.gitbook/assets/image (68).png" alt="" data-size="original">                                           |

{% embed url="https://youtu.be/zXkUVf51EME" %}

## B. Tạo Base từ template

* Tạo Base mới từ template sau: [https://aivgroupworking.sg.larksuite.com/base/HFqdbTYqRaEgrMsNABJlcmklgvd?table=tblXDQwkdbEoBYu7\&view=vewPA81xUf](https://aivgroupworking.sg.larksuite.com/base/HFqdbTYqRaEgrMsNABJlcmklgvd?table=tblXDQwkdbEoBYu7\&view=vewPA81xUf)&#x20;

<figure><img src="../.gitbook/assets/img_v3_0287_2a8e061c-f8da-4dfe-9aae-9dbe538173hu.png" alt=""><figcaption></figcaption></figure>

* Phân quyền **People in the organization can edit**

<figure><img src="../.gitbook/assets/img_v3_0287_74b9812d-0283-4972-b087-0c5de5f905hu (1).png" alt=""><figcaption></figcaption></figure>

* Lấy ID của bảng Lịch sử chat & Function Calling

<figure><img src="../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>



<figure><img src="../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

## C. Cài đặt trong Mindmaid&#x20;

* Bước 1: Vào phần Cài đặt

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

*   Bước 2: Nhập các thông tin&#x20;

    * Lark App ID
    * Lark App Secret
    * Base ID
    * Lịch sử chat Table ID
    * Function Calling Table ID&#x20;

    <figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Liên hệ với chúng tôi**

* 0961160917 (Zalo)
* Facebook: [https://www.facebook.com/hoaingocduongthu](https://www.facebook.com/hoaingocduongthu)
* Lark: [Ngọc ](https://www.larksuite.com/invitation/page/add\_contact/?token=f61t41d4-bcb8-41b3-b29e-398857h221l8\&unique\_id=mfjNlUNTxVNzsH8b6BmGFw==)
{% endhint %}
