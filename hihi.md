# Bài tập số 1: Hệ thống Quản lý Cho thuê Băng đĩa

## 1. Sơ đồ phân rã chức năng (BFD)

```mermaid
graph TD
    A["Hệ thống Quản lý Cho thuê Băng đĩa"] --> B1["1. Quản lý thẻ thuê"]
    A --> B2["2. Quản lý cho thuê"]
    A --> B3["3. Quản lý trả băng đĩa"]
    A --> B4["4. Quản lý báo cáo & khuyến mãi"]

    B1 --> B1_1["1.1. Tiếp nhận thông tin khách hàng"]
    B1 --> B1_2["1.2. Cấp thẻ thuê & Cập nhật CSDL"]

    B2 --> B2_1["2.1. Tiếp nhận yêu cầu thuê & Kiểm tra thẻ"]
    B2 --> B2_2["2.2. Tra cứu thông tin băng đĩa"]
    B2 --> B2_3["2.3. Lập hóa đơn và thanh toán"]

    B3 --> B3_1["3.1. Tiếp nhận yêu cầu trả băng đĩa"]
    B3 --> B3_2["3.2. Tra cứu & Cập nhật dữ liệu trả"]

    B4 --> B4_1["4.1. Lập báo cáo quản lý hàng tháng"]
    B4 --> B4_2["4.2. Gửi thư khuyến mãi hàng năm"]
