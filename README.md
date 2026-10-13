# [Sáng tạo -5] THIẾT KẾ CƠ CHẾ THEO DÕI KẾ HOẠCH SPRINT CHO ĐỘI RIKKEIGO

Với vai trò Lan (Scrum Master), tôi thiết kế cơ chế theo dõi kế hoạch Sprint cho đội RikkeiGo như sau:

## Phần 1 - Thiết kế cơ chế theo dõi kế hoạch Sprint

### Mục tiêu của cơ chế:
*   Phát hiện sớm rủi ro, đặc biệt là nguy cơ không đạt Sprint Goal trước ngày cuối Sprint.
*   Cung cấp căn cứ thực tế để đội RikkeiGo quyết định số Story Point (SP) sẽ cam kết trong Sprint Planning.
*   Đảm bảo không sử dụng Velocity hay Burndown làm KPI hoặc để so sánh giữa các đội.
*   Là cơ chế ngắn gọn, dễ duy trì và tái sử dụng cho mọi Sprint.

### Cơ chế theo dõi Sprint cho đội RikkeiGo:
Tôi thiết kế cơ chế gồm 4 thành phần chính, giúp Đức (Product Owner) và Developers theo dõi và ra quyết định hiệu quả.

#### 1. Bảng Tính toán Capacity (Capacity Calculator)
*   **Dữ liệu đầu vào:** Số ngày làm việc thực tế của từng Developer trong Sprint (trừ nghỉ phép, đào tạo), ước lượng phần trăm thời gian tập trung cho công việc của Sprint (Focus Factor).
*   **Ai cập nhật:** Developers (tự nguyện đóng góp thông tin về ngày nghỉ/cam kết ngoài Sprint), Scrum Master (tổng hợp).
*   **Khi nào:** Trước buổi Sprint Planning của mỗi Sprint.
*   **Giúp đội quyết định gì:** Cung cấp cái nhìn thực tế về "nguồn lực" có thể dành cho Sprint, giúp Developers và Product Owner ước lượng một cách hợp lý về khối lượng công việc có thể hoàn thành, từ đó đưa ra con số Story Point phù hợp cho Sprint. Điều này giúp tránh tranh luận vô căn cứ về số SP.

#### 2. Lịch sử Velocity của đội
*   **Dữ liệu đầu vào:** Tổng số Story Point của các Product Backlog Item (PBI) đã "Done" theo Definition of Done (DoD) vào cuối mỗi Sprint.
*   **Ai cập nhật:** Scrum Master.
*   **Khi nào:** Cuối mỗi Sprint (trong Sprint Review hoặc Retrospective).
*   **Giúp đội quyết định gì:** Cung cấp dữ liệu lịch sử về khả năng hoàn thành công việc của đội. Kết hợp với Capacity, đội có thể dự báo một khoảng Story Point khả thi cho Sprint sắp tới. Điều này tạo căn cứ vững chắc cho việc chọn số SP trong Sprint Planning mà không biến Velocity thành chỉ tiêu so sánh.

#### 3. Biểu đồ Burndown Sprint
*   **Dữ liệu đầu vào:** Tổng số Story Point còn lại của các Product Backlog Item trong Sprint Backlog.
*   **Ai cập nhật:** Developers.
*   **Khi nào:** Hằng ngày tại Daily Scrum.
*   **Giúp đội quyết định gì:** Theo dõi tiến độ hoàn thành công việc của Sprint Backlog so với đường lý tưởng. Giúp Developers sớm nhận biết các chướng ngại vật (impediments) hoặc tình trạng chậm trễ, từ đó chủ động điều chỉnh kế hoạch trong Sprint để đạt Sprint Goal. Đây là công cụ chính để phát hiện rủi ro trước ngày cuối Sprint.

#### 4. Nhật ký thay đổi Sprint Backlog (Sprint Backlog Change Log)
*   **Dữ liệu đầu vào:** Bất kỳ Product Backlog Item nào được thêm, bớt hoặc thay đổi phạm vi trong Sprint Backlog sau Sprint Planning.
*   **Ai cập nhật:** Product Owner (khi thay đổi PBI), Scrum Master (ghi nhận và đảm bảo sự minh bạch).
*   **Khi nào:** Mỗi khi có sự thay đổi về phạm vi của Sprint Backlog.
*   **Giúp đội quyết định gì:** Đảm bảo mọi thay đổi đều được ghi lại với lý do rõ ràng và được xem xét dưới ánh sáng của Sprint Goal. Nếu một PBI bị loại bỏ hoặc thêm vào, lý do phải liên quan đến việc đạt được Sprint Goal. Điều này giúp đội tập trung vào Sprint Goal và không bị phân tâm bởi các yêu cầu phát sinh không liên quan. Nó cũng giúp theo dõi sự ổn định của Sprint Backlog.

### Giải quyết 3 vấn đề lặp lại của đội RikkeiGo:

1.  **Đến ngày cuối Sprint mới biết Sprint Goal không đạt:**
    *   **Giải pháp:** Biểu đồ Burndown Sprint (thành phần 3) và Daily Scrum. Burndown cung cấp cái nhìn trực quan, cập nhật hằng ngày về tiến độ. Nếu đường Burndown không giảm hoặc giảm chậm hơn dự kiến, Developers sẽ phát hiện sớm tại Daily Scrum và có thể điều chỉnh kế hoạch hoặc báo cáo impediment cho Scrum Master. Nhật ký thay đổi Sprint Backlog (thành phần 4) cũng giúp giữ Sprint Goal làm điểm tham chiếu.

2.  **Mỗi buổi Sprint Planning lại tranh luận nên nhận bao nhiêu Story Point (SP):**
    *   **Giải pháp:** Bảng Tính toán Capacity (thành phần 1) và Lịch sử Velocity của đội (thành phần 2). Capacity cung cấp cái nhìn về nguồn lực thực tế, Velocity cung cấp dữ liệu lịch sử về khả năng hoàn thành. Kết hợp hai dữ liệu này, đội có thể đưa ra một khoảng SP hợp lý và có căn cứ để cam kết, giảm bớt tranh luận và tăng tính thực tế cho kế hoạch Sprint.

3.  **Quản lý muốn dùng Velocity để xếp hạng đội này với đội phát triển ứng dụng tài xế:**
    *   **Giải pháp:** Cơ chế được thiết kế để sử dụng Velocity (thành phần 2) chỉ như một công cụ nội bộ của đội để dự báo và cải thiện. Quy tắc nghiệp vụ số 3 ("Không dùng Velocity hay Burndown làm Key Performance Indicator (KPI) hoặc để so sánh các đội") là cốt lõi. Tôi sẽ dùng thông tin từ Nhật ký thay đổi Sprint Backlog (thành phần 4) và kết quả của Sprint Review (không phải là thành phần của cơ chế theo dõi nhưng là sự kiện của Scrum) để cung cấp cho quản lý các chỉ số phù hợp hơn. (Chi tiết sẽ được trình bày ở Phần 2)

### Tuân thủ quy tắc nghiệp vụ (mục 3):

*   **Không quy đổi SP sang giờ; không dùng Velocity hay Burndown làm Key Performance Indicator (KPI) hoặc để so sánh các đội:** Đã được thiết kế rõ ràng trong mục đích của Velocity và Burndown, chỉ dùng làm công cụ nội bộ để hỗ trợ dự báo và theo dõi tiến độ. Tôi, với vai trò Lan (Scrum Master), sẽ truyền đạt điều này và đảm bảo đội tuân thủ.
*   **Sprint Goal là điểm tham chiếu khi quyết định giữ, đổi hay bỏ bớt phạm vi trong Sprint:** Đã được tích hợp trong Nhật ký thay đổi Sprint Backlog, nơi mọi thay đổi phải được xem xét qua lăng kính Sprint Goal.
*   **Cơ chế gồm 3–4 thành phần để đội duy trì được mỗi Sprint:** Đã thiết kế 4 thành phần, tất cả đều đơn giản và dễ duy trì hằng ngày/hằng Sprint.

## Phần 2 - Xử lý tình huống

### Tình huống 1: Ngày 4–6 của một Sprint, Burndown nằm ngang dù Developers vẫn làm đủ giờ.

*   **Cơ chế phát hiện và phản ứng:**
    *   **Phát hiện:** Tại buổi Daily Scrum vào ngày thứ 5 hoặc thứ 6, Developers sẽ xem biểu đồ Burndown Sprint và nhận thấy đường Burndown không giảm trong 2-3 ngày liên tiếp, mặc dù mọi người vẫn đang làm việc.
    *   **Giả thuyết kiểm chứng được:** Có thể các Task quá lớn nên chưa Product Backlog Item (PBI) nào đạt trạng thái "Done"; Developers đang làm dở quá nhiều PBI cùng lúc mà chưa hoàn thành dứt điểm PBI nào; hoặc đội đang chờ một yếu tố bên ngoài (như phản hồi từ bên thứ 3, môi trường test chưa sẵn sàng).
    *   **Điều chỉnh dựa trên Sprint Goal:** Đội cần thảo luận tại Daily Scrum để tìm ra nguyên nhân và đưa ra giải pháp. Nếu các Task quá lớn, Developers cần chia nhỏ hơn để có thể "Done" PBI sớm hơn. Nếu làm dở quá nhiều, cần tập trung hoàn thành từng PBI một. Nếu do yếu tố bên ngoài, Scrum Master cần hỗ trợ gỡ bỏ trở ngại (impediment). Nếu có PBI không còn đóng góp trực tiếp vào Sprint Goal, Product Owner có thể xem xét việc loại bỏ nó để giảm phạm vi và tăng khả năng đạt được Sprint Goal của các PBI còn lại.

### Tình huống 2: Sprint tới, 2 trong 4 Developers nghỉ mỗi người 3 ngày, Capacity giảm khoảng 15%.

*   **Ghi nhận thay đổi Capacity trước Sprint Planning:**
    *   Thông tin về ngày nghỉ của 2 Developers sẽ được ghi nhận vào Bảng Tính toán Capacity trước buổi Sprint Planning. Với 2/4 Developers nghỉ mỗi người 3 ngày trong Sprint (giả sử Sprint 10 ngày làm việc), tổng số ngày làm việc của đội giảm đi 6 ngày. Nếu trước đây đội có 4 Developers * 10 ngày = 40 ngày làm việc khả dụng, nay còn 40 - 6 = 34 ngày. Tỷ lệ giảm là (6/40) * 100% = 15%.
*   **Điều chỉnh dự báo từ chuỗi Velocity (18, 20, 19, 15, 13 SP):**
    *   Velocity trung bình của 5 Sprint gần nhất: (18+20+19+15+13) / 5 = 17 SP.
    *   Tuy nhiên, ta thấy Velocity có xu hướng giảm nhẹ trong 2 Sprint gần đây (15, 13 SP). Việc giảm Capacity 15% là một yếu tố đáng kể. 
    *   Với Capacity giảm 15% và xu hướng Velocity giảm, dự báo Story Point cho Sprint tới sẽ thấp hơn đáng kể so với trung bình và cả 2 Sprint gần nhất. Thay vì trừ máy móc 15% từ Velocity trung bình hoặc từ Sprint gần nhất, đội nên thận trọng hơn. Một dự báo hợp lý có thể nằm trong khoảng **11-13 SP**. Điều này thấp hơn hai Sprint gần nhất (15 và 13 SP), phản ánh sự suy giảm đáng kể về Capacity và duy trì sự thận trọng trước xu hướng.
*   **Nêu giả định:**
    *   Giả định rằng năng suất làm việc của các Developers còn lại (hoặc trong những ngày làm việc của 2 Developers nghỉ) vẫn giữ nguyên như cũ.
    *   Không có sự cố lớn, trở ngại nghiêm trọng hoặc yêu cầu khẩn cấp phát sinh trong Sprint làm ảnh hưởng thêm đến năng suất.

### Tình huống 3: Trả lời đề nghị xếp hạng đội theo Velocity của quản lý.

*   **Vì sao không so sánh Velocity giữa hai đội (đội RikkeiGo và đội phát triển ứng dụng tài xế):**
    *   Mỗi đội có một "Reference Story" và cách ước lượng Story Point (SP) riêng, dựa trên kinh nghiệm, ngữ cảnh sản phẩm, và sự hiểu biết về độ phức tạp/rủi ro của riêng đội mình. Điều này khiến SP không phải là một đơn vị đo lường tuyệt đối và không thể so sánh chéo giữa các đội khác nhau.
    *   Việc so sánh Velocity và xếp hạng các đội sẽ tạo áp lực và khuyến khích hành vi không mong muốn, như "thổi phồng" SP để trông có vẻ "năng suất" hơn, dẫn đến mất đi ý nghĩa thực sự của SP là một công cụ ước lượng nội bộ.
*   **Thông tin phù hợp hơn để quản lý theo dõi đội:**
    *   Thay vì Velocity, quản lý có thể tập trung vào các chỉ số liên quan đến giá trị kinh doanh và chất lượng sản phẩm. Các thông tin phù hợp hơn bao gồm:
        *   **Tỷ lệ đạt Sprint Goal:** Cho biết đội có thường xuyên hoàn thành mục tiêu đề ra trong Sprint không.
        *   **Tính năng đã phát hành (Features Released):** Số lượng các tính năng có giá trị đã được đưa ra thị trường hoặc người dùng cuối.
        *   **Phản hồi của khách hàng:** Mức độ hài lòng của khách hàng đối với sản phẩm/tính năng đã phát triển.
        *   **Số lỗi sau phát hành (Defects Post-Release):** Chất lượng của sản phẩm được bàn giao.
        *   **Thời gian đưa ra thị trường (Time to Market):** Thời gian từ khi một ý tưởng được chấp nhận đến khi nó đến tay người dùng.
    *   Các chỉ số này cung cấp một cái nhìn toàn diện hơn về hiệu suất của đội trong việc tạo ra giá trị kinh doanh, thay vì chỉ tập trung vào một con số ước lượng nội bộ.