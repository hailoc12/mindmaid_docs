# Hướng dẫn nâng cao - Tạo trợ lý ảo GPTs mới

**Bước 1: Tại tab Bảng điều khiển, Click button Tạo Trợ lý ảo mới, sau đó chọn Tạo bot GPTs**

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

**Bước 2: Chọn gói Trợ lý ảo**

Chi tiết so sánh các gói Trợ lý ảo Mindmaid: https://mindmaid.ai/price

<figure><img src="https://lh7-us.googleusercontent.com/nr9JZEB4feLK0X_Pe3_2LUjsU4PsxUZDx0Ek2ZsxpCHhzp2aQo5KaiiAxrVlK3Vzylm2xr5GqiqbiA_Y37rD-d_kNHprjOvj3gJDx70KKNgosBXn4SCF2V0j0xpZlUJubEzhUrkE5-qlgIVI4neg7ec" alt=""><figcaption></figcaption></figure>

**Bước 3: Điền thông tin Trợ lý ảo, sao đó chọn Tạo mới**

* Tên trợ lý ảo: Tên gọi để phân biệt các chatbot và hiển thị với người dùng
* Mô tả: mô tả sơ bộ về chatbot
* Open API key: Mã duy nhất được cung cấp bởi OpenAI để cho phép bạn truy cập và sử dụng dịch vụ của họ. Hướng dẫn lấy API Key[ xem tại đây](https://workbetter.vn/huong-dan-lay-chatgpt-api-key/).&#x20;
* Model: Chọn mô hình GPT 4 hoặc GPT 3.5
* Thiết lập Bật/Tắt một số chức năng

#### Bước 4: Hướng dẫn sử dụng function calling kết hợp action trong gpts

**Function calling**

* Trong menu cài đặt "Function calling" gọi tắt là FC có thể tùy chọn tạo một FC hoặc nhiều FC để thực hiện các tác vụ đặc biệt ví dụ như: Lấy số điện thoại, email người dùng nhập vào, ...
* Một FC có thể viết như sau:

```
{
  "name": "mindmaid_phone_email", # Tên của Function
  "description": "Get name or phone number or email address of the user", # Mô tả Function
  "parameters": {
    "type": "object", # Loại parameter nên để mặc định object
    "required": [ # Yêu cầu các trường nào bắt buộc phải có dữ liệu ở đây là location
      "location"
    ],
    "properties": { # Chi tiết các trường thông tin cần lấy
      "name": { # Tên (Cần viết tiếng anh không dấu và cách nhau bằng _)
        "type": "string", # Loại dữ liệu của trường ở đây là string
        "description": "the name of the user" # Mô tả trường dữ liệu này là gì (càng chi tiết càng tốt và nên có ví dụ)
      },
      "email": { 
        "type": "string",
        "description": "the email address of the user"
      },
      "phone": {
        "type": "string",
        "description": "The phone number of Vietnamese"
      }
    }
  }
}
```

* Lưu ý name của function calling không nên viết trùng nhau khi nhập nhiều function calling cho một gpts

**Actions**

<figure><img src="../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Action là một tính năng giúp gpts có thể dựa vào Function calling để từ đó tương tác với dữ liệu bên ngoài qua API
* Để Action hoạt động bắt buộc bạn phải có Function calling trước đó
* Nhập các thông tin cần thiết của Action:
  * Tên hàm: Ở đây cần chọn tên hàm là một trong các function calling đã tạo trước đó
  * Địa chỉ API: Là địa chỉ API bên ngoài của bạn mà gpts sẽ sử dụng
  * Phương thức call API: Là phương thức gọi API của bạn ví dụ: GET hoặc POST
  * API Key: Là Key của API nếu có  (có thể để trống nếu API không yêu cầu)
  * Loại xác thực: Là loại xác thực API của bạn ở đây hỗ trợ 2 kiểu là Bearer/API Key nếu có (có thể để trống nếu API không yêu cầu)
  * Template trả lời: Là mẫu hướng dẫn gpts trả lời mặc định nếu không muốn sử dụng dữ liệu đầu ra của API làm context trả lời

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

* **Lưu ý**: Action chỉ được kích hoạt khi Function calling gắn với Action đó được kích hoạt.

Sau khi điền xong, bấm **Thêm mới**

<figure><img src="https://lh7-us.googleusercontent.com/bKDihKfJCGfSX6626ldBk2tUivE4xGsoMEy-nkp5nuWq5Jk7ol49cqfN54eYkWi3KBJhnt41T1NGNP315oBBUJseBdULfwNkWjl4oXBCcsFwFaguFDATSk690jAtUwevlwGa-qEDpyt0TQI6ZoITEr4" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Như vậy bạn đã tạo Trợ lý ảo thành công!



{% hint style="info" %}
Bạn có thể xem video hướng dẫn dưới đây!
{% endhint %}

{% embed url="https://youtu.be/azBR4894VCQ" %}
