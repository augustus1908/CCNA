# EtherChannel

![](https://images.viblo.asia/2c50fe9e-1c3e-4bb8-b4df-9c6428ba88c5.png)

![](https://images.viblo.asia/9b0d7c6b-3796-4648-9834-e21b0e74ca4e.png)

![](https://images.viblo.asia/92213fa6-3abc-4079-a0af-f4237b30a77a.png)

![](https://images.viblo.asia/2b893980-26d3-49bf-894f-d60d2b8f15df.gif)


- EtherChannel là một kỹ thuật nhóm hai hay nhiều đường kết nối truyền tải dữ liệu vật lý (Link Aggregation) thành một đường ảo duy nhất (Logic) có Port ảo thậm chí cả MAC ảo nhằm mục đích tăng tốc độ truyền dữ liệu và tăng khả năng dự phòng (Redundancy) cho hệ thống
- Công nghệ EtherChannel có thể bó từ 2 đến 8 link FE, GE, 10GE thành 1 link logical. Khi đó, switch đối xử các port thuộc EtherChannel như 1 port duy nhất.

- Traffic không phải lúc nào cũng được phân bố đồng đều qua các đường link thuộc EtherChannel, mà nó phụ thuộc vào phương pháp load balancing mà switch sử dụng và mẫu traffic trong mạng.
Nếu một trong các link thuộc EtherChannel bị down thì traffic sẽ tự động được chuyển sang link khác trong channel chỉ trong vòng vài miliseconds. Khi link up trở lại thì traffic được phân bố lại như cũ.

