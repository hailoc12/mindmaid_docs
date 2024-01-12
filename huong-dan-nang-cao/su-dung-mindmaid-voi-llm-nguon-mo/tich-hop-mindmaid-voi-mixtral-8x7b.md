# Tích hợp Mindmaid với Mixtral-8x7B



> Sử dụng LLM mã nguồn mở là một trong những hướng phát triển nhanh hiện nay để tiết kiệm chi phí sử dụng API ChatGPT. Mindmaid hiện tương thích với toàn bộ các LLM nguồn mở và có thể kết nối dễ dàng. Hướng dẫn dưới đây đưa ra ví dụ sử dụng Mindmaid với model Mixtral-8x7B-Instruct-v0.1 có chất lượng gần tương đương chatgpt 3.5 và chi phí rẻ hơn 4 lần.

### 1. Truy cập Anyscale (Anyscale đang cho miễn phí 10$ với tài khoản đăng ký mới)

* Truy cập Anyscale và đăng ký tài khoản với đường dẫn: [https://app.endpoints.anyscale.com/login](https://app.endpoints.anyscale.com/login)
* Lấy API Key từ Anyscale: [https://app.endpoints.anyscale.com/credentials](https://app.endpoints.anyscale.com/credentials)

<figure><img src="../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

* Lựa chọn model mà anyscale đang hỗ trợ, ở hướng dẫn này sử dụng model mistralai/Mixtral-8x7B-Instruct-v0.1

<figure><img src="../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

* Có thể xem số dư Anyscale tại đây: [https://app.endpoints.anyscale.com/billing](https://app.endpoints.anyscale.com/billing)

### 2. Sử dụng thông tin đã có của Anyscale tạo chatbot Mindmaid

* Truy cập Mindmaid: [https://mindmaid.ai/](https://mindmaid.ai/)
* Tạo hoặc chọn một chatbot cần sử dụng thông tin Open source LLM
*   Điền thông tin của Anyscale đã có ở bước 1 gồm có:

    * Url API: [https://api.endpoints.anyscale.com/v1](https://api.endpoints.anyscale.com/v1) (Hoặc bất kỳ API opensource LLM mà bạn sử dụng)
    * API Key: Key của bạn lấy được ở bước 1 (Hoặc api key riêng của opensource LLM mà bạn sử dụng
    * Model open source: Tên model cần sử dụng (chọn 1 trong các options dưới đây)
      * meta-llama/Llama-2-7b-chat-hf&#x20;
      * meta-llama/Llama-2-13b-chat-hf&#x20;
      * Meta-Llama/Llama-Guard-7b&#x20;
      * meta-llama/Llama-2-70b-chat-hf&#x20;
      * Open-Orca/Mistral-7B-OpenOrca&#x20;
      * codellama/CodeLlama-34b- Instruct-hf&#x20;
      * HuggingFaceH4/zephyr-7b-beta&#x20;
      * mistralai/Mistral-7B-Instruct-v0.1&#x20;
      * mistralai/Mixtral-8x7B-Instruct- v0.1&#x20;
      * thenlper/gte-large
    * Bật sử dụng LLM Open source\




    <figure><img src="../../.gitbook/assets/CleanShot 2023-12-19 at 18.32.06@2x.png" alt=""><figcaption><p>Mixtral-8x7B có chất lượng tượng đương GPT3.5 và tương thích mọi tính năng của Mindmaid</p></figcaption></figure>
