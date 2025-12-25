Dựa trên nội dung từ trang 114 đến 125 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục **5.1: Kiểm soát truy cập**. Đây là phần kiến thức cực kỳ quan trọng, thường chiếm tỷ trọng lớn trong các câu hỏi về quản trị hệ thống.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 5 (MỤC 5.1)
**Chủ đề: Kiểm soát truy cập (Access Control)**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Ba dịch vụ cấu thành (Mục 5.1.1)
Hệ thống kiểm soát truy cập (KSTC) gồm bộ ba:
1.  **Xác thực (Authentication):** Xác minh tính chân thực của thông tin nhận dạng (Bạn là ai?).
2.  **Trao quyền (Authorization):** Cấp quyền dựa trên chính sách (Bạn được làm gì?).
3.  **Quản trị (Administration):** Thêm, bớt, sửa đổi thông tin người dùng và quyền hạn.

### 2. Bốn cơ chế kiểm soát truy cập (Mục 5.1.2) - TRỌNG TÂM

| Cơ chế | Tên tiếng Anh | Đặc điểm nhận diện (Từ khóa) | Ví dụ / Kỹ thuật |
|:---|:---|:---|:---|
| **Tùy chọn** | **DAC** | **Chủ sở hữu** đối tượng có toàn quyền cấp/hủy quyền cho người khác. | Ma trận ACM, Danh sách ACL. |
| **Bắt buộc** | **MAC** | Hệ thống áp đặt dựa trên **Nhãn nhạy cảm** (Mật, Tối mật). Chủ sở hữu không có quyền tự cho phép. | Mô hình Bell-LaPadula (Quân đội). |
| **Dựa trên vai trò** | **RBAC** | Quyền gán cho **Vai trò (Role)**, người dùng được kết nạp vào vai trò đó. | Nhóm Giáo viên, Nhóm Sinh viên. |
| **Dựa trên luật** | **Rule-Based** | Dựa trên các **luật định trước** (IP, thời gian, giao thức). | Tường lửa (Firewall), Proxy. |

### 3. Mô hình Bell-LaPadula (MAC)
Dùng để bảo vệ tính **Bí mật**, gồm 2 quy tắc vàng:
*   **Đọc xuống (Read Down):** Người ở mức bảo mật cao được đọc tài liệu ở mức thấp hơn hoặc bằng.
*   **Ghi lên (Write Up):** Người ở mức bảo mật thấp chỉ được ghi vào tài liệu ở mức cao hơn hoặc bằng (để tránh rò rỉ thông tin từ cao xuống thấp).

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 118: Khâu nào trong hệ thống kiểm soát truy cập có nhiệm vụ xác minh tính đúng đắn của thông tin nhận dạng mà người dùng cung cấp?**
A. Trao quyền (Authorization).
B. Quản trị (Administration).
C. Xác thực (Authentication).
D. Kiểm toán (Auditing).

**Câu 119: Trong cơ chế kiểm soát truy cập nào, chủ sở hữu của đối tượng có quyền cao nhất trong việc cấp hoặc hủy quyền truy cập của người dùng khác đối với đối tượng đó?**
A. MAC (Mandatory Access Control).
B. RBAC (Role-Based Access Control).
C. DAC (Discretionary Access Control).
D. Rule-based Access Control.

**Câu 120: Kỹ thuật "Ma trận kiểm soát truy cập" (ACM) ít được sử dụng trên thực tế hiện nay vì lý do chính nào?**
A. Không đảm bảo an toàn thông tin.
B. Kích thước ma trận quá lớn và tồn tại nhiều ô rỗng gây lãng phí bộ nhớ.
C. Không hỗ trợ quyền đọc và ghi đồng thời.
D. Chỉ sử dụng được cho hệ điều hành Windows.

**Câu 121: Theo mô hình bảo mật Bell-LaPadula, một người dùng ở mức bảo mật "Mật" (Confidential) có quyền thực hiện hành động nào sau đây?**
A. Đọc tài liệu ở mức "Tối mật".
B. Ghi dữ liệu vào tài liệu ở mức "Không phân loại".
C. Đọc tài liệu ở mức "Mật" hoặc "Không phân loại".
D. Thay đổi quyền truy cập của Quản trị viên.

**Câu 122: Ưu điểm lớn nhất của kiểm soát truy cập dựa trên vai trò (RBAC) là gì?**
A. Cho phép người dùng tự do chia sẻ dữ liệu.
B. Phù hợp với mô hình phân cấp tự nhiên của tổ chức, dễ dàng quản lý và thay đổi quyền hạn.
C. Tốc độ thực thi nhanh hơn mã hóa đối xứng.
D. Không cần thực hiện khâu xác thực.

**Câu 123: Một hệ thống xác thực sử dụng Thẻ thông minh (Smartcard) yêu cầu người dùng nhập thêm mã PIN được gọi là xác thực mấy nhân tố?**
A. 1 nhân tố.
B. 2 nhân tố.
C. 3 nhân tố.
D. Không nhân tố nào.

---

## III. GIẢI THÍCH & PHÂN TÍCH CHI TIẾT

*   **Đáp án Câu 118: C.** (Trang 114). Ghi nhớ: Xác thực = Kiểm tra ID/Pass. Trao quyền = Kiểm tra quyền sau khi đã vào.
*   **Đáp án Câu 119: C.** DAC (Tùy chọn) đề cao quyền của **Chủ sở hữu (Owner)**.
*   **Đáp án Câu 120: B.** (Trang 116). ACM là ma trận 2 chiều (Chủ thể x Đối tượng). Trong mạng lớn, ma trận này cực kỳ thưa (ô rỗng nhiều), nên người ta dùng ACL (Danh sách) để thay thế.
*   **Đáp án Câu 121: C.** (Trang 118). Áp dụng quy tắc **"Đọc xuống"**: Cấp "Mật" chỉ được đọc tài liệu "Mật" (bằng) hoặc "Không phân loại" (thấp hơn). Đọc "Tối mật" (cao hơn) là vi phạm tính bí mật.
*   **Đáp án Câu 122: B.** (Trang 119). RBAC giúp quản trị viên không phải gán quyền cho từng người (mất công), mà chỉ cần gán vào "Nhóm/Vai trò".
*   **Đáp án Câu 123: B.** (Trang 122). Gồm: (1) Cái bạn có - Thẻ thông minh và (2) Cái bạn biết - mã PIN.

---

## IV. MẸO GHI NHỚ (STUDY TIPS)

### 1. Phân biệt DAC vs MAC
*   **DAC (Discretionary):** Tự tay mình cho (Tùy ý mình).
*   **MAC (Mandatory):** Máy/Hệ thống ép buộc (Luật nhà nước/Quân đội).

### 2. Quy tắc Bell-LaPadula (CỰC HAY HỎI)
Hãy nhớ câu khẩu hiệu để đảm bảo Bí mật:
*   **"No Read Up"** (Không đọc lên cao - tránh lộ bí mật cấp trên).
*   **"No Write Down"** (Không ghi xuống thấp - tránh làm lộ tài liệu mật vào chỗ không mật).
*   $\rightarrow$ Suy ra: **Đọc xuống, Ghi lên.**

### 3. Công nghệ xác thực (Mục 5.1.3)
*   **Mật khẩu:** Độ an toàn thấp nhất, khuyến nghị đổi mỗi 3-6 tháng.
*   **Sinh trắc (Biometric):** Độ an toàn cao nhất, nhưng chi phí đắt và có tỷ lệ nhận dạng sai.

---
Dựa trên nội dung từ trang 125 đến trang 130 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục **5.2 (Tường lửa - Firewall)**. Đây là phần kiến thức mang tính ứng dụng cao, đề thi thường tập trung vào việc **phân loại các thế hệ tường lửa** và **nhận diện các hạn chế**.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 5 (MỤC 5.2)
**Chủ đề: Tường lửa (Firewall)**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Khái niệm và Vị trí (Mục 5.2.1)
*   **Bản chất:** Là thiết bị phần cứng hoặc phần mềm bảo vệ mạng nội bộ khỏi đe dọa bên ngoài.
*   **Vị trí triển khai:** Luôn đặt ở **cổng vào (gateway)** của mạng nội bộ. Mọi gói tin ra/vào đều phải đi qua tường lửa.
*   **Cơ chế:** Lọc gói tin dựa trên tập các **Luật (Rules)** được xây dựng từ chính sách an ninh của tổ chức.

### 2. Phân loại tường lửa (Mục 5.2.2) - TRỌNG TÂM THI

**a. Theo giao thức mạng (3 loại):**
*   **Tường lửa lọc gói (Packet-filtering):** Làm việc ở mức thấp (tầng mạng/IP). Kiểm tra địa chỉ IP, cổng (port). Tốc độ rất nhanh.
*   **Cổng ứng dụng (Application-level gateway/Proxy):** Làm việc ở mức cao nhất (tầng ứng dụng). Hiểu được nội dung các giao thức cụ thể (HTTP, FTP, SMTP). An toàn cao nhưng chậm.
*   **Cổng chuyển mạch (Circuit-level gateway):** Hoạt động ở mức thấp nhất (tầng phiên), cơ chế giống bộ chuyển mạch (Switch).

**b. Theo khả năng lưu trạng thái:**
*   **Có trạng thái (Stateful):** Nhớ được các kết nối đang hoạt động. Chỉ cho phép gói tin thuộc về một phiên đã thiết lập đi qua. **Chống tấn công giả mạo tốt hơn.**
*   **Không trạng thái (Stateless):** Lọc từng gói tin riêng rẽ, không quan tâm nó thuộc kết nối nào. Dễ bị tấn công giả mạo IP.

### 3. Các kỹ thuật kiểm soát (Mục 5.2.3)
*   **Dịch vụ:** Mở/đóng cổng (ví dụ: mở cổng 80 cho Web, đóng các cổng khác).
*   **Hướng:** Kiểm soát luồng đi ra (**Outgoing**) hoặc đi vào (**Incoming**).
*   **Người dùng:** Áp dụng cho từng định danh cụ thể (thường là người dùng nội bộ).
*   **Hành vi:** Lọc nội dung (thư rác, giới hạn truy cập một phần máy chủ web).

### 4. Hạn chế của Tường lửa (Mục 5.2.4) - DỄ RA CÂU HỎI SUY LUẬN
*   Không chống lại được tấn công **không đi qua tường lửa** (ví dụ: tấn công qua đường quay số trực tiếp, USB).
*   Không chống được **mối đe dọa từ bên trong** (người dùng nội bộ phá hoại).
*   Không ngăn được virus/mã độc nằm trong các file **đã bị nén hoặc mã hóa**.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 124: Tường lửa thường được triển khai tại vị trí nào trong cấu trúc mạng của một tổ chức?**
A. Cài đặt trên mọi máy tính cá nhân của nhân viên.
B. Tại cổng kết nối (gateway) giữa mạng nội bộ và mạng bên ngoài.
C. Nằm bên trong cơ sở dữ liệu của máy chủ.
D. Tại các điểm truy cập WiFi công cộng.

**Câu 125: Loại tường lửa nào hoạt động ở tầng ứng dụng và có khả năng lọc chi tiết các yêu cầu (request) của giao thức HTTP hoặc FTP?**
A. Tường lửa lọc gói (Packet-filtering).
B. Cổng chuyển mạch (Circuit-level gateway).
C. Cổng ứng dụng (Application-level gateway/Proxy).
D. Tường lửa cá nhân.

**Câu 126: Điểm khác biệt cốt lõi của "Tường lửa có trạng thái" (Stateful Firewall) so với tường lửa thông thường là gì?**
A. Nó có tốc độ xử lý nhanh hơn gấp 10 lần.
B. Nó có khả năng ghi nhớ và phân biệt các gói tin thuộc về các kết nối mạng đang hoạt động.
C. Nó chỉ có thể cài đặt trên phần cứng chuyên dụng của Cisco.
D. Nó không cần sử dụng các luật để lọc gói tin.

**Câu 127: Kỹ thuật kiểm soát nào của tường lửa cho phép xác định luồng dữ liệu là từ trong mạng nội bộ đi ra (Outgoing) hay từ ngoài vào trong (Incoming)?**
A. Kiểm soát dịch vụ.
B. Kiểm soát hướng.
C. Kiểm soát người dùng.
D. Kiểm soát hành vi.

**Câu 128: Tường lửa KHÔNG có khả năng ngăn chặn hiệu quả loại tấn công nào sau đây?**
A. Tấn công giả mạo địa chỉ IP từ bên ngoài.
B. Tấn công rà quét cổng từ Internet.
C. Mối đe dọa tấn công từ chính người dùng bên trong mạng nội bộ.
D. Tấn công truy cập trái phép vào cổng dịch vụ bị cấm.

**Câu 129: Tại sao tường lửa thường khó ngăn chặn các file bị nhiễm mã độc được vận chuyển vào hệ thống?**
A. Vì tường lửa không có luật chặn virus.
B. Vì các file này thường ở dạng nén hoặc mã hóa khiến tường lửa không thể kiểm tra nội dung.
C. Vì mã độc luôn có kích thước nhỏ hơn kích thước gói tin IP.
D. Vì tường lửa chỉ làm việc với địa chỉ MAC.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 124: B.** (Trang 126). Tường lửa giống như "trạm gác cổng", mọi thứ muốn vào/ra đều phải qua nó.
*   **Đáp án Câu 125: C.** (Trang 127). Từ khóa: **Proxy = Tầng ứng dụng = Lọc nội dung HTTP/FTP**.
*   **Đáp án Câu 126: B.** (Trang 128). "State" nghĩa là trạng thái. Nó nhớ được gói tin này có nằm trong một cuộc trò chuyện hợp lệ đã bắt đầu từ trước hay không.
*   **Đáp án Câu 127: B.** (Trang 129). "Hướng" (Direction) chính là chiều của gói tin.
*   **Đáp án Câu 128: C.** (Trang 130). Đây là một hạn chế kinh điển: Tường lửa bảo vệ biên giới, không thể quản lý được "gián điệp" đã ở sẵn trong nhà.
*   **Đáp án Câu 129: B.** (Trang 130). Nếu dữ liệu đã được nén hoặc mã hóa, tường lửa chỉ nhìn thấy một khối ký tự vô nghĩa và buộc phải cho qua nếu nguồn/đích hợp lệ.

---

## IV. MẸO GHI NHỚ (STUDY TIPS)
*   **Packet-filtering:** Nhìn "vỏ phong bì" (IP/Port).
*   **Application-level:** Đọc "nội dung bức thư" (Data/Command).
*   **Stateful:** Nhớ "đã gặp người này chưa" (Session table).
*   **Nhược điểm tường lửa:** Hãy nhớ cụm từ **"Nội gián - Không đi qua cửa - Mã hóa"**. (Tường lửa bó tay với 3 trường hợp này).

---
Dựa trên nội dung từ trang 130 đến trang 136 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục **5.3 (Các hệ thống phát hiện và ngăn chặn xâm nhập IDS/IPS)**. 

Đây là một lớp phòng vệ cực kỳ quan trọng trong mô hình phòng thủ chiều sâu, thường được hỏi rất kỹ về **cơ chế phát hiện** và **vị trí triển khai** trong sơ đồ mạng.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 5 (MỤC 5.3)
**Chủ đề: Hệ thống IDS và IPS**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Phân biệt IDS và IPS (Mục 5.3.1)
Cả hai đều giám sát lưu lượng và hành vi hệ thống, nhưng khác nhau ở **hành động phản ứng**:
*   **IDS (Intrusion Detection System):** Hệ thống **phát hiện** xâm nhập.
    *   *Hành động:* Giám sát, ghi log và gửi cảnh báo (Alert).
    *   *Cơ chế:* Thụ động (**Passive**), thường kết nối vào Switch/Router để nhận bản sao gói tin.
*   **IPS (Intrusion Prevention System):** Hệ thống **ngăn chặn** xâm nhập.
    *   *Hành động:* Bao gồm cả chức năng của IDS cộng thêm khả năng **ngăn chặn/dừng** hành vi tấn công ngay lập tức.
    *   *Cơ chế:* Chủ động (**Active**), được ghép vào **giữa đường truyền** (In-line).

### 2. Phân loại theo nguồn dữ liệu (Mục 5.3.2)
*   **NIDS (Network-based):** Giám sát cả một phân đoạn mạng.
    *   *Ưu điểm:* Bảo vệ nhiều máy cùng lúc.
    *   *Hạn chế:* Khó xử lý lưu lượng quá lớn hoặc dữ liệu bị mã hóa. 
    *   *Đại diện:* **Snort** (phổ biến nhất, mã nguồn mở).
*   **HIDS (Host-based):** Cài đặt trên từng máy cụ thể (Agent).
    *   *Ưu điểm:* Phát hiện chính xác các hành vi lạm dụng bên trong hệ điều hành máy đó.
    *   *Hạn chế:* Chi phí cài đặt và bảo trì cao khi mạng có nhiều máy.
    *   *Đại diện:* **OSSEC**.

### 3. Kỹ thuật phát hiện (Mục 5.3.3) - TRỌNG TÂM THI
*   **Dựa trên chữ ký (Signature-based):** Đối soát dữ liệu với cơ sở dữ liệu các mẫu tấn công đã biết.
    *   *Ưu:* Chính xác với tấn công cũ, tốc độ cao, ít tốn tài nguyên.
    *   *Nhược:* **Không phát hiện được tấn công mới** (Zero-day).
*   **Dựa trên bất thường (Anomaly-based):** Xây dựng hồ sơ hành vi "bình thường" (huấn luyện), sau đó so sánh với hành vi hiện tại.
    *   *Ưu:* Có tiềm năng phát hiện **tấn công mới**.
    *   *Nhược:* **Tỷ lệ cảnh báo sai (False Positive) cao**, tốn tài nguyên hệ thống.
    *   *Ví dụ:* Sử dụng giá trị **Entropy** của IP nguồn để phát hiện DDoS (DDoS làm Entropy giảm đột biến).

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 130: Điểm khác biệt cơ bản nhất về chức năng giữa hệ thống IPS và IDS là gì?**
A. IPS có khả năng ghi log còn IDS thì không.
B. IPS có khả năng chủ động ngăn chặn tấn công, trong khi IDS chủ yếu làm nhiệm vụ giám sát và cảnh báo.
C. IDS hoạt động trên tầng ứng dụng, còn IPS hoạt động trên tầng vật lý.
D. IDS chỉ dành cho máy tính cá nhân, còn IPS dành cho mạng doanh nghiệp.

**Câu 131: Theo sơ đồ mạng tiêu chuẩn (Hình 5.20), hệ thống IPS thường được triển khai tại vị trí nào?**
A. Kết nối song song với Switch để nhận bản sao dữ liệu.
B. Ghép vào giữa đường truyền truyền thông (In-line), phía sau tường lửa.
C. Đứng trước tường lửa để lọc mọi gói tin từ Internet.
D. Cài đặt trực tiếp bên trong cơ sở dữ liệu.

**Câu 132: Hệ thống Snort được giáo trình phân loại vào nhóm nào sau đây?**
A. Hệ thống phát hiện xâm nhập cho máy (HIDS).
B. Hệ thống phát hiện xâm nhập mạng (NIDS).
C. Phần mềm diệt virus thời gian thực.
D. Tường lửa không trạng thái.

**Câu 133: Đâu là hạn chế lớn nhất của kỹ thuật "Phát hiện xâm nhập dựa trên chữ ký" (Signature-based)?**
A. Tỷ lệ cảnh báo sai rất cao.
B. Yêu cầu tài nguyên tính toán cực lớn.
C. Không có khả năng phát hiện các cuộc tấn công mới chưa có trong cơ sở dữ liệu.
D. Không thể ghi lại log hành vi tấn công.

**Câu 134: Kỹ thuật phát hiện xâm nhập dựa trên "Bất thường" (Anomaly-based) thường phải trải qua 2 giai đoạn chính nào?**
A. Quét cổng và Chặn địa chỉ IP.
B. Huấn luyện (xây dựng hồ sơ bình thường) và Phát hiện.
C. Mã hóa và Giải mã dữ liệu.
D. Cài đặt Agent và Cấu hình tường lửa.

**Câu 135: Tại sao kỹ thuật phát hiện dựa trên bất thường lại thường có tỷ lệ cảnh báo sai (False Positive) cao hơn so với dựa trên chữ ký?**
A. Vì nó sử dụng các thuật toán học máy phức tạp.
B. Vì một hành vi bất thường của người dùng đôi khi chỉ là sự thay đổi thói quen chứ không phải là một cuộc tấn công thực sự.
C. Vì nó không có khả năng giám sát lưu lượng mạng.
D. Vì nó chỉ hoạt động trên các máy chủ cũ.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 130: B.** (Trang 131). "P" trong IPS là **Prevention** (Ngăn chặn). Đây là từ khóa quan trọng nhất.
*   **Đáp án Câu 131: B.** (Trang 130). Để ngăn chặn được gói tin độc hại, IPS buộc phải nằm "ngáng đường" (In-line) để có thể hủy gói tin đó trước khi nó tới đích.
*   **Đáp án Câu 132: B.** (Trang 132). Snort là tượng đài của NIDS mã nguồn mở.
*   **Đáp án Câu 133: C.** (Trang 134). Chữ ký giống như một "danh sách đen". Nếu kẻ gian dùng một chiêu thức mới hoàn toàn chưa có trong danh sách, hệ thống sẽ cho qua.
*   **Đáp án Câu 134: B.** (Trang 135). Hệ thống cần biết thế nào là "ngoan" (Huấn luyện) thì mới biết ai đang "hư" (Phát hiện).
*   **Đáp án Câu 135: B.** (Trang 136). Đây là nhược điểm chí mạng của Anomaly-based. Ví dụ: Một nhân viên đột nhiên làm việc khuya (bất thường) có thể bị hệ thống báo động nhầm là hacker xâm nhập.

---

## IV. BẢNG SO SÁNH NHANH ĐỂ GHI NHỚ

| Đặc điểm | Dựa trên Chữ ký (Signature) | Dựa trên Bất thường (Anomaly) |
|:---|:---|:---|
| **Cơ chế** | So khớp mẫu (Match patterns) | So sánh với hành vi chuẩn (Baseline) |
| **Tấn công cũ** | Rất hiệu quả | Hiệu quả trung bình |
| **Tấn công mới** | **Bó tay** | Có khả năng phát hiện |
| **Cảnh báo sai** | Thấp | **Cao** |
| **Tài nguyên** | Thấp | Cao (tốn CPU/RAM để phân tích) |

---
Dựa trên nội dung từ trang 138 đến trang 146 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục **6.1: Quản lý an toàn thông tin**. 

Đây là phần lý thuyết về quy trình quản trị, đòi hỏi bạn phải nhớ chính xác các **định nghĩa**, **thành phần của rủi ro** và **phân loại các phương pháp/kiểm soát**.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 6 (MỤC 6.1)
**Chủ đề: Quản lý và Đánh giá rủi ro An toàn thông tin**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Khái niệm Tài sản và Quản lý (Mục 6.1.1)
*   **Tài sản (Asset):** Gồm Phần cứng, Phần mềm và quan trọng nhất là **Thông tin**.
*   **Quản lý ATTT:** Là một tiến trình (không phải hành động một lần) nhằm bảo vệ tài sản với **chi phí phù hợp**.
*   **3 câu hỏi cốt lõi:** (1) Tài sản nào cần bảo vệ? (2) Đe dọa nào đối với tài sản? (3) Biện pháp ứng phó là gì?
*   **3 khâu chính:** (1) Xác định mục đích/hồ sơ rủi ro $\rightarrow$ (2) Đánh giá rủi ro $\rightarrow$ (3) Triển khai biện pháp kiểm soát.

### 2. Mô hình Rủi ro (Mục 6.1.2) - TRỌNG TÂM
*   **Công thức rủi ro (Hình 6.2):** Rủi ro là sự giao thoa của **3 nhân tố**:
    1.  **Tài sản** (Asset)
    2.  **Mối đe dọa** (Threat - yếu tố bên ngoài)
    3.  **Lỗ hổng bảo mật** (Vulnerability - yếu tố bên trong)

### 3. Bốn phương pháp tiếp cận đánh giá rủi ro (Mục 6.1.2.2)
| Phương pháp | Đặc điểm nhận diện | Đối tượng phù hợp |
|:---|:---|:---|
| **Đường cơ sở (Baseline)** | Đơn giản nhất, dựa trên quy tắc thực hành tốt nhất. | Tổ chức quy mô **nhỏ**, nguồn lực hạn chế. |
| **Không chính thức** | Dựa trên kiến thức chuyên gia, không đánh giá toàn diện. | Tổ chức quy mô **nhỏ và vừa**. |
| **Phân tích chi tiết** | Toàn diện, chính thức, 9 bước xử lý, tốn thời gian. | Tổ chức **Chính phủ**, quy mô **lớn**, hạ tầng quốc gia. |
| **Kết hợp (Combined)** | Đi từ Đường cơ sở $\rightarrow$ Không chính thức $\rightarrow$ Phân tích chi tiết. | Tổ chức quy mô **vừa và lớn**. |

### 4. Sáu loại kiểm soát (Control) - Mục 6.1.4.2
*   **Kiểm soát quản lý:** Chính sách, lập kế hoạch, hướng dẫn.
*   **Kiểm soát vận hành:** Thực thi bởi **con người** là chủ yếu (ví dụ: quy trình vận hành).
*   **Kiểm soát kỹ thuật:** Sử dụng phần cứng, phần mềm (ví dụ: xác thực, tường lửa).
*   **Kiểm soát hỗ trợ:** Các kiểm soát chung ở lớp dưới.
*   **Kiểm soát ngăn ngừa:** Chặn vi phạm xảy ra.
*   **Kiểm soát phát hiện và phục hồi:** Đáp trả và khắc phục sau sự cố.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 136: Theo giáo trình, quản lý an toàn thông tin là một tiến trình phải trả lời được bao nhiêu câu hỏi cốt lõi?**
A. 2 câu hỏi.
B. 3 câu hỏi.
C. 4 câu hỏi.
D. 5 câu hỏi.

**Câu 137: Nhân tố nào sau đây KHÔNG nằm trong mô hình 3 nhân tố chính cấu thành rủi ro an toàn thông tin?**
A. Tài sản (Asset).
B. Mối đe dọa (Threat).
C. Chi phí đầu tư (Cost).
D. Lỗ hổng bảo mật (Vulnerability).

**Câu 138: Phương pháp đánh giá rủi ro nào thực hiện các kiểm soát an ninh ở mức cơ bản dựa trên các tài liệu quy tắc thực hành tốt nhất của ngành và phù hợp với tổ chức nhỏ?**
A. Phương pháp phân tích chi tiết.
B. Phương pháp không chính thức.
C. Phương pháp đường cơ sở (Baseline).
D. Phương pháp kết hợp.

**Câu 139: Tại sao phương pháp phân tích chi tiết rủi ro thường chỉ phù hợp với các tổ chức lớn hoặc các tổ chức chính phủ?**
A. Vì nó không đòi hỏi kiến thức chuyên gia.
B. Vì chi phí về thời gian, nguồn lực và yêu cầu trình độ chuyên gia rất cao.
C. Vì nó chỉ thực hiện được trên hệ điều hành Windows.
D. Vì nó là phương pháp đơn giản nhất.

**Câu 140: Bước đầu tiên (Bước 1) trong quy trình 9 bước phân tích chi tiết rủi ro an toàn thông tin là gì?**
A. Nhận dạng các mối đe dọa.
B. Nhận dạng các lỗ hổng bảo mật.
C. Mô tả đặc điểm hệ thống.
D. Đề xuất các kiểm soát.

**Câu 141: Loại kiểm soát nào liên quan đến các cơ chế và thủ tục được thực hiện "chủ yếu bởi con người" hơn là bởi hệ thống?**
A. Kiểm soát kỹ thuật.
B. Kiểm soát quản lý.
C. Kiểm soát vận hành (Operational control).
D. Kiểm soát hỗ trợ.

**Câu 142: Hoạt động xác thực và trao quyền truy cập cho người dùng được phân loại vào nhóm kiểm soát nào?**
A. Kiểm soát quản lý.
B. Kiểm soát vận hành.
C. Kiểm soát kỹ thuật (Technical control).
D. Kiểm soát ngăn ngừa.

---

## III. GIẢI THÍCH & PHÂN TÍCH CHI TIẾT

*   **Đáp án Câu 136: B.** (Trang 138). 3 câu hỏi: Tài sản nào? Đe dọa nào? Biện pháp gì?
*   **Đáp án Câu 137: C.** (Hình 6.2 trang 139). Chi phí là yếu tố cần cân nhắc khi quản lý, nhưng không phải là thành phần định nghĩa nên "Rủi ro".
*   **Đáp án Câu 138: C.** (Trang 140). Từ khóa: **"Đường cơ sở" = "Cơ bản" + "Tổ chức nhỏ"**.
*   **Đáp án Câu 139: B.** (Trang 141). Phân tích chi tiết đòi hỏi xem xét từng thành phần một nên rất chậm và tốn kém.
*   **Đáp án Câu 140: C.** (Trang 142). Bạn phải biết hệ thống có gì trước (Bước 1) thì mới biết nó sợ cái gì (Bước 2).
*   **Đáp án Câu 141: C.** (Trang 145). Đây là bẫy phân biệt: Kỹ thuật (Hardware/Software) vs Vận hành (Con người/Quy trình).
*   **Đáp án Câu 142: C.** (Trang 145). Xác thực dùng code hoặc thiết bị nên là kiểm soát Kỹ thuật.

---

## IV. GỢI Ý FLASHCARD GHI NHỚ NHANH

*   **Thành phần rủi ro:** Tài sản + Đe dọa + Lỗ hổng. (Thiếu 1 trong 3 thì không có rủi ro).
*   **9 bước phân tích:** Nhớ 3 bước đầu: **Hệ thống $\rightarrow$ Đe dọa $\rightarrow$ Lỗ hổng**.
*   **Combined Approach:** Baseline (Thấp) $\rightarrow$ Không chính thức (Trung bình) $\rightarrow$ Chi tiết (Cao).
*   **Operational Control:** Nhớ từ khóa **"Con người"**.

---
Dựa trên nội dung từ trang 147 đến trang 149 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục **6.2: Các chuẩn quản lý và Chu trình PDCA**.

Phần này thường xuất hiện trong đề thi dưới dạng phân biệt số hiệu các chuẩn ISO và xác định các hoạt động cụ thể thuộc pha nào trong chu trình PDCA.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 6 (MỤC 6.2)
**Chủ đề: Chuẩn ISO/IEC 27000 và Chu trình PDCA**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Hệ thống chuẩn ISO/IEC 27000
Bạn cần nhớ tên và chức năng của các chuẩn con phổ biến nhất:

| Số hiệu chuẩn | Tên/Nội dung chính | Đặc điểm cần nhớ |
|:---|:---|:---|
| **ISO/IEC 27000** | Tổng quan và Từ vựng | Giải thích thuật ngữ cho cả bộ chuẩn. |
| **ISO/IEC 27001** | **Các yêu cầu (Requirements)** | Là chuẩn chính để xây dựng **ISMS**. Chỉ tập trung vào việc **phải làm gì**, không dạy cách làm. |
| **ISO/IEC 27002** | Quy tắc thực hành | Đưa ra các khuyến nghị, hướng dẫn chi tiết cách thực hiện. |
| **ISO/IEC 27005** | Quản lý rủi ro ATTT | Chuyên sâu về quy trình đánh giá và xử lý rủi ro. |

*   **Lưu ý:** Việt Nam đã chấp thuận bộ chuẩn này thành tiêu chuẩn quốc gia (**TCVN**). Ví dụ: ISO 27001 tương ứng với TCVN ISO/IEC 27001.

### 2. Chu trình PDCA trong chuẩn ISO/IEC 27001
Đây là mô hình lặp lại để duy trì và cải tiến hệ thống ISMS:

1.  **Plan (Lập kế hoạch):** 
    *   Định nghĩa phạm vi, chính sách của ISMS.
    *   Nhận dạng, đánh giá và **lựa chọn phương pháp/biện pháp kiểm soát rủi ro**.
2.  **Do (Thực hiện):** 
    *   Thực thi kế hoạch và các biện pháp kiểm soát.
    *   **Đào tạo chuyên môn và giáo dục ý thức** cho nhân viên.
    *   Quản lý tài nguyên và hoạt động.
3.  **Check (Giám sát):** 
    *   Đánh giá tính hiệu quả.
    *   Thực hiện **Kiểm toán (Audit) nội bộ**.
    *   Ghi lại các hành động và sự kiện ảnh hưởng.
4.  **Act (Cải tiến):** 
    *   Thực hiện các hành động **sửa chữa và ngăn chặn**.
    *   Áp dụng bài học kinh nghiệm.
    *   Thảo luận kết quả với các bên liên quan.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 143: Chuẩn nào trong bộ chuẩn ISO/IEC 27000 tập trung vào việc đưa ra các "Yêu cầu" (Requirements) để xây dựng Hệ thống quản lý an toàn thông tin (ISMS)?**
A. ISO/IEC 27000.
B. ISO/IEC 27001.
C. ISO/IEC 27002.
D. ISO/IEC 27005.

**Câu 144: Chuẩn ISO/IEC 27002 khác với ISO/IEC 27001 ở điểm cơ bản nào?**
A. ISO 27002 là chuẩn bắt buộc, ISO 27001 là tự nguyện.
B. ISO 27001 đưa ra các yêu cầu phải thực hiện, còn ISO 27002 đưa ra các hướng dẫn và quy tắc thực hành chi tiết.
C. ISO 27002 chỉ dành cho lĩnh vực quân sự.
D. ISO 27001 chỉ dành cho phần cứng, ISO 27002 chỉ dành cho phần mềm.

**Câu 145: Trong chu trình PDCA, việc "Lựa chọn các mục tiêu và biện pháp kiểm soát rủi ro" thuộc về pha nào?**
A. Pha Plan.
B. Pha Do.
C. Pha Check.
D. Pha Act.

**Câu 146: Hoạt động "Đào tạo chuyên môn và giáo dục ý thức về an toàn thông tin" cho nhân viên được thực hiện trong pha nào của chu trình PDCA?**
A. Pha Plan.
B. Pha Do.
C. Pha Check.
D. Pha Act.

**Câu 147: Việc thực hiện "Kiểm toán nội bộ" (Internal Audit) để đánh giá tính hiệu quả của ISMS thuộc pha nào?**
A. Pha Plan.
B. Pha Do.
C. Pha Check.
D. Pha Act.

**Câu 148: Pha "Act" (Hành động/Cải tiến) trong chu trình PDCA bao gồm nội dung nào sau đây?**
A. Nhận dạng các rủi ro.
B. Thực thi các thủ tục phát hiện sự cố.
C. Thực hiện các hành động sửa chữa và ngăn chặn dựa trên kết quả giám sát.
D. Đề ra phạm vi của ISMS.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 143: B.** (Trang 147). Đây là chuẩn quan trọng nhất mà mọi doanh nghiệp muốn có chứng chỉ ISMS đều phải tuân theo.
*   **Đáp án Câu 144: B.** (Trang 147). Mẹo nhớ: **27001 = "What"** (Phải làm gì), **27002 = "How"** (Làm như thế nào).
*   **Đáp án Câu 145: A.** (Trang 149). Mọi việc liên quan đến "thiết kế", "đề ra", "lựa chọn phương án" đều nằm ở pha **Lập kế hoạch (Plan)**.
*   **Đáp án Câu 146: B.** (Trang 149). Đào tạo là một phần của việc "Triển khai" hệ thống vào thực tế, nên thuộc pha **Do**.
*   **Đáp án Câu 147: C.** (Trang 149). Từ khóa: Audit, Đánh giá tính hiệu quả $\rightarrow$ Thuộc pha **Check** (Kiểm tra).
*   **Đáp án Câu 148: C.** (Trang 149). Pha Act là pha cuối cùng của một vòng lặp, dùng để sửa sai và tối ưu hóa hệ thống cho vòng lặp tiếp theo.

---

## IV. MẸO GHI NHỚ (STUDY TIPS)

### 1. Phân biệt ISO 27001 và 27002
Hãy tưởng tượng:
*   **ISO 27001** giống như **Luật giao thông**: Bạn *phải* dừng khi đèn đỏ, *phải* có bằng lái (Đây là các Yêu cầu).
*   **ISO 27002** giống như **Sổ tay lái xe an toàn**: Hướng dẫn bạn nên quan sát gương thế nào, đạp phanh ra sao cho êm (Đây là các Quy tắc thực hành).

### 2. Chu trình PDCA
*   **Plan:** Nghĩ (Suy nghĩ, chọn lựa, viết chính sách).
*   **Do:** Làm (Cài đặt, dạy học, vận hành).
*   **Check:** Nhìn (Soát lỗi, kiểm toán, xem báo cáo).
*   **Act:** Sửa (Sửa lỗi, cải tiến, rút kinh nghiệm).

---
Dưới đây là phần tài liệu ôn tập cuối cùng cho **Chương 6 (Mục 6.3 & 6.4)**. Đây là phần kiến thức về khung pháp lý và quy tắc ứng xử, thường xuất hiện dưới dạng các câu hỏi so sánh hoặc nhận diện các bộ luật quan trọng của Việt Nam và quốc tế.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 6 (MỤC 6.3 & 6.4)
**Chủ đề: Pháp luật, Chính sách và Đạo đức An toàn thông tin**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Phân biệt Luật, Chính sách và Đạo đức (Mục 6.3.1)
Đây là điểm cực kỳ hay bẫy trong đề thi trắc nghiệm:
*   **Luật (Law):** Do chính quyền ban hành, có tính **bắt buộc**. Vi phạm bị xử lý theo chế tài nhà nước.
*   **Chính sách (Policy):** Là "luật nội bộ" của tổ chức. **Lưu ý:** Trong quản trị, việc "thiếu hiểu biết chính sách" có thể được coi là một cách bào chữa chấp nhận được (khác với luật).
*   **Đạo đức (Ethics):** Dựa trên văn hóa và niềm tin về hành vi đúng/sai. **Không** được thực thi bởi chính quyền.

### 2. Các bộ luật quốc tế cần nhớ (Mục 6.3.2)
*   **CFA Act (1986):** Quy định về tội phạm lừa đảo và lạm dụng máy tính.
*   **HIPAA (1996):** Bảo mật dữ liệu **y tế**. Vi phạm có thể bị phạt tới 250.000 USD.
*   **USA PATRIOT Act (2001):** Cho phép chính phủ theo dõi mạng để phòng chống **khủng bố**.
*   **DMCA:** Luật bản quyền kỹ thuật số thiên niên kỷ.

### 3. Pháp luật Việt Nam (Mục 6.3.3) - CỰC KỲ QUAN TRỌNG
Bạn cần nhớ chính xác tên và hiệu lực của 2 bộ luật trụ cột:
1.  **Luật An toàn thông tin mạng (Luật số 86/2015/QH13):** Có hiệu lực từ **01/07/2016**.
2.  **Luật An ninh mạng (Luật số 24/2018/QH14):** Có hiệu lực từ **01/01/2019**.
3.  **Nghị định 90/2008/NĐ-CP:** Quy định về chống **thư rác**.

### 4. Đạo đức và Quy tắc ứng xử (Mục 6.4)
*   **Bộ quy tắc 10 điều răn của máy tính (Ten Commandments):** Do Viện đạo đức máy tính Hoa Kỳ đưa ra. (Ví dụ: Không dùng máy tính để gây hại, không trộm cắp file, không tạo bằng chứng giả...).
*   **Thực trạng tại Việt Nam:** Tỷ lệ vi phạm bản quyền phần mềm hiện rất cao (đến khoảng **90%**).

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 149: Điểm khác biệt lớn nhất giữa "Luật" và "Đạo đức" trong lĩnh vực an toàn thông tin là gì?**
A. Luật chỉ dành cho máy tính, đạo đức dành cho con người.
B. Luật được thực thi bởi các cơ quan chính quyền, còn đạo đức thì không.
C. Đạo đức có tính bắt buộc cao hơn luật.
D. Luật không dựa trên các giá trị văn hóa.

**Câu 150: Theo giáo trình, một đặc điểm khác biệt giữa "Chính sách" và "Luật" là gì?**
A. Chính sách luôn luôn bắt buộc hơn luật.
B. Việc thiếu hiểu biết chính sách có thể là một cách bào chữa chấp nhận được, còn luật thì không.
C. Chính sách chỉ áp dụng cho người quản trị hệ thống.
D. Luật không có chế tài xử phạt rõ ràng như chính sách.

**Câu 151: Đạo luật HIPAA (1996) của Hoa Kỳ tập trung vào việc bảo vệ tính bí mật và an toàn của loại dữ liệu nào?**
A. Dữ liệu tài chính ngân hàng.
B. Dữ liệu an ninh quốc phòng.
C. Dữ liệu y tế của người bệnh.
D. Dữ liệu bản quyền phần mềm.

**Câu 152: Luật An toàn thông tin mạng của Việt Nam (số 86/2015/QH13) chính thức có hiệu lực từ ngày nào?**
A. 01/01/2015.
B. 01/07/2016.
C. 01/01/2019.
D. 12/06/2018.

**Câu 153: Luật An ninh mạng của Việt Nam (số 24/2018/QH14) có hiệu lực thi hành từ thời điểm nào?**
A. 01/07/2016.
B. 01/01/2018.
C. 01/01/2019.
D. 01/07/2019.

**Câu 154: Văn bản pháp luật nào sau đây tại Việt Nam quy định về vấn đề "chống thư rác"?**
A. Luật CNTT 2006.
B. Luật An ninh mạng 2018.
C. Nghị định số 90/2008/NĐ-CP.
D. Luật Hình sự.

**Câu 155: Theo "10 điều răn về đạo đức máy tính", hành vi nào sau đây được coi là vi phạm đạo đức?**
A. Sử dụng phần mềm có bản quyền.
B. Tham gia đào tạo chuyên môn về ATTT.
C. Sử dụng tài nguyên máy tính của người khác khi không được phép hoặc không bồi thường thỏa đáng.
D. Sao lưu dữ liệu định kỳ.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 149: B.** (Trang 150). Đây là định nghĩa phân loại căn bản nhất giữa quy tắc cứng (Luật) và quy tắc mềm (Đạo đức).
*   **Đáp án Câu 150: B.** (Trang 150). Chi tiết này rất hay xuất hiện trong đề thi vì nó nhấn mạnh tầm quan trọng của việc phổ biến chính sách trong tổ chức.
*   **Đáp án Câu 151: C.** (Trang 151). Mẹo nhớ: **H**IPAA $\rightarrow$ **H**ealth (Y tế).
*   **Đáp án Câu 152: B.** (Trang 152). Nhớ cặp số: **Luật 2015 $\rightarrow$ Hiệu lực 2016**.
*   **Đáp án Câu 153: C.** (Trang 153). Nhớ cặp số: **Luật 2018 $\rightarrow$ Hiệu lực 2019**.
*   **Đáp án Câu 154: C.** (Trang 152). Đây là nghị định chuyên biệt về rác (Spam).
*   **Đáp án Câu 155: C.** (Trang 155). Điều răn số 7: "Không sử dụng tài nguyên máy tính của người khác...".

---

## IV. BẢNG TỔNG KẾT LUẬT VIỆT NAM (DÀNH CHO GHI NHỚ NHANH)

| Tên Luật | Năm ban hành | Ngày hiệu lực | Phạm vi chính |
|:---|:---|:---|:---|
| **ATTT Mạng** | 2015 | **01/07/2016** | Hoạt động ATTT mạng, mật mã dân sự, tiêu chuẩn kỹ thuật. |
| **An ninh mạng** | 2018 | **01/01/2019** | Bảo vệ an ninh quốc gia, trật tự an toàn xã hội trên không gian mạng. |

---
