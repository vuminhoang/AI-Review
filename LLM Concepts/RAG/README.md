# Contents
[ ] Chunking Strategies 
[ ] Chunking Strategies Practice
[ ] Advanced RAG techniques

# Một vài kinh nghiệm xử lý RAG
## 1. Extend chunk
- Để phù hợp với kích thước của embedding nên nhiều khi ta có thể phải chia chunk khá nhỏ, dẫn đến việc các đoạn relevants kể cả tìm được cũng không đủ thông tin. Cần tìm 1 cách nào đó để truyền được nhiều thông tin cho LLMs hơn (ngoài thay đổi model embedding to hơn).
- Cách đã làm: Extend chunk đã tìm được lên: Sau khi tìm được chunk, regex nó vào đoạn trong văn bản gốc, mở rộng lên 2 phía đầu và cuối.
-> Khá hiệu quả trong dự án PDF Chatter, khi chỉ cần dùng embedding cỡ nhỏ và chính xác cho tiếng việt nhưng vẫn kiếm được đầy đủ thông tin. 
