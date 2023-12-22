# Tích hợp Mindmaid với VinaLlama-7b

> Sử dụng LLM mã nguồn mở là một trong những hướng phát triển nhanh hiện nay để tiết kiệm chi phí sử dụng API ChatGPT. Mindmaid hiện tương thích với toàn bộ các LLM nguồn mở và có thể kết nối dễ dàng. Hướng dẫn dưới đây đưa ra ví dụ sử dụng Mindmaid với model VinaLlama-7b - model LLM tiếng Việt có chất lượng tốt nhất hiện nay, tương đương với ChatGPT 3.5.&#x20;

### Giới thiệu về VinaLlama-7B

{% embed url="https://huggingface.co/vilm/vinallama-7b" %}

VinaLlama-7B hiện là mô hình ngôn ngữ cỡ nhỏ (SLM) có chất lượng tốt nhất (state-of-the-art) của tiếng Việt. Model này đạt chất lượng tương đương ChatGPT 3.5 trong hầu hết các nhiệm vụ bằng tiếng Việt, và có kết quả vượt xa model PhoGPT được công bố trước đó.&#x20;

![](<../../../.gitbook/assets/image (26).png>)&#x20;

### Mục tiêu của việc tích hợp VinaLlama-7B vào Mindmaid&#x20;

Model VinaLlama-7B nguồn mở với khả năng xử lý tiếng Việt tốt và có thể chạy trên Laptop/PC là sự thay thế tốt cho API ChatGPT, giúp giảm giá thành sử dụng Chatbot AI và tăng tính bảo mật về dữ liệu cho doanh nghiệp. VinaLlama-7B cũng cho phép những người muốn tìm hiểu build chatbot AI có thể bắt đầu với chi phí thấp.

### Chuẩn bị&#x20;

Để thực hiện được hướng dẫn này, bạn cần có:

1. Tài khoản Mindmaid từ gói Pro trở lên&#x20;
2. Tài khoản Cloudflare & một domain.&#x20;
3. Máy tính:

* Cấu hình lý tưởng: Macbook chip M1/M2 16Gb RAM hoặc Laptop/PC có card đồ họa (Nvidia/AMD) có VRAM >=6 GB
* Cấu hình tối thiểu: laptop/pc core i5, 8Gb RAM

### Hướng dẫn&#x20;

#### Bước 1: Cài đặt ứng dụng LMStudio lên máy

1. tải LMStudio tại: [https://lmstudio.ai](https://lmstudio.ai)
2. cài đặt LMStudio lên máy

#### Bước 2: Tải model VinaLlama-7B

1. mở ứng dụng LMStudio
2. gõ vào ô tìm kiếm "VinaLlama"
3. download model về máy:

* nếu máy bạn chỉ có CPU, hãy chọn download vinallama-2.7b-chat-GGUF
* nếu máy bạn là MacOS M1/M2, hoặc có card NVIDIA, chọn download model vinallama-7b-chat\_q5\_0.gguf để đạt chất lượng tối nhất

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-21 at 19.08.07@2x.png" alt=""><figcaption></figcaption></figure>

#### Bước 3: Chọn model và cấu hình

1. Ấn vào biểu tượng chat ở menu bên trái
2. Sau đó chọn model vinallama-7b-chat\_q5\_0.gguf hoặc vinallama-2.7b-chat.gguf đã tải ở Bước 2

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-19 at 23.49.17@2x.png" alt=""><figcaption></figcaption></figure>

3. Tinh chỉnh cấu hình ở sidebar bên phải

* bật GPU Acceleration nếu máy bạn dùng Macbook M1/M2 hoặc có card đồ họa

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-21 at 19.13.31@2x.png" alt=""><figcaption></figcaption></figure>

* bật "Keep entire model in RAM" để tăng tốc mô hình nếu máy bạn có 16GB RAM trở lên

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-21 at 19.15.14@2x.png" alt=""><figcaption></figcaption></figure>

* Nếu máy bạn hạn chế về RAM (CPU) hoặc VRAM (GPU), khiến mô hình không chạy được, thì có thể giảm "Context Length" xuống 300 tới 500 để giảm tải.

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-21 at 19.19.36@2x.png" alt=""><figcaption></figcaption></figure>

#### Bước 4: Chat thử&#x20;

1. Click vào biểu tượng chat ở bên trái&#x20;
2. Gõ nội dung chat vào ô User. Nếu bot trả lời thì có nghĩa đã chạy model thành công

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-21 at 19.23.31@2x.png" alt=""><figcaption></figcaption></figure>

#### Bước 5: Chạy API Server

Để kết nối model VinaLlama chạy trên máy của bạn với chatbot Mindmaid, cần tạo API Server và kết nối nó tới Mindmaid. Rất may LMStudio có hỗ trợ tính năng này, giúp thực hiện nó khá đơn giản

1. Click vào biểu tượng thứ tư ở sidebar trái, sau đó ấn Start Server để khởi động API Server giúp kết nối tới model VinaLlama.
2. Nếu Server logs hiển thị như hình dưới thì bạn đã chạy API Server thành công tại địa chỉ http://localhost:1234. Tuy nhiên địa chỉ này chỉ truy cập được từ máy bạn, chứ chưa thể truy cập từ Internet, do đó cần làm thêm Bước 6 bên dưới.&#x20;

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-21 at 19.26.44@2x.png" alt=""><figcaption></figcaption></figure>

#### Bước 6: Cho phép kết nối tới API Server từ Internet

Có nhiều giải pháp khác nhau để cho phép truy cập API Server trên laptop/PC cá nhân từ Internet như port forwarding, port tunneling...trong hướng dẫn này chúng ta sẽ sử dụng ngrok vì nó miễn phí và dễ cài đặt.

1. Đăng ký tài khoản tại [https://ngrok.com](https://dashboard.ngrok.com/get-started/setup/macos)
2. Chọn phiên bản ngrok phù hợp với hệ điều hành của máy bạn, và cài đặt theo hướng dẫn của ngrok
3. Khi chạy lệnh ngrok để thiết lập port tunnel, bạn nhớ chọn port 1234 (là port của API Server đã thiết lập ở bước 5). Kết quả như hình dưới đây là đã cài đặt thành công. Lưu ý đoạn "[https://7c00-2405-4803-fc0b-58d0-58ae-a803-4e51-f9c9.ngrok-free.app](https://7c00-2405-4803-fc0b-58d0-58ae-a803-4e51-f9c9.ngrok-free.app)" chính là địa chỉ API Server sẽ cần sử dụng ở bước tiếp theo.&#x20;

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-21 at 19.46.40@2x.png" alt=""><figcaption></figcaption></figure>

#### Bước 7: Cài đặt chatbot Mindmaid để thay thế API ChatGPT bằng API VinaLlama

1. Truy cập Mindmaid: [https://mindmaid.ai/](https://mindmaid.ai/)
2. Tạo mới hoặc chọn một chatbot cần sử dụng thông tin Open source LLM
3. Vào mục "Cài đặt trợ lý ảo", bật chức năng "Sử dụng LLM tùy chỉnh"&#x20;

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-22 at 08.52.30@2x (1).png" alt=""><figcaption></figcaption></figure>

4. Điền thông tin API Server vào bot:&#x20;

* Tên LLM tùy chỉnh: bạn điền "VinaLlama" hoặc tên khác cũng được.
* API Key của LLM tùy chỉnh: bạn điền "not-needed"
* Địa chỉ API của LLM tùy chỉnh (cái này quan trọng nhất, phải điền chính xác): bạn điền https://{url ngrok trả về ở bước 6)/v1. Ví dụ: "[https://7c00-2405-4803-fc0b-58d0-58ae-a803-4e51-f9c9.ngrok-free.app](https://7c00-2405-4803-fc0b-58d0-58ae-a803-4e51-f9c9.ngrok-free.app)/v1". Lưu ý cần thêm "/v1" ở cuối.

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-22 at 09.07.39@2x.png" alt=""><figcaption></figcaption></figure>



5. **Lưu  ý: nếu bạn muốn huấn luyện bot với dữ liệu riêng, thì vẫn cần điền OpenAI Key như bình thường vì API ChatGPT sẽ được sử dụng trong quá trình cho bot học dữ liệu.**

#### **Bước 8: Sử dụng thử / tích hợp vào website, fanpage**

1. Để chat thử với bot, bạn vào mục "Giao diện preview" để chat

<figure><img src="../../../.gitbook/assets/CleanShot 2023-12-22 at 09.14.31@2x.png" alt=""><figcaption></figcaption></figure>

2. Để tích hợp bot vào website, fanpage, mời bạn tham khảo link tới các bài viết hướng dẫn đã có:

{% content-ref url="../../../huong-dan-co-ban/6.-hdsd-mindmaid-tich-ho-p-website.md" %}
[6.-hdsd-mindmaid-tich-ho-p-website.md](../../../huong-dan-co-ban/6.-hdsd-mindmaid-tich-ho-p-website.md)
{% endcontent-ref %}

{% content-ref url="../../../huong-dan-co-ban/7.-hdsd-mindmaid-tich-hop-facebook.md" %}
[7.-hdsd-mindmaid-tich-hop-facebook.md](../../../huong-dan-co-ban/7.-hdsd-mindmaid-tich-hop-facebook.md)
{% endcontent-ref %}
