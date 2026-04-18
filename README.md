# Zalo-AI-2025
Link cuộc thi: https://challenge.zalo.ai/portal/road-buddy.
Đề bài bao gồm 1 tập dữ liệu.
Tập train bao gồm 1490 file video tình huống về luật giao thông đường bộ và một file json chứa hỏi và đáp án tương ứng với các trường hợp
Tập test bao gồm 480 file video tình huống và một file json chứa câu hỏi

Yêu cầu đưa ra đáp án tương ứng phù hợp với các câu hỏi

Cách tiếp cận và giải: sử dụng mô hình vllm ở đây là :SmolVlm để finetune và inference
Một số kỹ thuật học được: các mô hình vllm chứa hàng triệu tham số, việc train lại là bất khả thi và khó hội tụ, chỉ train lại trên tập dữ liệu có sẵn - trích xuất từ 3 tới 5 frame trên mỗi video để dùng finetune, chỉnh sửa lại câu prompt tại inference và bước train để nâng cao hiệu suất

<img width="1359" height="679" alt="image" src="https://github.com/user-attachments/assets/7ba11b3e-75c5-4293-be7e-6da2cefe6fe3" />


