# Bike Sharing Data Analysis

## Giới thiệu
Dự án này thực hiện phân tích dữ liệu dịch vụ xe đạp công cộng nhằm tìm hiểu hành vi người dùng, xu hướng sử dụng và đưa ra các insight giúp cải thiện dịch vụ.

## Dataset
 https://www.kaggle.com/datasets/raymondmutyaba/divvytripdata/data

## Mục tiêu
- Làm sạch và xử lý dữ liệu thô từ nhiều file CSV
- Phân tích sự khác biệt giữa hai nhóm người dùng: **member** (thành viên) và **casual** (khách vãng lai)
- Khám phá xu hướng sử dụng theo thời gian (giờ, ngày trong tuần, tháng)
- Phát hiện các giá trị bất thường (outlier) và xử lý phù hợp
- Trực quan hóa dữ liệu để hỗ trợ việc ra quyết định

## Dữ liệu sử dụng
- Dữ liệu gồm nhiều file CSV từ tháng 10/2020 đến 9/2021
- Các trường chính: `ride_id`, `rideable_type`, `started_at`, `ended_at`, `start_station_name`, `end_station_name`, `start_lat`, `start_lng`, `end_lat`, `end_lng`, `member_casual`

## Các bước phân tích
1. **Tiền xử lý dữ liệu:** Gộp file, xử lý thiếu, loại bỏ trùng lặp, tạo các trường mới (`rental_minutes`, `day_of_week`, `hour`)
2. **Phân tích mô tả:** Thống kê số chuyến đi, thời gian thuê trung bình, phân bố loại xe, phân tích theo nhóm người dùng
3. **Phân tích theo thời gian:** Số chuyến đi theo giờ, ngày trong tuần, tháng; heatmap số chuyến đi theo ngày và giờ
4. **Phân tích theo nhóm:** So sánh member/casual về số lượng, thời gian thuê, hành vi sử dụng
5. **Phân tích địa lý:** (Nếu có) Phân tích các trạm phổ biến, khoảng cách di chuyển
6. **Trực quan hóa dữ liệu:** Boxplot, histogram, countplot, heatmap, v.v.
7. **Tìm insight và tổng hợp:** Đưa ra các phát hiện chính và đề xuất cải tiến dịch vụ

## Kết quả nổi bật
- Phát hiện sự khác biệt rõ rệt giữa member và casual về thời gian thuê, thời điểm thuê xe
- Xác định các khung giờ và ngày cao điểm sử dụng dịch vụ
- Đưa ra các đề xuất giúp tối ưu vận hành và nâng cao trải nghiệm khách hàng
