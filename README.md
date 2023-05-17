# Project Android
# ỨNG DỤNG SQLITE XÂY DỰNG CHƯƠNG TRÌNH ANROID QUẢN LÝ HOẠT ĐỘNG THU CHI CÁ NHÂN
-	Ứng dụng cài đặt trên điện thoại chạy hệ điều hành Android
-	Hệ thống phải đáp ứng và lưu trữ đầy đủ, bảo mật thông tin của người dùng
-	Ứng dụng có đầy đủ các chức năng như:  
	Quản lý đăng kí 
	Quản lý đăng nhập
	Quản lý thu
	Quản lý chi
	Quản lý ví tiền
	Thống kê, báo cáo 
![image](https://github.com/Ni2103/Project_Android/assets/89075130/5e34d861-8a22-4219-b868-35ebfe0643cb)
# Đặc tả chức năng của ứng dụng
![image](https://github.com/Ni2103/Project_Android/assets/89075130/82d5f35b-c90f-42c1-a276-dee750a34a55)
Sơ đồ Use case tổng quát quản lý chi tiêu cá nhân
-	Đặc tả use case tạo tài khoản mới:
+	Luồng sự kiện chuẩn:
	1: Nhập tài khoản và mật khẩu
	2: Hệ thống kiểm tra
	3: Đăng nhập thành công
+	Ngoại lệ:
•	Tạo tài khoản không hợp lệ khi trong tài khoản đã tồn tại tài khoản đó. Nếu đã tồn tại yêu cầu tạo tài khoản mới.
-	Đặc tả use case đăng nhập:
	Luồng sự kiện chuẩn:
•	1: Nhập tài khoản và mật khẩu
•	2: Hệ thống kiểm tra
•	3: Đăng nhập thành công
	Ngoại lệ:
•	Đăng nhập không hợp lệ khi nhập sai tài khoản, mật khẩu hoặc tài khoản đó không tồn tại, hệ thống yêu cầu đăng nhập lại. Nếu chưa có tài khoản cần đăng kí tài khoản mới.
-	Đặc tả use case hỗ trợ người dùng:
	Luồng sự kiện chuẩn:
•	1: Hệ thống thực hiện đăng nhập
•	2: Người dùng chọn danh mục chức năng hỗ trợ người dùng
S -1: Nếu chức năng là “Đăng kí tài khoản” hệ thống thực hiện luồng sự kiện con “Đăng kí tài khoản mới cho người dùng”
S -2: Nếu chức năng là “Đăng nhập” hệ thống thực hiện luồng sự kiện con “Đăng nhập cho người dùng”
S -3: Nếu chức năng là “Đăng xuất” hệ thống thực hiện luồng sự kiện con “Đăng xuất”
	Luồng sự kiện con:
•	S -1: Đăng kí tài khoản mới cho người dùng
1: Người dùng nhập thông tin tên đăng nhập và mật khẩu cần tạo
2: Hệ thống lưu lại thông tin 
3: Đăng kí tài khoản thành công
•	S -2: Đăng nhập cho người dùng:
1: Nhập tài khoản và mật khẩu
2: Hệ thống kiểm tra
3: Đăng nhập thành công
•	S -3: Đăng xuất:
1: Người dùng chọn vào “Đăng xuất”
2: Hệ thống đăng xuất khỏi tài khoản người dùng
-	Đặc tả use case quản lý nguồn thu:
+ Luồng sự kiện chẩn:
	1: Hệ thống thực hiện đặc tả Đăng nhập
	2: Người dùng chọn danh mục nguồn thu
S -1: Nếu chức năng là Thêm hệ thống thực hiện luồng sự kiện con “Thêm nguồn thu”
S -2: Nếu chức năng là Sửa hệ thống thực hiện luồng sự kiện con “Sửa nguồn thu”
S -3: Nếu chức năng là Xóa hệ thống thực hiện luồng sự kiện con “Xóa nguồn thu”
	Luồng sự kiện con:
•	S -1: Thêm nguồn thu:
1: Người dùng chọn vào “Thêm nguồn thu”
2: Người dùng nhập vào thông tin nguồn thu cần thêm
3: Hệ thống lưu lại thông tin nguồn thu
4: Hệ thống hiển thị thông tin nguồn thu
•	S -2: Sửa nguồn thu:
1: Người dùng chọn vào thông tin nguồn thu cần sửa và chọn “Sửa nguồn thu”
2: Người dùng chỉnh sửa thông tin nguồn thu
3: Hệ thống lưu lại thông tin nguồn thu
4: Hệ thống hiển thị thông tin
•	S -3: Xóa nguồn thu:
1: Người dùng chọn vào thông tin nguồn thu cần xóa và chọn “Xóa nguồn thu”
2: Hệ thống thực hiện xóa nguồn thu
3: Hệ thống lưu lại thông tin nguồn thu
4: Hệ thống hiển thị thông tin
-	Đặc tả use case quản lý khoản chi:
+ Luồng sự kiện chẩn:
	1: Hệ thống thực hiện đặc tả Đăng nhập
	2: Người dùng chọn danh mục khoản chi
S -1: Nếu chức năng là Thêm hệ thống thực hiện luồng sự kiện con “Thêm khoản chi”
S -2: Nếu chức năng là Sửa hệ thống thực hiện luồng sự kiện con “Sửa khoản chi”
S -3: Nếu chức năng là Xóa hệ thống thực hiện luồng sự kiện con “Xóa khoản chi”
	Luồng sự kiện con:
•	S -1: Thêm khoản chi:
1: Người dùng chọn vào “Thêm khoản chi”
2: Người dùng nhập vào thông tin khoản chi cần thêm
3: Hệ thống lưu lại thông tin khoản chi
4: Hệ thống hiển thị thông tin khoản chi
•	S -2: Sửa khoản chi:
1: Người dùng chọn vào thông tin nguồn thu cần sửa và chọn “Sửa khoản chi”
2: Người dùng chỉnh sửa thông tin khoản chi
3: Hệ thống lưu lại thông tin khoản chi
4: Hệ thống hiển thị thông tin
•	S -3: Xóa khoản chi:
1: Người dùng chọn vào thông tin khoản chi cần xóa và chọn “Xóa khoản chi”
2: Hệ thống thực hiện xóa khoản chi
3: Hệ thống lưu lại thông tin khoản chi
4: Hệ thống hiển thị thông tin
-	Đặc tả use case quản lý ví tiền:
+ Luồng sự kiện chẩn:
	1: Hệ thống thực hiện đặc tả Đăng nhập
	2: Người dùng chọn danh mục quản lý ví tiền
S -1: Nếu chức năng là Thêm hệ thống thực hiện luồng sự kiện con “Thêm ví tiền”
S -2: Nếu chức năng là Sửa hệ thống thực hiện luồng sự kiện con “Sửa ví tiền”
S -3: Nếu chức năng là Xóa hệ thống thực hiện luồng sự kiện con “Xóa ví tiền”
S -4: Nếu chức năng là Xem thông tin hệ thống thực hiện luồng sự kiện con “Xem thông tin ví tiền”

	Luồng sự kiện con:
•	S -1: Thêm ví tiền:
1: Người dùng chọn vào “Thêm ví tiền”
2: Người dùng nhập vào thông tin ví tiền cần thêm
3: Hệ thống lưu lại thông tin ví tiền
4: Hệ thống hiển thị thông tin ví tiền
•	S -2: Sửa ví tiền:
1: Người dùng chọn vào thông tin nguồn thu cần sửa và chọn “Sửa ví tiền”
2: Người dùng chỉnh sửa thông tin ví tiền
3: Hệ thống lưu lại thông tin ví tiền
4: Hệ thống hiển thị thông tin
•	S -3: Xóa ví tiền:
1: Người dùng chọn vào thông tin ví tiền cần xóa và chọn “Xóa ví tiền”
2: Hệ thống thực hiện xóa ví tiền
3: Hệ thống lưu lại thông tin ví tiền
4: Hệ thống hiển thị thông tin
•	S -4: Xem thông tin ví tiền:
1: Người dùng chọn vào thông tin ví tiền cần xem và chọn “Xem thông tin ví tiền”
2: Hệ thống thực hiện hiển thị thông tin ví tiền
-	Đặc tả use case quản lý danh mục thu/ chi:
+ Luồng sự kiện chẩn:
	1: Hệ thống thực hiện đặc tả Đăng nhập
	2: Người dùng chọn danh mục quản lý danh mục thu/chi
S -1: Nếu chức năng là Thêm hệ thống thực hiện luồng sự kiện con “Thêm danh mục thu chi”
S -2: Nếu chức năng là Sửa hệ thống thực hiện luồng sự kiện con “Sửa danh mục thu chi”
S -3: Nếu chức năng là Xóa hệ thống thực hiện luồng sự kiện con “Xóa danh mục thu chi”
	Luồng sự kiện con:
•	S -1: Thêm danh mục thu/ chi:
1: Người dùng chọn vào “Thêm danh mục thu/chi”
2: Người dùng nhập vào thông tin danh mục thu/chi cần thêm
3: Hệ thống lưu lại thông tin danh mục thu/chi
4: Hệ thống hiển thị thông tin danh mục thu/chi
•	S -2: Sửa danh mục thu/chi:
1: Người dùng chọn vào thông tin danh mục thu chi cần sửa và chọn “Sửa danh mục thu chi”
2: Người dùng chỉnh sửa thông tin danh mục thu/chi
3: Hệ thống lưu lại thông tin danh mục thu/chi
4: Hệ thống hiển thị thông tin
•	S -3: Xóa danh mục thu/chi:
1: Người dùng chọn vào thông tin danh mục thu/chi cần xóa và chọn “Xóa danh mục thu/chi”
2: Hệ thống thực hiện xóa danh mục thu/chi
3: Hệ thống lưu lại thông tin danh mục thu/chi
4: Hệ thống hiển thị thông tin
-	Đặc tả use case thống kê, báo cáo thu/chi
+ Luồng sự kiện chẩn:
	1: Hệ thống thực hiện đặc tả Đăng nhập
	2: Người dùng chọn danh mục thống kê, báo cáo thu/chi
S -1: Nếu chức năng là tạo biểu đồ thống kê chi tiêu trong ngày thì hệ thống thực hiện luồng sự kiện con “Tạo biểu đồ thống kê chi tiêu trong ngày”
S -2: Nếu chức năng là tạo biểu đồ thống kê nguồn thu nhập trong ngày thì hệ thống thực hiện luồng sự kiện con “Tạo thống kê nguồn thu nhập trong ngày”
S -3: Nếu chức năng là tạo biểu đồ thống kê chi tiêu hằng ngày thì hệ thống thực hiện luồng sự kiện con “Tạo biểu đồ thống kê chi tiêu hằng ngày”
	Luồng sự kiện con:
S -1: Tạo biểu đồ thống kê chi tiêu trong ngày
1: Người dùng chọn ngày cần thống kê
2: Hệ thống hiển thị thông tin thống kê chi tiêu trong ngày mà người dùng yêu cầu.
S -2: Tạo thống kê nguồn thu nhập trong ngày
1: Người dùng chọn ngày và nguồn thu nhập cần thống kê
2: Hệ thống hiển thị thông tin thống kê nguồn thu nhập trong ngày mà người dùng yêu cầu.
S -3: Tạo biểu đồ thống kê chi tiêu hằng ngày
1: Người dùng chọn tạo biểu đồ thống kê chi tiêu hằng ngày
2: Hệ thống hiển thị thông tin thống kê chi tiêu hằng ngày mà người dùng yêu cầu.
# Mô hình luồng dữ liệu(DFD)
#	Mô hình dòng dữ liệu mức 0
![image](https://github.com/Ni2103/Project_Android/assets/89075130/d8fc6b58-6357-47bc-ab75-7ae961372c37)
# 	Mô hình dòng dữ liệu mức 1
![image](https://github.com/Ni2103/Project_Android/assets/89075130/14e37c4e-d7f8-4569-b712-f792369a6483)

#	Mô hình dòng dữ liệu mức 2
- 	Mô hình dòng dữ liệu mức 2 cho ô xử lý 1.0 “Quản lý nguồn thu”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/9287fae8-4140-4b5f-a5cf-dbac38f7e925)
- 	Mô hình dòng dữ liệu mức 2 cho ô xử lý 2.0 “Quản lý khoản chi”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/afd8cf84-b4cf-47bd-ae02-3a5006b60b32)
- 	Mô hình dòng dữ liệu mức 2 cho ô xử lý 3.0 “Quản lý ví tiền”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/3ac5130b-2c77-4938-af17-2a3f25f44ba4)
-	Mô hình dòng dữ liệu mức 2 cho ô xử lý 4.0 “Quản lý danh mục thu/chi”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/762f6e63-ace2-487d-9709-5f1371d98b3c)
-	Mô hình dòng dữ liệu mức 2 cho ô xử lý 5.0 “Thống kê”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/a14b4e7f-83e0-43ea-a4fe-de0da94130fc)
# Mô hình thực thể kết hợp(ERD)
![image](https://github.com/Ni2103/Project_Android/assets/89075130/0a76a9ba-2775-4387-a22b-06424f40b18a)

# XÂY DỰNG CƠ SỞ DỮ LIỆU
<img width="429" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/7e442edc-97c8-442f-bca5-8404ca424ff3">
<img width="425" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/e5bc6b6c-a601-420a-b6d3-e5c91d1d4f5c">
<img width="446" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/16d73409-015a-483c-a4a6-ce88a53bd35c">
<img width="436" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/94c58a9d-4c04-4b81-88b3-d0ea988ef23a">
<img width="427" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/fdecfdbd-2827-4e2a-8ad1-5e9ef4c0ede2">


# SƠ ĐỒ TỔ CHỨC GIAO DIỆN
![image](https://github.com/Ni2103/Project_Android/assets/89075130/5d6804fb-7026-44ca-9242-af2f7ac06bde)
# Màn hình chào
![image](https://github.com/Ni2103/Project_Android/assets/89075130/a7baa030-89e9-4ad2-b94c-2fe7d455911e)
-	Đây là màn hình khởi động ứng dụng, bấm vào nút ‘Start’ để bắt đầu sử dụng ứng dụng
# Màn hình giao diện đăng kí
![image](https://github.com/Ni2103/Project_Android/assets/89075130/0134f1f7-e346-4b80-883a-65df0a809545)
-	Người dùng mở ứng dụng màn hình đăng nhập sẽ mở lên trước. Nếu người dùng chưa có tài khoản thì bấm vào nút Register để tạo một tài khoản mới, màn hình sẽ chuyển sang giao diện đăng kí tài khoản
-	Sau khi gõ đầy đủ các thông tin, người dùng bấm vào nút Register để đăng kí
-	Sau khi tạo thành công màn hình sẽ hiển thị thống báo đã tạo thành công và chuyển sang giao diện màn hình đăng nhập
# Màn hình giao diện đăng nhập
![image](https://github.com/Ni2103/Project_Android/assets/89075130/62f81635-b2fe-4030-bc16-1b2f077ef897)
-	Gõ tên đăng nhập và mật khẩu tương ứng
-	Sau khi gõ đầy đủ các thông tin, người dùng bấm vào nút Login
-	Hệ thống sẽ tiến hành kiểm tra thông tin tài khoản đã được tạo trong cơ sở dữ liệu
+	Đăng nhập thành công: nếu thông tin chính xác, người dùng sẽ có thể truy cập được vào màn hình chính của ứng dụng
+	Đăng nhập thất bại: thông tin đăng nhập không chính xác, yêu cầu nhập lại và hiện thông báo “login failed”


# Màn hình trang chủ 
![image](https://github.com/Ni2103/Project_Android/assets/89075130/a9be4000-0353-4a91-a240-d08cc97475df)
-	Tại trang chủ, có thể xem tình hình chi/ tiêu biến động theo ngày
-	Có thể xem danh sách các nguồn tài khoản thu nhập 
-	Các khoản chi đã thêm
-	Ngoài ra, nếu nhấn vào ‘dấu cộng’ ở phía trên màn hình có thể tới giao diện thêm nguồn thu hay là các khoản chi tiêu mới

# Màn hình thống kê
![image](https://github.com/Ni2103/Project_Android/assets/89075130/dbc52463-e839-4bfb-aa08-50a68a112bf1)
-	Tại màn hình này, có thể xem được thống kê các khoản chi tiêu trong ngày hiện tại (nếu có)
-	Xem thống kê thu nhập trong ngày (nếu có) và các khoản chi tiêu 
-	Ngoài ra, nếu nhấn vào ‘dấu cộng’ ở phía trên màn hình có thể tới giao diện thêm nguồn thu hay là các khoản chi tiêu mới.

#  Màn hình thêm nguồn thu/ khoản chi
![image](https://github.com/Ni2103/Project_Android/assets/89075130/87e40f0f-fa23-4b9a-88ce-7316fe256d13)
-	Thêm: Hiển thị màn hình thêm mới nguồn thu / khoản chi, cho phép người dùng chọn các danh mục tương ứng cần cần thêm
-	Các danh mục tronng nguồn thu nhập hay khoản chi tiêu sẽ được quản lý trong danh sách danh mục
-	Sau khi thêm nguồn thu nhập hay khoản chi tiêu mới thì giao diện sẽ hiển thị tương ứng với danh mục đã chọn cho phép người dùng nhập vào số tiền tương ứng, ghi chú, thời gian.
-	Bấm lưu để thêm 
+ Trường hợp nếu người dùng không nhập số tiền thì sẽ có thông báo ‘ Bạn không được để trống số tiền’ , khi đó người dùng chưa thể lưu được  và phải cung cấp số tiền tương ứng thì mới hoàn tất thủ tục lưu 

# Màn hình cài đặt
![image](https://github.com/Ni2103/Project_Android/assets/89075130/95efc1f1-82a0-47d9-ad1a-596e55642a6b)
-	Tại giao diện cài đặt, người dùng có thể:
+ Xem thông tin ví tiền, thêm ví tiền mới, cập nhật hoặc xóa ví tiền hiện tại
+ Cập nhật loại tiền tệ mới
+ Xem các danh mục tương ứng với nguồn thu hoặc khoản chi. Ngoài ra có thể thêm mới một danh mục tương ứng hoặc cập nhật, xóa một danh mục đã có.
+ Xem thông tin liên hệ, gửi phản hồi cho ứng dụng
+ Đăng xuất khỏi tài khoản hiện tại

# Màn hình thêm ví tiền
![image](https://github.com/Ni2103/Project_Android/assets/89075130/11e4577b-4b41-45f6-8fac-ebe951771cef)
-	Khi người dùng nhấn vào ‘dấu cộng’ ở góc phải trên cùng của ứng dụng thì sẽ hiện lên giao diện để thêm ví tiền mới
-	Người dùng nhập tên ví tiền mới, số tiền cho ví tiền đó
+ Trường hợp nếu người dùng không nhập tên ví tiền hay số tiền mà nhấn vào nút “Hoàn thành’ sẽ có một cảnh báo yêu cầu người dùng nhập đầy đủ thông tin 
-	Sau khi nhập đầu đủ, người dùng bấm nút Hoàn tất, màn hình hiện thống báo ‘ví tiền mới được thêm’

 # Màn hình cập nhật/ xóa ví tiền
 ![image](https://github.com/Ni2103/Project_Android/assets/89075130/783af689-b11b-457b-8d8e-77f7c5a38467)
 -	Nếu người dùng muốn xóa hay chỉnh sửa ví tiền nào thì có thể nhấn vào ví tiền đó. Một sự lựa chọn sẽ hiện ra cho phép xóa hoặc cập nhật ví tiền
-	Nếu người dùng bấm vào nút xóa thì ví tiền đó sẽ bị xóa khỏi danh mục, nếu nhấn vào nút chỉnh sửa thì màn hình sẽ hiện lên giao diện chỉnh sửa thông tin ví tiền cho người dùng
-	Sau cùng người dùng bấm nút Hoàn thành để lưu lại thông tin đã cập nhật
# Màn hình chỉnh sửa loại tiền tệ
![image](https://github.com/Ni2103/Project_Android/assets/89075130/dcc32c9b-bbc9-4773-8ad3-ef0733d9280c)
-	Người dùng có thể chỉnh sửa loại tiền tệ tương ứng kho nhấn vào mục loại tiền tệ, sau khi chỉnh sửa xong bấm ‘Chỉnh sửa’ để lưu thông tin vừa thay đổi

# Màn hình thêm danh mục mới 
![image](https://github.com/Ni2103/Project_Android/assets/89075130/224c1faf-237e-43a8-94bc-3f9a1455f8f2)
-	Tại chức năng Danh mục trong phần Cài đặt, người dùng có thể quản lý tất cả danh sách danh mục nguồn thu và khoản chi của người dùng.  Khi nhấn vào ‘dấu cộng ‘ở góc trên bên phải màn hình, người dùng có thể thêm mới một danh mục tương ứng với nguồn thu hoặc khoản chi.
# Màn hình cập nhật/ xóa danh mục
![image](https://github.com/Ni2103/Project_Android/assets/89075130/24cf27de-922c-42ce-b6dd-d4d5ab01fd4c)
-	Nếu người dùng muốn xóa hay chỉnh sửa danh mục thì có thể nhấn vào danh mục đó. Một sự lựa chọn sẽ hiện ra cho phép xóa hoặc cập nhật danh mục đó.
-	Nếu người dùng bấm vào nút xóa thì danh mục đó sẽ bị xóa khỏi danh sách, nếu nhấn vào nút chỉnh sửa thì màn hình sẽ hiện lên giao diện chỉnh sửa thông tin danh mục cho người dùng.
-	Sau cùng người dùng bấm nút Hoàn thành để lưu lại thông tin đã cập nhật
	![image](https://github.com/Ni2103/Project_Android/assets/89075130/5662958e-620b-4755-90a9-725997e882d1)

# Màn hình thông tin liên hệ
![image](https://github.com/Ni2103/Project_Android/assets/89075130/fb7fcb13-72a1-4e8f-b6a4-ecab80ab640b)
-	Màn hình này sẽ hiện thi thông tin nhóm thực hiện đề tài 
Hiện tại chưa có tính này gì
