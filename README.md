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


