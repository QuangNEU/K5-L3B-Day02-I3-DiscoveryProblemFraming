# Phần cá nhân (của Quang)

## 2. Scan problem (CP1)

Quang scan 5 problem, đạt mức tối thiểu 5.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận được tài liệu môn học hoặc requirement đồ án dài nhiều trang, tôi muốn có ngay một bản tóm tắt các ý chính và phần việc cần làm, để nắm bắt yêu cầu nhanh chóng mà không phải cày từng chữ | Bản thân tôi, Nhóm làm bài tập | Mất trung bình 45–60 phút để đọc hiểu một tài liệu môn học/công nghệ mới, tần suất 2–3 lần/tuần |
| 2 | Pain từ người khác | Khi các bạn trong nhóm cần tập trung cao độ để code hoặc làm đồ án, họ muốn hạn chế và chặn xao nhãng từ điện thoại, để không bị đứt mạch suy nghĩ và tránh kéo chậm tiến độ chung | Bạn học, Thành viên nhóm đồ án, Cả nhóm | 3/4 bạn trong nhóm liên tục than phiền trên nhóm chat vì mất 1.5–2 tiếng lướt mạng xã hội lúc học; 2 tuần gần nhất có 2 bạn trễ deadline task nhóm do mất tập trung |
| 3 | Lặp lại | Khi cần ôn tập lại thuật toán trước kỳ phỏng vấn, tôi muốn thống kê nhanh các dạng bài (DP, Graph, v.v.) hay làm sai hoặc tốn nhiều thời gian, để tối ưu việc luyện tập thay vì dò lại lịch sử giải bài từ đầu | Bản thân tôi | Tốn 30–45 phút mỗi cuối tuần lướt lại lịch sử submit trên LeetCode/HackerRank để tự note lại các bài cần làm lại |
| 4 | Tốn thời gian | Khi hệ thống báo lỗi liên quan đến luồng dữ liệu realtime, tôi muốn gom toàn bộ log từ backend (framework, database, cache) về một màn hình theo thứ tự thời gian, để tra cứu nguyên nhân chéo nhanh chóng thay vì mở từng tab terminal lẻ tẻ | Bản thân tôi, Team Backend | Mất trung bình 45–60 phút mò mẫm log mỗi khi fix bug liên quan đến đồng bộ dữ liệu; xảy ra 1–2 lần/tuần |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi kết thúc chuyến đi dài và nghe xong các podcast, tôi muốn có ngay các gạch đầu dòng từ khóa và kiến trúc cốt lõi vừa được nhắc tới, để lưu vào não và note cá nhân mà không phải tua lại audio để chép | Bản thân tôi | Dành 2–3 tiếng/ngày trên xe buýt nghe kỹ thuật nhưng thường quên khoảng 40% chi tiết nếu không mở máy tính ghi chép lại ngay lúc đó |

**AI gợi ý thêm:** Sau khi tự scan các ý đầu, Quang hỏi AI gợi ý qua 4 lăng kính và giữ lại ý #4 và #5. Bỏ qua các ý tưởng giải pháp AI quá rộng như "trợ lý học tập toàn năng" vì thiếu quy trình thật.

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tóm tắt tài liệu môn học / requirement (#1) | Quy trình rõ, tốn thời gian cày cuốc, impact trực tiếp tới việc học và tiến độ làm đồ án của nhóm | Chất lượng tóm tắt có đủ sâu không, sợ sót edge case |
| 2 | Gom log realtime tra cứu bug (#4) | Pain thật, tốn thời gian dò thủ công chéo các tab, lặp lại mỗi khi code backend | Có dễ truy cập và gom luồng log liên tục tự động không? Hay chỉ cần code Rule là đủ? |
| 3 | Tóm tắt kiến thức từ Podcast (#5) | Lặp lại hằng ngày (đi xe buýt 2-3 tiếng), dễ đo lường kết quả | AI có nhận diện và hiểu đúng các thuật ngữ chuyên ngành (System Design) không? |

---

### Problem Card #1 — Tóm tắt tài liệu môn học / requirement đồ án

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận được tài liệu môn học hoặc requirement đồ án dài nhiều trang, tôi muốn có ngay một bản tóm tắt các ý chính và phần việc cần làm, để nắm bắt yêu cầu nhanh chóng mà không phải cày từng chữ. |
| Actor | Sinh viên IT (Tôi) / Trưởng nhóm đồ án |
| Thời điểm / bối cảnh | Lúc bắt đầu sprint mới hoặc nhận đề bài môn học/đồ án mới (tài liệu dài 10-20 trang). |
| Quy trình hiện tại | 1. Tải tài liệu (PDF/Doc) · 2. Đọc lướt mục lục · 3. Đọc chi tiết từng phần · 4. Highlight & trích xuất yêu cầu · 5. Chia task cho nhóm |
| Bottleneck | Bước 3 và 4 (Đọc chi tiết và trích xuất yêu cầu): khoảng 45 phút, dễ mất tập trung và sót ý. |
| Impact | 60 phút/tài liệu; tuần có 2-3 tài liệu tốn khoảng 3 tiếng; các thành viên trong nhóm phải chờ đợi để hiểu đề bài. |
| Success metric | Tổng thời gian đọc và lọc task từ 60 phút xuống dưới 15 phút, số lượng task bị hiểu sai yêu cầu = 0. |
| Phương án không dùng AI | Dùng highlight PDF truyền thống hoặc xin giảng viên/người giao đề cung cấp checklist (rất khó vì giảng viên thường đưa tài liệu dài). Chưa giảm được thời gian tự đọc. |
| Giả thuyết về AI | Đưa tài liệu vào AI rút trích ý chính, action items. Tôi review, đối chiếu với bản gốc trước khi chia task. |
| Cảm nhận nhanh | Workflow |

**Quy trình nháp hiện tại — 60 phút:**
> [1 Tải tài liệu: 2'] → [2 Đọc lướt mục lục: 3'] → [3 Đọc chi tiết: 30'] ← BOTTLENECK 
> → [4 Highlight & lọc yêu cầu: 15'] ← BOTTLENECK 
> → [5 Chia task: 10']

**AI phản biện card #1:**
| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 45-60 phút áp dụng cho tài liệu dài bao nhiêu? | Đồng ý | Bổ sung định mức: "tài liệu dài 10-20 trang". |
| AI tóm tắt có thể bỏ sót yêu cầu kỹ thuật (edge cases). | Đồng ý | Thêm boundary: AI quét ý chính, tôi VẪN PHẢI kiểm tra lại trước khi chia task. |
| Nên làm Agent tự tạo ticket trên Jira luôn? | Không | Giữ bước "Tôi chia task" làm boundary để kiểm soát tiến độ, không giao AI. |

---

### Problem Card #2 — Gom log realtime tra cứu bug

| Trường | Nội dung |
|---|---|
| Job Story | Khi hệ thống báo lỗi liên quan đến luồng dữ liệu realtime, tôi muốn gom toàn bộ log từ backend (framework, database, cache) về một màn hình theo thứ tự thời gian, để tra cứu nguyên nhân chéo nhanh chóng thay vì mở từng tab terminal lẻ tẻ. |
| Actor | Dev Backend (Tôi) |
| Thời điểm / bối cảnh | Khi hệ thống báo lỗi trong quá trình dev/test các luồng dữ liệu đồng bộ (vd: gọi API có kết hợp DB và Redis). |
| Quy trình hiện tại | 1. Mở terminal API · 2. Mở log DB · 3. Mở log Cache/Redis · 4. Dò timestamp và so khớp sự kiện thủ công · 5. Xác định lỗi |
| Bottleneck | Bước 4 (Dò timestamp & so khớp sự kiện thủ công): khoảng 25 phút. |
| Impact | 45-60 phút mò mẫm log mỗi lần fix bug; xảy ra 1-2 lần/tuần, làm đứt mạch suy nghĩ khi code. |
| Success metric | Thời gian tra cứu và gom log từ 45 phút xuống dưới 10 phút/lần fix bug. |
| Phương án không dùng AI | Tự viết script bash gom log thủ công hoặc chia nhỏ màn hình terminal. Vẫn tốn sức nhìn bằng mắt thường. |
| Giả thuyết về AI | AI (hoặc script có AI) parse các file log, chuẩn hóa timestamp và highlight các điểm bất thường/lỗi chéo. Tôi tự xác định bug từ dữ liệu đã gom. |
| Cảm nhận nhanh | Rule / Workflow |

**Quy trình nháp hiện tại — 45 phút:**
> [1 Mở terminal API: 5'] → [2 Mở log DB: 5'] → [3 Mở log Redis: 5'] 
> → [4 Dò timestamp & so khớp: 25'] ← BOTTLENECK 
> → [5 Xác định dòng code lỗi: 5']

**AI phản biện card #2:**
| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chỉ cần dùng ELK stack hoặc Rule script là đủ gom log, nhảy sang AI quá sớm? | Đồng ý 1 phần | Rule làm tốt việc gom, nhưng AI sẽ mạnh ở bước "nhận diện điểm bất thường/lỗi logic" giữa các luồng. Sẽ xác định rõ ở CP6. |

---

### Problem Card #3 — Tóm tắt kiến thức từ Podcast

| Trường | Nội dung |
|---|---|
| Job Story | Khi kết thúc chuyến đi dài và nghe xong các podcast về System Design, tôi muốn có ngay các gạch đầu dòng từ khóa và kiến trúc cốt lõi vừa được nhắc tới, để lưu vào não và note cá nhân mà không phải tua lại audio để chép. |
| Actor | Sinh viên IT tự học (Tôi) |
| Thời điểm / bối cảnh | Về đến nhà sau chuyến đi xe buýt dài (2-3 tiếng) nghe podcast hoặc audiobook kỹ thuật. |
| Quy trình hiện tại | 1. Nghe podcast trên xe · 2. Về nhà mở máy tính/Notion · 3. Cố nhớ lại các ý chính · 4. Tua lại đoạn audio bị quên · 5. Gõ lại note |
| Bottleneck | Bước 3 và 4 (Nhớ lại và tua lại audio): tốn 25 phút, dễ quên 40% chi tiết quan trọng. |
| Impact | Lãng phí thời gian học trên xe do rơi rụng kiến thức; tốn thêm 30 phút mỗi ngày để chép lại note. |
| Success metric | Lưu lại được >90% keyword quan trọng; thời gian làm note giảm từ 30 phút xuống dưới 5 phút. |
| Phương án không dùng AI | Vừa nghe vừa gõ note trên điện thoại (gây say xe, mất an toàn). |
| Giả thuyết về AI | Cung cấp link/transcript podcast cho AI tóm tắt, hoặc tôi ghi âm bằng giọng nói các keyword nhớ được rồi AI tự đắp thịt thành bản note hoàn chỉnh. |
| Cảm nhận nhanh | Workflow |

**Quy trình nháp hiện tại — 32 phút (không tính thời gian nghe):**
> [1 Mở Notion: 2'] → [2 Cố nhớ lại ý: 10'] ← BOTTLENECK 
> → [3 Tua lại đoạn quên: 15'] ← BOTTLENECK 
> → [4 Gõ note: 5']

**AI phản biện card #3:**
| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI có thể hiểu sai hoặc dịch sai các thuật ngữ System Design chuyên sâu không? | Đồng ý | Thêm boundary: Phải sử dụng prompt ép AI giữ nguyên thuật ngữ tiếng Anh gốc, không tự ý dịch sang tiếng Việt. | 