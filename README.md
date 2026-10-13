Phân tích lỗi & Lập bảng Test Cases (trình bày trong README.md):
Đọc hiểu mã nguồn, xác định dòng lệnh sai logic và phân tích nguyên nhân kỹ thuật dẫn đến sự cố nghiệp vụ.
- khi sử dụng cấu trúc if (prop) thì các trường hợ, như 0, false, "", null, undefined thì đều cho giá trị falsy. ở bài trên nếu sự dụng cấu trúc if (prop) sẽ dẫn đến sai nếu ng dùng nhập isActive: false thì nó sẽ nhận giá trị sai.
Lập bảng 02 Test Cases đối chứng gồm các cột: Trường hợp kiểm thử, Dữ liệu đầu vào, Kết quả sai thực tế, Kết quả đúng mong đợi.

Trường hợp kiểm thử: Cập nhật trạng thái false
Dữ liệu đầu vào: updatedData.isActive = false
Kết quả sai thực tế: vẫn giá trị cũ vì bị bỏ qua
Kết quả đúng mong đợi: targetDevice.isActive =false

Trường hợp kiểm thử: Cập nhật công suất về 0
Dữ liệu đầu vào: updatedData.powerWatts = 0
Kết quả sai thực tế: vẫn giá trị cũ vì bị bỏ qua
Kết quả đúng mong đợi: targetDevice.powerWatts = 0

