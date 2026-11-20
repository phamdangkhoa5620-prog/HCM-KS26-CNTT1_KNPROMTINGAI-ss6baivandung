
# XÂY DỰNG CHUỖI PROMPT VIẾT BÀI PR SẢN PHẨM CÔNG NGHỆ BẰNG PROMPT CHAINING

## 1. Mục tiêu

- Thành thạo Prompt Chaining để xử lý tác vụ phức tạp qua nhiều công đoạn.
- Biết cách truyền và kế thừa ngữ cảnh (Context) giữa các prompt.
- Xây dựng quy trình viết bài PR chuyên nghiệp, chuyên sâu, hạn chế lặp ý.
- Biết cách xử lý khi AI bị ngắt do giới hạn Token bằng Continue Prompting.
- Đảm bảo nội dung nhất quán về cấu trúc, thông điệp và giọng văn.

## 2. Bối cảnh bài toán

Phòng Marketing cần viết bài PR dài 1.000–1.500 từ giới thiệu sản phẩm AI Chatbot doanh nghiệp.

Nếu sử dụng một prompt duy nhất, AI có thể gặp các vấn đề:
- Nội dung hời hợt, thiếu chiều sâu.
- Lặp ý giữa các phần.
- Xác định sai đối tượng khách hàng.
- Dàn ý thiếu logic.
- Tối ưu SEO chưa tốt.
- Bị ngắt nội dung khi vượt giới hạn Token.

**Giải pháp:** Sử dụng Prompt Chaining gồm 3 bước liên kết. Đầu ra của bước trước là đầu vào bắt buộc của bước tiếp theo.

## 3. Thiết kế quy trình Prompt Chaining

### Bước 1: Nghiên cứu khách hàng mục tiêu và Pain Points

- **Role:** Chuyên gia nghiên cứu thị trường và phân tích khách hàng công nghệ.
- **Input:** Thông tin sản phẩm AI Chatbot:
  - Tự động trả lời khách hàng.
  - Tư vấn sản phẩm.
  - Chăm sóc khách hàng 24/7.
  - Phân tích dữ liệu tương tác.
  - Tích hợp hệ thống doanh nghiệp.
- **Đối tượng:** Doanh nghiệp vừa và nhỏ, thương mại điện tử, bộ phận chăm sóc khách hàng.

**Process:**
1. Xác định nhóm khách hàng mục tiêu.
2. Phân tích đặc điểm và hành vi khách hàng.
3. Xác định ít nhất 5 Pain Points, nguyên nhân và hậu quả.
4. Đề xuất tính năng giải quyết từng vấn đề.
5. Xác định lợi ích nổi bật của sản phẩm.

**Output format:**
- `CUSTOMER_PROFILE`
- `PAIN_POINTS`
- `VALUE_PROPOSITION`

**Constraints:**
- Phân tích thực tế, logic.
- Không tự tạo số liệu chưa được xác minh.
- Sử dụng giọng văn chuyên nghiệp.
- Trình bày rõ ràng để làm đầu vào cho Prompt 2.

**Đầu ra bước 1:**

- Khách hàng mục tiêu: Doanh nghiệp vừa và nhỏ, doanh nghiệp thương mại điện tử.
- Nhu cầu: Tăng tốc độ phản hồi, giảm chi phí, nâng cao trải nghiệm khách hàng.
- Pain Points:
  1. Nhân viên CSKH quá tải.
  2. Khách hàng phải chờ đợi lâu.
  3. Chi phí nhân sự cao.
  4. Khó quản lý và phân tích dữ liệu.
  5. Bỏ lỡ khách hàng ngoài giờ làm việc.
- Giải pháp: Tự động hóa tư vấn, hỗ trợ 24/7, quản lý dữ liệu và phân tích tương tác.
- Giá trị: Tiết kiệm chi phí, tăng hiệu suất và cải thiện trải nghiệm khách hàng.

### Bước 2: Xây dựng dàn ý bài PR (Outline)

- **Role:** Chuyên gia Content Marketing và SEO công nghệ.
- **Input:** Toàn bộ kết quả từ Prompt 1.

**Process:**
1. Phân tích Customer Profile và Pain Points.
2. Xác định thông điệp chính.
3. Xây dựng tiêu đề hấp dẫn.
4. Viết đoạn mở đầu (Lead).
5. Xây dựng hệ thống H2/H3.
6. Đề xuất từ khóa SEO.
7. Sắp xếp nội dung theo trình tự: Thực trạng → Giải pháp → Tính năng → Lợi ích → Ứng dụng → CTA.

**Output format:**
- `CONTENT_STRATEGY`
- `SEO_KEYWORDS`
- `ARTICLE_OUTLINE`

**Constraints:**
- Dàn ý logic, có sự liên kết.
- Mỗi tiêu đề có mục tiêu riêng.
- Không lặp ý giữa các phần.
- Nội dung bám sát Pain Points.
- Phù hợp bài viết dài 1.000–1.500 từ.
- Có thể sử dụng trực tiếp cho Prompt 3.

**Đầu ra bước 2:**

- **Tiêu đề:** AI Chatbot doanh nghiệp – Giải pháp tự động hóa chăm sóc khách hàng trong thời đại số.
- **Lead:** Giới thiệu những khó khăn trong chăm sóc khách hàng và nhu cầu tự động hóa của doanh nghiệp.

**Hệ thống nội dung:**

- **H2.1: Thách thức trong chăm sóc khách hàng hiện nay**
  - H3: Nhân viên quá tải, chi phí vận hành cao.
  - H3: Khách hàng phải chờ đợi lâu.

- **H2.2: AI Chatbot – Giải pháp tự động hóa**
  - H3: Tự động trả lời và tư vấn khách hàng.
  - H3: Hỗ trợ khách hàng 24/7.

- **H2.3: Lợi ích nổi bật của AI Chatbot**
  - H3: Tiết kiệm chi phí và nhân lực.
  - H3: Nâng cao trải nghiệm khách hàng.
  - H3: Phân tích dữ liệu kinh doanh.

- **H2.4: Ứng dụng AI Chatbot trong doanh nghiệp**
  - H3: Ứng dụng trong thương mại điện tử.
  - H3: Ứng dụng trong dịch vụ và chăm sóc khách hàng.

- **CTA:** Đăng ký tư vấn và trải nghiệm giải pháp AI Chatbot doanh nghiệp.

### Bước 3: Triển khai bài viết PR và tối ưu SEO

- **Role:** Chuyên gia Content Marketing và SEO có kinh nghiệm viết bài PR công nghệ.
- **Input:** Toàn bộ kết quả Prompt 1 và Prompt 2.

**Requirements:**
1. Viết bài dài 1.000–1.500 từ.
2. Có tiêu đề hấp dẫn, đúng chủ đề.
3. Lead tập trung giải quyết Pain Points.
4. Đầy đủ các mục H2/H3 theo dàn ý.
5. Phân tích rõ tính năng và lợi ích sản phẩm.
6. Sử dụng từ khóa SEO tự nhiên.
7. Có ví dụ minh họa thực tế.
8. Có CTA rõ ràng, thuyết phục.

**Yêu cầu SEO:**
- Từ khóa chính xuất hiện trong tiêu đề, Lead và nội dung.
- Từ khóa phụ được phân bổ tự nhiên trong H2/H3.
- Không nhồi nhét từ khóa.
- Meta Description dài 150–160 ký tự.
- Nội dung dễ đọc, dễ hiểu.

**Context consistency:**
- Giữ nguyên đối tượng khách hàng.
- Không thay đổi thông điệp chính.
- Giữ nguyên cấu trúc và thứ tự tiêu đề.
- Duy trì giọng văn chuyên nghiệp.
- Không tự thêm thông tin hoặc số liệu chưa được xác minh.

**Output format:**
1. SEO Title.
2. Meta Description.
3. Headline.
4. Lead.
5. Nội dung H2/H3.
6. CTA.

**Constraints:**
- Không bỏ sót nội dung trong dàn ý.
- Không lặp ý giữa các phần.
- Không viết nội dung chung chung.
- Nếu thiếu dữ liệu sản phẩm, phải ghi rõ thông tin cần bổ sung.
- Nếu vượt giới hạn Token, dừng ở cuối đoạn hoàn chỉnh và thông báo vị trí đã dừng.

## 4. Quy trình truyền dữ liệu giữa các Prompt

Quy trình thực hiện:

```text
PROMPT 1
Nghiên cứu khách hàng và Pain Points
        |
        v
CUSTOMER_PROFILE
PAIN_POINTS
VALUE_PROPOSITION
        |
        v
PROMPT 2
Xây dựng chiến lược nội dung và dàn ý
        |
        v
CONTENT_STRATEGY
SEO_KEYWORDS
ARTICLE_OUTLINE
        |
        v
PROMPT 3
Viết bài PR hoàn chỉnh và tối ưu SEO
        |
        v
BÀI PR HOÀN CHỈNH
1.000–1.500 TỪ
```

**Nguyên tắc truyền Context:**
- Không bỏ qua đầu ra của prompt trước.
- Không tự ý thay đổi khách hàng mục tiêu.
- Giữ nguyên thông điệp, cấu trúc và giọng văn.
- Nếu thông tin giữa các bước mâu thuẫn, yêu cầu xác nhận trước khi tiếp tục.
- Luôn sử dụng kết quả bước trước làm dữ liệu đầu vào cho bước sau.

## 5. Xử lý lỗi đứt gãy ngữ cảnh khi đạt giới hạn Token

Sử dụng kỹ thuật **Continue Prompting** để yêu cầu AI tiếp tục viết chính xác từ vị trí đã dừng.

**Các yêu cầu khi tiếp tục:**
- Giữ nguyên chủ đề, mục tiêu và giọng văn.
- Tuân thủ dàn ý H2/H3 ban đầu.
- Không viết lại nội dung đã hoàn thành.
- Không lặp lại tiêu đề hoặc đoạn văn trước.
- Tiếp tục đúng vị trí đang viết.
- Duy trì từ khóa SEO.
- Đảm bảo tổng bài viết đạt 1.000–1.500 từ.

**Thông tin cần cung cấp cho AI:**
1. Nội dung đã hoàn thành.
2. Tiêu đề cuối cùng đã viết xong.
3. Vị trí cần tiếp tục.
4. Đoạn cuối của phản hồi trước.
5. Dàn ý ban đầu để duy trì ngữ cảnh.

**Mẫu Continue Prompting:**

```text
Hãy tiếp tục viết bài PR AI Chatbot doanh nghiệp
từ chính xác vị trí đã dừng ở phản hồi trước.

Yêu cầu:
- Giữ nguyên chủ đề và giọng văn chuyên nghiệp.
- Tuân thủ dàn ý H2/H3 ban đầu.
- Không viết lại nội dung đã hoàn thành.
- Không lặp lại tiêu đề hoặc đoạn văn trước.
- Tiếp tục từ phần nội dung còn thiếu.
- Duy trì từ khóa SEO tự nhiên.
- Đảm bảo tổng bài viết đạt 1.000–1.500 từ.

Nội dung đã hoàn thành:
[DÁN NỘI DUNG ĐÃ VIẾT]

Tiêu đề cuối cùng:
[DÁN TIÊU ĐỀ CUỐI]

Vị trí cần tiếp tục:
[GHI RÕ PHẦN CẦN VIẾT TIẾP]

Đoạn cuối phản hồi trước:
[DÁN ĐOẠN CUỐI]

Chỉ viết tiếp phần còn thiếu.
```

**Nguyên tắc xử lý:**
- Lưu lại nội dung đã hoàn thành trước khi tiếp tục.
- Cung cấp lại dàn ý nếu AI mất ngữ cảnh.
- Xác định chính xác tiêu đề và đoạn cuối.
- Không yêu cầu AI viết lại phần đã xong.
- Kiểm tra sự liên kết giữa phần cũ và phần mới.

## 6. Kiểm tra và đánh giá kết quả

Sử dụng các tiêu chí sau để đánh giá chất lượng bài PR:

- **Độ dài:** Đạt 1.000–1.500 từ.
- **Tiêu đề:** Hấp dẫn, đúng chủ đề và có từ khóa chính.
- **Nội dung:** Đầy đủ, chuyên sâu, giải quyết đúng Pain Points.
- **Cấu trúc:** Có H1, H2, H3 rõ ràng, logic.
- **SEO:** Có từ khóa chính, từ khóa phụ và Meta Description.
- **Giọng văn:** Chuyên nghiệp, dễ hiểu, đáng tin cậy.
- **Tính nhất quán:** Không thay đổi đối tượng và thông điệp.
- **CTA:** Rõ ràng, có tính thuyết phục.
- **Context:** Không mất hoặc sai lệch ngữ cảnh giữa các bước.
- **Tính chính xác:** Không tự tạo số liệu hoặc thông tin sản phẩm.

## 7. Kết luận

Prompt Chaining giúp chia một nhiệm vụ phức tạp thành nhiều công đoạn nhỏ có liên kết và kế thừa dữ liệu.

- **Prompt 1:** Nghiên cứu khách hàng mục tiêu và xác định Pain Points.
- **Prompt 2:** Xây dựng chiến lược nội dung, từ khóa SEO và dàn ý bài PR.
- **Prompt 3:** Viết bài PR hoàn chỉnh, chuyên sâu và tối ưu SEO.

Kết hợp với **Continue Prompting** giúp xử lý tình trạng AI bị ngắt do giới hạn Token, duy trì ngữ cảnh và hạn chế lặp nội dung.

**Kết quả đạt được:** Xây dựng quy trình viết bài PR sản phẩm công nghệ chuyên nghiệp, có cấu trúc rõ ràng, nội dung chuyên sâu, chuẩn SEO và đảm bảo tính nhất quán từ đầu đến cuối.
