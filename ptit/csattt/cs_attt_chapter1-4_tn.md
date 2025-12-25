
# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 1 (MỤC 1.1 & 1.2)
**Môn: Cơ sở An toàn Thông tin**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. "Trái tim" của ATTT: Tam giác CIA
| Thuộc tính | Tên tiếng Anh | Bản chất (Từ khóa nhận diện) | Biện pháp/Công cụ tiêu biểu |
|:---|:---|:---|:---|
| **Bí mật** | Confidentiality | Chỉ người **có thẩm quyền** mới được truy cập. | Mã hóa, VPN, bảo vệ vật lý. |
| **Toàn vẹn** | Integrity | Chỉ người có thẩm quyền mới được **sửa đổi**. | Chữ ký số, **Hàm băm (Hash)**. |
| **Sẵn sàng** | Availability | Truy cập được **bất cứ khi nào** có yêu cầu. | Cân bằng tải, Điện toán đám mây. |

*   **Lưu ý mở rộng:** Ngoài CIA, các thuộc tính bổ sung bao gồm: *Xác thực (Authenticity), Không chối bỏ (Non-repudiation), Hữu dụng (Utility), Sở hữu (Possession).*

### 2. Phân biệt các khái niệm cơ bản (Dễ nhầm lẫn)
*   **Tài sản (Asset):** Gồm tài sản **Lô gíc** (web, dữ liệu) và tài sản **Vật lý** (máy tính, thiết bị mạng).
*   **Mối đe dọa (Threat):** Bất kỳ **hành động** nào có thể gây hư hại tài sản (chưa nhất thiết đã xảy ra).
*   **Tấn công (Attack):** Hành động **có chủ ý hoặc không** làm thỏa hiệp hệ thống. Chia làm 2 loại: **Chủ động** và **Thụ động**.
*   **Truy cập (Access):** Khả năng sử dụng, xử lý, sửa đổi hoặc gây ảnh hưởng của một **Chủ thể** lên một **Đối tượng** khác.

### 3. Hệ thống thông tin (HTTT)
*   **Mô hình vận hành:** Đầu vào (Input) $\rightarrow$ Xử lý (Processing) $\rightarrow$ Đầu ra (Output).
*   **Thành phần HTTT dựa trên máy tính:** (1) Phần cứng, (2) Phần mềm, (3) Mạng/Truyền thông, (4) Cơ sở dữ liệu, (5) Thủ tục.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG (PRACTICE TEST)

**Câu 1: Định nghĩa hình thức của An toàn thông tin tập trung vào việc bảo vệ bộ ba thuộc tính nào sau đây?**
A. Bí mật, Xác thực, Sẵn sàng.
B. Bí mật, Toàn vẹn, Sẵn sàng.
C. Toàn vẹn, Sẵn sàng, Không chối bỏ.
D. Bí mật, Toàn vẹn, Hữu dụng.

**Câu 2: Để đảm bảo dữ liệu được coi là "Toàn vẹn", cần thỏa mãn đồng thời 3 điều kiện nào?**
A. Không bị thay đổi, Hợp lệ, Chính xác.
B. Không bị thay đổi, Bí mật, Sẵn sàng.
C. Chính xác, Kịp thời, Có bản quyền.
D. Hợp lệ, Duy nhất, Không thể xóa bỏ.

**Câu 3: Một nhân viên vô tình làm đổ nước gây hỏng máy chủ. Hành động này được phân loại là:**
A. Tấn công chủ động.
B. Tấn công thụ động.
C. Tấn công (có thể không có chủ ý).
D. Không phải là tấn công vì không có mục đích phá hoại.

**Câu 4: Tỷ lệ phục vụ (A) để đo tính sẵn sàng của hệ thống được tính bằng công thức nào? (Trong đó U là Uptime, D là Downtime)**
A. $A = D / (U + D)$
B. $A = U / D$
C. $A = U / (U + D)$
D. $A = (U - D) / U$

**Câu 5: Việc sao lưu dữ liệu ra các hệ thống lưu trữ đặt ở một vị trí khác (ngoại vi) được gọi là gì và thuộc lĩnh vực nào?**
A. Offsite backup - Đảm bảo thông tin.
B. Remote access - An ninh mạng.
C. Data Recovery - An toàn máy tính.
D. Cloud Storage - Quản lý rủi ro.

---

## III. GIẢI THÍCH & MẸO GHI NHỚ (RATIONALES)

*   **Đáp án Câu 1: B.** Đây là kiến thức nền tảng (Tam giác CIA). Các đáp án khác có trộn lẫn các thuộc tính bổ sung.
*   **Đáp án Câu 2: A.** (Trang 18 giáo trình). Nhớ từ khóa: **"Không đổi - Hợp lệ - Chính xác"**. Thi trắc nghiệm rất hay hỏi về "bộ ba" điều kiện này.
*   **Đáp án Câu 3: C.** (Trang 15 giáo trình). Định nghĩa Tấn công (Attack) bao gồm cả hành động **"có chủ ý hoặc KHÔNG có chủ ý"**. Đây là điểm bẫy cực lớn vì sinh viên thường nghĩ tấn công phải là hacker.
*   **Đáp án Câu 4: C.** Mẹo nhớ: Tỷ lệ sẵn sàng = (Thời gian sống) / (Tổng thời gian).
*   **Đáp án Câu 5: A.** (Trang 14 giáo trình). Ghi nhớ thuật ngữ **"Offsite backup"**.

---

## IV. GỢI Ý FLASHCARD (TỰ KIỂM TRA NHANH)
*   **Mặt A:** 3 thành phần chính của An toàn thông tin?
*   **Mặt B:** An toàn máy tính và dữ liệu; An ninh mạng; Quản lý an toàn thông tin.
*   **Mặt A:** Sự khác biệt lớn nhất giữa An ninh mạng và An ninh không gian mạng?
*   **Mặt B:** An ninh không gian mạng (Cybersecurity) không bị giới hạn bởi biên giới quốc gia về mặt vật lý.

Dựa trên nội dung từ trang 19 đến trang 23 của giáo trình, tôi tiếp tục biên soạn tài liệu ôn tập cho mục 1.3 và 1.4. Đây là những phần có rất nhiều chi tiết kỹ thuật và danh sách, cực kỳ dễ xuất hiện trong các câu hỏi trắc nghiệm về **phân loại** và **nhận diện**.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 1 (MỤC 1.3 & 1.4)

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Ba thành phần chính của ATTT (Mục 1.3)
Ba thành phần này có quan hệ mật thiết và giao thoa với nhau. Điểm chung của cả ba là **Chính sách ATTT**.

*   **An toàn máy tính và dữ liệu:** Bảo vệ phần cứng, phần mềm, dữ liệu trên máy tính. Tập trung vào: OS, ứng dụng, kiểm soát truy cập tại chỗ, phòng chống mã độc, sao lưu.
*   **An ninh mạng (Network Security):** Bảo vệ thông tin **trên đường truyền**. Công cụ chính: Firewall, Proxy, VPN, SSL/TLS, IDS/IPS. 
    *   *Lưu ý:* **Cyber Security** (An ninh không gian mạng) là thuật ngữ dùng khi nói về an ninh mạng Internet toàn cầu, không giới hạn biên giới vật lý.
*   **Quản lý ATTT:** Quản lý và giám sát việc thực thi. Nội dung cốt lõi là **Quản lý rủi ro (Risk Management)** (Nhận dạng và đánh giá rủi ro). Thực hiện theo **chu trình lặp lại** (Hình 1.10).

### 2. Bảy vùng (Domain) hạ tầng CNTT (Mục 1.4) - CỰC KỲ QUAN TRỌNG
Bạn cần nhớ tên vùng và các nguy cơ đặc trưng của vùng đó:

| Tên vùng (Domain) | Thành phần tiêu biểu | Nguy cơ/Mối đe dọa đặc trưng |
|:---|:---|:---|
| **1. Người dùng (User)** | Nhân viên, khách | **Nguy cơ lớn nhất** do khó đoán định hành vi; thiếu ý thức; tống tiền; phá hoại nội bộ. |
| **2. Máy trạm (Workstation)** | PC, Laptop, thiết bị tính toán | Tiếp xúc trực tiếp với vùng Người dùng; lỗ hổng OS/phần mềm; mã độc từ USB/CD. |
| **3. Mạng LAN** | Switch, Hub, máy chủ nội bộ | Truy cập trái phép LAN vật lý; nghe lén sóng WLAN; cấu hình máy chủ sai. |
| **4. LAN-to-WAN** | Router, Firewall | **Thăm dò và rà quét (Scanning)** trái phép các cổng dịch vụ từ bên ngoài. |
| **5. Mạng WAN** | Internet | Dữ liệu truyền dạng rõ bị **nghe lén**; tấn công DoS/DDoS; mã độc qua email. |
| **6. Truy cập từ xa** | VPN client, Broadband | **Tấn công vét cạn (Brute force)** mật khẩu; rò rỉ dữ liệu từ xa. |
| **7. Hệ thống/Ứng dụng** | Web server, DNS, Email | Lỗ hổng phần mềm ứng dụng; truy cập trái phép vào trung tâm dữ liệu/phòng máy. |

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 6: Thành phần nào sau đây được coi là "điểm chung" giao thoa giữa An toàn máy tính, An ninh mạng và Quản lý ATTT?**
A. Quản lý rủi ro.
B. Chính sách an toàn thông tin.
C. Tường lửa và mã hóa.
D. Sao lưu dự phòng.

**Câu 7: Theo giáo trình, vùng nào trong hạ tầng CNTT được đánh giá là có nhiều mối đe dọa và nguy cơ nhất?**
A. Vùng mạng WAN.
B. Vùng hệ thống/ứng dụng.
C. Vùng người dùng.
D. Vùng LAN-to-WAN.

**Câu 8: Tấn công "vét cạn" (brute force) vào tên người dùng và mật khẩu là mối đe dọa điển hình nhất của vùng nào?**
A. Vùng máy trạm.
B. Vùng truy cập từ xa (Remote Access).
C. Vùng mạng LAN.
D. Vùng người dùng.

**Câu 9: Nội dung cốt lõi của "Quản lý an toàn thông tin" là gì?**
A. Cài đặt tường lửa và IDS.
B. Quản lý rủi ro (Risk management).
C. Ban hành luật an ninh mạng.
D. Mã hóa toàn bộ dữ liệu máy tính.

**Câu 10: Việc dữ liệu thường được truyền dưới dạng "rõ" (cleartext) dẫn đến nguy cơ bị nghe lén cao nhất ở vùng nào?**
A. Vùng mạng WAN (Internet).
B. Vùng máy trạm.
C. Vùng LAN-to-WAN.
D. Vùng mạng LAN.

---

## III. GIẢI THÍCH & "BẪY" TRẮC NGHIỆM

*   **Đáp án Câu 6: B.** Nhìn vào Hình 1.9 (trang 20), bạn sẽ thấy sơ đồ Venn. "Chính sách" nằm ở vùng giao nhau của cả 3 vòng tròn.
*   **Đáp án Câu 7: C.** (Trang 23). Giáo trình ghi rõ: *"Vùng người dùng là vùng có nhiều mối đe dọa và nguy cơ nhất do người dùng có bản chất khó đoán định..."* $\rightarrow$ Rất dễ nhầm với vùng WAN vì WAN có nhiều hacker, nhưng nội bộ (User) mới là nguy cơ lớn nhất.
*   **Đáp án Câu 8: B.** (Trang 24). Mặc dù vùng nào cũng có thể bị thử mật khẩu, nhưng giáo trình xếp "Tấn công vét cạn mật khẩu" là nguy cơ **điển hình** của vùng Truy cập từ xa.
*   **Đáp án Câu 9: B.** (Trang 19). Quản lý ATTT tập trung vào giám sát và thực thi, nhưng cốt lõi là Quản lý rủi ro.
*   **Đáp án Câu 10: A.** (Trang 23). Từ khóa: **"Mạng WAN... hầu hết dữ liệu được truyền dưới dạng rõ... dễ bị nghe lén"**.

---

## IV. MẸO GHI NHỚ NHANH (MNEMONICS)
Để nhớ 7 vùng, hãy nhớ theo hành trình của một gói tin:
1.  **User** (Người dùng ngồi vào máy)
2.  **Workstation** (Bật máy trạm lên)
3.  **LAN** (Nối vào mạng nội bộ)
4.  **LAN-to-WAN** (Đi qua cửa ngõ Router/Firewall)
5.  **WAN** (Đi ra Internet)
6.  **Remote Access** (Nếu đi từ ngoài vào lại công ty thì dùng vùng này)
7.  **System/App** (Đích đến cuối cùng là các Máy chủ dịch vụ)

Đây là phần biên soạn cuối cùng của Chương 1, tập trung vào mục **1.5 (Nguyên tắc và Mô hình tổng quát)**. Đây là phần mang tính "tổng kết" toàn bộ chương, thường xuyên xuất hiện trong các câu hỏi thi về mặt hệ thống và tư duy quản lý.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 1 (MỤC 1.5)

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Nguyên tắc "Phòng vệ nhiều lớp có chiều sâu" (Defense in Depth)
*   **Bản chất:** Tạo ra **nhiều lớp bảo vệ** bổ sung cho nhau. Một công cụ đơn lẻ (dù hiện đại) không bao giờ là đủ. Kẻ tấn công phải vượt qua tất cả các lớp mới đạt được mục đích.
*   **Tam giác cân bằng:** Khi thiết kế hệ thống ATTT, phải luôn cân bằng giữa 3 yếu tố:
    1.  **Mức an toàn (Security)**
    2.  **Chi phí (Cost)**
    3.  **Tính hữu dụng (Usability)** - Khả năng cung cấp tính năng hữu ích cho người dùng.

### 2. Mô hình phòng vệ 7 lớp (Hình 1.14)
Đây là mô hình phân loại theo mức độ truy cập từ ngoài vào trong. Bạn cần nhớ thứ tự từ lớp ngoài cùng (bao bọc) đến lớp trong cùng (đối tượng cần bảo vệ):
1.  **Chính sách, thủ tục, ý thức** (Lớp ngoài cùng - con người/quy trình).
2.  **Vật lý** (Cổng, cửa, khóa, camera).
3.  **Ngoại vi** (Điểm tiếp giáp mạng ngoài).
4.  **Mạng nội bộ** (Các phân đoạn mạng bên trong).
5.  **Máy tính (Host)** (Từng thiết bị cụ thể).
6.  **Ứng dụng** (Phần mềm cụ thể).
7.  **Dữ liệu** (Lớp trong cùng - mục tiêu cốt lõi).

### 3. Mô hình phòng vệ 3 lớp chính (Hình 1.15)
Giáo trình cũng chia thành 3 lớp lớn với các lớp con cụ thể:
*   **Lớp An ninh cơ quan/tổ chức:**
    *   Bảo vệ vật lý.
    *   Chính sách & Thủ tục.
*   **Lớp An ninh mạng:**
    *   Bảo vệ vùng hạn chế (DMZ).
    *   Tường lửa (Firewall) & VPN.
*   **Lớp An ninh hệ thống (System Integrity):**
    *   **Tăng cường an ninh hệ thống (System hardening):** Cài đặt và cấu hình an toàn.
    *   **Quản trị tài khoản người dùng:** Phân quyền.
    *   **Quản lý bản vá (Patch Management):** Cập nhật lỗi an ninh định kỳ.
    *   **Phát hiện và ngăn chặn phần mềm độc hại.**

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 11: Nguyên tắc chủ đạo xuyên suốt trong đảm bảo an toàn thông tin được đề cập trong giáo trình là gì?**
A. Bảo mật bằng sự che giấu (Security by obscurity).
B. Phòng vệ nhiều lớp có chiều sâu (Defense in depth).
C. Tối ưu hóa chi phí đầu tư.
D. Công khai thuật toán mã hóa.

**Câu 12: Trong "Tam giác cân bằng" của ATTT, nếu một hệ thống cực kỳ an toàn nhưng lại quá khó sử dụng đối với nhân viên, thì hệ thống đó đang vi phạm yếu tố nào?**
A. Chi phí (Cost).
B. Mức an toàn (Security).
C. Tính hữu dụng (Usability).
D. Tính toàn vẹn (Integrity).

**Câu 13: Trong mô hình phòng vệ 7 lớp, đối tượng nào nằm ở lớp trong cùng (lớp thứ 7)?**
A. Ứng dụng.
B. Máy tính (Host).
C. Dữ liệu.
D. Chính sách và ý thức.

**Câu 14: Lớp "Chính sách, thủ tục và ý thức" nằm ở vị trí nào trong mô hình 7 lớp phòng vệ?**
A. Lớp trong cùng.
B. Lớp ngoài cùng.
C. Lớp thứ 5, ngay sau lớp ứng dụng.
D. Giao thoa giữa tất cả các lớp.

**Câu 15: Hoạt động "Quản lý bản vá" (Patch Management) và "Tăng cường an ninh hệ thống" (System hardening) thuộc lớp an ninh nào sau đây?**
A. An ninh mạng.
B. An ninh cơ quan/tổ chức.
C. An ninh hệ thống.
D. An ninh vật lý.

---

## III. GIẢI THÍCH & PHÂN TÍCH LỖI SAI

*   **Đáp án Câu 11: B.** (Trang 24). Đây là nguyên tắc cốt lõi nhất được tác giả nhấn mạnh.
*   **Đáp án Câu 12: C.** (Trang 24). Một hệ thống tốt phải cân bằng. Quá khó dùng nghĩa là tính hữu dụng (Usability) thấp.
*   **Đáp án Câu 13: C.** (Trang 25). Hãy tưởng tượng dữ liệu là "viên ngọc" được bao bọc bởi 6 lớp vỏ khác. Kẻ tấn công phải vượt qua tất cả để chạm vào dữ liệu.
*   **Đáp án Câu 14: B.** (Trang 25). Con người và quy định là lớp phòng vệ đầu tiên ngăn chặn các ý định tấn công ngay từ vòng ngoài.
*   **Đáp án Câu 15: C.** (Trang 26). Hãy nhớ: Những gì tác động trực tiếp lên cấu hình máy tính (Cài đặt, cập nhật phần mềm, quản lý tài khoản) đều thuộc về **An ninh hệ thống**.

---

## IV. BẢNG TỔNG HỢP NHANH ĐỂ SO SÁNH (Dành cho câu hỏi so sánh)

| Chức năng/Hoạt động | Thuộc lớp (Mô hình 3 lớp) |
|:---|:---|
| Camera, khóa cửa, thẻ từ | An ninh cơ quan/tổ chức (Vật lý) |
| Quy trình phục hồi sau sự cố | An ninh cơ quan/tổ chức (Chính sách & Thủ tục) |
| VPN, Tường lửa, DMZ | An ninh mạng |
| **Cài đặt, cấu hình hệ thống (Hardening)** | An ninh hệ thống |
| **Cài đặt bản vá lỗi (Patching)** | An ninh hệ thống |
| Diệt virus, chống mã độc | An ninh hệ thống |

---
Dựa trên nội dung mục 2.1 (trang 27-31) của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm. Phần này tập trung mạnh vào việc **phân loại mức độ nghiêm trọng** và **các con số thống kê** – vốn là "mỏ vàng" cho các câu hỏi thi trắc nghiệm nhận biết.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 2 (MỤC 2.1)
**Chủ đề: Tổng quan về lỗ hổng bảo mật và điểm yếu hệ thống**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Phân biệt Điểm yếu (Weakness) và Lỗ hổng (Vulnerability)
*   **Điểm yếu hệ thống:** Là lỗi, khiếm khuyết tồn tại trong hệ thống (do thiết kế, cài đặt, lập trình, quản trị hoặc cấu hình). Điểm yếu có thể có ở cả **Phần cứng** và **Phần mềm**.
*   **Lỗ hổng bảo mật:** Là một điểm yếu **cho phép kẻ tấn công khai thác** để gây tổn hại đến các thuộc tính CIA.
*   *Tư duy trắc nghiệm:* Mọi lỗ hổng đều là điểm yếu, nhưng không phải điểm yếu nào cũng là lỗ hổng (nếu nó không thể bị khai thác).

### 2. Phân loại mức độ nghiêm trọng (Theo Microsoft)
Đây là phần cực kỳ hay hỏi thi, bạn cần nhớ "điều kiện cần" để khai thác:

| Mức độ | Tên tiếng Anh | Đặc điểm nhận diện (Từ khóa) |
|:---|:---|:---|
| **Nguy hiểm** | Critical | **Không cần tương tác** của người dùng (ví dụ: sâu mạng tự lây). |
| **Quan trọng** | Important | **Cần có tương tác** của người dùng (ví dụ: lừa người dùng mở file, click link). |
| **Trung bình** | Moderate | Kẻ tấn công phải ở **cùng mạng cục bộ (LAN)** hoặc dùng kỹ thuật xã hội. |
| **Thấp** | Low | Phải có quyền **truy cập cục bộ** hoặc **truy cập vật lý** trực tiếp. |

### 3. Các con số thống kê "biết nói"
*   **Thành phần chứa nhiều lỗ hổng nhất:** Phần mềm ứng dụng (**83%**), tiếp theo là Hệ điều hành (13%) và Phần cứng (4%).
*   **Mức độ phổ biến:** Lỗ hổng mức **Trung bình** chiếm đa số (khoảng 68%).
*   **Hệ điều hành & Ứng dụng tiêu điểm:** 
    *   Hệ điều hành có nhiều lỗ hổng nhất (2015-2019): **Debian Linux** và **Android**.
    *   Ứng dụng có nhiều lỗ hổng nhất: Các sản phẩm của **Adobe** (Acrobat Reader, Flash Player) và các **Trình duyệt web**.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 1: Nguyên nhân dẫn đến sự tồn tại của các điểm yếu hệ thống có thể là do:**
A. Lỗi thiết kế hoặc lỗi lập trình.
B. Lỗi cài đặt hoặc lỗi cấu hình hoạt động.
C. Lỗi quản trị.
D. Tất cả các phương án trên.

**Câu 16 (Tiếp nối chương 1): Theo Microsoft, lỗ hổng bảo mật cho phép kẻ tấn công thực hiện mã khai thác mà "không cần tương tác của người dùng" được xếp vào cấp độ nào?**
A. Thấp (Low).
B. Trung bình (Moderate).
C. Quan trọng (Important).
D. Nguy hiểm (Critical).

**Câu 17: Điểm khác biệt cơ bản nhất giữa lỗ hổng mức "Nguy hiểm" và mức "Quan trọng" là gì?**
A. Khả năng gây thiệt hại đến tính Bí mật.
B. Yêu cầu về sự tương tác của người dùng.
C. Yêu cầu về quyền truy cập vật lý.
D. Khả năng khắc phục lỗi.

**Câu 18: Theo số liệu thống kê năm 2014, lỗ hổng bảo mật xuất hiện chủ yếu ở thành phần nào của hệ thống?**
A. Hệ thống phần cứng (4%).
B. Hệ điều hành (13%).
C. Phần mềm ứng dụng (83%).
D. Các thiết bị ngoại vi.

**Câu 19: Lỗ hổng mà kẻ tấn công "phải ở trong cùng mạng cục bộ với hệ thống nạn nhân" để khai thác thì được xếp vào mức độ nào?**
A. Nguy hiểm.
B. Quan trọng.
C. Trung bình.
D. Thấp.

**Câu 20: Hệ điều hành nào sau đây đứng đầu danh sách về số lượng lỗ hổng được phát hiện trong giai đoạn 2015-2019?**
A. Microsoft Windows 10.
B. Debian Linux và Android.
C. Ubuntu Linux.
D. Enterprise Linux Server.

---

## III. GIẢI THÍCH & MẸO "BẮT BÀI"

*   **Đáp án Câu 1: D.** (Trang 28). Một hệ thống phức tạp luôn tồn tại lỗi ở mọi khâu từ thiết kế đến vận hành.
*   **Đáp án Câu 16: D.** Từ khóa "Không tương tác" = Nguy hiểm nhất (Critical).
*   **Đáp án Câu 17: B.** Đây là bẫy so sánh. Cả hai đều có thể gây hại như nhau (vi phạm CIA), nhưng Critical thì tự động lây lan, còn Important thì phải "lừa" được người dùng làm gì đó.
*   **Đáp án Câu 18: C.** Nhớ con số **83%** (hoặc từ khóa "phần lớn tồn tại trong phần mềm ứng dụng").
*   **Đáp án Câu 19: C.** Nhớ điều kiện biên: Cùng mạng LAN = Trung bình (Moderate).
*   **Đáp án Câu 20: B.** (Trang 30). Windows 10 chỉ đứng thứ 5. Đứng đầu là Debian và Android do sự bùng nổ của thiết bị di động và IoT.

---

## IV. MẸO GHI NHỚ (STUDY TIPS)
Để nhớ 4 mức độ của Microsoft, hãy nhớ theo **"Khoảng cách"** giữa kẻ tấn công và nạn nhân:
1.  **Nguy hiểm:** Kẻ tấn công ở đâu cũng được, nạn nhân không làm gì cũng dính (Khoảng cách vô tận, tương tác bằng 0).
2.  **Quan trọng:** Kẻ tấn công gửi "mồi", nạn nhân phải cắn câu (Cần tương tác).
3.  **Trung bình:** Kẻ tấn công phải lẻn được vào chung cái sân (Mạng LAN) hoặc dùng miệng lưỡi (Kỹ thuật xã hội).
4.  **Thấp:** Kẻ tấn công phải sờ được vào máy (Truy cập vật lý/cục bộ).

---

Dựa trên nội dung từ trang 32 đến trang 37 của giáo trình, tôi đã biên soạn tài liệu ôn tập cho phần **Lỗi tràn bộ đệm (Buffer Overflow)**. Đây là phần kỹ thuật trọng tâm nhất của chương 2, đòi hỏi bạn phải nắm vững cơ chế vận hành của bộ nhớ.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 2 (MỤC 2.2.1)
**Chủ đề: Lỗi tràn bộ đệm (Buffer Overflow)**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Bản chất và Nguyên nhân
*   **Định nghĩa:** Xảy ra khi ứng dụng ghi dữ liệu vượt quá phạm vi (giới hạn đầu hoặc cuối) của bộ nhớ đệm.
*   **Hậu quả:** Ứng dụng ngừng hoạt động, mất dữ liệu, hoặc kẻ tấn công chiếm quyền kiểm soát hệ thống.
*   **Nguyên nhân gốc rễ:** Người lập trình **không kiểm tra** (hoặc kiểm tra thiếu) kích thước dữ liệu đầu vào.
*   **Ngôn ngữ rủi ro cao:** C, C++ và Hợp ngữ (do sử dụng các thư viện không an toàn như `strcpy()`).

### 2. Các vùng nhớ của chương trình (Hình 2.7)
Bạn cần nhớ chức năng của 4 vùng nhớ chính để không bị nhầm lẫn:
1.  **Vùng mã thực hiện (Executable code):** Lưu mã lệnh của chương trình.
2.  **Vùng dữ liệu toàn cục (Data):** Lưu các biến toàn cục.
3.  **Vùng cấp phát động (Heap):** Lưu dữ liệu được cấp phát/giải phóng trong quá trình chạy.
4.  **Vùng ngăn xếp (Stack):** Lưu tham số gọi hàm, dữ liệu cục bộ và **Địa chỉ trở về (Return address)**.

### 3. Cơ chế khai thác lỗi trên Stack
*   **Mục tiêu cốt lõi:** Ghi đè lên **Địa chỉ trở về (ret)** nằm trong ngăn xếp.
*   **Cách thức:** Kẻ tấn công gửi một chuỗi dữ liệu lớn (chứa mã độc) để làm tràn bộ đệm cục bộ, dữ liệu tràn sẽ đè lên ô nhớ `sfp` (con trỏ khung) và sau đó là ô `ret`.
*   **Shellcode:** Là đoạn mã máy (viết bằng ASM, C...) được kẻ tấn công chèn vào bộ đệm để thực thi (ví dụ: gọi lệnh `/bin/sh`).
*   **Lệnh NOP (No Operation):** Được chèn vào trước Shellcode để tăng khả năng thành công nếu địa chỉ `ret` không trỏ chính xác vào điểm bắt đầu của mã độc.

### 4. Ví dụ điển hình: Sâu SQL Slammer (2003)
*   **Đối tượng:** Microsoft SQL Server 2000.
*   **Giao thức/Cổng:** **UDP** cổng **1434**.
*   **Đặc điểm:** Tốc độ lây lan cực nhanh (75.000 máy chủ trong 30 phút). Sâu "lành tính" (không phá hoại file) nhưng gây nghẽn mạng nghiêm trọng.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 21: Vùng nhớ nào sau đây được chương trình sử dụng để lưu các biến cục bộ, tham số gọi hàm và địa chỉ trở về?**
A. Heap (Cấp phát động).
B. Data (Dữ liệu toàn cục).
C. Stack (Ngăn xếp).
D. Executable code (Mã thực hiện).

**Câu 22: Trong tấn công tràn bộ đệm, kẻ tấn công tìm cách ghi đè lên thành phần nào sau đây để thay đổi luồng thực thi của chương trình?**
A. Biến toàn cục.
B. Địa chỉ trở về (Return address).
C. Lệnh NOP.
D. Nhân hệ điều hành.

**Câu 23: Lệnh NOP (No Operation) có vai trò gì trong một chuỗi tấn công tràn bộ đệm?**
A. Là mã độc dùng để xóa dữ liệu.
B. Dùng để làm đệm, giúp tăng khả năng thực thi Shellcode khi địa chỉ nhảy không chính xác.
C. Dùng để mã hóa Shellcode.
D. Dùng để ngăn chặn hệ thống phát hiện xâm nhập.

**Câu 24: Cơ chế bảo vệ DEP (Data Execution Prevention) ngăn chặn tấn công tràn bộ đệm bằng cách nào?**
A. Ngẫu nhiên hóa địa chỉ bộ nhớ.
B. Thêm mã Canary vào trước địa chỉ trở về.
C. Không cho phép thực hiện mã trong vùng nhớ dành cho dữ liệu (như Stack/Heap).
D. Kiểm tra kích thước mọi dữ liệu đầu vào.

**Câu 25: Sâu SQL Slammer khai thác lỗi tràn bộ đệm trên Microsoft SQL Server 2000 thông qua giao thức và cổng dịch vụ nào?**
A. TCP cổng 80.
B. UDP cổng 1434.
C. TCP cổng 443.
D. UDP cổng 53.

**Câu 26: Kỹ thuật ngẫu nhiên hóa sơ đồ địa chỉ cấp phát các ô nhớ trong ngăn xếp để gây khó khăn cho kẻ tấn công được gọi là gì?**
A. DEP.
B. Canary.
C. ASLR.
D. Hardening.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 21: C.** Đây là đặc tính cơ bản của Stack. Heap dùng cho cấp phát động (`malloc`, `new`), còn Stack dùng cho các hàm.
*   **Đáp án Câu 22: B.** (Trang 35). Mục tiêu của mọi cuộc tấn công tràn bộ đệm ngăn xếp là chiếm quyền điều khiển bằng cách ghi đè `ret`.
*   **Đáp án Câu 23: B.** (Trang 36). NOP là "lệnh không làm gì", nó tạo ra một "máng trượt" để địa chỉ trở về chỉ cần rơi vào vùng NOP là sẽ trượt xuống đúng mã độc Shellcode.
*   **Đáp án Câu 24: C.** (Trang 38). DEP = Ngăn thực thi dữ liệu. Nếu kẻ tấn công chèn mã vào Stack (vùng dữ liệu), DEP sẽ không cho mã đó chạy.
*   **Đáp án Câu 25: B.** (Trang 37). Đây là chi tiết kỹ thuật thường xuyên xuất hiện trong đề thi. Nhớ: **Slammer - UDP - 1434**.
*   **Đáp án Câu 26: C.** ASLR (Address Space Layout Randomization). Mẹo nhớ: **R** trong ASLR là **Random** (Ngẫu nhiên).

---

## IV. BẢNG SO SÁNH CÁC CƠ CHẾ PHÒNG CHỐNG (Trang 38)

| Kỹ thuật | Cách hoạt động |
|:---|:---|
| **DEP** | Cấm chạy mã lệnh trong vùng Stack/Heap. |
| **ASLR** | Thay đổi vị trí các ô nhớ mỗi lần chạy (kẻ tấn công không biết địa chỉ `ret` ở đâu để ghi đè). |
| **Canary** | Đặt một "con chim báo bão" (số ngẫu nhiên) trước địa chỉ `ret`. Nếu số này bị đổi $\rightarrow$ phát hiện có tràn bộ đệm. |
| **Ngôn ngữ an toàn** | Dùng Java, .NET thay vì C/C++ để tự động quản lý bộ nhớ. |

---

Dựa trên nội dung từ trang 38 đến trang 40 của giáo trình, tôi đã biên soạn tài liệu ôn tập cho mục **2.2.2: Lỗi không kiểm tra đầu vào (Unvalidated input)**. Đây là lỗ hổng phổ biến nhất trong bảo mật ứng dụng web và thường xuyên xuất hiện trong các câu hỏi thi về tấn công SQL Injection.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 2 (MỤC 2.2.2)
**Chủ đề: Lỗi không kiểm tra đầu vào (Unvalidated input)**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Khái niệm và Nguồn gốc
*   **Bản chất:** Chương trình không kiểm tra hoặc kiểm tra thiếu (không đầy đủ) dữ liệu đầu vào.
*   **Tầm quan trọng:** Luôn nằm trong nhóm lỗ hổng dẫn đầu của **OWASP** (Dự án bảo mật ứng dụng web mở).
*   **Các nguồn dữ liệu đầu vào phổ biến:**
    *   Trường dữ liệu văn bản (text fields).
    *   Các lệnh qua **địa chỉ URL**.
    *   File (âm thanh, hình ảnh, đồ họa) do người dùng cung cấp.
    *   Đối số dòng lệnh (command line arguments).
    *   Dữ liệu từ mạng hoặc nguồn không tin cậy.

### 2. Hai dạng tấn công chính (Khai thác)
*   **Dạng 1: Gây lỗi hệ thống.** Cung cấp dữ liệu quá lớn hoặc sai định dạng khiến ứng dụng bị lỗi thực thi (ví dụ: lỗi 500 Internal Server Error).
*   **Dạng 2: Chèn mã khai thác (Injection).** Chèn các đoạn mã độc vào dữ liệu đầu vào để thực hiện các hành vi trái phép trên hệ thống nạn nhân. Điển hình nhất là **SQL Injection**.

### 3. Tấn công SQL Injection (Trọng tâm)
Kẻ tấn công sử dụng các ký tự đặc biệt để thay đổi cấu trúc câu lệnh SQL gốc.
*   **Ký tự dấu chấm phẩy ( ; ):** Dùng để kết thúc câu lệnh hiện tại và bắt đầu một câu lệnh mới (thực hiện nhiều lệnh theo mẻ - batch).
*   **Ký tự hai dấu gạch ngang ( -- ):** Dùng để bắt đầu phần **chú thích** (comment), từ đó loại bỏ hiệu lực của các đoạn lệnh còn lại phía sau.
*   **Ký tự dấu nháy đơn ( ' ):** Dùng để đóng/mở chuỗi dữ liệu trong SQL.

### 4. Biện pháp phòng chống
*   **Lọc dữ liệu (Filtering):** Kiểm tra kích thước, định dạng và sự hợp lý của dữ liệu.
*   **Loại bỏ ký tự đặc biệt:** Cần lọc bỏ các ký tự như `*`, `'`, `=`, `--`.
*   **Loại bỏ từ khóa ngôn ngữ:** Chặn các từ khóa như `SELECT`, `INSERT`, `UPDATE`, `DELETE`, `DROP`.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 27: Tổ chức nào sau đây chuyên thống kê các lỗi bảo mật ứng dụng web và xếp lỗi "không kiểm tra đầu vào" vào nhóm dẫn đầu?**
A. IEEE.
B. OWASP.
C. ISO.
D. IETF.

**Câu 28: Kẻ tấn công chèn thêm một câu lệnh `DELETE FROM tbl_products` vào sau một từ khóa tìm kiếm. Để câu lệnh này thực hiện được, kẻ tấn công thường sử dụng ký tự nào để ngăn cách giữa các câu lệnh?**
A. Dấu hai chấm ( : ).
B. Dấu chấm phẩy ( ; ).
C. Dấu gạch ngang ( - ).
D. Dấu nháy kép ( " ).

**Câu 29: Trong tấn công SQL Injection, ký tự `--` được sử dụng với mục đích gì?**
A. Để bắt đầu một câu lệnh xóa.
B. Để kết thúc một câu lệnh tìm kiếm.
C. Để bắt đầu phần chú thích, nhằm vô hiệu hóa phần còn lại của câu lệnh SQL gốc.
D. Để mã hóa dữ liệu đầu vào.

**Câu 30: Đâu là giải pháp hiệu quả nhất để phòng chống tấn công chèn mã khai thác vào dữ liệu đầu vào?**
A. Cài đặt phần mềm diệt virus trên máy chủ.
B. Mã hóa toàn bộ cơ sở dữ liệu.
C. Sử dụng các bộ lọc (filter) để loại bỏ các ký tự đặc biệt và từ khóa nhạy cảm.
D. Tăng cấu hình phần cứng của máy chủ web.

**Câu 31: Một trang web hiển thị lỗi "500 Internal Server Error" khi người dùng nhập một chuỗi ký tự quá dài vào ô tìm kiếm. Đây là ví dụ của dạng tấn công khai thác lỗi không kiểm tra đầu vào nào?**
A. Chèn mã khai thác (Injection).
B. Cung cấp dữ liệu quá lớn hoặc sai định dạng để gây lỗi ứng dụng.
C. Tấn công vét cạn mật khẩu.
D. Tấn công nghe lén đường truyền.

---

## III. GIẢI THÍCH & PHÂN TÍCH CHI TIẾT

*   **Đáp án Câu 27: B.** OWASP (Open Web Application Security Project) là cái tên bạn buộc phải nhớ khi học về bảo mật web.
*   **Đáp án Câu 28: B.** (Trang 14/40). Dấu chấm phẩy `;` cho phép thực hiện nhiều lệnh SQL trong một chuỗi lệnh (batch processing).
*   **Đáp án Câu 29: C.** (Trang 14/40). Đây là kỹ thuật rất phổ biến để "vứt bỏ" phần logic phía sau của câu lệnh gốc mà người lập trình đã soạn sẵn.
*   **Đáp án Câu 30: C.** (Trang 14/40). Việc lọc (Filtering) là chốt chặn quan trọng nhất tại tầng ứng dụng trước khi dữ liệu được gửi đến Cơ sở dữ liệu.
*   **Đáp án Câu 31: B.** (Trang 13/39). Đây là dạng khai thác đơn giản nhất bằng cách phá vỡ cấu trúc xử lý thông thường của ứng dụng thông qua kích thước dữ liệu quá lớn.

---

## IV. BẢNG TỔNG HỢP CÁC KÝ TỰ CẦN LỌC (Trang 40)

| Ký tự/Từ khóa | Mục đích tấn công |
|:---|:---|
| `'` (Nháy đơn) | Thay đổi ranh giới giữa dữ liệu và mã lệnh. |
| `;` (Chấm phẩy) | Ghép thêm câu lệnh thứ 2, thứ 3 vào sau lệnh gốc. |
| `--` (Hai gạch) | Vô hiệu hóa các điều kiện kiểm tra phía sau câu lệnh. |
| `DROP` | Xóa sổ hoàn toàn một bảng dữ liệu hoặc cơ sở dữ liệu. |
| `DELETE` | Xóa các bản ghi trong bảng. |

---
Dựa trên nội dung từ trang 40 đến trang 42 của giáo trình, tôi đã biên soạn tài liệu ôn tập cho mục **2.2.3 đến 2.2.6**. Đây là phần kiến thức về quản trị hệ thống và các lỗi logic (như Race condition), rất hay xuất hiện trong các câu hỏi tình huống của bài thi trắc nghiệm.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 2 (MỤC 2.2.3 - 2.2.6)
**Chủ đề: Kiểm soát truy cập, Hệ mật mã và Các lỗi bảo mật khác**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Kiểm soát truy cập (Access Control) - Mục 2.2.3 & 2.2.4
Kiểm soát truy cập là trả lời câu hỏi: **Ai (Chủ thể)** được truy cập đến **Cái gì (Đối tượng)**. Quy trình gồm 2 khâu then chốt:
*   **Xác thực (Authentication):** Xác minh "Bạn là ai?" (nhận diện tính chân thực của thông tin).
*   **Trao quyền/Ủy quyền (Authorization):** Xác minh "Bạn được làm gì?" (cấp quyền sau khi đã xác thực).

**Các điểm yếu thường gặp:**
*   Mật khẩu để ở dạng **rõ (cleartext)** hoặc quá đơn giản.
*   Ứng dụng chạy bằng tài khoản **Quản trị (Admin/Root)** $\rightarrow$ Nếu bị hack, kẻ tấn công có toàn quyền hệ thống.
*   Chỉ ẩn link trên giao diện mà không kiểm tra quyền ở phía máy chủ (người dùng gõ trực tiếp URL vẫn vào được).

**Nguyên tắc vàng để phòng chống:**
*   **Nguyên tắc quyền tối thiểu (Least Privilege):** Chỉ cấp quyền vừa đủ để thực hiện nhiệm vụ.
*   Không dùng tài khoản Admin để chạy ứng dụng thông thường.

### 2. Điểm yếu trong các hệ mật mã - Mục 2.2.5
*   Sử dụng giải thuật **lỗi thời/yếu**: DES, MD4, MD5.
*   Sử dụng khóa quá ngắn hoặc dễ đoán.
*   **Vấn đề trao đổi khóa:** Khóa bí mật bị lộ khi truyền qua môi trường không an toàn (Internet).
*   Sử dụng chứng chỉ số đã hết hạn hoặc bị thu hồi.

### 3. Lỗi thao tác file và Điều kiện đua tranh (Race Condition) - Mục 2.2.6
*   **Lỗi file:** Cho phép tải file lên máy chủ mà không kiểm tra định dạng hoặc không cấm quyền thực thi $\rightarrow$ Kẻ tấn công tải mã độc lên và chạy.
*   **Điều kiện đua tranh (Race condition):** 
    *   *Bản chất:* Xảy ra khi có sự thay đổi **trật tự/thời gian** của 2 hay nhiều sự kiện làm thay đổi hành vi hệ thống.
    *   *Khai thác:* Kẻ tấn công lợi dụng khoảng thời gian cực ngắn giữa lúc hệ thống "kiểm tra" và "thực hiện" để chèn mã độc hoặc đổi tên file.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 32: Quy trình kiểm soát truy cập thông thường bao gồm 2 khâu chính nào sau đây?**
A. Nhận dạng và Mã hóa.
B. Xác thực và Trao quyền.
C. Đăng nhập và Thoát.
D. Lọc dữ liệu và Kiểm tra file.

**Câu 33: Việc cấp quyền truy cập cho người dùng ở mức "vừa đủ để thực thi nhiệm vụ" được gọi là nguyên tắc gì?**
A. Nguyên tắc bảo mật đa lớp.
B. Nguyên tắc quyền tối thiểu (Least privilege).
C. Nguyên tắc tin cậy tuyệt đối.
D. Nguyên tắc phòng thủ chiều sâu.

**Câu 34: Một trang web không thực hiện kiểm tra quyền trên từng trang mà chỉ ẩn đi các liên kết đến trang đó trên menu. Điểm yếu này thuộc khâu nào?**
A. Xác thực (Authentication).
B. Trao quyền (Authorization).
C. Mã hóa (Cryptography).
D. Kiểm soát vật lý.

**Câu 35: Thuật ngữ "Race condition" (Điều kiện đua tranh) dùng để chỉ loại lỗi bảo mật nào?**
A. Lỗi tràn bộ nhớ đệm do dữ liệu quá lớn.
B. Lỗi mật mã do sử dụng khóa quá ngắn.
C. Lỗi xảy ra do sự thay đổi trật tự hoặc thời gian của các sự kiện.
D. Lỗi do người dùng nhập sai mật khẩu quá nhiều lần.

**Câu 36: Các giải thuật mật mã nào sau đây được giáo trình liệt kê là đã lạc hậu và có lỗ hổng không nên sử dụng?**
A. AES và SHA-256.
B. DES và MD5.
C. RSA và ECC.
D. PGP và SSL.

**Câu 37: Tại sao không nên sử dụng tài khoản quản trị (root/administrator) để thực thi các chương trình ứng dụng?**
A. Vì làm hệ thống chạy chậm hơn.
B. Vì tài khoản này không hỗ trợ chạy ứng dụng.
C. Vì nếu ứng dụng bị chiếm quyền, kẻ tấn công sẽ có toàn quyền kiểm soát hệ thống.
D. Vì tài khoản quản trị không có quyền truy cập Internet.

---

## III. GIẢI THÍCH & GHI CHÚ (RATIONALES)

*   **Đáp án Câu 32: B.** (Trang 40). Đây là khái niệm căn bản. Nhớ: Kiểm soát truy cập = Xác thực + Trao quyền.
*   **Đáp án Câu 33: B.** (Trang 41). **Least Privilege** là từ khóa cực kỳ quan trọng trong quản trị an ninh mạng.
*   **Đáp án Câu 34: B.** (Trang 41). Hệ thống đã biết người dùng là ai (đã xác thực), nhưng không kiểm tra xem người dùng đó "được phép vào trang này hay không" (lỗi trao quyền).
*   **Đáp án Câu 35: C.** (Trang 42). Từ khóa nhận diện Race condition trong trắc nghiệm luôn là: **"thứ tự" (order)** hoặc **"thời gian" (timing/interval)**.
*   **Đáp án Câu 36: B.** (Trang 41). Nhớ bộ ba "tử thần": **DES, MD4, MD5**.
*   **Đáp án Câu 37: C.** (Trang 40). Đây là lỗi cấu hình/quản trị phổ biến dẫn đến hậu quả nghiêm trọng nhất.

---

## IV. MẸO GHI NHỚ NHANH
*   **Xác thực vs Trao quyền:** Hãy nghĩ đến việc đi máy bay. Bạn đưa CMND cho nhân viên soi là **Xác thực** (xem bạn đúng là bạn không). Bạn đưa vé để vào phòng chờ thương gia là **Trao quyền** (xem bạn có quyền vào đó không).
*   **Race condition:** Hãy nghĩ đến cuộc đua. Kẻ tấn công tìm cách "về đích" (thực hiện mã độc) trong lúc hệ thống còn đang bận "soát vé" (kiểm tra tính hợp lệ).

---
Dựa trên nội dung từ trang 42 đến trang 46 của giáo trình, tôi đã biên soạn phần tài liệu ôn tập cuối cùng của Chương 2. Phần này tập trung vào các **nguồn thông tin**, **nguyên tắc quản lý** và các **tên công cụ cụ thể**. Đây là phần rất dễ lấy điểm nếu bạn nhớ được đặc điểm riêng biệt của từng công cụ.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 2 (MỤC 2.3 - 2.4)
**Chủ đề: Quản lý lỗ hổng và Công cụ rà quét bảo mật**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Nguyên tắc Quản lý và Khắc phục (Mục 2.3)
*   **Nguyên tắc chung:** Phải cân bằng giữa **An toàn (Security)** - **Chi phí (Cost)** - **Tính hữu dụng (Usability)**.
*   **Các nguồn cập nhật thông tin lỗ hổng uy tín:**
    *   **CVE** (Common Vulnerabilities and Exposures): Danh sách các lỗ hổng phổ biến.
    *   **NVD** (National Vulnerability Database): Cơ sở dữ liệu lỗ hổng quốc gia Hoa Kỳ.
    *   **OWASP**: Chuyên về bảo mật ứng dụng Web.
*   **Chiến lược phòng chống:**
    *   **Cập nhật bản vá (Patch Management):** Là biện pháp thiết yếu nhất (Windows Update, Google Update Service...).
    *   **Giảm bề mặt tiếp xúc:** Sử dụng Tường lửa (Firewall), Proxy để chặn các cổng/dịch vụ không cần thiết.
    *   **Phát triển phần mềm an toàn:** Đưa yêu cầu an ninh vào mọi khâu của quy trình phát triển.

### 2. Các công cụ rà quét (Scanner) - Mục 2.4
Bạn cần phân biệt rõ công cụ nào quét **Hệ thống** và công cụ nào quét **Web**:

| Nhóm công cụ | Tên phần mềm tiêu biểu | Đặc điểm ghi nhớ (Từ khóa) |
|:---|:---|:---|
| **Rà quét Hệ thống** | **MBSA** (Microsoft Baseline Security Analyzer) | **Miễn phí**, nhanh, **chỉ quét được đồ của Microsoft** (Windows, Office, SQL Server). |
| **Rà quét Hệ thống** | **Nessus** | Quét được **nhiều hệ điều hành** (Linux, Windows...); phí bản quyền cao, chậm. |
| **Rà quét Web** | **Acunetix** | Tốc độ nhanh, giao diện trực quan, kết hợp kiểm thử hộp trắng/hộp đen. |
| **Rà quét Web** | **IBM AppScan**, **SQLmap** | SQLmap chuyên về lỗ hổng chèn mã SQL. |

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 38: Để cập nhật thông tin mới nhất về các lỗ hổng bảo mật đã được công bố trên toàn thế giới, người quản trị nên tham khảo nguồn nào sau đây?**
A. IEEE.
B. CVE hoặc NVD.
C. Wikipedia.
D. Facebook Security Group.

**Câu 39: Đâu là hạn chế lớn nhất của công cụ rà quét lỗ hổng Microsoft Baseline Security Analyzer (MBSA)?**
A. Tốc độ rà quét rất chậm.
B. Phí bản quyền rất cao.
C. Chỉ có khả năng rà quét hệ điều hành và ứng dụng của Microsoft.
D. Không có giao diện đồ họa.

**Câu 40: Công cụ nào sau đây có khả năng rà quét tìm điểm yếu trên nhiều hệ điều hành khác nhau (Windows, Linux, Unix...) và các ứng dụng đa dạng?**
A. MBSA.
B. Nessus Vulnerability Scanner.
C. Notepad++.
D. Windows Defender.

**Câu 41: Công cụ nào sau đây được giáo trình nhắc đến như một trong những bộ công cụ quét lỗ hổng website phổ biến nhất hiện nay?**
A. MBSA.
B. Acunetix Web Vulnerability Scanner.
C. Wireshark.
D. Nessus.

**Câu 42: Theo giáo trình, ưu điểm nổi bật của công cụ Acunetix là gì?**
A. Miễn phí hoàn toàn.
B. Tốc độ nhanh, giao diện trực quan và có cơ sở dữ liệu hàng ngàn mẫu tấn công.
C. Tích hợp sẵn trong hệ điều hành Windows.
D. Chỉ chuyên dùng để quét lỗ hổng phần cứng.

**Câu 43: Công cụ SQLmap thường được sử dụng cho mục đích gì?**
A. Rà quét lỗ hổng trên hệ điều hành Linux.
B. Kiểm tra cấu hình tường lửa.
C. Rà quét lỗ hổng chèn mã SQL (SQL Injection) trên các website.
D. Cập nhật bản vá cho Windows.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 38: B.** (Trang 42). CVE và NVD là hai "thư viện" lỗ hổng tiêu chuẩn toàn cầu được nhắc tới trong giáo trình.
*   **Đáp án Câu 39: C.** (Trang 44). Tên gọi đã nói lên tất cả: "Microsoft Baseline...". Nó không thể quét được Linux hay các phần mềm của hãng khác như Adobe, Oracle.
*   **Đáp án Câu 40: B.** (Trang 45). Nessus là công cụ "đa năng" và chuyên nghiệp hơn MBSA, nhưng bù lại nó đắt tiền và chậm hơn.
*   **Đáp án Câu 41: B.** (Trang 45). Đây là công cụ hàng đầu cho web. Lưu ý: Nessus cũng có thể quét web nhưng Acunetix chuyên biệt và phổ biến hơn cho mục đích này.
*   **Đáp án Câu 42: B.** (Trang 46). Acunetix được đánh giá cao vì tính dễ dùng và kho dữ liệu mẫu tấn công phong phú.
*   **Đáp án Câu 43: C.** (Trang 45). Từ khóa: **SQLmap $\rightarrow$ SQL Injection**.

---

## IV. MẸO GHI NHỚ Tên Công Cụ
*   **MBSA**: "M" là Microsoft $\rightarrow$ Chỉ quét đồ Microsoft.
*   **Nessus**: Nghe giống "Necessary" (Cần thiết) $\rightarrow$ Một công cụ chuyên nghiệp cần thiết cho mọi hệ điều hành.
*   **Acunetix**: Nghe giống "Accurate" (Chính xác) $\rightarrow$ Quét web chính xác và nhanh chóng.
*   **SQLmap**: "Bản đồ SQL" $\rightarrow$ Dùng để tìm đường tấn công vào cơ sở dữ liệu SQL.

---
Dựa trên nội dung từ trang 48 đến trang 52 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục 3.1 và 3.2. Phần này tập trung vào các **định nghĩa phân loại tấn công** và **nhận diện công cụ**, vốn là những câu hỏi "ăn điểm" nhưng rất dễ nhầm lẫn nếu không nhớ rõ từ khóa.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 3 (MỤC 3.1 & 3.2)
**Chủ đề: Khái quát về Tấn công và Công cụ hỗ trợ**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Công thức cốt lõi (Mục 3.1.2)
*   **Tấn công = Mối đe dọa + Lỗ hổng bảo mật.**
*   *Tư duy trắc nghiệm:* Mối đe dọa là khách quan (không triệt tiêu được hoàn toàn), Lỗ hổng là chủ quan (có thể giảm thiểu). Tấn công chỉ xảy ra khi có cả hai.

### 2. Phân loại tấn công theo MỤC ĐÍCH (4 loại chính)
Đây là phần cực kỳ hay hỏi về định nghĩa từ khóa:
*   **Giả mạo (Fabrication):** Tạo ra thông tin sai (email giả, IP giả) để đánh lừa.
*   **Chặn bắt (Interception):** Nghe lén hoặc chuyển hướng thông tin (tấn công vào tính **Bí mật**).
*   **Gây ngắt quãng (Interruption):** Làm quá tải, làm chậm hoặc ngắt kênh truyền (tấn công vào tính **Sẵn sàng**).
*   **Sửa đổi (Modification):** Thay đổi nội dung dữ liệu trên đường truyền hoặc trong file (tấn công vào tính **Toàn vẹn**).

### 3. Phân loại tấn công theo HÌNH THỨC (2 kiểu chính)
*   **Tấn công Thụ động (Passive):** Chỉ nghe lén, giám sát lưu lượng, **KHÔNG gây thay đổi** hệ thống. 
    *   *Đặc điểm:* Thường là giai đoạn đầu để thu thập thông tin cho tấn công chủ động.
*   **Tấn công Chủ động (Active):** Đột nhập, **SỬA ĐỔI** dữ liệu, giành quyền truy cập trái phép.

### 4. Công cụ hỗ trợ tấn công (Mục 3.2)
Bạn cần nhớ tên công cụ và cổng dịch vụ (Port) tương ứng:
*   **Quét cổng (Port Scanner):** Tìm cổng mở để biết dịch vụ đang chạy.
    *   *Cổng cần nhớ:* **80/443** (Web), **25** (Email/SMTP), **1433** (SQL Server), **53** (DNS).
    *   *Công cụ:* **Nmap, Zenmap** (Giao diện đồ họa của Nmap), Angry IP Scanner.
*   **Nghe lén (Sniffer):** Bắt các gói tin trên mạng.
    *   *Công cụ:* **Tcpdump, Wireshark**.
*   **Ghi phím gõ (Keylogger):** Ghi lại mọi phím người dùng gõ. Có cả dạng phần cứng (khớp nối) và phần mềm.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 44: Theo giáo trình, một cuộc tấn công bảo mật chỉ có thể trở thành hiện thực khi có sự tồn tại đồng thời của hai yếu tố nào?**
A. Hacker và Virus.
B. Mối đe dọa và Lỗ hổng bảo mật.
C. Máy tính và Internet.
D. Phần mềm độc hại và Sai sót của người dùng.

**Câu 45: Dạng tấn công nào làm ngắt, làm chậm kênh truyền thông hoặc làm quá tải hệ thống nhằm ngăn cản việc truy cập của người dùng hợp pháp?**
A. Giả mạo (Fabrication).
B. Chặn bắt (Interception).
C. Gây ngắt quãng (Interruption).
D. Sửa đổi (Modification).

**Câu 46: Một cuộc tấn công chỉ thực hiện việc nghe lén và giám sát lưu lượng trên đường truyền mà không gây ra bất kỳ thay đổi nào trên hệ thống được gọi là:**
A. Tấn công chủ động (Active attack).
B. Tấn công vật lý.
C. Tấn công thụ động (Passive attack).
D. Tấn công giả mạo.

**Câu 47: Khẳng định nào sau đây là ĐÚNG khi nói về mối quan hệ giữa tấn công thụ động và tấn công chủ động?**
A. Tấn công chủ động luôn diễn ra trước tấn công thụ động.
B. Tấn công thụ động thường là giai đoạn đầu của một cuộc tấn công chủ động.
C. Tấn công thụ động gây thiệt hại lớn hơn tấn công chủ động.
D. Hai loại tấn công này không có mối liên hệ nào với nhau.

**Câu 48: Khi sử dụng công cụ quét cổng, nếu thấy cổng 25 đang mở, kẻ tấn công có thể xác định dịch vụ nào sau đây đang hoạt động?**
A. Dịch vụ Web (HTTP).
B. Dịch vụ tên miền (DNS).
C. Dịch vụ gửi/nhận email (SMTP).
D. Dịch vụ quản trị cơ sở dữ liệu SQL Server.

**Câu 49: Công cụ nào sau đây thường được sử dụng để bắt các gói tin truyền trên mạng nhằm mục đích nghe lén thông tin nhạy cảm?**
A. Zenmap.
B. Wireshark.
C. Keylogger.
D. Angry IP Scanner.

**Câu 50: Thiết bị phần cứng được cắm vào giữa cổng bàn phím và máy tính để ghi lại thông tin người dùng nhập vào được gọi là:**
A. Sniffer phần cứng.
B. Port scanner vật lý.
C. Keylogger phần cứng.
D. Firewall ngoại vi.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 44: B.** (Trang 49). Đây là định nghĩa toán học cơ bản của chương 3.
*   **Đáp án Câu 45: C.** Từ khóa "ngăn cản truy cập", "làm chậm" $\rightarrow$ Ngắt quãng (Interruption).
*   **Đáp án Câu 46: C.** (Trang 49). Đặc điểm nhận diện quan trọng nhất của tấn công thụ động là **"không gây ra thay đổi"**.
*   **Đáp án Câu 47: B.** (Trang 49). Tấn công thụ động dùng để "trinh sát", thu thập thông tin trước khi ra đòn chủ động.
*   **Đáp án Câu 48: C.** (Trang 50). Bạn phải thuộc danh sách: 80/443 (Web), 25 (Email), 1433 (SQL), 53 (DNS).
*   **Đáp án Câu 49: B.** Wireshark là Sniffer phổ biến nhất. Zenmap và Angry IP là công cụ Quét cổng.
*   **Đáp án Câu 50: C.** (Trang 52 và Hình 3.3). Ghi phím gõ bằng khớp nối vật lý là Keylogger phần cứng.

---

## IV. MẸO GHI NHỚ (MNEMONICS)
*   **4 mục đích tấn công (F-I-I-M):**
    *   **F**abrication = **F**ake (Giả mạo).
    *   **I**nterception = **I**nside look (Chặn bắt/Nghe lén).
    *   **I**nterruption = **I**nterrupt (Ngắt quãng/Ngừng trệ).
    *   **M**odification = **M**ake change (Sửa đổi).
*   **Cổng dịch vụ (Ports):**
    *   25: "Gửi 25 bức thư" (Email).
    *   53: "Năm ba cái tên" (DNS - Tên miền).
    *   1433: Số của SQL Server.

---
Dựa trên nội dung từ trang 52 đến trang 58 của giáo trình, tôi đã biên soạn tài liệu ôn tập cho phần **Tấn công mật khẩu** và **Tấn công chèn mã SQL (nâng cao)**. Đây là những phần kiến thức trọng tâm, thường xuyên xuất hiện các câu hỏi yêu cầu hiểu rõ cơ chế lệnh và các con số tiêu chuẩn.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 3 (MỤC 3.3.1 & 3.3.2)

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Tấn công mật khẩu (Mục 3.3.1)
Có 2 hình thức chính bạn cần phân biệt rõ qua từ khóa:
*   **Tấn công từ điển (Dictionary attack):** Sử dụng danh sách các từ có **tần suất sử dụng cao** đã được biên soạn sẵn. 
    *   *Ưu điểm:* Giảm số lần thử, tăng tốc độ nếu người dùng đặt mật khẩu đơn giản.
*   **Tấn công vét cạn (Brute force attack):** Sinh ra **tất cả các tổ hợp** ký tự, số... một cách tự động. 
    *   *Cơ chế:* Thường dùng đối với mật khẩu đã mã hóa (hacker mã hóa tổ hợp vừa sinh ra rồi so sánh với chuỗi hash thu thập được).

**Tiêu chuẩn mật khẩu an toàn (Cực kỳ hay hỏi số liệu):**
*   **Người dùng thường:** Độ dài $\ge$ **8 ký tự**, gồm 4 loại (hoa, thường, số, đặc biệt).
*   **Quản trị viên:** Độ dài $\ge$ **10 ký tự**.
*   **Thời hạn thay đổi:** 3 tháng hoặc 6 tháng.
*   **Chốt chặn:** Khóa tài khoản nếu nhập sai **3 lần** liên tục.

### 2. Tấn công chèn mã SQL - SQL Injection (Mục 3.3.2)
Đây là phần nâng cao, đi sâu vào các kỹ thuật khai thác logic:

*   **Vượt qua xác thực (Bypass):** Sử dụng chuỗi `' OR 1=1--`. 
    *   `OR 1=1` khiến mệnh đề WHERE luôn đúng.
    *   `--` biến phần kiểm tra mật khẩu phía sau thành chú thích (vô hiệu hóa).
*   **Thao tác dữ liệu trái phép:** Dùng dấu chấm phẩy ( `;` ) để kết thúc lệnh gốc và chèn thêm lệnh `DELETE`, `UPDATE`, `INSERT`.
*   **Đánh cắp thông tin (Data Theft):**
    *   Sử dụng `ORDER BY` hoặc `UNION SELECT` để tìm số lượng cột.
    *   Truy cập các bảng hệ thống (Metadata): `sys.tables`, `sys.columns` (trong MSSQL).
*   **Chiếm quyền điều khiển máy chủ:** Sử dụng các thủ tục hệ thống như `xp_cmdshell` (trong MSSQL) để chạy lệnh của hệ điều hành (ví dụ: `dir`, `shutdown`, `net stop`).

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 51: Dạng tấn công mật khẩu nào sử dụng danh sách các mật khẩu phổ biến được biên soạn sẵn để giảm số lần thử và tăng khả năng thành công?**
A. Tấn công vét cạn (Brute force).
B. Tấn công dựa trên từ điển (Dictionary attack).
C. Tấn công nghe lén (Sniffing).
D. Tấn công kỹ thuật xã hội.

**Câu 52: Theo giáo trình, mật khẩu dành cho "người quản trị hệ thống" cần đảm bảo độ dài tối thiểu là bao nhiêu ký tự?**
A. 6 ký tự.
B. 8 ký tự.
C. 10 ký tự.
D. 12 ký tự.

**Câu 53: Để phòng chống tấn công mật khẩu, hệ thống nên thực hiện cơ chế nào sau đây khi người dùng nhập sai thông tin nhiều lần?**
A. Tự động gửi mật khẩu mới về email.
B. Khóa tài khoản trong một khoảng thời gian sau 3 lần đăng nhập lỗi liên tục.
C. Hiển thị mật khẩu cũ để người dùng nhớ lại.
D. Yêu cầu đổi tên đăng nhập.

**Câu 54: Trong cuộc tấn công SQL Injection vào Form đăng nhập, chuỗi ký tự `' OR 1=1--` có tác dụng gì?**
A. Làm hỏng cơ sở dữ liệu của website.
B. Mã hóa tên đăng nhập của quản trị viên.
C. Làm cho điều kiện xác thực luôn đúng và vô hiệu hóa phần kiểm tra mật khẩu.
D. Tự động xóa tài khoản quản trị.

**Câu 55: Kẻ tấn công sử dụng câu lệnh `Samsung Galaxy S20'; DELETE FROM tbl_products;--` vào ô tìm kiếm. Dấu chấm phẩy ( ; ) trong chuỗi này có vai trò gì?**
A. Dùng để bắt đầu phần chú thích.
B. Dùng để ngăn cách giữa hai câu lệnh SQL để thực hiện theo lô (batch).
C. Dùng để đóng chuỗi ký tự đang tìm kiếm.
D. Dùng để báo hiệu kết thúc toàn bộ phiên làm việc.

**Câu 56: Thủ tục hệ thống nào của Microsoft SQL Server thường bị kẻ tấn công lợi dụng để thực hiện các lệnh của hệ điều hành nhằm chiếm quyền điều khiển máy chủ?**
A. `sp_addlogin`.
B. `xp_cmdshell`.
C. `UNION SELECT`.
D. `ORDER BY`.

**Câu 57: Đâu là giải pháp hiệu quả nhất để ngăn chặn triệt để tấn công SQL Injection?**
A. Chỉ cài đặt phần mềm diệt virus trên máy chủ.
B. Sử dụng thủ tục lưu trữ (Stored Procedure) hoặc tham số hóa dữ liệu (Parameterized).
C. Yêu cầu người dùng đặt mật khẩu phức tạp.
D. Ẩn các thông báo lỗi của hệ quản trị cơ sở dữ liệu.

---

## III. GIẢI THÍCH & PHÂN TÍCH CHI TIẾT

*   **Đáp án Câu 51: B.** Nhớ từ khóa: **"Danh sách biên soạn sẵn" = Từ điển**.
*   **Đáp án Câu 52: C.** (Trang 53). Người dùng thường là 8, Quản trị là 10. Đừng nhầm lẫn giữa hai con số này.
*   **Đáp án Câu 53: B.** (Trang 53). Đây là biện pháp ngăn chặn tấn công vét cạn (Brute force) hiệu quả nhất.
*   **Đáp án Câu 54: C.** (Trang 55). `1=1` luôn đúng, `OR` với bất kỳ cái gì cũng ra đúng. `--` là "phù thủy" biến mọi lệnh kiểm tra pass phía sau thành vô nghĩa.
*   **Đáp án Câu 55: B.** (Trang 56). SQL hỗ trợ chạy nhiều lệnh cùng lúc (batch), dấu `;` là dấu phân cách.
*   **Đáp án Câu 56: B.** (Trang 57). Nhớ từ khóa: **xp_cmdshell $\rightarrow$ Command Shell $\rightarrow$ Lệnh HĐH**.
*   **Đáp án Câu 57: B.** (Trang 58). Lọc dữ liệu chỉ là bước đầu, **Tham số hóa (Parameterized)** mới là kỹ thuật tách biệt hoàn toàn dữ liệu khỏi mã lệnh, khiến mã độc không thể thực thi.

---

## IV. MẸO GHI NHỚ LỆNH (TECH TIPS)
Khi gặp các câu hỏi về SQL Injection, hãy nhớ:
*   `UNION SELECT` hoặc `ORDER BY`: Dùng để **thăm dò** cấu trúc (cột, bảng).
*   `DELETE`, `DROP`, `UPDATE`: Dùng để **phá hoại/sửa đổi**.
*   `xp_cmdshell`: Dùng để **leo thang đặc quyền** (chiếm quyền máy chủ).
*   `--` hoặc `/*`: Dùng để **vô hiệu hóa** phần còn lại của câu lệnh.

---
Dựa trên nội dung từ trang 59 đến trang 64 của giáo trình, tôi đã biên soạn tài liệu ôn tập cho phần **Tấn công từ chối dịch vụ (DoS)** và **Từ chối dịch vụ phân tán (DDoS)**. 

Đây là phần kiến thức cực kỳ quan trọng, thường xuyên xuất hiện các câu hỏi liên quan đến **sơ đồ bắt tay 3 bước**, **địa chỉ giả mạo** và **cấu trúc mạng máy tính ma (Botnet)**.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 3 (MỤC 3.3.3 & 3.3.4)
**Chủ đề: Tấn công DoS và DDoS**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Tấn công từ chối dịch vụ (DoS) - Mục 3.3.3
*   **Mục đích:** Ngăn chặn người dùng hợp pháp truy cập tài nguyên mạng.
*   **Phân loại theo cơ chế:**
    *   **Tấn công lô gíc:** Khai thác lỗi phần mềm (Ví dụ: SQL Slammer khai thác lỗi tràn bộ đệm).
    *   **Tấn công gây ngập lụt:** Gửi lượng lớn yêu cầu để làm cạn kiệt tài nguyên/băng thông.
*   **Các kỹ thuật điển hình:**
    *   **SYN Flood:** Khai thác điểm yếu trong **thủ tục bắt tay 3 bước (3-way handshake)** của giao thức TCP. Kẻ tấn công gửi gói **SYN**, nhận **SYN-ACK** nhưng **KHÔNG gửi lại gói ACK**. Hệ thống nạn nhân bị điền đầy **Bảng kết nối (Backlog)**.
    *   **Smurf:** Sử dụng giao thức **ICMP (Ping)** và **địa chỉ quảng bá (broadcast)**. Kẻ tấn công giả mạo địa chỉ IP nguồn là địa chỉ của nạn nhân, gửi yêu cầu Ping đến địa chỉ quảng bá. Tất cả máy trong mạng đó đồng loạt phản hồi về máy nạn nhân.

### 2. Tấn công từ chối dịch vụ phân tán (DDoS) - Mục 3.3.4
*   **Điểm khác biệt với DoS:** Phạm vi tấn công lớn hơn, hàng ngàn máy tham gia, phân tán toàn cầu, cực kỳ khó lần vết.
*   **Thành phần trong mạng Botnet:**
    *   **Bot/Zombie:** Các máy tính ma bị chiếm quyền điều khiển và cài đặt mã độc (agent).
    *   **Handler/Master:** Các máy trung gian dùng để điều khiển các Bot.
    *   **C&C (Command and Control):** Hệ thống máy chủ lệnh và điều khiển của kẻ tấn công.
*   **Hai dạng kiến trúc:**
    *   **DDoS trực tiếp (Direct):** Các Bot gửi yêu cầu trực tiếp đến nạn nhân.
    *   **DDoS gián tiếp/phản xạ (Reflective):** Các Bot gửi yêu cầu giả mạo địa chỉ nạn nhân đến các máy **Phản xạ (Reflectors)**. Các máy này phản hồi về nạn nhân. *Lưu ý: Reflectors không bị kẻ tấn công chiếm quyền điều khiển nhưng bị lợi dụng.*

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 58: Tấn công DoS sử dụng sâu SQL Slammer để khai thác lỗi tràn bộ đệm trong phần mềm được phân loại là dạng tấn công nào?**
A. Tấn công gây ngập lụt.
B. Tấn công lô gíc.
C. Tấn công giả mạo.
D. Tấn công nghe lén.

**Câu 59: Trong thủ tục bắt tay 3 bước của giao thức TCP, gói tin nào được máy chủ gửi lại sau khi nhận được yêu cầu mở kết nối từ máy khách?**
A. SYN.
B. ACK.
C. SYN-ACK.
D. FIN.

**Câu 60: Kẻ tấn công SYN Flood thực hiện hành vi nào sau đây để làm cạn kiệt tài nguyên Bảng kết nối (Backlog) của máy chủ?**
A. Gửi liên tục các gói tin ACK.
B. Gửi gói tin SYN và hoàn tất bắt tay 3 bước thật nhanh.
C. Gửi gói tin SYN nhưng không bao giờ gửi lại gói tin xác nhận ACK cuối cùng.
D. Ngắt kết nối mạng của máy chủ ngay lập tức.

**Câu 61: Kỹ thuật tấn công Smurf lợi dụng điểm yếu của giao thức nào và địa chỉ nào để gây ngập lụt đường truyền của nạn nhân?**
A. Giao thức HTTP và địa chỉ IP tĩnh.
B. Giao thức ICMP và địa chỉ quảng bá (broadcast).
C. Giao thức FTP và địa chỉ IP của máy chủ DNS.
D. Giao thức TCP và địa chỉ Gateway.

**Câu 62: Điểm khác biệt chính giữa tấn công DDoS và tấn công DoS là gì?**
A. DDoS sử dụng mã độc tinh vi hơn.
B. DDoS có phạm vi tấn công lớn, huy động số lượng máy tấn công cực lớn từ nhiều vị trí địa lý.
C. DoS luôn gây thiệt hại lớn hơn DDoS.
D. DoS chỉ thực hiện được trên mạng không dây.

**Câu 63: Trong kiến trúc tấn công DDoS gián tiếp (Reflective DDoS), các máy "Phản xạ" (Reflectors) có đặc điểm gì?**
A. Là các máy đã bị kẻ tấn công chiếm quyền điều khiển hoàn toàn.
B. Là các máy chủ có băng thông lớn bị lợi dụng để gửi phản hồi đến nạn nhân nhưng không chịu sự điều khiển trực tiếp của kẻ tấn công.
C. Là các máy chủ điều khiển (C&C) của hacker.
D. Là các máy tính cá nhân cài đặt phần mềm diệt virus.

**Câu 64: Giải pháp nào sau đây giúp phòng chống tấn công SYN Flood bằng cách chỉ cấp phát bộ nhớ đầy đủ cho kết nối khi nó đã được xác nhận (bước 3)?**
A. Tăng kích thước Bảng kết nối.
B. Sử dụng kỹ thuật lọc địa chỉ giả mạo.
C. Sử dụng SYN cache hoặc SYN cookies.
D. Giảm thời gian chờ (timeout).

---

## III. GIẢI THÍCH & "BẪY" THI TRẮC NGHIỆM

*   **Đáp án Câu 58: B.** (Trang 59). Hãy nhớ: Khai thác lỗi phần mềm = Lô gíc; Gửi nhiều dữ liệu = Ngập lụt.
*   **Đáp án Câu 59: C.** (Trang 59). Thứ tự bắt tay 3 bước: **(1) SYN $\rightarrow$ (2) SYN-ACK $\rightarrow$ (3) ACK**.
*   **Đáp án Câu 60: C.** (Trang 60). Mục tiêu của SYN Flood là tạo ra các kết nối "dở dang" (half-open) để chiếm chỗ trong Backlog.
*   **Đáp án Câu 61: B.** (Trang 61). Từ khóa: **Smurf = ICMP + Broadcast**.
*   **Đáp án Câu 62: B.** (Trang 62). Chữ "D" đầu tiên trong DDoS là **Distributed** (Phân tán), thể hiện tính quy mô và đa vị trí.
*   **Đáp án Câu 63: B.** (Trang 63-64). Đây là một điểm bẫy: Reflectors **không phải** là Bot/Zombie (không bị cài mã độc điều khiển), chúng chỉ thực hiện phản hồi theo đúng giao thức tiêu chuẩn nhưng bị hacker "mượn tay" bằng địa chỉ giả mạo.
*   **Đáp án Câu 64: C.** (Trang 61). SYN cache là kỹ thuật trì hoãn việc cấp phát tài nguyên cho đến khi chắc chắn kết nối đó là hợp lệ.

---

## IV. MẸO GHI NHỚ BẰNG HÌNH ẢNH
*   **SYN Flood:** Giống như một người liên tục gọi đồ ăn (SYN) nhưng khi nhân viên mang đồ ra (SYN-ACK) thì người đó bỏ đi, không trả tiền (ACK). Cửa hàng hết chỗ ngồi vì những đơn hàng dở dang.
*   **Smurf:** Giống như kẻ xấu cầm loa thông báo (Broadcast) giữa đám đông rằng: "Hãy gửi quà cho anh A tại địa chỉ X" (Giả mạo IP nạn nhân). Cả đám đông đồng loạt gửi quà khiến anh A bị ngộp.
*   **Botnet:** Attacker (Tướng) $\rightarrow$ Handlers (Lính truyền tin) $\rightarrow$ Bots/Zombies (Đội quân ma).

---
Dựa trên nội dung từ trang 64 đến trang 67 của giáo trình, tôi đã biên soạn tài liệu ôn tập cho nhóm các kỹ thuật tấn công hạ tầng và đường truyền: **Giả mạo địa chỉ, Nghe lén, Người đứng giữa** và **Tấn công Email**.

Đây là những phần lý thuyết rất hay được hỏi dưới dạng các tình huống mô phỏng gói tin đi từ mạng này sang mạng khác.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 3 (MỤC 3.3.5 - 3.3.8)
**Chủ đề: Spoofing, Sniffing, MITM và Mail Attack**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Tấn công giả mạo địa chỉ (Address Spoofing) - Mục 3.3.5
*   **Bản chất:** Sử dụng địa chỉ IP giả làm IP nguồn để vượt qua hàng rào kiểm soát an ninh (Firewall/Router).
*   **Mục tiêu:** Thường giả mạo địa chỉ IP nội bộ của mạng LAN để chiếm lòng tin của các máy khác trong cùng mạng.
*   **Phòng chống:** Kỹ thuật lọc địa chỉ giả mạo trên Router/Firewall: **Chặn tất cả các gói tin đi từ mạng NGOÀI vào mạng LAN nếu chúng có địa chỉ IP nguồn thuộc dải nội bộ của LAN.**

### 2. Tấn công nghe lén (Sniffing/Eavesdropping) - Mục 3.3.6
*   **Phân loại:** Là tấn công **Thụ động (Passive)**.
*   **Mục tiêu:** Thu thập thông tin nhạy cảm (ID, mật khẩu, thẻ tín dụng) truyền dưới dạng **RÕ (Cleartext)**.
*   **Môi trường nguy cơ cao:** Mạng WiFi không được mã hóa đủ mạnh hoặc các thiết bị mạng cũ như HUB (gửi gói tin đến tất cả các cổng).

### 3. Tấn công kiểu người đứng giữa (Man-In-The-Middle - MITM) - Mục 3.3.7
*   **Cơ chế:** Kẻ tấn công đứng giữa hai bên (A và B), chặn bắt gói tin của A gửi cho B và ngược lại. Cả A và B đều tin rằng mình đang trao đổi trực tiếp với nhau.
*   **Hành động:** Kẻ tấn công có thể nghe lén, giải mã (nếu biết khóa) và sửa đổi nội dung thông điệp.
*   **Phòng chống:** Sử dụng **Chứng thư số (Digital Certificate)** và **Chữ ký số (Digital Signature)** để hai bên xác thực danh tính của nhau và đảm bảo tính toàn vẹn.

### 4. Tấn công Bom thư và Thư rác (Mail Attack) - Mục 3.3.8
*   **Bom thư (Mail Bombing):** Là một dạng tấn công **DoS** (từ chối dịch vụ). Kẻ tấn công gửi số lượng lớn email làm tê liệt hộp thư và máy chủ nạn nhân.
*   **Thư rác (Spam):** Email quảng cáo hoặc chứa mã độc gửi hàng loạt. Chiếm khoảng **70-80%** lượng email trên Internet.
*   **Phòng chống:** Sử dụng các tiêu chuẩn bảo mật email như **SPF, DKIM, S/MIME** để xác thực máy chủ gửi email hợp lệ.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 65: Kỹ thuật phòng chống giả mạo địa chỉ IP (IP Spoofing) hiệu quả nhất trên các bộ định tuyến là gì?**
A. Yêu cầu mọi máy tính trong mạng phải cài đặt phần mềm diệt virus.
B. Chặn các gói tin đi từ mạng ngoài vào mạng LAN nếu địa chỉ IP nguồn là địa chỉ nội bộ của mạng LAN đó.
C. Mã hóa toàn bộ dữ liệu truyền trong mạng LAN.
D. Thay đổi địa chỉ IP của máy chủ hàng ngày.

**Câu 66: Tấn công nghe lén (Sniffing) thường được thực hiện thông qua việc lắng nghe trên các thiết bị mạng nào sau đây?**
A. Card mạng, Hub, Switch, Router.
B. Chỉ duy nhất trên máy chủ Web.
C. Chỉ trên các ổ đĩa cứng của người dùng.
D. Trên các màn hình hiển thị thông tin công cộng.

**Câu 67: Khẳng định nào sau đây là ĐÚNG nhất về tấn công kiểu "Người đứng giữa" (MITM)?**
A. Kẻ tấn công trực tiếp phá hủy hệ thống của nạn nhân.
B. Kẻ tấn công đóng vai trò trung gian, chặn bắt và chuyển tiếp thông tin khiến hai bên tin rằng họ đang trao đổi trực tiếp với nhau.
C. Kẻ tấn công gửi hàng triệu email làm tê liệt máy chủ.
D. Kẻ tấn công sử dụng kỹ thuật xã hội để hỏi mật khẩu người dùng.

**Câu 68: Trong mô hình tấn công người đứng giữa (Hình 3.13), nếu Hacker C muốn đánh lừa Công ty A, Hacker C sẽ làm gì khi nhận được thông điệp thiết lập phiên bảo mật từ A gửi cho B?**
A. Xóa bỏ thông điệp đó ngay lập tức.
B. Giả làm B để trao đổi khóa với A, đồng thời giả làm A để trao đổi khóa với B.
C. Gửi một thông báo lỗi cho A.
D. Tăng tốc độ đường truyền cho A.

**Câu 69: Tấn công bằng "Bom thư" (Mail bombing) làm tê liệt máy chủ nhận thư thực chất là một biến thể của dạng tấn công nào?**
A. Tấn công nghe lén.
B. Tấn công từ chối dịch vụ (DoS).
C. Tấn công giả mạo địa chỉ.
D. Tấn công phần mềm độc hại.

**Câu 70: Các giải pháp như SPF (Sender Policy Framework) và DKIM (DomainKeys Identified Mail) được sử dụng để phòng chống loại tấn công nào?**
A. Tấn công tràn bộ đệm.
B. Tấn công nghe lén trong mạng WiFi.
C. Tấn công lạm dụng hệ thống email (Bom thư, thư rác).
D. Tấn công chiếm quyền điều khiển máy chủ DNS.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 65: B.** (Trang 65). Đây là nguyên tắc lọc gói tin cơ bản. Một gói tin từ Internet đi vào không bao giờ được phép mang địa chỉ IP nguồn là của máy đang nằm bên trong LAN. Nếu có, chắc chắn là giả mạo.
*   **Đáp án Câu 66: A.** (Trang 65). Sniffing bắt gói tin trên mọi điểm của môi trường truyền dẫn (Card mạng, Hub, Switch...).
*   **Đáp án Câu 67: B.** (Trang 66). Từ khóa: **"Chặn bắt và chuyển tiếp"** + **"Hai bên tin rằng họ trao đổi trực tiếp"**.
*   **Đáp án Câu 68: B.** (Trang 67). Hacker C thực hiện hai phiên làm việc giả mạo song song để "đứng giữa" luồng dữ liệu.
*   **Đáp án Câu 69: B.** (Trang 67). Bom thư gây ngập lụt tài nguyên hệ thống nhận thư $\rightarrow$ Gây ngừng trệ dịch vụ $\rightarrow$ DoS.
*   **Đáp án Câu 70: C.** (Trang 68). SPF và DKIM giúp xác minh email gửi đi thực sự đến từ máy chủ của tên miền đó, tránh việc hacker dùng máy chủ giả để gửi bom thư hoặc thư rác.

---

## IV. BẢNG TỔNG HỢP NHANH

| Tấn công | Mục tiêu chính | Công cụ/Kỹ thuật then chốt |
|:---|:---|:---|
| **Spoofing** | Vượt rào bảo vệ (Firewall) | Giả mạo IP nguồn (Source IP). |
| **Sniffing** | Đánh cắp thông tin nhạy cảm | Wireshark, Tcpdump (Passive attack). |
| **MITM** | Kiểm soát luồng trao đổi bí mật | Chặn bắt và chuyển tiếp khóa/thông điệp. |
| **Mail Bomb** | Làm sập máy chủ email | Gửi số lượng lớn email (DoS). |

---
Dựa trên nội dung từ trang 68 đến trang 71 của giáo trình, tôi đã biên soạn tài liệu ôn tập cho mục **3.3.9 (Kỹ thuật xã hội)** và **3.3.10 (Pharming)**.

Đây là những hình thức tấn công nhắm vào **con người** và **cấu trúc hệ thống tên miền**, thường xuất hiện trong các câu hỏi tình huống thực tế của bài thi trắc nghiệm.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 3 (MỤC 3.3.9 - 3.3.10)
**Chủ đề: Social Engineering, Phishing và Pharming**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Tấn công kỹ thuật xã hội (Social Engineering) - Mục 3.3.9
*   **Bản chất:** Là tấn công **phi kỹ thuật** (không dùng mã độc hay bẻ khóa trực tiếp).
*   **Mục tiêu:** Nhắm vào "mắt xích yếu nhất" là **Con người**.
*   **Điểm yếu khai thác:** Sự cả tin, ngây thơ, tò mò hoặc lòng tham của người dùng.
*   **Các ví dụ điển hình:**
    *   **Trò lừa đảo Nigeria 4-1-9:** Hứa hẹn chia lợi nhuận từ một khoản tiền thừa kế lớn để lừa nạn nhân chuyển trước một khoản "phí giao dịch".
    *   **Phishing (Lừa đảo qua email):** Gửi email giả mạo các tổ chức tài chính, ngân hàng (eBay, Royal Bank) để bẫy người dùng cung cấp thông tin tài khoản hoặc click vào link giả.

### 2. Tấn công Pharming - Mục 3.3.10
*   **Bản chất:** Kiểu tấn công vào **trình duyệt**, khiến người dùng gõ đúng địa chỉ trang web thật nhưng lại bị chuyển hướng sang trang web độc hại của kẻ tấn công.
*   **Hai dạng thực hiện pharming:**
    1.  **Chiếm quyền trình duyệt (Browser hijacking):** Cài đặt virus hoặc trình cắm (plug-in/add-on) độc hại vào máy nạn nhân để tự động chuyển hướng trang web.
    2.  **Tấn công máy chủ DNS:** Xâm nhập máy chủ DNS để sửa đổi bản ghi IP, thay địa chỉ IP thật của website bằng địa chỉ IP của kẻ tấn công.

### 3. So sánh Phishing và Pharming (Điểm bẫy trắc nghiệm)
| Đặc điểm | Phishing (Lừa đảo) | Pharming |
|:---|:---|:---|
| **Cách thức dụ dỗ** | Dùng email "mồi" để lừa người dùng click vào link giả. | Người dùng tự gõ đúng địa chỉ website thật. |
| **Kỹ thuật** | Dựa nhiều vào tâm lý. | Dựa vào mã độc trình duyệt hoặc can thiệp DNS. |
| **Độ nguy hiểm** | Dễ phát hiện hơn nếu kiểm tra URL. | Khó phát hiện hơn vì người dùng tin rằng mình đã gõ đúng địa chỉ. |

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 71: Loại tấn công nào sau đây được giáo trình định nghĩa là "tấn công phi kỹ thuật" nhắm vào các điểm yếu cố hữu của con người như sự cả tin và lòng tham?**
A. Tấn công SQL Injection.
B. Tấn công kỹ thuật xã hội (Social Engineering).
C. Tấn công SYN Flood.
D. Tấn công giả mạo địa chỉ IP.

**Câu 72: Theo giáo trình, trò lừa đảo "Nigeria 4-1-9" nổi tiếng khai thác điểm yếu nào của nạn nhân?**
A. Lỗi cấu hình hệ điều hành.
B. Sự ngây thơ và lòng tham.
C. Sử dụng mật khẩu ngắn.
D. Không cài đặt phần mềm diệt virus.

**Câu 73: Hình thức "Phishing" thường được thực hiện thông qua công cụ nào để bẫy người dùng cung cấp thông tin cá nhân?**
A. Các lệnh trong dòng lệnh CMD.
B. Gửi các email giả mạo từ các tổ chức uy tín (ngân hàng, trang đấu giá).
C. Tấn công vào các bộ định tuyến WiFi công cộng.
D. Cài đặt các đoạn mã JavaScript vào cơ sở dữ liệu.

**Câu 74: Tấn công Pharming có đặc điểm gì nổi bật khiến người dùng khó phát hiện hơn so với Phishing?**
A. Nạn nhân bị mất kết nối Internet hoàn toàn.
B. Nạn nhân bị lừa cung cấp mật khẩu qua điện thoại.
C. Nạn nhân vẫn bị dẫn tới trang web giả dù đã nhập đúng địa chỉ trang web thật trên trình duyệt.
D. Hệ điều hành của nạn nhân bị khóa và yêu cầu tiền chuộc.

**Câu 75: Việc kẻ tấn công xâm nhập vào máy chủ DNS để sửa đổi địa chỉ IP của một website hợp pháp thành địa chỉ IP máy chủ của kẻ tấn công được gọi là:**
A. Tấn công từ chối dịch vụ.
B. Tấn công nghe lén đường truyền.
C. Tấn công Pharming (dạng 2).
D. Tấn công vét cạn mật khẩu.

**Câu 76: Biện pháp phòng chống tấn công Social Engineering hiệu quả nhất theo giáo trình là gì?**
A. Cài đặt tường lửa thế hệ mới.
B. Sử dụng các thuật toán mã hóa mạnh hơn.
C. Đào tạo, giáo dục nâng cao ý thức cảnh giác cho người dùng.
D. Cấm người dùng sử dụng email cá nhân tại nơi làm việc.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 71: B.** Social Engineering không dùng mã máy, nó dùng "mã tâm lý".
*   **Đáp án Câu 72: B.** (Trang 68). Nhớ ví dụ Nigeria 4-1-9 là điển hình của Social Engineering.
*   **Đáp án Câu 73: B.** Phishing gắn liền với hình ảnh "Email lừa đảo" (Ví dụ eBay/Royal Bank ở trang 69).
*   **Đáp án Câu 74: C.** (Trang 70). Đây là điểm khác biệt cốt lõi: Pharming "cướp" đích đến của trình duyệt.
*   **Đáp án Câu 75: C.** (Trang 70). Pharming đánh vào máy chủ DNS là dạng tấn công hạ tầng rất nguy hiểm vì ảnh hưởng đến nhiều người dùng cùng lúc.
*   **Đáp án Câu 76: C.** (Trang 69). Vì mục tiêu là con người, nên giải pháp kỹ thuật chỉ là phụ, nhận thức con người mới là quan trọng nhất.

---

## IV. MẸO GHI NHỚ (STUDY TIPS)
*   **Phishing:** Nghĩ đến việc "Đi câu" (Fishing). Hacker dùng "mồi" là email giả để câu thông tin của bạn.
*   **Pharming:** Nghĩ đến việc "Trang trại" (Farm). Hacker đầu độc nguồn nước/đất (DNS) để dẫn dụ cả đàn gia súc (người dùng) đi nhầm đường.
*   **Social Engineering:** Nhớ từ khóa **"Phi kỹ thuật"** và **"Con người"**.

---
Dựa trên nội dung từ trang 72 đến trang 73 của giáo trình, tôi đã biên soạn tài liệu ôn tập cho mục **3.3.11 (Tấn công APT)**. 

APT là hình thức tấn công phức tạp và nguy hiểm nhất trong an toàn thông tin hiện nay, thường xuất hiện trong các câu hỏi thi về **tư duy chiến lược** và **các giai đoạn tấn công**.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 3 (MỤC 3.3.11)
**Chủ đề: Tấn công APT (Advanced Persistent Threat)**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Định nghĩa và Bản chất
*   **APT** (Advanced Persistent Threat): Tấn công có chủ đích, được thiết kế riêng cho từng mục tiêu cụ thể nhằm đánh cắp thông tin giá trị và gửi ra ngoài.
*   **Hai thuộc tính cốt lõi:**
    1.  **Tiên tiến (Advanced):** Sử dụng các kỹ thuật cao cấp, bài bản, kết hợp nhiều phương pháp, có khả năng ẩn mình và thay đổi liên tục.
    2.  **Kiên trì/Dai dẳng (Persistent):** Mục tiêu xác định rõ ràng, có thể theo đuổi hàng tháng hoặc hàng năm. Khi đã vào được hệ thống, chúng cài cắm mã độc thường trú và không bao giờ tự dừng lại.

### 2. Các giai đoạn của một cuộc tấn công APT (Cực kỳ hay hỏi thứ tự)
Bạn cần nhớ 6 bước diễn tiến theo thời gian:
1.  **Truy cập ban đầu:** Lây nhiễm mã độc qua bẫy người dùng hoặc khai thác lỗ hổng.
2.  **Thâm nhập và triển khai:** Cài đặt mã độc thường trú, duy trì kết nối với máy chủ điều khiển (C&C).
3.  **Mở rộng truy cập và di chuyển ngang:** Xâm nhập sâu hơn vào các máy khác, thiết lập **Cửa hậu (Backdoor)**.
4.  **Giai đoạn tấn công:** Giám sát, trích xuất dữ liệu, nén và mã hóa dữ liệu để chuẩn bị chuyển đi.
5.  **Gây thiệt hại:** Vận chuyển dữ liệu ra ngoài. *Mẹo:* Kẻ tấn công có thể dùng tấn công DDoS để đánh lạc hướng người quản trị ở giai đoạn này.
6.  **Tấn công tiếp theo:** Tiếp tục giám sát qua cửa hậu để chờ cơ hội xâm nhập sâu hơn trong tương lai.

### 3. Chiến lược phòng chống
*   Không có công cụ đơn lẻ nào chặn được APT. Cần **Phòng vệ chiều sâu**.
*   Kết hợp: Tường lửa + Kiểm soát truy cập + Hệ thống diệt mã độc + Giám sát xâm nhập (IDS) + Chính sách an toàn nghiêm ngặt + Đào tạo con người.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 77: Thuật ngữ "APT" (Advanced Persistent Threat) dùng để chỉ loại hình tấn công nào?**
A. Tấn công tự động bằng virus để phá hỏng ổ cứng.
B. Tấn công có chủ đích, sử dụng kỹ thuật tiên tiến và kéo dài dai dẳng vào một mục tiêu cụ thể.
C. Tấn công nghe lén mật khẩu trong mạng WiFi công cộng.
D. Tấn công gửi thư rác hàng loạt để quảng cáo sản phẩm.

**Câu 78: Đặc điểm "Persistent" (Kiên trì/Dai dẳng) trong tấn công APT được thể hiện rõ nhất qua hành vi nào của kẻ tấn công?**
A. Sử dụng các thuật toán mã hóa phức tạp nhất.
B. Tấn công liên tục vào nhiều mục tiêu khác nhau cùng lúc.
C. Duy trì mã độc thường trú lâu dài trong hệ thống và âm thầm thu thập thông tin trong nhiều tháng, thậm chí nhiều năm.
D. Sử dụng hàng triệu máy tính ma (Botnet) để gây ngập lụt đường truyền.

**Câu 79: Trong các giai đoạn của tấn công APT, kẻ tấn công thường thực hiện việc nén và mã hóa dữ liệu nhạy cảm ở giai đoạn nào?**
A. Truy cập ban đầu.
B. Thâm nhập lần đầu.
C. Giai đoạn tấn công (trước khi vận chuyển ra ngoài).
D. Giai đoạn gây thiệt hại.

**Câu 80: Để đánh lạc hướng người quản trị và xóa dấu vết khi đang thực hiện việc chuyển dữ liệu ra ngoài, kẻ tấn công APT có thể sử dụng thêm dạng tấn công nào?**
A. Tấn công nghe lén.
B. Tấn công DDoS.
C. Tấn công kỹ thuật xã hội.
D. Tấn công từ điển.

**Câu 81: Giai đoạn "Di chuyển ngang" (Lateral movement) trong tấn công APT có mục đích chính là gì?**
A. Gửi email lừa đảo cho khách hàng của nạn nhân.
B. Xâm nhập từ máy này sang các máy tính khác trong cùng hệ thống để tìm kiếm thêm dữ liệu nhạy cảm.
C. Tắt tường lửa của hệ thống.
D. Cập nhật phiên bản mới cho phần mềm diệt virus của nạn nhân.

**Câu 82: Theo giáo trình, chiến lược tổng quát nhất để phòng chống tấn công APT là gì?**
A. Chỉ cần cài đặt một phần mềm diệt virus mạnh nhất.
B. Cấm hoàn toàn nhân viên sử dụng Internet.
C. Kết hợp nhiều lớp phòng vệ (phòng vệ chiều sâu) cùng với việc đào tạo ý thức người dùng và giám sát nghiêm ngặt.
D. Thay đổi toàn bộ hệ thống máy tính định kỳ hàng tháng.

---

## III. GIẢI THÍCH & PHÂN TÍCH CHI TIẾT

*   **Đáp án Câu 77: B.** Đây là định nghĩa đầy đủ nhất về APT.
*   **Đáp án Câu 78: C.** (Trang 72). Khác với các cuộc tấn công "đánh nhanh thắng nhanh", APT ưu tiên sự tồn tại kín đáo và lâu dài.
*   **Đáp án Câu 79: C.** (Trang 72). Dữ liệu cần được "đóng gói" (nén, mã hóa) để tránh bị các hệ thống giám sát mạng phát hiện khi đang trên đường truyền ra ngoài.
*   **Đáp án Câu 80: B.** (Trang 73). Đây là một chiến thuật rất tinh vi: dùng DDoS làm rối loạn hệ thống để người quản trị bận đối phó với việc nghẽn mạng mà không chú ý đến việc dữ liệu đang bị rò rỉ.
*   **Đáp án Câu 81: B.** (Trang 72). "Di chuyển ngang" là từ khóa kỹ thuật để chỉ việc mở rộng phạm vi kiểm soát bên trong nội bộ hệ thống.
*   **Đáp án Câu 82: C.** (Trang 73). Với APT, không có "viên đạn bạc" (giải pháp duy nhất), chỉ có sự phối hợp đa lớp mới hiệu quả.

---

## IV. MẸO GHI NHỚ (STUDY TIPS)
Hãy tưởng tượng cuộc tấn công APT giống như một cuộc **"Gián điệp đột nhập vào cung điện"**:
1.  **Lẻn vào:** Qua cửa sổ hoặc đóng giả người làm (Truy cập ban đầu).
2.  **Ẩn nấp:** Trốn dưới gầm giường, tạo chỗ ở bí mật (Thâm nhập & Triển khai).
3.  **Lục lọi:** Lẻn từ phòng này sang phòng khác tìm kho báu (Di chuyển ngang).
4.  **Đóng gói:** Cho vàng bạc vào túi, bọc kín lại (Tấn công/Trích xuất).
5.  **Tẩu tán:** Ném đồ ra ngoài, trong lúc đồng bọn đốt lửa ở cổng trước để lính canh mất tập trung (Gây thiệt hại/Vận chuyển dữ liệu).
6.  **Để lại tai mắt:** Để lại một người ở lại trong cung điện để tiếp tục nghe ngóng (Tấn công tiếp theo).

---
Dựa trên nội dung từ trang 73 đến trang 82 của giáo trình, tôi đã biên soạn tài liệu ôn tập cho mục **3.4 (Các dạng phần mềm độc hại - Malware)**. Đây là phần có lượng kiến thức cực kỳ lớn, yêu cầu bạn phải phân biệt được các đặc tính lây nhiễm khác nhau của từng loại mã độc.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 3 (MỤC 3.4)
**Chủ đề: Các dạng phần mềm độc hại (Malware)**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Phân loại theo phương pháp lây nhiễm (Hình 3.18)
Đây là bảng quan trọng nhất để trả lời các câu hỏi về phân loại:

| Nhóm | Đặc điểm | Thành viên tiêu biểu |
|:---|:---|:---|
| **Cần chương trình chủ (Host)** | Không thể chạy độc lập, phải "ký sinh" vào file khác hoặc cần hành động của người dùng. | **Virus**, Trojan, Logic Bomb, Backdoor, Rootkit, Adware, Spyware. |
| **Không cần chủ (Independent)** | Có khả năng tự chạy, tự lây lan qua mạng mà không cần sự can thiệp của con người. | **Worm (Sâu)**, Zombie/Bot. |

### 2. Đặc điểm nhận diện các loại Malware cụ thể

*   **Bom lô gic (Logic Bomb):** Chỉ "phát nổ" (xoá file, tắt hệ thống) khi thoả mãn một **điều kiện** cụ thể (giờ giấc, ngày tháng, sự xuất hiện của 1 file).
*   **Trojan Horse:** Giả danh chương trình có ích (game, công cụ) để lừa người dùng cài đặt. **Không tự nhân bản**.
*   **Cửa hậu (Backdoor):** Điểm truy cập bí mật không qua kiểm tra an ninh (thường do lập trình viên để lại để gỡ lỗi nhưng bị lợi dụng).
*   **Vi rút (Virus):** Sửa đổi các file khác để lây nhiễm. Cần file thực thi được kích hoạt mới bắt đầu chạy.
    *   *Macro Virus:* Chỉ lây vào file Microsoft Office (Word, Excel) qua ngôn ngữ VBA.
*   **Sâu (Worm):** Tự nhân bản và lây lan qua mạng. Ví dụ: **Code Red** (lây qua lỗi máy chủ IIS), **Nimda** (tốc độ nhanh nhất).
*   **Zombie/Bot:** Máy tính bị chiếm quyền điều khiển, nhận lệnh từ máy chủ **C&C (Command & Control)**. Nhiều Bot hợp thành **Botnet**.
*   **Rootkit:** Tập hợp công cụ giúp chiếm quyền quản trị cao nhất (**Root/Admin**) và che giấu sự hiện diện của mình cực kỳ tinh vi.
*   **Adware & Spyware:** Adware (quảng cáo), Spyware (thu thập thông tin nhạy cảm: thẻ tín dụng, mật khẩu).

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 83: Theo giáo trình, loại phần mềm độc hại nào sau đây có khả năng tự lây nhiễm mà không cần chương trình chủ hay sự hỗ trợ của người dùng?**
A. Virus.
B. Trojan horse.
C. Sâu (Worm).
D. Bom lô gic.

**Câu 84: Loại mã độc nào thường "ẩn mình" dưới dạng một chương trình có ích để lừa người dùng kích hoạt, sau đó thực hiện các tác vụ ngầm mà người dùng không có quyền truy cập trực tiếp?**
A. Rootkit.
B. Trojan horse.
C. Macro virus.
D. Backdoor.

**Câu 85: Một nhân viên quản trị mạng bị sa thải đã cài đặt mã độc để xóa toàn bộ dữ liệu công ty vào đúng ngày sinh nhật của giám đốc. Đây là ví dụ điển hình của loại mã độc nào?**
A. Sâu mạng.
B. Bom lô gic (Logic bomb).
C. Phần mềm gián điệp.
D. Email virus.

**Câu 86: Đặc điểm khác biệt lớn nhất giữa Sâu (Worm) và Vi rút (Virus) là gì?**
A. Sâu phá hoại dữ liệu mạnh hơn Virus.
B. Sâu có khả năng tự nhân bản và lây lan qua mạng mà không cần hành động của người dùng, trong khi Virus cần gắn vào vật chủ.
C. Virus chỉ lây qua email, còn Sâu lây qua USB.
D. Virus là phần mềm độc lập, còn Sâu là chương trình ký sinh.

**Câu 87: Loại mã độc nào chuyên lây nhiễm vào các tài liệu của bộ phần mềm Microsoft Office thông qua ngôn ngữ Visual Basic for Applications (VBA)?**
A. Boot virus.
B. File virus.
C. Macro virus.
D. Nimda.

**Câu 88: Mạng máy tính ma (Botnet) được kẻ tấn công điều khiển thông qua hệ thống nào sau đây?**
A. Máy chủ DNS công cộng.
B. Máy chủ lệnh và điều khiển (Command and Control - C&C).
C. Tường lửa của nạn nhân.
D. Mạng WiFi không dây.

**Câu 89: Mục đích chính của Rootkit là gì?**
A. Hiển thị thật nhiều quảng cáo trên màn hình người dùng.
B. Giành quyền truy cập hệ thống ở mức quản trị (root/admin) và che giấu sự hiện diện của kẻ tấn công.
C. Tự động gửi email rác cho tất cả mọi người.
D. Mã hóa dữ liệu để đòi tiền chuộc.

**Câu 90: Đâu là nguyên tắc chung trong phòng chống phần mềm độc hại được giáo trình khuyến nghị?**
A. Chỉ cần cài đặt một phần mềm diệt virus duy nhất.
B. Phòng vệ theo chiều sâu (nhiều lớp nhóm biện pháp).
C. Cấm hoàn toàn việc sử dụng thẻ nhớ USB.
D. Sử dụng tài khoản Administrator cho mọi hoạt động hàng ngày.

---

## III. GIẢI THÍCH & PHÂN TÍCH CHI TIẾT

*   **Đáp án Câu 83: C.** (Trang 74). Bạn cần nhớ biểu đồ phân loại: Worm và Bot là "Independent" (Độc lập).
*   **Đáp án Câu 84: B.** (Trang 75). Trojan lấy tên từ điển tích "Con ngựa thành Troy" – vẻ ngoài đẹp đẽ (hữu ích) nhưng bên trong chứa quân lính (mã độc). Trojan **không tự nhân bản**.
*   **Đáp án Câu 85: B.** (Trang 74). Từ khóa "vào đúng ngày sinh nhật" $\rightarrow$ Đây là điều kiện thời gian $\rightarrow$ Logic Bomb. Ví dụ thực tế trong sách là vụ Timothy Lloyd (Omega Engineering).
*   **Đáp án Câu 86: B.** (Trang 77). Đây là câu hỏi kinh điển. Virus cần người dùng "mở file", Worm tự "bò" qua mạng.
*   **Đáp án Câu 87: C.** (Trang 76). Từ khóa: **Macro = Office = VBA**.
*   **Đáp án Câu 88: B.** (Trang 79). Mọi Botnet đều cần máy chủ C&C để nhận lệnh từ Hacker (Botmaster).
*   **Đáp án Câu 89: B.** (Trang 80). Rootkit là loại mã độc "đẳng cấp" nhất vì nó can thiệp vào nhân hệ thống, rất khó bị phần mềm Antivirus thông thường phát hiện.
*   **Đáp án Câu 90: B.** (Trang 81). Giáo trình nhấn mạnh "Phòng vệ chiều sâu" là chiến lược tổng quát cho mọi vấn đề an toàn thông tin.

---

## IV. MẸO GHI NHỚ "BỘ BA NGUY HIỂM"
*   **Virus:** Cần **Vật chủ** (V - V).
*   **Worm:** Tự **Bò** qua mạng (W - Web/Network).
*   **Trojan:** **Giả danh** (Lừa đảo).

---
Dựa trên nội dung từ trang 85 đến trang 93 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục 4.1 và 4.2. Phần này chứa đựng các khái niệm mang tính nền tảng và lịch sử, rất dễ xuất hiện trong các câu hỏi kiểm tra về thuật ngữ và phân biệt các loại hình mã hóa.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 4 (MỤC 4.1 & 4.2)
**Chủ đề: Khái quát về mã hóa và Các phương pháp mã hóa cơ bản**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Thuật ngữ nền tảng (Mục 4.1.1)
*   **Bản rõ (Plaintext):** Thông tin gốc, có thể hiểu được.
*   **Bản mã (Ciphertext):** Thông tin đã bị xáo trộn, không thể hiểu được.
*   **Không gian khóa (Keyspace):** Tập hợp tất cả các khóa có thể có. Nếu khóa dài $n$ bit $\rightarrow$ Không gian khóa là $2^n$. Khóa càng dài, hệ mã hóa càng an toàn trước tấn công vét cạn.
*   **Thám mã (Cryptanalysis):** Quá trình phá mã mà không biết trước thuật toán và khóa.

### 2. Phân loại hệ mã hóa theo Khóa
*   **Mã hóa đối xứng (Symmetric):** Sử dụng **1 khóa duy nhất** (khóa bí mật/khóa chia sẻ) cho cả mã hóa và giải mã. 
    *   *Đặc điểm:* Tốc độ nhanh, nhưng quản lý và phân phối khóa rất khó khăn (đặc biệt khi số lượng người dùng lớn).
*   **Mã hóa bất đối xứng (Asymmetric):** Sử dụng **1 cặp khóa** (Khóa công khai - Public key để mã hóa; Khóa riêng - Private key để giải mã).
    *   *Đặc điểm:* Quản lý khóa đơn giản, nhưng tốc độ thực thi chậm hơn nhiều so với mã hóa đối xứng.

### 3. Phương pháp xử lý dữ liệu (Mục 4.1.3)
*   **Mã hóa dòng (Stream cipher):** Mã hóa **từng bit hoặc từng ký tự** một. Sử dụng bộ sinh luồng khóa (Keystream generator). Ví dụ: **RC4, A5/1, A5/2**.
*   **Mã hóa khối (Block cipher):** Chia dữ liệu thành các khối có kích thước cố định (**64 bit hoặc 128 bit**). Ví dụ: **DES, 3-DES, AES, Blowfish**.

### 4. Các phương pháp mã hóa cơ bản/cổ điển (Mục 4.2)
*   **Thay thế (Substitution):** Thay giá trị này bằng giá trị khác. Điển hình là **Caesar cipher** (dịch 3 vị trí: A $\rightarrow$ D, L $\rightarrow$ O).
*   **Hoán vị (Permutation):** Đổi chỗ/sắp xếp lại các phần tử trong khối mà không thay đổi giá trị của chúng. Nếu khối không đủ ký tự thì phải **chèn thêm dấu trắng (padding)**.
*   **XOR:** Sử dụng phép toán logic XOR bit-với-bit giữa bản rõ và khóa.
*   **Vernam (One-time pad):** Khóa có độ dài bằng bản rõ và chỉ dùng 1 lần duy nhất.
*   **Mã hóa sách (Book cipher):** Dùng tọa độ (Trang, Dòng, Từ) trong một cuốn sách để làm mã.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 91: Nếu một hệ mã hóa sử dụng khóa có kích thước 64 bit, thì "Không gian khóa" (Keyspace) của hệ mã này là bao nhiêu?**
A. $64^2$
B. $2^{64}$
C. $64 \times 2$
D. $2^6$

**Câu 92: Ưu điểm nổi bật nhất của hệ mã hóa khóa đối xứng so với hệ mã hóa khóa bất đối xứng là gì?**
A. Quản lý và phân phối khóa dễ dàng hơn.
B. Độ an toàn tuyệt đối, không thể bị phá mã.
C. Tốc độ thực thi nhanh hơn.
D. Không cần giữ bí mật khóa.

**Câu 93: Loại mã hóa nào thực hiện biến đổi dữ liệu trên từng bit hoặc từng ký tự của bản rõ tại một thời điểm?**
A. Mã hóa khối (Block cipher).
B. Mã hóa dòng (Stream cipher).
C. Hàm băm (Hash function).
D. Mã hóa hoán vị.

**Câu 94: Trong phương pháp mã hóa Caesar cổ điển, bản rõ "LOVE" sẽ được chuyển thành bản mã nào sau đây?**
A. ORYH.
B. MPHW.
C. KNUF.
D. LOV E.

**Câu 95: Khi thực hiện mã hóa hoán vị cho một bản rõ, nếu khối dữ liệu cuối cùng không đủ kích thước quy định thì cần thực hiện thao tác nào?**
A. Xóa bỏ phần dư đó.
B. Chèn thêm các ký tự trống (padding).
C. Chuyển sang phương pháp mã hóa thay thế.
D. Giảm kích thước khóa xuống.

**Câu 96: Phương pháp mã hóa nào sử dụng một chuỗi ký tự nối thêm (one-time pad) có độ dài bằng bản rõ và mỗi ký tự trong chuỗi chỉ dùng một lần duy nhất?**
A. Mã hóa XOR.
B. Mã hóa Vernam.
C. Mã hóa Caesar.
D. Mã hóa khối AES.

**Câu 97: Theo giáo trình, mã hóa thông tin có thể đảm bảo được những thuộc tính an toàn nào sau đây?**
A. Bí mật và Toàn vẹn.
B. Xác thực và Không thể chối bỏ.
C. Sẵn sàng.
D. Cả A và B đều đúng.

---

## III. GIẢI THÍCH & "MẸO" PHÂN BIỆT

*   **Đáp án Câu 91: B.** Công thức Keyspace luôn là $2^n$ (với n là số bit).
*   **Đáp án Câu 92: C.** (Trang 94/10). Hãy nhớ: **Đối xứng = Nhanh**, **Bất đối xứng = Tiện lợi quản lý khóa**.
*   **Đáp án Câu 93: B.** (Trang 88). Từ khóa: **"Từng bit/ký tự" $\rightarrow$ Dòng (Stream)**.
*   **Đáp án Câu 94: A.** Caesar dịch 3: L(+3)=O, O(+3)=R, V(+3)=Y, E(+3)=H $\rightarrow$ ORYH.
*   **Đáp án Câu 95: B.** (Trang 92). Thuật ngữ chuyên môn là **Padding**.
*   **Đáp án Câu 96: B.** (Trang 92). Nhớ từ khóa: **One-time pad = Vernam**.
*   **Đáp án Câu 97: D.** (Trang 90). Mã hóa không chỉ để giữ bí mật mà còn dùng để kiểm tra toàn vẹn (Hàm băm), xác thực và chống chối bỏ (Chữ ký số). Tuy nhiên, mã hóa **ít khi** liên quan trực tiếp đến tính **Sẵn sàng** (Availability).

---

## IV. BẢNG SO SÁNH NHANH (STUDY TIPS)

| Đặc điểm | Mã hóa dòng (Stream) | Mã hóa khối (Block) |
|:---|:---|:---|
| **Đơn vị xử lý** | Từng bit/byte | Từng khối dữ liệu lớn |
| **Kích thước khối** | 1 bit/byte | 64 hoặc 128 bit |
| **Đại diện tiêu biểu** | RC4, A5/1 | DES, AES |
| **Ứng dụng chính** | Viễn thông, luồng dữ liệu | Lưu trữ dữ liệu, file |

---
Dựa trên nội dung từ trang 94 đến trang 102 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục **4.3.1 (Các giải thuật mã hóa đối xứng)**. 

Đây là phần có mật độ các con số (số bit, số vòng lặp) và các thuật ngữ kỹ thuật rất cao. Đây là "vùng trọng điểm" của các đề thi trắc nghiệm.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 4 (MỤC 4.3.1)
**Chủ đề: Giải thuật đối xứng (DES, 3-DES, AES)**

## I. BẢNG SO SÁNH TỔNG HỢP (TRỌNG TÂM THI)

| Đặc điểm | DES | 3-DES (TDEA) | AES (Rijndael) |
|:---|:---|:---|:---|
| **Kích thước khối** | 64 bit | 64 bit | **128 bit** |
| **Kích thước khóa** | 64 bit (hiệu dụng **56 bit**) | 112 hoặc 168 bit | **128, 192, 256 bit** |
| **Số vòng lặp** | 16 vòng | 16 vòng $\times$ 3 | 10, 12, hoặc 14 vòng |
| **Cấu trúc chính** | Hàm Feistel | Lặp lại DES 3 lần | Mạng hoán vị - thay thế |
| **Tình trạng** | Không còn an toàn | An toàn hơn DES nhưng chậm | **Tiêu chuẩn hiện tại**, rất nhanh |

---

## II. CHI TIẾT TỪNG GIẢI THUẬT (DỄ BỊ CÀI BẪY)

### 1. Giải thuật DES (Mục 4.3.1.2)
*   **Khóa:** Sử dụng khóa 64 bit nhưng thực tế chỉ dùng **56 bit** để mã hóa, 8 bit còn lại dùng để kiểm tra chẵn lẻ.
*   **Hàm Feistel (F):** Là hạt nhân của DES. Gồm 4 bước:
    1.  **Expansion (E):** Mở rộng 32 bit lên 48 bit.
    2.  **XOR:** Trộn với khóa phụ (subkey) 48 bit.
    3.  **Substitution (Si):** Sử dụng các bộ **S-box** để chuyển **6 bit đầu vào thành 4 bit đầu ra**. Đây là thành phần nhân an ninh của DES.
    4.  **Permutation (P):** Hoán vị cố định cho ra 32 bit.
*   **Lưu ý:** DES sử dụng cùng một giải thuật cho cả mã hóa và giải mã (chỉ đảo ngược thứ tự khóa phụ).

### 2. Giải thuật 3-DES (Mục 4.3.1.3)
*   **Cơ chế:** Mã hóa (K1) $\rightarrow$ Giải mã (K2) $\rightarrow$ Mã hóa (K3).
*   **Lựa chọn khóa:** 
    *   Lựa chọn 1 (K1, K2, K3 độc lập): Khóa dài **168 bit** (An toàn nhất).
    *   Lựa chọn 2 (K1=K3, K2 độc lập): Khóa dài **112 bit**.
*   **Nhược điểm lớn nhất:** Tốc độ thực thi chậm (do phải chạy DES 3 lần).

### 3. Giải thuật AES (Mục 4.3.1.4)
*   **Số vòng lặp tương ứng với khóa:**
    *   Khóa 128 bit $\rightarrow$ **10 vòng**.
    *   Khóa 192 bit $\rightarrow$ **12 vòng**.
    *   Khóa 256 bit $\rightarrow$ **14 vòng**.
*   **4 hàm biến đổi trong mỗi vòng lặp:**
    1.  **SubBytes:** Thay thế phi tuyến qua bảng S-box.
    2.  **ShiftRows:** Dịch dòng theo chu kỳ (Hàng 0 giữ nguyên, hàng 1 dịch 1, hàng 2 dịch 2...).
    3.  **MixColumns:** Trộn cột (Kết hợp 4 byte trong mỗi cột). *Lưu ý: Vòng lặp cuối cùng KHÔNG có hàm này.*
    4.  **AddRoundKey:** Kết hợp trạng thái (state) với khóa vòng bằng phép XOR.

---

## III. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 98: Trong giải thuật DES, mặc dù độ dài khóa là 64 bit nhưng kích thước hiệu dụng thực tế chỉ là bao nhiêu bit?**
A. 48 bit.
B. 56 bit.
C. 60 bit.
D. 64 bit.

**Câu 99: Thành phần nào sau đây được coi là "nhân an ninh" của giải thuật DES, thực hiện chuyển đổi phi tuyến tính 6 bit đầu vào thành 4 bit đầu ra?**
A. Bộ hoán vị (P).
B. Bộ mở rộng (E).
C. Các bộ thay thế (S-box).
D. Phép toán XOR.

**Câu 100: Giải thuật 3-DES lựa chọn 1 (sử dụng 3 khóa độc lập) có tổng kích thước bộ khóa là bao nhiêu bit?**
A. 112 bit.
B. 128 bit.
C. 168 bit.
D. 192 bit.

**Câu 101: Giải thuật AES với kích thước khóa 256 bit yêu cầu thực hiện bao nhiêu vòng lặp xử lý dữ liệu?**
A. 10 vòng.
B. 12 vòng.
C. 14 vòng.
D. 16 vòng.

**Câu 102: Trong mỗi vòng lặp chính của AES, hàm biến đổi nào thực hiện việc trộn dữ liệu giữa 4 byte trong cùng một cột của ma trận trạng thái (state)?**
A. SubBytes.
B. ShiftRows.
C. MixColumns.
D. AddRoundKey.

**Câu 103: Điểm khác biệt lớn nhất về cấu trúc giữa vòng lặp cuối cùng và các vòng lặp chính trước đó trong giải thuật AES là gì?**
A. Không có hàm SubBytes.
B. Không có hàm MixColumns.
C. Không có hàm AddRoundKey.
D. Sử dụng 2 lần hàm ShiftRows.

---

## IV. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 98: B.** (Trang 94). 8 bit còn lại chỉ dùng để kiểm tra lỗi (parity check), không tham gia vào độ mạnh mã hóa.
*   **Đáp án Câu 99: C.** (Trang 97). S-box là phần khó thám mã nhất trong DES. Nhớ thông số: **6 in $\rightarrow$ 4 out**.
*   **Đáp án Câu 100: C.** $56 \times 3 = 168$.
*   **Đáp án Câu 101: C.** (Trang 98). Mẹo nhớ: Bắt đầu từ 10 vòng cho khóa 128, mỗi lần tăng kích thước khóa (thêm 64 bit) thì cộng thêm 2 vòng. (10 $\rightarrow$ 12 $\rightarrow$ 14).
*   **Đáp án Câu 102: C.** Tên hàm đã nói lên chức năng: **Mix (Trộn) Columns (Cột)**.
*   **Đáp án Câu 103: B.** (Trang 99). Vòng cuối của AES luôn bỏ qua MixColumns để làm cho quá trình mã hóa và giải mã có cấu trúc đối xứng tương đương.

---

## V. MẸO GHI NHỚ NHANH (STUDY TIPS)
*   **Kích thước khối:** DES và 3-DES là "đồ cổ" nên chỉ có **64 bit**. AES là hiện đại nên là **128 bit**.
*   **Số vòng AES:** 128 bit (10 vòng), 192 bit (12 vòng), 256 bit (14 vòng). Cứ tăng thêm 64 bit khóa thì tăng 2 vòng.
*   **Cơ chế 3-DES:** Nhớ quy tắc **E-D-E** (Encrypt - Decrypt - Encrypt).

---
Dựa trên nội dung từ trang 102 đến trang 105 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục **4.3.2 (Mã hóa bất đối xứng RSA)**.

Phần này đặc biệt quan trọng vì đề thi thường hỏi về **quy trình toán học** và các **con số khuyến nghị**. Bạn cần nắm chắc các bước tính toán để giải các bài tập tình huống nhỏ.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 4 (MỤC 4.3.2)
**Chủ đề: Mã hóa bất đối xứng và Giải thuật RSA**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Đặc điểm hệ mã hóa bất đối xứng (Mục 4.3.2.1)
*   **Cặp khóa:** Mỗi thực thể sở hữu 1 cặp khóa gồm:
    *   **Khóa công khai (Public key):** Dùng để **mã hóa**, có thể phổ biến rộng rãi.
    *   **Khóa riêng (Private key):** Dùng để **giải mã**, phải giữ bí mật tuyệt đối.
*   **Ưu điểm:** Quản lý và phân phối khóa đơn giản (không cần kênh mật để trao đổi khóa bí mật như mã hóa đối xứng).
*   **Nhược điểm:** Tốc độ thực thi chậm hơn nhiều lần so với mã hóa đối xứng.
*   **Đại diện:** RSA, Rabin, ElGamal, McEliece, Knapsack.

### 2. Giải thuật RSA (Mục 4.3.2.2)
*   **Cơ sở an toàn:** Dựa trên độ khó của việc **phân tích một số nguyên cực lớn thành các thừa số nguyên tố**.
*   **Kích thước khóa khuyến nghị:** 
    *   Dưới 1024 bit: Không còn an toàn.
    *   Hiện tại (2010 - 2025): **2048 bit**.
    *   Tương lai: 3072 bit.

### 3. Quy trình toán học của RSA (Cần thuộc lòng)
1.  Chọn 2 số nguyên tố lớn $p$ và $q$.
2.  Tính $n = p \times q$ (n gọi là modulo).
3.  Tính giá trị hàm số Euler: $\Phi(n) = (p-1) \times (q-1)$.
4.  Chọn số nguyên $e$ sao cho $1 < e < \Phi(n)$ và $gcd(e, \Phi(n)) = 1$ ($e$ và $\Phi(n)$ là số nguyên tố cùng nhau).
5.  Tính số nguyên $d$ sao cho: $(d \times e) \equiv 1 \pmod{\Phi(n)}$.
    *   **Khóa công khai:** $(n, e)$
    *   **Khóa riêng:** $(n, d)$
6.  **Mã hóa:** $c = m^e \pmod n$ (với $m$ là bản rõ dạng số).
7.  **Giải mã:** $m = c^d \pmod n$.

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 104: Trong hệ mã hóa bất đối xứng, nếu người gửi A muốn gửi thông tin bí mật cho người nhận B, người A phải sử dụng khóa nào để mã hóa?**
A. Khóa công khai của A.
B. Khóa riêng của A.
C. Khóa công khai của B.
D. Khóa riêng của B.

**Câu 105: Giải thuật RSA được công bố năm 1977 dựa trên độ khó của bài toán toán học nào?**
A. Bài toán logarit rời rạc.
B. Bài toán phân tích số nguyên lớn thành thừa số nguyên tố.
C. Bài toán xếp balo (Knapsack).
D. Phép toán XOR bit.

**Câu 106: Trong quy trình sinh khóa RSA, sau khi chọn được 2 số nguyên tố $p=3$ và $q=11$, giá trị $\Phi(n)$ sẽ là bao nhiêu?**
A. 33
B. 20
C. 14
D. 30

**Câu 107: Theo giáo trình, để đảm bảo an toàn cho giai đoạn 2010-2020 và hiện tại, kích thước khóa RSA được khuyến nghị là bao nhiêu bit?**
A. 512 bit.
B. 1024 bit.
C. 2048 bit.
D. 4096 bit.

**Câu 108: Điều kiện để chọn số mũ mã hóa $e$ trong giải thuật RSA là gì?**
A. $e$ phải là số chẵn.
B. $e$ phải là ước số của $n$.
C. $gcd(e, \Phi(n)) = 1$ (tức $e$ và $\Phi(n)$ nguyên tố cùng nhau).
D. $e$ phải lớn hơn $n$.

**Câu 109: Công thức nào sau đây được sử dụng để giải mã (khôi phục bản rõ $m$ từ bản mã $c$) trong RSA?**
A. $m = c \times d \pmod n$
B. $m = c^e \pmod n$
C. $m = c^d \pmod n$
D. $m = c/d \pmod n$

**Câu 110: Để tăng cường độ an toàn cho cặp khóa RSA, hiệu số $|p - q|$ nên như thế nào?**
A. Càng nhỏ càng tốt.
B. Không được quá nhỏ (phải đủ lớn).
C. Phải bằng 0.
D. Không quan trọng.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 104: C.** Quy tắc vàng của mã hóa công khai: **Dùng khóa công khai của người nhận để mã hóa**. Chỉ có người nhận mới có khóa riêng tương ứng để mở.
*   **Đáp án Câu 105: B.** Đây là kiến thức lý thuyết nền tảng nhất của RSA.
*   **Đáp án Câu 106: B.** $\Phi(n) = (3-1) \times (11-1) = 2 \times 10 = 20$. (Lưu ý: Rất nhiều sinh viên nhầm lẫn tính $n = 3 \times 11 = 33$).
*   **Đáp án Câu 107: C.** (Trang 103). Con số **2048** là tiêu chuẩn hiện hành.
*   **Đáp án Câu 108: C.** (Trang 103). Nếu không thỏa mãn điều kiện này, ta không thể tìm được số $d$ nghịch đảo ở bước sau.
*   **Đáp án Câu 109: C.** (Trang 104). Nhớ cặp bài trùng: Mã hóa dùng $e$, Giải mã dùng $d$.
*   **Đáp án Câu 110: B.** (Trang 105). Nếu $p$ và $q$ quá gần nhau, kẻ tấn công có thể dễ dàng tìm ra chúng bằng cách thử các số quanh căn bậc hai của $n$.

---

## IV. MẸO GHI NHỚ TOÁN HỌC RSA
Để không nhầm lẫn 7 bước của RSA, hãy nhớ câu thần chú:
1.  **Chọn 2 Nguyên tố** ($p, q$)
2.  **Nhân ra Modulo** ($n = p \times q$)
3.  **Euler trừ 1** ($\Phi = (p-1)(q-1)$)
4.  **Chọn $e$ nguyên tố cùng nhau** (với $\Phi$)
5.  **Tìm $d$ nghịch đảo** (để $e \times d \equiv 1 \pmod \Phi$)
6.  **Mã mũ $e$, Giải mũ $d$** (tất cả đều $\pmod n$)

---
Dựa trên nội dung từ trang 105 đến trang 111 của giáo trình, tôi đã biên soạn tài liệu ôn tập trắc nghiệm cho mục **4.4 (Hàm băm mật mã)**. 

Hàm băm là một phần quan trọng để đảm bảo tính **Toàn vẹn (Integrity)**. Trong đề thi, phần này thường tập trung vào các tính chất toán học và độ dài bit đầu ra của từng giải thuật.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 4 (MỤC 4.4)
**Chủ đề: Hàm băm mật mã (Hash Functions)**

## I. TÓM LƯỢC TƯ DUY (QUICK-SCAN)

### 1. Đặc điểm cốt lõi của hàm băm (Mục 4.4.1.1)
Mọi hàm băm mật mã buộc phải có 2 tính chất tối thiểu:
*   **Nén (Compression):** Chuyển dữ liệu đầu vào độ dài bất kỳ thành chuỗi đầu ra độ dài cố định.
*   **Dễ tính toán:** Việc tính $h(x)$ từ $x$ phải nhanh và dễ dàng.

**3 thuộc tính an ninh nâng cao:**
1.  **Kháng tiền ảnh (Preimage resistance):** Cho trước giá trị băm $y$, không thể tìm lại được bản tin gốc $x$ sao cho $h(x) = y$. (Tính một chiều).
2.  **Kháng tiền ảnh thứ 2 (Second-preimage resistance):** Cho trước bản tin $x$, không thể tìm được bản tin $x' \neq x$ sao cho $h(x) = h(x')$.
3.  **Kháng va chạm (Collision resistance):** Không thể tìm được **bất kỳ** cặp bản tin $(x, x')$ khác nhau nào mà có cùng giá trị băm.

### 2. Phân loại hàm băm (Mục 4.4.1.2)
*   **Hàm băm không khóa (MDC - Modification Detection Code):** Chỉ dùng để phát hiện thay đổi dữ liệu. Gồm 2 loại con: **OWHF** (Hàm băm một chiều) và **CRHF** (Hàm băm kháng va chạm).
*   **Hàm băm có khóa (MAC - Message Authentication Code):** Dùng để xác thực thông điệp và đảm bảo tính toàn vẹn (cần một khóa bí mật dùng chung).

### 3. Các thông số giải thuật cần nhớ (Cực kỳ quan trọng)

| Giải thuật | Độ dài đầu ra (Bit) | Đặc điểm/Tình trạng |
|:---|:---|:---|
| **CRC-32** | 32 bit | Chỉ dùng để phát hiện lỗi đường truyền/lưu trữ. |
| **MD5** | **128 bit** | 4 vòng lặp. Hiện không còn an toàn. |
| **SHA-1** | **160 bit** | 80 vòng lặp. NIST khuyến nghị ngừng sử dụng từ 2011. |
| **SHA-2** | 224, **256**, 384, **512** | Tiêu chuẩn hiện tại (SHA-256, SHA-512). |
| **SHA-3** | 0 đến 512 bit | Kiến trúc mới, an toàn cao nhưng chưa phổ biến bằng SHA-2. |

---

## II. CÂU HỎI TRẮC NGHIỆM MÔ PHỎNG

**Câu 111: Thuộc tính nào của hàm băm đảm bảo rằng "không thể tìm lại được thông điệp gốc khi biết trước giá trị băm"?**
A. Tính nén.
B. Kháng tiền ảnh (Preimage resistance).
C. Kháng va chạm (Collision resistance).
D. Dễ tính toán.

**Câu 112: "Mã xác thực thông điệp" (MAC) khác với "Mã phát hiện sửa đổi" (MDC) ở điểm cơ bản nào?**
A. MAC có tốc độ băm nhanh hơn.
B. MAC sử dụng thêm một khóa bí mật trong quá trình băm.
C. MDC cho đầu ra có độ dài thay đổi.
D. MAC chỉ dùng cho các file văn bản.

**Câu 113: Hàm băm MD5 do Ronald Rivest thiết kế cho ra giá trị băm có độ dài bao nhiêu bit?**
A. 64 bit.
B. 128 bit.
C. 160 bit.
D. 256 bit.

**Câu 114: Giải thuật băm SHA-1 tạo ra chuỗi đại diện (digest) có kích thước là:**
A. 128 bit (32 số hexa).
B. 160 bit (40 số hexa).
C. 256 bit (64 số hexa).
D. 512 bit.

**Câu 115: Tại sao MD5 và SHA-1 hiện nay bị khuyến nghị không nên tiếp tục sử dụng cho các mục đích an ninh cao?**
A. Vì tốc độ tính toán quá chậm.
B. Vì kích thước đầu ra quá lớn gây tốn bộ nhớ.
C. Vì đã tồn tại các kỹ thuật khai thác lỗi và tìm được va chạm (collision).
D. Vì chúng không hỗ trợ tiếng Việt.

**Câu 116: Theo giáo trình, nhóm hàm băm nào hiện đang được sử dụng rộng rãi nhất trong các ứng dụng chữ ký số?**
A. MD2 và MD4.
B. SHA-0 và SHA-1.
C. SHA-2 (SHA-256, SHA-512).
D. CRC-32.

**Câu 117: Trong quá trình xử lý của SHA-1, thông điệp đầu vào được chia thành các khối có kích thước bao nhiêu bit?**
A. 128 bit.
B. 160 bit.
C. 512 bit.
D. 1024 bit.

---

## III. GIẢI THÍCH & PHÂN TÍCH

*   **Đáp án Câu 111: B.** Kháng tiền ảnh = Kháng việc tìm ngược lại "ảnh" ban đầu. Đây là tính chất chứng minh hàm băm là hàm một chiều.
*   **Đáp án Câu 112: B.** (Trang 106). MAC = Message + Key. MDC = Message only.
*   **Đáp án Câu 113: B.** MD5 = 128 bit. Hãy nhớ con số này vì nó rất hay xuất hiện trong thực tế (check MD5 checksum).
*   **Đáp án Câu 114: B.** (Trang 111). SHA-1 là 160 bit. Mẹo đổi sang số hexa: 160 bit / 4 bit mỗi số hexa = 40 ký tự.
*   **Đáp án Câu 115: C.** Một hàm băm bị coi là hỏng (broken) khi người ta tìm được cách tạo ra va chạm nhanh hơn phương pháp vét cạn. MD5 và SHA-1 đều đã bị tìm được va chạm.
*   **Đáp án Câu 116: C.** (Trang 109). SHA-2 là tiêu chuẩn vàng hiện nay cho SSL và Chữ ký số.
*   **Đáp án Câu 117: C.** (Trang 111). Cả MD5 và SHA-1 đều chia khối thông điệp (padding) thành các phần **512 bit** để xử lý lặp.

---

## IV. BẢNG TỔNG KẾT ĐỂ NHẬN DIỆN NHANH

| Đặc tính | MD5 | SHA-1 |
|:---|:---|:---|
| **Độ dài Digest** | **128 bit** | **160 bit** |
| **Số khối xử lý** | 512 bit | 512 bit |
| **Số vòng lặp** | 4 vòng (mỗi vòng 16 thao tác) | 80 vòng (mỗi vòng 1 thao tác) |
| **Người thiết kế** | Ronald Rivest | NSA (Hoa Kỳ) |

---
