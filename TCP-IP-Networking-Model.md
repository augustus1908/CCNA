# Mô hình mạng TCP/IP
Transmission Control Protocol/Internet Protocol

![alt](https://images.viblo.asia/653e97ca-c80d-415e-9547-7395a3309c32.png)

![alt](https://scontent.xx.fbcdn.net/v/t1.15752-9/247681995_248871810621317_3257950860253704432_n.png?_nc_cat=108&ccb=1-5&_nc_sid=aee45a&_nc_ohc=92hg98q7ZbsAX-vcs7u&_nc_oc=AQk_BuGfA-c-wkSgnNzHu-8RjxCpijwcX2WkLrJWczC9GFmG32mI7fUDwDNC_dZNRBbiClsEOsw74kvnKRyA3U6f&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=1d3e6465181402c80083edb597f839a5&oe=619F5F46)

## Lớp ứng dụng
* Giao thức lớp ứng dụng TCP / IP cung cấp dịch vụ cho phần mềm ứng dụng đang chạy trên máy tính. 
* Lớp ứng dụng không tự định nghĩa ứng dụng, nhưng nó định nghĩa các dịch vụ mà ứng dụng cần. 
* Ví dụ: giao thức ứng dụng HTTP xác định cách trình duyệt web có thể lấy nội dung của trang web từ máy chủ web. 
* Tóm lại, lớp ứng dụng cung cấp giao diện giữa phần mềm chạy trên máy tính và mạng của nó.

Ví dụ về cách thức hoạt động của HTTP
![alt](https://scontent.xx.fbcdn.net/v/t1.15752-9/p206x206/246612752_434208654785108_8409102494971154069_n.png?_nc_cat=104&ccb=1-5&_nc_sid=aee45a&_nc_ohc=JNwxkTRkbgwAX_qk3vW&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=b316a5d975f008a8551fb18628b51e01&oe=619DA897)

## Lớp giao vận
* Chịu trách nhiệm duy trì liên lạc đầu cuối trên toàn mạng.
* Tầng này có 2 giao thức chính là TCP ( Transmisson Control Protocol) và UDP ( User Datagram Protocol )

Ví dụ cơ bản về khôi phục lỗi TCP
![alt](https://scontent.xx.fbcdn.net/v/t1.15752-9/s552x414/247572600_391987402617992_3271709053625449633_n.png?_nc_cat=107&ccb=1-5&_nc_sid=aee45a&_nc_ohc=fsBolZ8hn8cAX-WZHZf&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=eeb0b7e312fcf2314dff69b278d1183b&oe=619F7300)

## Lớp liên mạng
* Xử lý quá trình truyền gói tin trên mạng
* Giao thức chủ yếu: the Internet Protocol (IP): IP cung cấp một số tính năng, quan trọng nhất là định địa chỉ và định tuyến

## Lớp vật lý và liên kết dữ liệu
* Lớp vật lý và liên kết dữ liệu của mô hình TCP / IP xác định các giao thức và phần cứng cần thiết để cung cấp dữ liệu qua một số mạng vật lý. 
* Lớp vật lý xác định cáp và năng lượng (ví dụ: tín hiệu điện) truyền qua cáp. 
* Lớp liên kết dữ liệu TCP / IP cung cấp các dịch vụ cho lớp phía trên nó trong mô hình (lớp mạng). Khi tiến trình IP của máy chủ hoặc bộ định tuyến chọn gửi gói IP đến bộ định tuyến hoặc máy chủ khác, máy chủ hoặc bộ định tuyến đó sẽ sử dụng chi tiết lớp liên kết để gửi gói đó đến máy chủ / bộ định tuyến tiếp theo.

Ví dụ về sử dụng Ethernet để định hướng gói tin
![alt](https://scontent.xx.fbcdn.net/v/t1.15752-9/s480x480/248265922_1047456922704726_5633732569652861715_n.png?_nc_cat=101&ccb=1-5&_nc_sid=aee45a&_nc_ohc=VWihwoamGhAAX9K8Jig&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=6ef8bcdaa5cdfecea42cc0d755c9a77b&oe=619D807E)

**Bước 1** Larry đóng gói gói tin IP giữa header Ethernet và trailer Ethernet, tạo ra một khung Ethernet 

**Bước 2** Larry truyền các bit của khung Ethernet một cách vật lý, sử dụng dòng điện chạy qua hệ thống cáp Ethernet.

**Bước 3** Bộ định tuyến R1 về mặt vật lý nhận tín hiệu điện qua cáp và tạo lại các bit tương tự bằng cách diễn giải ý nghĩa của các tín hiệu điện.

**Bước 4** Bộ định tuyến R1 đưa gói tin IP ra khỏi khung Ethernet bằng cách loại bỏ phần header và trailer Ethernet.


## Cách thức hoạt động của TCP/IP
Khi truyền dữ liệu , quá trình tiến hành từ lớp trên xuống lớp dưới, qua mỗi lớp dữ liệu được thêm vào thông tin điều khiển gọi là Header. Khi nhận dữ liệu thì quá trình xảy ra ngược lại, dữ liệu được truyền từ lớp dưới lên và qua mỗi lớp thì phần header tương ứng sẽ được lấy đi và khi đến  trên cùng thì dữ liệu không còn phần header nữa.
![alt](https://scontent.xx.fbcdn.net/v/t1.15752-9/s370x247/248689172_3155498911349100_2989058677557044256_n.png?_nc_cat=105&ccb=1-5&_nc_sid=aee45a&_nc_ohc=IqDV3G1OlgQAX9qlyuz&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=047497c4d15b66a2deb532d554a05a53&oe=619F2A25)

## So sánh mô hình OSI với TCP/IP
![alt](https://scontent.xx.fbcdn.net/v/t1.15752-9/p206x206/245671595_1043972833060110_5988413681567344834_n.png?_nc_cat=109&ccb=1-5&_nc_sid=aee45a&_nc_ohc=vu74fF8VwJ4AX_QxOG6&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=1f20c9b0bed3b50003881aa033989659&oe=619DCFA8)
