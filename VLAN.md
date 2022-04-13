# VLAN - Virtual Local Area Network

![](https://vnpro.vn/upload/user/images/Th%C6%B0%20Vi%E1%BB%87n/V%C3%AD%20d%E1%BB%A5%20v%E1%BB%81%20VLAN.jpg)

- VLAN là một kỹ thuật cho phép tạo lập các mạng LAN độc lập một cách logic trên cùng một Switch hay cùng một kiến trúc hạ tầng vật lý.

- Việc tạo lập nhiều mạng LAN ảo trong cùng một mạng cục bộ (giữa các khoa trong một trường học, giữa các cục trong một công ty,...) giúp giảm thiểu miền quảng bá (broadcast domain) cũng như tạo thuận lợi cho việc quản lý một mạng cục bộ rộng lớn

## Trunking

![](https://www.totolink.vn/public/uploads/img_article/vtplagivlantrunkingprotocollagiduongtrunklagi.png)

![](https://www.totolink.vn/public/uploads/img_article/vtplagivlantrunkingprotocollagiketnoitrunk.png)


## VTP - VLAN Trunking Protocol

VTP (VLAN Trunking Protocol) quảng bá các thông tin cấu hình VLAN đến các switch láng giềng để các cấu hình VLAN có thể được thực hiện trên một switch, trong khi tất cả các switch khác trong hệ thống mạng sẽ học thông tin VLAN này

VTP gửi thông điệp quảng bá qua “VTP domain” mỗi 5 phút một lần, hoặc khi có sự thay đổi xảy ra trong quá trình cấu hình VLAN. Một thông điệp VTP bao gồm “rivision-number”, tên VLAN (VLAN name), số hiệu VLAN. Bằng sự cấu hình VTP Server và việc quảng bá thông tin VTP tất cả các switch đều đồng bộ về tên VLAN và số liệu VLAN của tất cả các VLAN.

Một trong những thành phần quan trọng trong các thông tin quảng bá VTP là tham số “revision-number”.  Mỗi thành phần VTP server điều chỉnh thông tin VLAN, nó tăng “revision-number” lên 1, rồi sau đó VTP Server mới gửi thông tin quảng bá VTP đi. Khi một switch nhận một thông điệp VTP với “revision-number” lớn hơn, nó sẽ cập nhật cấu hình VLAN

![](https://www.totolink.vn/public/uploads/img_article/vtplagivlantrunkingprotocollagihoatdongcuavtp.png)





