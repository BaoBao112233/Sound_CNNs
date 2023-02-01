# Sound_CNNs

1. Chuẩn bị dữ liệu:
Tải file dữ liệu tại đường link: https://www.mediafire.com/file/e1baktuo93pi923/datawav.zip/file
Sau đó tạo thư mục wav và đưa dữ liệu vào thư mục.

Sử dụng câu lệnh: pip install -r setup.txt để cài đặt các thư viện cần thiết.

2. Tư tưởng thuật toán:
Thông thường có thể sử dụng mạng RNN, GRU, LSTM để xử lý âm thanh do âm thanh thuộc dạng dữ liệu tuần tự sequence. 
Tuy nhiên ta cũng có thể sử dụng mạng CNN để xử lý. 
Trước khi xử lý dữ liệu, ta cần có 1 bước để chuyển dữ liệu âm thanh sang hình ảnh spectrogram của nó.
*   Quá trình train:
- Bước 1: Chuyển hết toàn bọ dữ liệu wav sang file ảnh lưu vào các thư mục train và test khác nhau.
- Bước 2: Đọc các ảnh trong thư mục train và thực hiện train model. Chú ý là nhẵn đầu ra output sẽ ở trong file train.csv (cột class)
*   Quá trình test:
- Bước 1: Chuyển âm thanh cần test vè dạng file ảnh.
- Bước 2: Đưa file ảnh và mạng để predict ra class tương ứng.

3. Mã nguồn

4. Thực hiện chương trình dạy máy tính nghe và phân loại âm thanh