# Network

## Mục lục

### [1. What is network](#what is network)
### [2. Advantages and disadvantages of network](#advantages and disadvantages of network)
### [3. Common physical component of a network](#common physical component of a network)
### [4. Interpreting a network diagram](#interpreting a network diagram)
### [5. Compare physical topology and logical topology](#compare physical topology and logical topology)
### [6. Describe the network topologies](#describe the network topologies)
### [7. Describe the function and operation of hub, switch and router](#describe the function and operation of hub, switch and router)
### [8. Describe the function of firewall and gateway](#describe the function of firewall and gateway)
### [9. Describe the function and operation of layer2 switching, layer3 switching and router](#describe the function and operation of layer 2 switching, layer 3 switching and router)
### [10. Describe the function of LAN, MAN, WAN networks](#describe the function of LAN, MAN, WAN networks)
### [11. Internet definition](#internet definition)
### [12. Indentify the layers of the OSI Model](#indentify the layers of the OSI model)
### [13. Indentify the layers and Deep dive TCP/IP Stack](#indentify the layers and deep dive TCP/IP stack)
### [14. Compare and contrast OSI and TCP/IP](#compare and contrast OSI and TCP/IP)
### [15. Compare and contrast TCP and UDP protocols](#compare and contrast TCP and UDP protocols)
### [16. What is DNS , Telnet, DHCP, HTTP, FTP ?](#what is DNS , Telnet, DHCP, HTTP, FTP ?)
### [17. What is IPv4 ? Describe IPv4 Address Classes](#what is IPv4 ? Describe IPv4 Address Classes)
### [18. Network Architecture : definition, compare peer to peer and client to server](#network architecture : definition, compare peer to peer and client to server)

###[19. Compare and contrast IPv4 address types: Unicast Broadcast Multicast](#compare and contrast IPv4 address types: Unicast Broadcast Multicast)
###[20. Describe the need for private IPv4 addressing. Compare Public Network and Private Network](#describe the need for private IPv4 addressing. Compare Public Network and Private Network)
### [21. What happens when you type in a url in the brower?](#what happens when you type in a url in the brower?)

---

<a name="what is network"></a>

### 1. What is network

Một mạng gồm hay hay nhiều máy tính hoặc các thiết bị được kết nối với nhau có thể giao tiếp bằng một số tiêu chuẩn chung (được gọi là giao thức) nhằm trao đổi tài nguyên và dịch vụ.

<a name="advantages and disadvantages of network"></a>

### 2. Advantages and disadvantages of network

- Ưu điểm:
  - Dễ dàng kết nối cho mọi người
  - Dễ dàng giao tiếp, liên lạc khi kết nối mạng
 - Tiết kiệm thời gian và chi phí khi làm việc
 - Chia sẻ tài nguyên nhanh chóng, thuận tiện

- Nhược điểm:
 - Chi phí lắp đặt, tiền mua thiết bị tốn kém
 - Cần có kế hoạch bảo dưỡng, duy trì
 - Cần người có kinh nghiệm khi sửa chữa, thay thế
 - Nguy cơ mất an toàn khi kết nối mạng (virus, mất cắp thông tin, ...)

<a name="common physical component of a network"></a>

### 3. Common physical component of a network

Những thành phần vật lý của một mạng:
- PC: đóng vai trò điểm cuối trong mạng, chịu trách nhiệm gửi và nhận dữ liệu, có thể bao gồm cả máy chủ
- Router: bộ định tuyến
- Switch: thiết bị chuyển mạch
- Cable: cáp mạng
- Network Interface Card (NIC): card mạng

<a name="interpreting a network diagram"></a>

### 4. Interpreting a network diagram

>updating

<a name="compare physical topology and logical topology"></a>

### 5. Compare physical topology and logical topology

- Cấu trúc liên kết vật lý: cấu trúc liên kết vật lý của mạng đề cập đến thiết kế vật lý của mạng, nó thể hiện sự sắp xếp hoặc bố trí của máy tính, dây cáp và các thành phần khác trên mạng. Cấu trúc liên kết vật lý của mạng hoạt động ở lớp 1 (Vật lý) của Mô hình OSI.

- Cấu trúc liên kết logic: cấu trúc liên kết logic đề cập đến cách xử lý dữ liệu trong mạng bất kể cấu trúc liên kết vật lý của nó. Cấu trúc liên kết logic của mạng hoạt động ở lớp 2 (Liên kết dữ liệu).

<a name="describe the network topologies"></a>

### 6. Describe the network topologies

Cấu trúc liên kết mạng là sơ đồ mô tả sự sắp xếp mạng, kết nối các nút khác nhau  thông qua các đường kết nối. 

Có hai loại cấu trúc liên kết mạng:
- Cấu trúc liên kết vật lý
- Cấu trúc liên kết logic

Các cấu trúc liên kết mạng vật lý và logic của một mạng không nhất thiết phải giống hệt nhau. Tuy nhiên, cả cấu trúc liên kết vật lý và mạng có thể được phân loại thành 3 mô hình cơ bản:
- Bus topology: tất cả các thiết bị/nút được kết nối trực tiếp tới cùng một đường trục hoặc đường truyền.
Ưu điểm:
 - Chi phí hiệu quả
 - Hoạt động tốt với các mạng nhỏ
 - Nếu 1 nút bị lỗi, mạng vẫn hoạt động

 Nhược điểm:
 - Mạng sẽ tắt nếu có đứt cáp chính hoặc một trong các đầu nối bị đứt
 - Nếu lưu lượng mạng nặng hoặc các nút nhiều thì hiệu suất của mạng sẽ giảm

![Ảnh](https://upload.wikimedia.org/wikipedia/commons/4/47/BusNetwork.svg)

- Ring topology: tất cả các thiết bị/nút được kết nối với cáp tạo thành một vòng khép kín, trong đó mỗi nút kết nối với đúng hai nút khác, tạo thành một con đường duy nhất liên tục cho tín hiệu qua từng nút.
Ưu điểm:
 - Không cần máy chủ mạng để kiểm soát kết nối mạng giữa mỗi máy trạm
 - Tất cả dữ liệu đi theo một hướng, làm giảm khả năng mất dữ liệu

 Nhược điểm:
 - Tất cả dữ liệu được truyền qua mạng phải đi qua từng máy trạm trên mạng, điều này khiến độ trễ mạng lớn
 - Nếu 1 nút bị hỏng, toàn bộ mạng sẽ dừng hoạt động

![Ảnh](https://upload.wikimedia.org/wikipedia/commons/d/db/NetworkTopology-Ring.png)

- Star topology: mọi nút kết nối với một thiết bị mạng trung tâm, như hub , switch hoặc máy tính. Thiết bị mạng trung tâm hoạt động như một máy chủ và các thiết bị ngoại vi hoạt động như máy khách.
Ưu điểm:
 - Nếu 1 nút bị hỏng, các nút khác vẫn hoạt động bình thường
 - Có thể thêm hoặc gỡ thiết bị mà không làm gián đoạn mạng
 - Phù hợp với mạng cỡ lớn

 Nhược điểm:
 - Chi phí tốn kém
 - Nếu nút trung tâm bị hỏng, toàn bộ mạng sẽ dừng hoạt động

![Ảnh](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/StarNetwork.svg/527px-StarNetwork.svg.png)

<a name="describe the function and operation of hub, switch and router"></a>

### 7. Describe the function and operation of hub, switch and router

>updating

<a name="describe the function of firewall and gateway"></a>

### 8. Describe the function of firewall and gateway

>updating

<a name="describe the function and operation of layer 2 switching, layer 3 switching and router"></a>

### 9. Describe the function and operation of layer2 switching, layer3 switching and router

>updating

<a name="describe the function of LAN, MAN, WAN networks"></a>

### 10. Describe the function of LAN, MAN, WAN networks

>updating

<a name="internet definition"></a>

### 11. Internet definition

>updating

<a name="indentify the layers of the OSI model"></a>

### 12. Indentify the layers of the OSI model

>updating

<a name="indentify the layers and deep dive TCP/IP stack"></a>

### 13. Indentify the layers and deep dive TCP/IP stack

>updating

<a name="compare and contrast OSI and TCP/IP"></a>

### 14. Compare and contrast OSI and TCP/IP

>updating

<a name="compare and contrast TCP and UDP protocols"></a>

### 15. Compare and contrast TCP and UDP protocols

>updating

<a name="what is DNS , Telnet, DHCP, HTTP, FTP ?"></a>

### 16. What is DNS , Telnet, DHCP, HTTP, FTP ?

>updating

<a name="what is IPv4 ? Describe IPv4 Address Classes"></a>

### 17. What is IPv4 ? Describe IPv4 Address Classes

>updating

<a name="network architecture : definition, compare peer to peer and client to server"></a>

### 18. Network architecture : definition, compare peer to peer and client to server

>updating

<a name="compare and contrast IPv4 address types: Unicast Broadcast Multicast"></a>

### 19. Compare and contrast IPv4 address types: Unicast Broadcast Multicast

>updating

<a name="describe the need for private IPv4 addressing. Compare Public Network and Private Network"></a>

### 20. Describe the need for private IPv4 addressing. Compare Public Network and Private Network

>updating

<a name="what happens when you type in a url in the brower?"></a>

### 21. What happens when you type in a url in the brower?

>updating