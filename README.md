# Phân tích hiệu quả kinh doanh và phân phối thiết bị CNTT

## Giới thiệu

Dự án phân tích dữ liệu kinh doanh của doanh nghiệp phân phối thiết bị CNTT và thiết bị ngoại vi. Dữ liệu bao gồm thông tin đơn hàng, khách hàng, sản phẩm, nhân viên, dự án, nhà cung cấp và tồn kho.

Mục tiêu là đánh giá doanh thu, lợi nhuận, khách hàng, sản phẩm, kênh bán hàng, hoạt động dự án và tồn kho; từ đó xây dựng nền tảng cho dashboard Power BI phục vụ theo dõi hoạt động kinh doanh.

## Mục tiêu

- Đánh giá doanh thu, lợi nhuận và biên lợi nhuận.
- Phân tích xu hướng kinh doanh theo thời gian.
- Phân tích khách hàng theo phân khúc và địa bàn.
- Xác định sản phẩm, kênh bán hàng và nhân viên có đóng góp nổi bật.
- Phân tích doanh thu dự án và tình trạng tồn kho.
- Phát hiện các vấn đề như đơn hủy, tỷ lệ khách hàng quay lại thấp hoặc hàng tồn dưới ngưỡng an toàn.
- Đề xuất các giải pháp.
## Công cụ sử dụng

- **Python:** xử lý và phân tích dữ liệu.
- **Pandas, NumPy:** làm sạch, biến đổi và tổng hợp dữ liệu.
- **Matplotlib, Seaborn:** trực quan hóa và EDA.
- **SQL / PostgreSQL:** truy vấn và quản lý dữ liệu.
- **Power BI:** xây dựng kiến trúc dữ liệu và dashboard.
- **Jupyter Notebook:** lưu quy trình phân tích.
- **GitHub:** quản lý mã nguồn và tài liệu dự án.

## Dữ liệu

Dự án sử dụng các bảng dữ liệu chính:

| Bảng | Nội dung |
|---|---|
| `orders` | Đơn hàng, doanh thu, chi phí, lợi nhuận, trạng thái đơn |
| `customers` | Khách hàng, phân khúc, khu vực, điều khoản thanh toán |
| `products` | Sản phẩm, danh mục, thương hiệu, giá vốn, giá niêm yết |
| `employees` | Nhân viên, phòng ban, chi nhánh |
| `projects` | Dự án, loại dự án, giá trị hợp đồng, trạng thái |
| `suppliers` | Nhà cung cấp |
| `inventory` | Tồn kho theo sản phẩm và kho hàng |

## Quy trình thực hiện

```text
Dữ liệu thô
    ↓
Làm sạch và chuẩn hóa dữ liệu
    ↓
Khám phá dữ liệu (EDA)
    ↓
Phân tích theo câu hỏi nghiệp vụ
    ↓
Rút insight và đề xuất
    ↓
Thiết kế Star Schema
    ↓
Xây dựng dashboard Power BI
```

## Kết quả nổi bật

| Chỉ số | Giá trị |
|---|---:|
| Tổng doanh thu | 40.890.940.000 VNĐ |
| Tổng lợi nhuận | 5.212.958.000 VNĐ |
| Biên lợi nhuận | 12,75% |
| Số đơn hàng | 326 |
| Số khách hàng phát sinh giao dịch | 300 |
| Số sản phẩm phát sinh giao dịch | 106 |
| Số dự án | 35 |
| Doanh thu từ dự án | 10.311.810.000 VNĐ |
| Tỷ trọng doanh thu dự án | 25,22% |
| Doanh thu mất do đơn hủy | 401.930.000 VNĐ |

## Insight chính

- Hoạt động kinh doanh có xu hướng cao điểm vào quý IV, doanh thu cao nhất xuất hiện vào tháng 10/2023 với 3.726.850.000 VNĐ.
- Phân khúc khách hàng Doanh nghiệp là nhóm chủ lực, tạo ra 23.242.150.000 VNĐ doanh thu.
- Hà Nội là thị trường lớn nhất với 22.793.620.000 VNĐ doanh thu.
- Laptop là danh mục tạo doanh thu cao nhất, tiếp theo là Monitor và Desktop.
- Direct Sales là kênh tạo doanh thu và lợi nhuận cao nhất.
- Doanh thu từ dự án chiếm 25,22% tổng doanh thu, Laptop, Desktop và Monitor là các nhóm sản phẩm nổi bật trong đơn hàng dự án.
- Tỷ lệ khách hàng quay lại mới đạt 5,34%, cho thấy cần cải thiện hoạt động chăm sóc sau bán.
- Có 2 lý do hủy đơn chính là hết hàng và khách hàng thay đổi chính sách về ngân sách.

## Đề xuất

- Chuẩn bị tồn kho, nguồn lực bán hàng và chiến dịch tiếp thị từ cuối quý III cho mùa cao điểm quý IV.
- Tập trung giữ chân khách hàng Enterprise và tăng cơ hội bán chéo sản phẩm.
- Mở rộng có chọn lọc tại Hải Phòng, Bắc Ninh, Hưng Yên và Vĩnh Phúc để giảm phụ thuộc vào thị trường Hà Nội.
- Duy trì tồn kho an toàn cho Laptop, Monitor và Desktop.
- Duy trì Direct Sales là kênh trọng tâm do tạo doanh thu và lợi nhuận cao nhất.
- Xây dựng combo Laptop/Desktop với Mouse, Keyboard, Headset hoặc Webcam để tăng giá trị đơn hàng.
- Phân tích phương thức làm việc của nhóm nhân viên có doanh thu cao và xây dựng KPI kết hợp doanh thu, lợi nhuận, khách hàng mới và khách hàng quay lại.
- Giám sát chặt chẽ về vận hành kho và sẵn sàng có biện pháp ứng đối trong trường hợp hàng tồn kho không đủ đáp ứng và cần phải đưa ra những ràng buộc liên quan đến việc thay đổi ngân sách hay hàng hóa và nên có phương pháp đề xuất tránh để tình trạng khách hàng rời bỏ.
- Xây dựng cảnh báo sản phẩm dưới mức tồn kho an toàn hoặc chạm ngưỡng cần đặt hàng lại.
