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
# Sơ đồ phân cấp chức năng
![image](https://github.com/Ni2103/Project_Android/assets/89075130/a7e032f3-96d8-485f-bc7b-3aca09edbf0c)

# Đặc tả chức năng của ứng dụng
![image](https://github.com/Ni2103/Project_Android/assets/89075130/840d0597-888a-42e7-9755-c71ee093412e)
# Sơ đồ Use case tổng quát quản lý chi tiêu cá nhân
##	Đặc tả use case tạo tài khoản mới:
###	Luồng sự kiện chuẩn:
	1: Nhập tài khoản và mật khẩu
	2: Hệ thống kiểm tra
	3: Đăng nhập thành công
###	Ngoại lệ:
	Tạo tài khoản không hợp lệ khi trong tài khoản đã tồn tại tài khoản đó. Nếu đã tồn tại yêu cầu tạo tài khoản mới.
##	Đặc tả use case đăng nhập:
###	Luồng sự kiện chuẩn:
	1: Nhập tài khoản và mật khẩu
	2: Hệ thống kiểm tra
	3: Đăng nhập thành công
###	Ngoại lệ:
	Đăng nhập không hợp lệ khi nhập sai tài khoản, mật khẩu hoặc tài khoản đó không tồn tại, hệ thống yêu cầu đăng nhập lại. Nếu chưa có tài khoản cần đăng kí tài khoản mới.
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
![image](https://github.com/Ni2103/Project_Android/assets/89075130/b74f2c92-e9fd-4504-ab63-869b2880b931)
# 	Mô hình dòng dữ liệu mức 1
![image](https://github.com/Ni2103/Project_Android/assets/89075130/98a38926-4d88-4175-8625-d3e00accd834)

#	Mô hình dòng dữ liệu mức 2
- 	Mô hình dòng dữ liệu mức 2 cho ô xử lý 1.0 “Quản lý nguồn thu”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/a6ad5582-1355-43dc-a242-943d56a725fb)
- 	Mô hình dòng dữ liệu mức 2 cho ô xử lý 2.0 “Quản lý khoản chi”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/936be7cc-9802-4051-a94b-3284065b1f21)
- 	Mô hình dòng dữ liệu mức 2 cho ô xử lý 3.0 “Quản lý ví tiền”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/ff41bbd7-be28-4192-a04b-46aa4cdb7618)
-	Mô hình dòng dữ liệu mức 2 cho ô xử lý 4.0 “Quản lý danh mục thu/chi”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/2d2a71c3-300e-4056-ab61-0cb565c0a6e9)
-	Mô hình dòng dữ liệu mức 2 cho ô xử lý 5.0 “Thống kê”
![image](https://github.com/Ni2103/Project_Android/assets/89075130/cae78bee-f649-49d5-9eee-5e1edff22618)
# Mô hình thực thể kết hợp(ERD)
![image](https://github.com/Ni2103/Project_Android/assets/89075130/ee4c6378-25a1-4cad-850b-52c7cb8b1b42)
<img width="372" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/26683333-7670-4e51-afa0-34a17ed44b71">

# XÂY DỰNG CƠ SỞ DỮ LIỆU
<img width="432" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/51328e8f-3701-4eaf-8e21-f8d3d5d45017">
<img width="424" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/2142dd8e-e94c-461e-84a6-a8a8b463beb6">
<img width="430" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/614adcaf-5e96-4c95-b583-00bdabb210be">
<img width="434" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/61713bae-61ff-48f0-b25f-09e5c41857b9">
<img width="425" alt="image" src="https://github.com/Ni2103/Project_Android/assets/89075130/adc37daf-dc59-40fa-8947-4effbd8f1824">


# SƠ ĐỒ TỔ CHỨC GIAO DIỆN
![image](https://github.com/Ni2103/Project_Android/assets/89075130/c44c6678-98b9-4c35-8cba-00dee339a29c)
# Màn hình chào
![image](https://github.com/Ni2103/Project_Android/assets/89075130/39cb5e25-3f87-437a-b59b-43ab9df71765)
-	Đây là màn hình khởi động ứng dụng, bấm vào nút ‘Start’ để bắt đầu sử dụng ứng dụng
# Màn hình giao diện đăng kí
![image](https://github.com/Ni2103/Project_Android/assets/89075130/67ac90c8-9200-4e87-9c3b-8677145cd412)
-	Người dùng mở ứng dụng màn hình đăng nhập sẽ mở lên trước. Nếu người dùng chưa có tài khoản thì bấm vào nút Register để tạo một tài khoản mới, màn hình sẽ chuyển sang giao diện đăng kí tài khoản
-	Sau khi gõ đầy đủ các thông tin, người dùng bấm vào nút Register để đăng kí
-	Sau khi tạo thành công màn hình sẽ hiển thị thống báo đã tạo thành công và chuyển sang giao diện màn hình đăng nhập
# Màn hình giao diện đăng nhập
![image](https://github.com/Ni2103/Project_Android/assets/89075130/e20de5ea-411d-4b58-9e2b-993c52e79f94)
-	Gõ tên đăng nhập và mật khẩu tương ứng
-	Sau khi gõ đầy đủ các thông tin, người dùng bấm vào nút Login
-	Hệ thống sẽ tiến hành kiểm tra thông tin tài khoản đã được tạo trong cơ sở dữ liệu
+	Đăng nhập thành công: nếu thông tin chính xác, người dùng sẽ có thể truy cập được vào màn hình chính của ứng dụng
+	Đăng nhập thất bại: thông tin đăng nhập không chính xác, yêu cầu nhập lại và hiện thông báo “login failed”


# Màn hình trang chủ 
![image](https://github.com/Ni2103/Project_Android/assets/89075130/18145893-fbe6-439f-a57e-88a9388b60be)
-	Tại trang chủ, có thể xem tình hình chi/ tiêu biến động theo ngày
-	Có thể xem danh sách các nguồn tài khoản thu nhập 
-	Các khoản chi đã thêm
-	Ngoài ra, nếu nhấn vào ‘dấu cộng’ ở phía trên màn hình có thể tới giao diện thêm nguồn thu hay là các khoản chi tiêu mới

# Màn hình thống kê
![image](https://github.com/Ni2103/Project_Android/assets/89075130/4cf61852-505c-4bad-8922-552f9f0524da)
-	Tại màn hình này, có thể xem được thống kê các khoản chi tiêu trong ngày hiện tại (nếu có)
-	Xem thống kê thu nhập trong ngày (nếu có) và các khoản chi tiêu 
-	Ngoài ra, nếu nhấn vào ‘dấu cộng’ ở phía trên màn hình có thể tới giao diện thêm nguồn thu hay là các khoản chi tiêu mới.

#  Màn hình thêm nguồn thu/ khoản chi
![image](https://github.com/Ni2103/Project_Android/assets/89075130/497a7335-cab3-4543-8401-523389780c82)
-	Thêm: Hiển thị màn hình thêm mới nguồn thu / khoản chi, cho phép người dùng chọn các danh mục tương ứng cần cần thêm
-	Các danh mục tronng nguồn thu nhập hay khoản chi tiêu sẽ được quản lý trong danh sách danh mục
-	Sau khi thêm nguồn thu nhập hay khoản chi tiêu mới thì giao diện sẽ hiển thị tương ứng với danh mục đã chọn cho phép người dùng nhập vào số tiền tương ứng, ghi chú, thời gian.
-	Bấm lưu để thêm 
+ Trường hợp nếu người dùng không nhập số tiền thì sẽ có thông báo ‘ Bạn không được để trống số tiền’ , khi đó người dùng chưa thể lưu được  và phải cung cấp số tiền tương ứng thì mới hoàn tất thủ tục lưu 

# Màn hình cài đặt
![image](https://github.com/Ni2103/Project_Android/assets/89075130/e7537e6f-177c-436c-831c-e5c1339ab2fc)
-	Tại giao diện cài đặt, người dùng có thể:
+ Xem thông tin ví tiền, thêm ví tiền mới, cập nhật hoặc xóa ví tiền hiện tại
+ Cập nhật loại tiền tệ mới
+ Xem các danh mục tương ứng với nguồn thu hoặc khoản chi. Ngoài ra có thể thêm mới một danh mục tương ứng hoặc cập nhật, xóa một danh mục đã có.
+ Xem thông tin liên hệ, gửi phản hồi cho ứng dụng
+ Đăng xuất khỏi tài khoản hiện tại

# Màn hình thêm ví tiền
![image](https://github.com/Ni2103/Project_Android/assets/89075130/424ae28e-4b10-4bae-a29d-f583b8e06e1d)
-	Khi người dùng nhấn vào ‘dấu cộng’ ở góc phải trên cùng của ứng dụng thì sẽ hiện lên giao diện để thêm ví tiền mới
-	Người dùng nhập tên ví tiền mới, số tiền cho ví tiền đó
+ Trường hợp nếu người dùng không nhập tên ví tiền hay số tiền mà nhấn vào nút “Hoàn thành’ sẽ có một cảnh báo yêu cầu người dùng nhập đầy đủ thông tin 
-	Sau khi nhập đầu đủ, người dùng bấm nút Hoàn tất, màn hình hiện thống báo ‘ví tiền mới được thêm’

 # Màn hình cập nhật/ xóa ví tiền
 ![image](https://github.com/Ni2103/Project_Android/assets/89075130/67f5b588-779c-4cb7-a0a3-87de64a63167)
 -	Nếu người dùng muốn xóa hay chỉnh sửa ví tiền nào thì có thể nhấn vào ví tiền đó. Một sự lựa chọn sẽ hiện ra cho phép xóa hoặc cập nhật ví tiền
-	Nếu người dùng bấm vào nút xóa thì ví tiền đó sẽ bị xóa khỏi danh mục, nếu nhấn vào nút chỉnh sửa thì màn hình sẽ hiện lên giao diện chỉnh sửa thông tin ví tiền cho người dùng
-	Sau cùng người dùng bấm nút Hoàn thành để lưu lại thông tin đã cập nhật
# Màn hình chỉnh sửa loại tiền tệ
![image](https://github.com/Ni2103/Project_Android/assets/89075130/8390946e-92b0-4312-8b55-827104acf976)
-	Người dùng có thể chỉnh sửa loại tiền tệ tương ứng kho nhấn vào mục loại tiền tệ, sau khi chỉnh sửa xong bấm ‘Chỉnh sửa’ để lưu thông tin vừa thay đổi

# Màn hình thêm danh mục mới 
![image](https://github.com/Ni2103/Project_Android/assets/89075130/9492904d-abf8-4f54-8c08-e1f0cdc45287)
-	Tại chức năng Danh mục trong phần Cài đặt, người dùng có thể quản lý tất cả danh sách danh mục nguồn thu và khoản chi của người dùng.  Khi nhấn vào ‘dấu cộng ‘ở góc trên bên phải màn hình, người dùng có thể thêm mới một danh mục tương ứng với nguồn thu hoặc khoản chi.
# Màn hình cập nhật/ xóa danh mục
![image](https://github.com/Ni2103/Project_Android/assets/89075130/55d0eb4c-53c0-4f32-9d49-71a5b6e205d8)
-	Nếu người dùng muốn xóa hay chỉnh sửa danh mục thì có thể nhấn vào danh mục đó. Một sự lựa chọn sẽ hiện ra cho phép xóa hoặc cập nhật danh mục đó.
-	Nếu người dùng bấm vào nút xóa thì danh mục đó sẽ bị xóa khỏi danh sách, nếu nhấn vào nút chỉnh sửa thì màn hình sẽ hiện lên giao diện chỉnh sửa thông tin danh mục cho người dùng.
-	Sau cùng người dùng bấm nút Hoàn thành để lưu lại thông tin đã cập nhật
	![image](https://github.com/Ni2103/Project_Android/assets/89075130/5662958e-620b-4755-90a9-725997e882d1)

# Màn hình thông tin liên hệ
![image](https://github.com/Ni2103/Project_Android/assets/89075130/c43e4ffb-8961-4094-9cf8-e058b45f0d45)
-	Màn hình này sẽ hiện thi thông tin nhóm thực hiện đề tài 
-	Hiện tại tính này chưa được hoàn thiện
