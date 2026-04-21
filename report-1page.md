# Report 1 Page – FIT4012 Lab 2

## 1. Mục tiêu
Tóm tắt ngắn gọn mục tiêu của bài lab.

## 2. Cách làm
- Hoàn thiện Caesar Cipher cho chữ thường, dấu cách và giải mã.
- Hoàn thiện Rail Fence Cipher cho giải mã, giữ dấu cách, kiểm tra đầu vào và đọc file.
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Caesar Cipher
| Input | Key | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 3 | L ORYH BRX | Mã hóa đúng giữ khoảng trắng |
| hello world | 5 | mjqqt btwqi | không có nhận xét |
| LORYH BRX | 3 | ILOVE YOU  | Giải mã chính xác |

### 3.2 Rail Fence Cipher
| Input | Rails | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 2 | ILV O OEYU | không có nhận xét |
| I LOVE YOU | 4 | EYLVOOU | không có nhận xét |
| IOEOLVYU | 2 | IOEOLVYU | không có nhận xét |

### 3.3 Input validation / file input
- Trường hợp đầu vào không hợp lệ: không có nhận xét
- Kết quả đọc từ `data/input.txt`: không có nhận xét

## 4. Kết luận
Bài lab 2 đã giúp em củng cố kiến thức về các phương pháp mã hóa cổ điển, từ đó hiểu rõ hơn về tầm quan trọng của việc hoán vị và thay thế trong an toàn thông tin. Qua quá trình thực hiện, em rút ra được những điểm sau:

Điều học được: Em đã nắm vững cách triển khai thuật toán Caesar bằng toán tử modulo 26 và cách xây dựng ma trận zigzag để thực hiện Rail Fence Cipher. Ngoài ra, em cũng làm quen được với quy trình làm việc chuyên nghiệp trên GitHub Classroom, từ việc quản lý mã nguồn đến việc viết nhật ký và báo cáo minh chứng.

Khó khăn lớn nhất: Việc xây dựng hàm giải mã cho Rail Fence Cipher là thách thức lớn nhất, vì cần phải xác định chính xác vị trí của các ký tự trên khung zigzag trước khi điền dữ liệu từ bản mã vào. Việc quản lý các chỉ số (index) trong mảng hai chiều đòi hỏi sự tỉ mỉ cao.

Điều giúp hiểu rõ hơn: Việc trực quan hóa các đường ray (rails) thành hình vẽ và thực hiện chạy thử (trace) từng bước trên giấy đã giúp em hiểu rõ quy luật di chuyển của ký tự. Bên cạnh đó, việc thực hiện các test case với nhiều số lượng ray khác nhau giúp em nhận thấy sự thay đổi rõ rệt về độ phức tạp của bản mã.
