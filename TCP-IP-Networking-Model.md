# Mô hình mạng TCP/IP
Transmission Control Protocol/Internet Protocol

![alt](https://images.viblo.asia/653e97ca-c80d-415e-9547-7395a3309c32.png)

Tiến trình lịch sử: Từ mô hình độc quyền cho đến mô hình TCP / IP mở
![alt](https://f5-zpcloud.zdn.vn/2014813437060132607/b2b8c6de427a8e24d76b.jpg)


## Lớp ứng dụng
* Giao thức lớp ứng dụng TCP / IP cung cấp dịch vụ cho phần mềm ứng dụng đang chạy trên máy tính. 
* Lớp ứng dụng không tự định nghĩa ứng dụng, nhưng nó định nghĩa các dịch vụ mà ứng dụng cần. 
* Ví dụ: giao thức ứng dụng HTTP xác định cách trình duyệt web có thể lấy nội dung của trang web từ máy chủ web. 
* Tóm lại, lớp ứng dụng cung cấp giao diện giữa phần mềm chạy trên máy tính và mạng của nó.

Ví dụ về cách thức hoạt động của HTTP
![alt](https://f4-zpcloud.zdn.vn/1575355005448582221/e9cb86702ad4e68abfc5.jpg)


## Lớp giao vận
* Chịu trách nhiệm duy trì liên lạc đầu cuối trên toàn mạng.
* Tầng này có 2 giao thức chính là TCP ( Transmisson Control Protocol) và UDP ( User Datagram Protocol )

Ví dụ cơ bản về khôi phục lỗi TCP
![alt](https://f5-zpcloud.zdn.vn/6227076858807877996/da7c6572c2d60e8857c7.jpg)


## Lớp liên mạng
* Xử lý quá trình truyền gói tin trên mạng
* Giao thức chủ yếu: the Internet Protocol (IP): IP cung cấp một số tính năng, quan trọng nhất là định địa chỉ và định tuyến

![alt](https://f6-zpcloud.zdn.vn/4802052889340965246/af3e012fda8b16d54f9a.jpg)


## Lớp vật lý và liên kết dữ liệu
* Lớp vật lý và liên kết dữ liệu của mô hình TCP / IP xác định các giao thức và phần cứng cần thiết để cung cấp dữ liệu qua một số mạng vật lý. 
* Lớp vật lý xác định cáp và năng lượng (ví dụ: tín hiệu điện) truyền qua cáp. 
* Lớp liên kết dữ liệu TCP / IP cung cấp các dịch vụ cho lớp phía trên nó trong mô hình (lớp mạng). Khi tiến trình IP của máy chủ hoặc bộ định tuyến chọn gửi gói IP đến bộ định tuyến hoặc máy chủ khác, máy chủ hoặc bộ định tuyến đó sẽ sử dụng chi tiết lớp liên kết để gửi gói đó đến máy chủ / bộ định tuyến tiếp theo.

Ví dụ về sử dụng Ethernet để định hướng gói tin
![alt](https://f6-zpcloud.zdn.vn/523729655511780317/611e8c88562c9a72c33d.jpg)

**Bước 1** Larry đóng gói gói tin IP giữa header Ethernet và trailer Ethernet, tạo ra một khung Ethernet 

**Bước 2** Larry truyền các bit của khung Ethernet một cách vật lý, sử dụng dòng điện chạy qua hệ thống cáp Ethernet.

**Bước 3** Bộ định tuyến R1 về mặt vật lý nhận tín hiệu điện qua cáp và tạo lại các bit tương tự bằng cách diễn giải ý nghĩa của các tín hiệu điện.

**Bước 4** Bộ định tuyến R1 đưa gói tin IP ra khỏi khung Ethernet bằng cách loại bỏ phần header và trailer Ethernet.


## Cách thức hoạt động của TCP/IP
Khi truyền dữ liệu , quá trình tiến hành từ lớp trên xuống lớp dưới, qua mỗi lớp dữ liệu được thêm vào thông tin điều khiển gọi là Header. Khi nhận dữ liệu thì quá trình xảy ra ngược lại, dữ liệu được truyền từ lớp dưới lên và qua mỗi lớp thì phần header tương ứng sẽ được lấy đi và khi đến  trên cùng thì dữ liệu không còn phần header nữa.
![alt](https://f5-zpcloud.zdn.vn/6105852537827125756/4d47a04368e7a4b9fdf6.jpg)

![alt](https://f5-zpcloud.zdn.vn/269625471654586323/cd7f76c5be61723f2b70.jpg)



## So sánh mô hình OSI với TCP/IP
![alt](https://f5-zpcloud.zdn.vn/76802242870281224/7adc84db497f8521dc6e.jpg)
