4 bài toán cốt lõi

Bài toán 1 — Customer Segmentation
Phân khúc khách hàng dựa trên hành vi mua sắm.
- Khách hàng có những đặc điểm mua sắm nào khác biệt?
- Nhóm nào có giá trị cao, mua thường xuyên hoặc lâu chưa quay lại?
- Có thể chia khách hàng thành những phân khúc có ý nghĩa kinh doanh nào?
Đầu ra: Customer Segments và Customer Profiles.




Bài toán 2 — Product Preference Analysis
Xác định sở thích sản phẩm của từng phân khúc.
- Mỗi phân khúc thường mua sản phẩm hoặc ngành hàng nào?
- Những sản phẩm nào đóng góp nhiều vào chi tiêu của từng nhóm?
- Có thể lựa chọn sản phẩm nào để đưa vào chương trình promotion mục tiêu?
Đầu ra: Product Preferences by Segment.




Bài toán 3 — Promotion Effectiveness Analysis
Đánh giá phản ứng của khách hàng đối với các hoạt động promotion.
- Các phân khúc khác nhau như thế nào về hành vi sử dụng và đổi coupon?
- Campaign nào có mức độ phản hồi hoặc hành vi mua hàng liên quan tốt hơn?
- Promotion-associated purchasing khác gì so với các giao dịch còn lại?
Đầu ra: Promotion Performance và Segment Response Analysis.




Bài toán 4 — Promotion Strategy Optimization
Đề xuất chiến lược promotion phù hợp với từng phân khúc khách hàng.
- Nên ưu tiên phân khúc nào cho từng loại promotion?
- Nên áp dụng promotion cho sản phẩm nào trong từng phân khúc?
- Làm thế nào để tránh ưu đãi đại trà và phân bổ nguồn lực marketing hợp lý hơn?
Đầu ra: Segment × Product × Promotion Strategy Matrix.


## Cụ Thể



2. Pillar 1 — Customer Analytics
Mục tiêu: Xác định khách hàng có giá trị như thế nào, hành vi mua sắm ra sao và nên chia thành những nhóm nào.
ID	Business question	Ý nghĩa kinh doanh
BQ1	How does customer purchasing behavior vary across households?	So sánh chi tiêu, tần suất mua và số lượng hàng mua giữa các hộ gia đình.
BQ2	Which customers contribute the most to total sales?	Xác định nhóm khách hàng đóng góp lớn nhất vào doanh số.
BQ3	How can customers be segmented based on purchasing behavior and customer value?	Phân khúc bằng RFM hoặc các đặc trưng hành vi phù hợp.
BQ4	How do customer segments differ in their purchasing patterns and demographic characteristics?	So sánh hành vi mua hàng và đặc điểm nhân khẩu học giữa các phân khúc.
Dữ liệu sử dụng
- transaction_data.csv: lịch sử giao dịch, chi tiêu và hành vi mua hàng.
- hh_demographic.csv: đặc điểm nhân khẩu học của hộ gia đình.
KPI gợi ý
- Total Sales
- Active Households
- Average Spend per Household
- Purchase Frequency
- Recency
- Monetary Value
- Customer Segment Distribution
- Sales Contribution by Segment
Kết quả đầu ra: Customer Segmentation và Segment Profile.
Lưu ý: RFM là phương pháp phân khúc đề xuất, không phải trường dữ liệu có sẵn. Bạn cần tính các đặc trưng từ giao dịch và xác định rõ khoảng thời gian phân tích.
3. Pillar 2 — Product Analytics
Mục tiêu: Xác định sản phẩm và ngành hàng nào được từng phân khúc ưa chuộng, từ đó hỗ trợ lựa chọn sản phẩm cho promotion.
ID	Business question	Ý nghĩa kinh doanh
BQ5	Which products and product categories contribute most to total sales?	Xác định sản phẩm và ngành hàng chủ lực.
BQ6	How do product purchasing patterns differ across customer segments?	Tìm ra sự khác biệt về sở thích sản phẩm giữa các phân khúc.
BQ7	Which products or categories present opportunities for targeted promotions?	Xác định sản phẩm phù hợp để chạy coupon, discount hoặc cross-selling.
Dữ liệu sử dụng
- transaction_data.csv
- product.csv
KPI gợi ý
- Sales by Product / Category
- Quantity Sold
- Product Purchase Frequency
- Category Sales Contribution
- Product Penetration by Segment
- Promotion-associated Sales by Category
Kết quả đầu ra: Product Performance và Product Preference by Segment.
Lưu ý: Nếu dataset không có giá vốn, lợi nhuận hoặc dữ liệu đầy đủ về giá bán thông thường, bạn không nên kết luận sản phẩm nào có lợi nhuận cao nhất hay promotion nào đem lại lợi nhuận cao nhất. Doanh số không đồng nghĩa với lợi nhuận.
4. Pillar 3 — Marketing Analytics
Mục tiêu: Hiểu mức độ sử dụng coupon, phản hồi với campaign và mối liên hệ giữa promotion với hành vi mua sắm.
ID	Business question	Ý nghĩa kinh doanh
BQ8	How do customers respond to different marketing campaigns?	So sánh mức độ tham gia hoặc phản hồi giữa các campaign.
BQ9	How do coupon redemption behaviors differ across customer segments?	Xác định phân khúc nào có xu hướng sử dụng coupon nhiều hơn.
BQ10	How do purchasing patterns differ between promotion-associated and other transactions?	So sánh giá trị, số lượng và hành vi mua trong các giao dịch có thông tin promotion với các giao dịch còn lại.
BQ11	Which campaigns, coupons, or promotion types are associated with stronger customer engagement across segments?	Xác định sự kết hợp giữa phân khúc và hoạt động marketing đáng được ưu tiên nghiên cứu.
Dữ liệu sử dụng
File gốc	Vai trò
campaign_desc.csv	Thông tin mô tả campaign
campaign_table.csv	Hộ gia đình được phân bổ/nhận campaign
coupon.csv	Liên kết coupon với sản phẩm và campaign theo cấu trúc dữ liệu
coupon_redempt.csv	Dữ liệu coupon redemption
causal_data.csv	Thông tin liên quan đến display, mailer và hoạt động promotion theo sản phẩm/cửa hàng/thời gian
transaction_data.csv	Đối chiếu hành vi mua hàng
product.csv	Phân tích promotion theo sản phẩm
KPI gợi ý
- Campaign Reach
- Coupon Redemption Count
- Coupon Redemption Rate
- Average Spend by Segment
- Purchase Rate by Campaign Group
- Promotion-associated Sales
- Campaign Performance by Segment
Kết quả đầu ra: Campaign Performance, Coupon Analysis và Segment × Promotion Analysis.
Có hai điểm cần đặc biệt chú ý:
1. campaign_table.csv thể hiện việc phân bổ campaign đến hộ gia đình không đồng nghĩa với việc hộ gia đình đã phản hồi hoặc mua hàng.
2. Không nên mặc định mọi giao dịch trong thời gian có campaign đều là doanh số do campaign tạo ra. Muốn kết luận tác động tăng thêm cần thiết kế so sánh phù hợp và kiểm soát các yếu tố gây nhiễu.
5. Final Pillar — Promotion Strategy Optimization
Đây không phải một nhóm phân tích độc lập ngang hàng với ba trụ cột. Đây là kết quả tổng hợp của toàn bộ project.
BQ12 — Câu hỏi kinh doanh trung tâm
How can the retailer optimize promotion strategies by matching customer segments with relevant products and marketing offers?

Doanh nghiệp nên lựa chọn chiến lược promotion như thế nào bằng cách kết hợp phân khúc khách hàng, sở thích sản phẩm và phản hồi với hoạt động marketing?