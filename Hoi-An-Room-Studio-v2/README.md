# Hội An Room Studio

Studio nội thất 3D dựng theo ảnh phòng tham chiếu. Kích thước giả định 5,2 × 9 m, cao 3,5 m; không phải bản vẽ đo đạc.

Chạy `python3 -m http.server 5173 --directory dist`, mở http://localhost:5173.

Đổi ba bảng phối màu hoặc từng vật liệu; điều chỉnh giờ và bật/tắt đèn; xoay/zoom, chọn và kéo đồ nội thất, xoay 45°, thêm/xóa và hoàn tác. Các phím mũi tên dịch chuyển đồ đang chọn, R xoay, Delete xóa, Ctrl/Cmd+Z hoàn tác. Xuất ảnh PNG và sao chép link chứa trạng thái thiết kế. Không gửi thiết kế tới backend; trạng thái chỉ nằm trong URL khi người dùng bấm sao chép link.

Three.js 0.183.2 và OrbitControls được giữ cục bộ, theo giấy phép MIT. Font Google có fallback sans-serif/serif. Ảnh gốc do người dùng cung cấp. Mô hình và ứng dụng được viết riêng; không sao chép mã app tham chiếu.

## Bản nâng cấp hình ảnh

17 loại đồ nội thất. Bổ sung mô hình glTF có PBR từ Poly Haven; bo cạnh gỗ, khung ghế mây cong, đệm vải bo mềm và gối có đường viền. Rèm có nếp gấp, gốm có thành trong và miệng bình. Ánh sáng môi trường PMREM, GTAO làm rõ bóng tiếp xúc, khử răng cưa MSAA và tone mapping ACES. Đây là phối cảnh tương tác raster thời gian thực, chưa phải render path tracing của phần mềm kiến trúc. Vật liệu của mô hình nhập được giữ theo asset gốc; bảng phối màu áp dụng cho phòng và các đồ tự dựng.

Mô hình và texture lưu cục bộ. Khoảng 25 MB dữ liệu; tải đầu chậm hơn trên máy yếu.
