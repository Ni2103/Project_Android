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

