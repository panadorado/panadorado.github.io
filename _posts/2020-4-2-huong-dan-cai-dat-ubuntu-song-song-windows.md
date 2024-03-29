---
thumbnail: 202042ubuntu-windows.png
layout: post
title: Hướng dẫn cài đặt ubuntu song song với windows
excerpt: Bạn là một người dùng hệ điều hành Windows và muốn chuyển sang dùng Ubuntu
author: Panadora
category: [windows, unixlinux]
permalink: /huong-dan-cai-dat-ubuntu-song-song-windows.html
---

![winvslinux](../assets/images/202042ubuntu-windows.png)

**Bạn là một người dùng hệ điều hành `Windows` và muốn chuyển sang dùng `Ubuntu` để trải nghiệm sự mới của hệ điều hành mang nhân `linux`.**

Tuy nhiên việc bạn cài hoàn toàn 1 hệ điều hành `Ubuntu/Linux` lên một chiếc PC hoặc Laptop thì hết sức bình thường, nhưng điều đó sẽ quá xa lạ với 1 hệ điều hành mang đầy tính năng mới mẽ đối với bạn. Thì buộc bạn phải cài song song cả 2 hệ điều hành trên cùng một chiếc PC hoặc Laptop để tiện cho việc nghiên cứu và học tập.

Trong bài post này mình xin hướng dẫn các bạn cài đặt Ubuntu song song với Windows trên PC hoặc Laptop nhé.

**Bước 1: Cài đặt và tạo boot USB**

- Đầu tiện bạn cần tải phần mềm `rufus` để tạo boot USB <a href="https://rufus.ie/">tại đây</a>

- File `iso` chứa hệ điều hành `Ubuntu` <a href="https://ubuntu.com/#download">tại đây</a>

Tiếp theo bạn khởi tạo boot hệ điều hành ubuntu vào USB

Kết nối USB vào Máy tính và mở phần mềm rufus lên và cấu hình như sau:

![rufus-create-boot](https://www.how2shout.com/wp-content/uploads/2020/04/set-Rufus-to-create-Ubuntu-20.04-ISO-bootable-drive.png)

**Bước 2: Tiến hành cài đặt song song Ubuntu vào máy tính**

**Tổng hợp danh sách các phím truy cập BIOS cho bo mạch chủ của PC**

<article class="text-blog">
	<style>	
		table, th, td {
		  background: #dddd;
		  border: 1px solid #242424;
		  padding: 8px;
		}
	</style>
	<table>
		<tr>
			<th> Tên Mainboard PC </th>
			<th> Phím tắt </th>
		</tr>
		<tr>
			<td> Mainboard Abit </td>
			<td> phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard ASRock </td>
			<td> phím F2 </td>
		</tr>
		<tr>
			<td> Mainboard ASUS </td>
			<td> Phím DEL, Print hoặc F10 </td>
		</tr>
		<tr>
			<td> Mainboard BFG </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard FREESCALE </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard DFI </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard ECS Elitegroup </td>
			<td> Phím DEL hoặc F1 </td>
		</tr>
		<tr>
			<td> Mainboard EVGA </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard Foxconn </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard GIGABYTE </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard Intel </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard JetWay </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard Mach Speed </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard MSI (Micro-Star) </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard PCChips </td>
			<td> Phím DEL hoặc F1 </td>
		</tr>
		<tr>
			<td> Mainboard SAPPHIRE </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard Shuttle </td>
			<td> Del hoặc Ctrl + Alt + Esc </td>
		</tr>
		<tr>
			<td> Mainboard Soyo </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard Super Micro </td>
			<td> Phím DEL </td>
		</tr>
		<tr>
			<td> Mainboard TYAN </td>
			<td> DEL hoặc F4 </td>
		</tr>
		<tr>
			<td> Mainboard XFX </td>
			<td> DEL hoặc </td>
		</tr>
		<tr>
			<th> Tên Laptop </th>
			<th> Phím tắt </th>
		</tr>
	</table>
</article>
<br>
**Danh sách phím truy cập BIOS theo dòng máy**
<article class="text-blog">
	<style>	
		table, th, td {
		  background: #dddd;
		  border: 1px solid #242424;
		  padding: 5px;
		}
	</style>
	<table>
		<tr>
			<th> Tên Laptop </th>
			<th> Phím tắt </th>
		</tr>
		<tr>
			<td> Laptop SONY VAIO </td>
			<td> 
				Để vào được BIOS khi khởi động lại máy tính bạn cần nhấn và giữ phím F2 <br>
				Để vào được Recovery khi khởi động lại máy tính bạn cần nhấn và giữ phím F10 
			</td>
		</tr>
		<tr>
			<td> Laptop HP – COMPAQ </td>
			<td> 
				Một số dòng máy của HP thì bạn sẽ phải bấm Esc - nút Escape để vào BIOS.<br>
				Để vào được BIOS khi khởi động lại máy tính bạn cần nhấn và giữ phím F10<br>
				Để vào được Recovery khi khởi động lại máy tính bạn cần nhấn và giữ phím F11<br>
				Để vào được BOOT khi khởi động lại máy tính bạn cần nhấn và giữ phím F9
			</td>
		</tr>
		<tr>
			<td> Laptop ACER </td>
			<td> 
				Để vào được BOOT khi khởi động lại máy tính bạn cần nhấn và giữ phím F12<br>
				Để vào được BIOS khi khởi động lại máy tính bạn cần nhấn và giữ phím F2.<br>
			</td>
		</tr>
		<tr>
			<td> Laptop ASUS </td>
			<td> 
				Để vào được BIOS khi khởi động lại máy tính bạn cần nhấn và giữ phím ESC<br>
				Để vào được BOOT khi khởi động lại máy tính bạn cần nhấn và giữ phím F2 
			</td>
		</tr>
		<tr>
			<td> Laptop LENOVO THINKPAD </td>
			<td> 
				Để vào được BIOS khi khởi động lại máy tính bạn cần nhấn và giữ phím F1<br>
				Để vào được Recovery khi khởi động lại máy tính bạn cần nhấn và giữ phím ThinkVantage<br>
				Để vào được BOOT khi khởi động lại máy tính bạn cần nhấn và giữ phím F12 
			</td>
		</tr>
		<tr>
			<td> Laptop DELL </td>
			<td> 
				Để vào được BIOS khi khởi động lại máy tính bạn cần nhấn và giữ phím F2<br>
				Để vào được Recovery khi khởi động lại máy tính bạn cần nhấn và giữ phím F8 rồi chọn Repair your Computer<br>
				Để vào được BOOT khi khởi động lại máy tính bạn cần nhấn và giữ phím F12 
			</td>
		</tr>
	</table>
</article>
<br>

*Lưu ý: trước khi cài đặt Ubuntu yêu cầu các bạn tắt `Security Boot` và chọn đúng Chuẩn boot bạn đang sử dụng nếu không nhớ bạn có thể nguyên chuẩn MBR (BIOS hoặc UEFI) như Bước 1 `Cài đặt và tạo boot USB`*

Sau đó chọn Boot USB để vào giao diện cài đặt hệ điều hành `Ubuntu`:

![boot-ubuntu](https://ubuntucommunity.s3-us-east-2.amazonaws.com/original/2X/a/ad5e454a9fd45fd56d90da951702c2f2224cd32a.png)

+ Bạn chọn `Install Ubuntu`, chọn ngôn ngữ `English`
![install-Ubuntu](https://res.cloudinary.com/developerhub/image/upload/v1628792525/v2_5265/surwiscpmlo1rlmcu4ih.png)

+ Keyboard (mặt định `English US`)
<center><img class="img-thumbnail" src="https://www.upsieutoc.com/images/2020/04/03/ubuntu-pic-3.png" alt="ubuntu-pic-3.png" border="0"></center><br>

+ Phần `Update and other software` bạn chọn `Normal installation` và tích vào 2 hàng ở phần Other option
![install-Ubuntu-UpdateAndSoftware](https://phoenixnap.com/kb/wp-content/uploads/2021/04/choose-starting-applications-for-ubuntu-20.04.png)

+ Phần `Installation type` nếu cài song song bạn chọn `Something else`, nếu bạn muốn cài đặt hoàn toàn Ubuntu thì bạn chọn `Erea disk and install Ubuntu`.
![install-something-else](https://www.tecmint.com/wp-content/uploads/2012/10/choose-something-scenarios2.png)

+ Phần `Installation type` trong phần này các bắt đầu khởi tạo phân vùng như sau:

Bạn click vào phân vùng **`free space`** 
Tiếp tục chọn **`+`** khởi tạo phân vùng **`Swap area`**:
Phần Size (dung lượng) bạn set cho gắp đôi dung lương `RAM` nhé ví dụ:<br>
RAM 2GB -> Swap sẽ là 4GB (1024KB x 4 = 4096KB)<br>
RAM 4GB -> Swap sẽ là 8GB (1024KB x 8 = 8192KB)

Phần Type for the new partition: **`Logical`**<br>
Phần Use as: **`Swap area`**

![create-swap-ubuntu](https://i.stack.imgur.com/tyX1B.png)

Phần **`free space`** còn lại bạn dùng làm Phân vùng chính để cài `Ubuntu` <br>
Phần Type for the new partition: **`Primary`** <br>
Phần Use as: **`Ext4 journaling file system`**
tiếp tục click vào **`Continue`**

Sau đó bạn chọn thông tin như sau:

**Where are you?: `Ho Chi Minh`**
![Region-HCM](https://blogsofts.net/wp-content/uploads/2021/05/cach-cai-ubuntu-8.png)

**Who are you?:**<br>
Your name: **`< tên user bạn muốn đặt >`**<br>
Your computer's name: **`< tên cho máy tính bạn muốn đặt >`**<br>
Pick a username: **`< tên tài khoảng bạn muốn đặt >`**<br>
Choose a password: **`< mật khẩu bạn muốn đặt >`**<br>
Confirm your password: **`< xác nhận lại mật khẩu >`**

![Create-User](https://i.stack.imgur.com/TdMDH.png)

Click vào **`continue`** để tiến hành cài đặt **`Ubuntu`**.<br>
Sau khi cài đặt hoàn tất, các bạn khởi động lại máy tính và màn hình Dual-Boot Ubuntu với Windows hiện lên. Bạn có thể sử dụng phím mũi tên để di chuyển đến hệ điều hành muốn khởi động và nhấn Enter, lựa chọn Ubuntu để vào Ubuntu hoặc **`Windows Boot Manager`** để truy cập vào Windows.

![Screen-Ubuntu](https://upload.wikimedia.org/wikipedia/commons/4/42/Ubuntu-20.04-cat.png)