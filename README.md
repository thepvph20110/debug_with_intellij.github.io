# Hướng dẫn Debug với Intellij

## Debug là gì ?
- là quá trình tìm kiếm ra lỗi hay nguyên nhân gây ra lỗi (bug ở đâu) để có hướng sửa lỗi (fix bug). 
Việc kiểm soát lỗi của rất nhiều các dòng code là việc không hề đơn giản với những người lập trình viên chưa có nhiều kinh nghiệm. 
##	Mục đích 
- Debug không chỉ là để loại bỏ lỗi (error) khỏi chương trình mà quan trọng hơn còn để giúp lập trình viên hiểu rõ hơn sự thực thi của chương trình.
Một lập trình viên không có khả năng Debug hiệu quả thì cũng giống như bị mù vậy.

## Trong bài viết này mình sẽ hướng dẫn các bạn cách debug với intellij thông qua 1 vidu đơn giản
- vidu: mình tạo ra 1 project ( java ) nhập từ bàn phím 2 số a và b . tính tổng 2 số a và b và in ra kết quả.

![DEMO](https://user-images.githubusercontent.com/109200115/189867315-c85a82f7-3a39-49b8-86e5-b560d7264230.png)

### Bước 1: Breakpoint dòng muốn debug -> chạy chương trình debug

- **breakpoint** : là để kiểm tra cách chương trình hoạt động trong thời gian chạy, chúng ta cần tạm dừng việc thực thi của nó trước đoạn mã bị nghi ngờ. Điều này được thực hiện bằng cách thiết lập các điểm ngắt. Các điểm ngắt chỉ ra các dòng mã nơi chương trình sẽ bị tạm dừng để bạn kiểm tra trạng thái của nó.

- **Cách đặt breakpoint** : Click chuột vào lề trái của dòng đó. Lúc này breakpoint sẽ được toggle, click thêm lần nữa để xóa (như hình).

![Breakpoint](https://user-images.githubusercontent.com/109200115/189867744-d667000b-0453-4a02-8fa8-a1d723c42ea4.png)

### Bước 2: Bắt đầu nhập số a -> thực hiện chạy tiếp các dòng sau breakpoint -> thực hiện tương tự nhập số b 

![nhapa](https://user-images.githubusercontent.com/109200115/189869155-ea26884c-5d9c-4f61-b110-0f39996576d7.png)

![nhapb](https://user-images.githubusercontent.com/109200115/189869184-b15986e8-c46d-47bb-a884-245abf5c58b6.png)

- **Lưu ý** : Dòng code được highlight sẽ chưa thực hiện, chỉ khi bạn đi tiếp qua dòng khác thì dòng trước đó mới được thực thi.

### Bước 3: khi nhập và chạy hết các dòng muốn debug thì giá trị của các biến sẽ hiển thị bên cạnh biến đó -> nếu trường hợp biến khác với giá trị  nhập vào thì dòng đó xảy ra lỗi -> tiến hành fix bug 

![DEMO](https://user-images.githubusercontent.com/109200115/189869552-06034fae-7511-4a82-9361-bfd30edea3e5.png)

### Kết luận
- để quá trình fix bug diễn ra nhanh chóng , chúng ta cần biết debug để tìm ra dòng gặp lỗi 
