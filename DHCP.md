# DHCP
### Dynamic Host Configuration Protocol

là giao thức tự động cấp phát địa chỉ IP đến các thiết bị trong mạng

- DHCP client : Là một thiết bị bất kì có khả năng kết nối internet và giao tiếp với máy chủ DHCP như điện thoại thông minh, máy tính, laptop, máy in….
- DHCP server : Là thiết bị cấp phát địa chỉ IP
- DHCP relay agents : Là thiết bị trung gian để chuyển tiếp yêu cầu giữa DHCP client và DHCP server
- DHCP Lease : Là khoảng thời gian thiết bị giữ nguyên địa chỉ IP trước khi nó được thay đổi và gia hạn. Cụ thể, mỗi địa chỉ IP sẽ có một vòng đời nhất định. Khi hết thời gian này nó sẽ được cấp một địa chỉ mới.


### Cách thức hoạt động:

![](https://www.totolink.vn/public/uploads/img_article/dhcplagitimhieuvedhcpcachthuchoatdongcuadhcp.jpg)

Khi muốn kết nối với mạng thiết bị sẽ gửi yêu cầu `DHCP DISCOVER` đến máy chủ. Máy chủ DHCP sẽ tìm địa chỉ IP khả dụng rồi cung cấp cho thiết bị cùng với gói `DHCP OFFER`.

Sau khi nhận được địa chỉ, thiết bị sẽ phản hồi với máy chủ bằng một gói tin `DHCP REQUEST`. Đây là lúc chấp nhận yêu cầu, máy chủ sẽ gửi tin báo nhận (ACK) xác nhận thiết bị đã có IP và thời gian sử dụng IP đến khi có địa chỉ mới.




