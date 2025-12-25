Đây là tài liệu ôn tập tối ưu hoá cho hình thức thi trắc nghiệm, dựa trên nội dung **Chương 1 (Mục 1.1 và 1.2)** của bài giảng bạn đã cung cấp.

Tài liệu được thiết kế để giúp bạn phản xạ nhanh, tránh bẫy và tính toán chính xác.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: HỆ ĐẾM & CHUYỂN ĐỔI CƠ SỐ
**(Phạm vi: Mục 1.1 & 1.2)**

### PHẦN A: GIẢI PHẪU TỪ KHÓA & ĐỊNH NGHĨA (Ghi nhớ nhanh)

Trong trắc nghiệm, giảng viên thường hỏi về các thuật ngữ hoặc đơn vị đo lường.

1.  **Các đơn vị dữ liệu (Cực kỳ quan trọng):**
    *   **Bit (Binary Digit):** Đơn vị thông tin nhỏ nhất (chỉ có 0 hoặc 1).
    *   **Nibble:** Nhóm **4 bit**.
    *   **Byte:** Nhóm **8 bit**.
    *   **Word:** Phụ thuộc hệ thống (thường là 16, 32, hoặc 64 bit).
2.  **Vị trí trọng số:**
    *   **LSB (Least Significant Bit):** Bit có trọng số **bé nhất** (nằm ngoài cùng bên **phải** - $2^0$).
    *   **MSB (Most Significant Bit):** Bit có trọng số **lớn nhất** (nằm ngoài cùng bên **trái** - $2^{n-1}$).
3.  **Giá trị Hexa (Hệ 16) cần thuộc lòng:**
    *   0-9: Giữ nguyên.
    *   **A = 10, B = 11, C = 12, D = 13, E = 14, F = 15**.
    *   *(Mẹo nhớ: F là Full, là giá trị lớn nhất của 4 bit $1111_2$, tức là 15, không phải 16).*

---

### PHẦN B: QUY TRÌNH TÍNH TOÁN "NHANH - GỌN"

Đừng làm theo cảm tính, hãy áp dụng đúng thuật toán cho từng dạng bài:

#### 1. Chuyển từ Thập phân (10) sang Nhị/Bát/Hex (N)
*   **Phần Nguyên (Trước dấu phẩy):** Chia liên tiếp cho cơ số N -> Lấy **SỐ DƯ** -> Viết **NGƯỢC** (từ dưới lên).
*   **Phần Lẻ (Sau dấu phẩy):** Nhân liên tiếp với cơ số N -> Lấy **PHẦN NGUYÊN** -> Viết **XUÔI** (từ trên xuống).

#### 2. Chuyển từ Nhị/Bát/Hex (N) sang Thập phân (10)
*   **Công thức tổng quát:** $\sum (\text{Ký số} \times \text{Cơ số}^{\text{Vị trí}})$.
*   *Lưu ý:* Vị trí sau dấu phẩy là số mũ âm ($N^{-1}, N^{-2}, \dots$).

#### 3. Chuyển đổi nhanh giữa Nhị phân (2) $\leftrightarrow$ Bát phân (8) / Hex (16)
*   **Quy tắc:** Không cần đổi sang trung gian là hệ 10.
    *   Hệ 8: Gom nhóm **3 bit** ($2^3 = 8$).
    *   Hệ 16: Gom nhóm **4 bit** ($2^4 = 16$).
*   **Điểm xuất phát (QUAN TRỌNG):** Luôn bắt đầu từ **dấu phẩy** đi ra hai phía.

---

### PHẦN C: "BẪY" VÀ CÁC LỖI SAI PHỔ BIẾN (High Alert)

Đây là phần quyết định điểm số của bạn. Hãy chú ý những điểm giảng viên thường gài bẫy:

**🔴 Bẫy 1: Hướng gom nhóm bit**
*   *Tình huống:* Đổi $11010,01_2$ sang Hex.
*   *Lỗi sai:* Gom từ trái sang phải một mạch ($1101$ rồi $001...$).
*   *Chính xác:* Phải lấy dấu phẩy làm mốc.
    *   Phần nguyên (sang trái): $\underline{0001} \ \underline{1010}$.
    *   Phần lẻ (sang phải): $\underline{0100}$ (Thêm số 0 vào cho đủ 4 bit).
    *   Kết quả: $1A,4_{16}$.

**🔴 Bẫy 2: Phép nhân phần lẻ không dừng**
*   *Tình huống:* Đổi $0,3_{10}$ sang nhị phân.
*   *Thực tế:* Phép nhân sẽ lặp lại vô tận ($0,3 \times 2 = 0,6 \to 0,6 \times 2 = 1,2 \to 0,2 \times 2 = 0,4...$).
*   *Cách xử lý:* Đề bài trắc nghiệm thường sẽ hỏi "lấy 4 bit sau dấu phẩy" hoặc đáp án là giá trị gần đúng. Đừng hoảng khi thấy nhân mãi không hết số 0.

**🔴 Bẫy 3: Nhầm lẫn giá trị Hex**
*   Khi cộng trừ hệ Hex: $A + 1 = B$ (không phải 11). $F + 1 = 10_{16}$ (tức là $16_{10}$).
*   Rất nhiều bạn tính: $9 + 1 = A$ (Đúng), nhưng $9 + 2 = B$ (Sai, $9+2=11_{10}=B_{16}$). Hãy cẩn thận khi cộng qua mốc 9.

**🔴 Bẫy 4: Quên số 0 ở giữa**
*   *Tình huống:* Đổi $10001_2$ sang Hex.
*   *Gom nhóm:* $0001 \ 0001$.
*   *Kết quả:* $11_{16}$.
*   *Bẫy:* Nếu chuỗi là $100001$ -> Nhóm: $0010 \ 0001$ -> Kết quả $21_{16}$. Hãy viết tách nhóm rõ ràng ra giấy nháp.

---

### PHẦN D: CÂU HỎI GIẢ LẬP (MOCK TEST)

Thử sức với các câu hỏi sau (Đáp án & Giải thích ở dưới):

**Câu 1:** Số nhị phân $10110,11_2$ tương ứng với số thập phân nào?
A. 22,3
B. 22,75
C. 20,75
D. 22,6

**Câu 2:** Chuyển đổi số $3F,8_{16}$ sang hệ nhị phân.
A. 0011 1111, 1000
B. 0011 1111, 0100
C. 11 1111, 0001
D. 11 1111, 1000

**Câu 3:** Kết quả của phép tính $9_{16} + 8_{16}$ là:
A. $17_{16}$
B. $11_{16}$
C. $10_{16}$
D. $21_{16}$

**Câu 4:** Trong hệ thập lục phân (Hex), giá trị của ký tự 'E' là:
A. 13
B. 14
C. 15
D. 16

**Câu 5:** Nibble là thuật ngữ dùng để chỉ:
A. 2 bit
B. 4 bit
C. 8 bit
D. 16 bit

---

### ĐÁP ÁN & GIẢI THÍCH CHI TIẾT

**Câu 1: B (22,75)**
*   *Giải thích:*
    *   Phần nguyên: $10110 = 1\cdot 2^4 + 0 + 1\cdot 2^2 + 1\cdot 2^1 + 0 = 16 + 4 + 2 = 22$.
    *   Phần lẻ: $0,11 = 1\cdot 2^{-1} + 1\cdot 2^{-2} = 0,5 + 0,25 = 0,75$.
    *   Tổng: 22,75.
*   *Mẹo trắc nghiệm:* Nhìn phần lẻ $0,11_2$ chắc chắn lớn hơn $0,5$. Loại A, D. Tính phần nguyên là xong.

**Câu 2: A**
*   *Giải thích:* Tách từng ký tự Hex ra 4 bit nhị phân.
    *   $3 \to 0011$
    *   $F \to 1111$
    *   $8 \to 1000$
*   *Lưu ý:* Đáp án D thiếu các số 0 ở đầu (mặc dù về giá trị không sai nhưng chuẩn 4 bit thì A đầy đủ hơn, tuy nhiên nếu đề bài cho D mà không có A thì chọn D). Nhưng đáp án A là chuẩn form nhất. Đáp án B sai vì $8_{16} = 1000_2$.

**Câu 3: B ($11_{16}$)**
*   *Giải thích:*
    *   Đổi ra thập phân: $9 + 8 = 17$.
    *   Đổi $17_{10}$ sang Hex: $17 / 16 = 1$ dư **1**.
    *   Viết ngược: $11_{16}$.
*   *Cảnh báo:* Đừng chọn A ($17_{16}$ là sai vì hệ 16 không có ký số 17).

**Câu 4: B (14)**
*   *Giải thích:* Nhớ bảng: A=10, B=11, C=12, D=13, **E=14**, F=15.

**Câu 5: B (4 bit)**
*   *Giải thích:* Kiến thức định nghĩa cơ bản trong giáo trình (Trang 2 PDF).
    *   2 bit = Crumb/Tydbit
    *   8 bit = Byte

---

Đây là phần tài liệu quan trọng và "khó nuốt" nhất của Chương 1. Trong đề thi trắc nghiệm, các câu hỏi phân loại điểm 9-10 thường nằm ở phần **Tràn số (Overflow)** và **Bù 2**.

Dưới đây là tài liệu ôn tập được thiết kế sâu sắc để bạn hiểu bản chất, nhưng trình bày đủ gọn gàng để dễ học thuộc.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: SỐ HỌC NHỊ PHÂN CÓ DẤU
**(Phạm vi: Mục 1.3)**

### PHẦN A: BẢN CHẤT & BIỂU DIỄN SỐ (Deep Dive)

Máy tính không hiểu dấu "-" hay "+". Nó chỉ có bit 0 và 1. Vì vậy, ta phải quy ước bit đầu tiên (MSB - Bit trọng số lớn nhất) làm **Bit Dấu**.
*   **0** là Dương (+)
*   **1** là Âm (-)

Có 3 cách để biểu diễn số âm, bạn cần phân biệt rõ sự khác nhau:

#### 1. Phương pháp Dấu - Lượng (Sign-Magnitude)
*   **Cách làm:** Bit đầu là dấu, các bit còn lại là giá trị tuyệt đối.
*   **Ví dụ (8 bit):**
    *   $+9 = \mathbf{0}0001001$
    *   $-9 = \mathbf{1}0001001$
*   **Nhược điểm (Thi hay hỏi):** Có **hai số 0** ($+0$ và $-0$). Điều này gây lãng phí và khó khăn cho mạch tính toán.

#### 2. Phương pháp Bù 1 (1's Complement)
*   **Cách làm:** Đảo ngược tất cả các bit của số dương (0 thành 1, 1 thành 0).
*   **Ví dụ (8 bit):**
    *   $+9 = 00001001$
    *   $-9 = 11110110$ (Bù 1)
*   **Nhược điểm:** Vẫn tồn tại hai số 0.

#### 3. Phương pháp Bù 2 (2's Complement) - QUAN TRỌNG NHẤT
Đây là phương pháp máy tính hiện đại sử dụng.
*   **Cách làm:** Lấy Bù 1 cộng thêm 1.
*   **Ví dụ (8 bit):**
    *   Bước 1 (Lấy số dương): $00001001$ (+9)
    *   Bước 2 (Đảo bit - Bù 1): $11110110$
    *   Bước 3 (Cộng 1): $11110111$ (Đây là -9 trong Bù 2)
*   **Ưu điểm:** Chỉ có **một số 0** duy nhất. Dễ dàng thực hiện phép trừ bằng phép cộng.

> **MẸO TÍNH NHANH BÙ 2 (Không cần đảo rồi cộng):**
> 1.  Nhìn số nhị phân gốc từ Phải sang Trái.
> 2.  Giữ nguyên tất cả các bit **cho đến khi gặp số 1 đầu tiên**.
> 3.  Giữ nguyên số 1 đó.
> 4.  **Đảo ngược tất cả các bit còn lại** bên trái nó.
> *Ví dụ:* Tìm bù 2 của `01010100`
> *   Giữ nguyên `100` (từ phải sang).
> *   Đảo ngược đoạn trước đó (`01010` -> `10101`).
> *   Kết quả: `10101100`.

---

### PHẦN B: PHẠM VI BIỂU DIỄN (Range) - Cần thuộc lòng

Giảng viên rất thích ra câu hỏi: *"Với n bit, số nguyên có dấu biểu diễn theo phương pháp bù 2 có giá trị trong khoảng nào?"*

| Phương pháp | Công thức | Ví dụ với 8 bit (n=8) | Lưu ý |
| :--- | :--- | :--- | :--- |
| **Không dấu** | $0$ đến $2^n - 1$ | 0 đến 255 | Luôn dương |
| **Dấu - Lượng** | $-(2^{n-1}-1)$ đến $+(2^{n-1}-1)$ | -127 đến +127 | Mất 1 giá trị do có hai số 0 |
| **Bù 1** | $-(2^{n-1}-1)$ đến $+(2^{n-1}-1)$ | -127 đến +127 | Mất 1 giá trị do có hai số 0 |
| **Bù 2** | $-2^{n-1}$ đến $+(2^{n-1}-1)$ | **-128** đến +127 | **Lệch về phía âm** (Biểu diễn được nhiều hơn 1 số âm) |

---

### PHẦN C: CÁC QUY TẮC PHÉP TÍNH & BẪY TRÀN SỐ (Overflow)

Đây là phần khó nhất. Hãy chú ý kỹ.

#### 1. Quy tắc cộng/trừ
Phép trừ $A - B$ thực chất là $A + (-B)$. Ta chỉ cần tìm bù của B rồi cộng với A.

*   **Đối với Bù 1:** Nếu phép cộng có **nhớ ra khỏi bit dấu** (bit thừa), ta phải **CỘNG** bit đó ngược lại vào hàng đơn vị (End-around carry).
*   **Đối với Bù 2:** Nếu phép cộng có **nhớ ra khỏi bit dấu**, ta **BỎ** bit đó đi (Discard carry).

> **Trong thi trắc nghiệm:** 99% đề sẽ hỏi về **Bù 2**. Hãy nhớ khẩu quyết: **"Bù 2 thì Bỏ nhớ thừa"**.

#### 2. Hiện tượng TRÀN SỐ (Overflow) - Cách phát hiện
Tràn số xảy ra khi kết quả tính toán vượt quá khả năng biểu diễn của số bit cho trước (ví dụ dùng 4 bit mà kết quả ra tới 16 hoặc -9).

**Làm sao để phát hiện tràn số khi nhìn vào phép tính?**
Hãy nhìn vào **Bit dấu (MSB)** của 2 số hạng và kết quả:

1.  **Dương + Dương = Âm** $\rightarrow$ **TRÀN** (Vô lý, 2 số dương cộng lại sao ra âm được?)
2.  **Âm + Âm = Dương** $\rightarrow$ **TRÀN** (Vô lý, nợ cộng nợ sao ra tiền dư được?)
3.  **Dương + Âm** $\rightarrow$ **KHÔNG BAO GIỜ TRÀN** (Yên tâm tính).

> **Ví dụ minh họa (Hệ 4 bit, Bù 2):**
> *   Phạm vi: -8 đến +7.
> *   Tính: $(+5) + (+4)$
>     *   $+5 = 0101$
>     *   $+4 = 0100$
>     *   Cộng: $1001$ (Đây là số -7 trong bù 2).
> *   **Phân tích:** Dương + Dương ra Âm (bit đầu là 1). **Kết luận: Tràn số.** (Vì $5+4=9$, mà 4 bit chỉ chứa được tối đa là 7).

---

### PHẦN D: CÂU HỎI GIẢ LẬP & PHÂN TÍCH

**Câu 1:** Trong hệ thống số nhị phân bù 2 (2's complement) 8 bit, giá trị biểu diễn nhỏ nhất và lớn nhất là:
A. -127 đến +128
B. -128 đến +127
C. -127 đến +127
D. 0 đến 255

> **Đáp án: B.**
> *Giải thích:* Bù 2 bị lệch về phía âm. Công thức $-2^{n-1}$ đến $2^{n-1}-1$.
> $2^7 = 128$. Vậy là $-128$ đến $+127$.

**Câu 2:** Cho số nhị phân $X = 11101000$ (biểu diễn theo Bù 2). Giá trị thập phân của X là bao nhiêu?
A. -24
B. -23
C. +232
D. -104

> **Đáp án: A.**
> *Giải thích (Cách làm ngược):*
> 1. Thấy bit đầu là 1 -> Số Âm.
> 2. Muốn biết trị tuyệt đối, hãy lấy Bù 2 của nó lần nữa.
> 3. $X = 11101000$. Giữ nguyên `1000` cuối, đảo phần trước: `0001` + `1000` = $00011000_2$.
> 4. $00011000_2 = 16 + 8 = 24$.
> 5. Vậy số gốc là **-24**.

**Câu 3:** Thực hiện phép cộng hai số bù 2 (4 bit): $1001 + 1100$. Kết quả và trạng thái cờ báo tràn (Overflow flag) là:
A. 0101, Tràn
B. 0101, Không tràn
C. 10101, Tràn
D. 0011, Tràn

> **Đáp án: B.**
> *Giải thích:*
> *   $1001$ (-7)
> *   $1100$ (-4)
> *   Cộng: $1 + 1001 + 1100 = 10101$.
> *   Quy tắc Bù 2: Bỏ bit nhớ thừa (bit 1 ở đầu) -> Kết quả còn $0101$ (+5).
> *   Check Tràn: Âm (-7) + Âm (-4) = Dương (+5). **Lý ra phải là TRÀN**.
> *   *Tuy nhiên, hãy xem kỹ lại:*
>     *   $-7 + (-4) = -11$.
>     *   4 bit bù 2 biểu diễn từ -8 đến +7. -> -11 nằm ngoài phạm vi -> **TRÀN**.
>     *   Nhưng tại sao đáp án B lại là 0101?
>     *   Tính toán máy tính: $1001 + 1100 = 10101$ -> Bỏ bit nhớ cao nhất -> còn $0101$.
>     *   Xét dấu: Âm + Âm = Dương ($0101$). -> Kết luận: Có Tràn (Overflow).
> *   **ĐÍNH CHÍNH:** Xin lỗi, tôi cần tính toán lại cẩn thận theo đúng logic máy tính cho bạn.
>     *   $1001$ (-7)
>     *   $1100$ (-4)
>     *   Tổng = $10101$. Bỏ bit 1 đầu tiên (carry out). Kết quả lưu trong 4 bit là $0101$ (+5).
>     *   Logic Tràn: Âm + Âm ra Dương -> **CÓ TRÀN**.
>     *   Vậy đáp án đúng phải là **A. 0101, Tràn**. (Xin lỗi vì sự nhầm lẫn ở trên, đây là ví dụ thực tế về việc dễ bị lừa!).

**Câu 4:** Đặc điểm nào sau đây KHÔNG PHẢI của phương pháp Bù 1?
A. Tồn tại hai giá trị biểu diễn cho số 0.
B. Phép cộng phức tạp hơn Bù 2 (phải xử lý bit nhớ).
C. Phạm vi biểu diễn đối xứng (-127 đến +127).
D. Bit dấu luôn là 0.

> **Đáp án: D.**
> *Giải thích:* Bù 1 là số có dấu, nên bit dấu phụ thuộc vào số đó âm hay dương (1 là âm, 0 là dương), không phải "luôn là 0".

---

**Tóm tắt chiến thuật học phần 1.3:**
1.  Thuộc công thức phạm vi (Range) của Bù 2.
2.  Thành thạo cách đổi Bù 2 nhanh (Giữ bit 1 đầu tiên từ phải sang).
3.  Nhớ quy tắc cộng Bù 2 (Bỏ bit nhớ thừa).
4.  Nhớ quy tắc Tràn (Dương+Dương=Âm, Âm+Âm=Dương).

---
Dưới đây là tài liệu ôn tập chuyên sâu cho **Mục 2.1: Các hàm chuyển mạch cơ bản**.

Mặc dù đây là phần mở đầu có vẻ đơn giản, nhưng trong thi trắc nghiệm, sinh viên thường mất điểm vì đọc không kỹ câu hỏi về **mô hình mạch điện** (công tắc) hoặc nhầm lẫn giữa ngôn ngữ toán học và ngôn ngữ mạch.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CÁC HÀM LOGIC CƠ BẢN
**(Phạm vi: Mục 2.1 - Chương 2)**

### PHẦN A: BẢN CHẤT & TỪ KHÓA (Ghi nhớ cực nhanh)

Hãy liên kết các khái niệm sau lại với nhau thành một chuỗi để phản xạ ngay lập tức:

| Tên Hàm | Ký hiệu Toán học | Tên phép toán | Mô hình Công tắc (Switch) | Đặc điểm cốt lõi (Mẹo nhớ) |
| :--- | :---: | :--- | :--- | :--- |
| **AND** | $A . B$ hoặc $AB$ | **Tích** logic (Phép Nhân) | **Nối tiếp** (Series) | Chỉ **ĐÚNG** khi **TẤT CẢ** đều đúng. |
| **OR** | $A + B$ | **Tổng** logic (Phép Cộng) | **Song song** (Parallel) | Chỉ **SAI** khi **TẤT CẢ** đều sai. |
| **NOT** | $\bar{A}$ | **Đảo** / Phủ định | **Song song với tải** (Shunt) | Luôn **NGƯỢC** lại. |

---

### PHẦN B: PHÂN TÍCH SÂU MÔ HÌNH MẠCH ĐIỆN (Trọng tâm)

Giáo trình của bạn sử dụng mô hình mạch điện (Công tắc, Điện trở R, Đèn LED) để giải thích logic. Đây là phần dễ bị hỏi lắt léo nhất.

#### 1. Mạch AND (Nối tiếp)
*   **Cấu tạo:** Các công tắc (A, B) mắc **nối tiếp** nhau và nối tiếp với đèn LED.
*   **Nguyên lý:** Dòng điện muốn đi qua đèn thì cầu nối phải liền mạch từ đầu này sang đầu kia. Nếu hở bất kỳ chỗ nào $\rightarrow$ Mất điện.
*   **Logic:** Đèn sáng (F=1) $\Leftrightarrow$ A đóng (1) **VÀ** B đóng (1).

#### 2. Mạch OR (Song song)
*   **Cấu tạo:** Các công tắc (A, B) mắc **song song** với nhau.
*   **Nguyên lý:** Dòng điện giống như dòng nước, nó có nhiều đường để đi. Nếu đường A tắc, nó đi đường B. Chỉ khi cả hai đường đều tắc thì nước mới không chảy được.
*   **Logic:** Đèn sáng (F=1) $\Leftrightarrow$ Có ít nhất một công tắc đóng (1).
*   **Bẫy:** Trong đời sống ta hay nói "Ăn cơm hoặc ăn phở" (chọn 1 trong 2). Nhưng trong Logic OR, "Ăn cả cơm và phở" (A=1, B=1) thì kết quả vẫn là ĐÚNG (F=1).

#### 3. Mạch NOT (Cực kỳ lưu ý - Phần khó hiểu nhất)
Đây là phần lạ nhất so với tư duy thông thường. Tại sao đóng công tắc mà đèn lại tắt?

*   **Cấu tạo:** Công tắc A mắc **song song với đèn LED** (nhưng nối tiếp với điện trở R ở phía trước).
*   **Cơ chế vật lý (Short Circuit - Ngắn mạch):**
    *   Khi công tắc A **MỞ (0)**: Dòng điện đi qua điện trở R, không qua được nhánh A nên buộc phải đi qua đèn LED $\rightarrow$ Đèn **SÁNG (1)**.
    *   Khi công tắc A **ĐÓNG (1)**: Dòng điện cực kỳ "lười", nó luôn chọn đường đi có điện trở thấp nhất. Sợi dây công tắc A có điện trở gần bằng 0, trong khi đèn LED có điện trở cao hơn. $\rightarrow$ Toàn bộ dòng điện chạy qua công tắc A, bỏ qua đèn LED $\rightarrow$ Đèn **TẮT (0)**.
*   **Kết luận:** Trạng thái đèn luôn ngược với trạng thái công tắc ($A=1 \to F=0; A=0 \to F=1$).

---

### PHẦN C: CÁCH ĐỌC BIỂU ĐỒ VENN (Lý thuyết tập hợp)

Trong hình 2-1 (Trang 15), các phép toán được biểu diễn bằng hình học:

1.  **Phép AND (Giao):** Phần chung giữa hai vòng tròn A và B. (Chỉ lấy phần gạch chéo nằm trong cả hai).
2.  **Phép OR (Hợp):** Lấy toàn bộ diện tích của cả hai vòng tròn A và B (kể cả phần chung và phần riêng).
3.  **Phép NOT (Phần bù):** Là phần nằm trong hình vuông nhưng **nằm ngoài** vòng tròn A.

---

### PHẦN D: CÁC MỆO LÀM BÀI TRẮC NGHIỆM

Khi gặp câu hỏi về bảng chân lý (Truth Table), đừng dò từng dòng. Hãy dùng quy tắc **"Tìm kẻ khác biệt"**:

1.  **Với hàm AND:** Đi tìm số **0**.
    *   Chỉ cần thấy **một đầu vào là 0** $\rightarrow$ Kết quả chắc chắn là **0**.
    *   (Không cần quan tâm các đầu vào còn lại là gì).
2.  **Với hàm OR:** Đi tìm số **1**.
    *   Chỉ cần thấy **một đầu vào là 1** $\rightarrow$ Kết quả chắc chắn là **1**.
3.  **Với hàm nhiều biến (Ví dụ: F = A.B.C.D...):**
    *   Nếu là AND: Chỉ cần 1 biến bằng 0, cả biểu thức bằng 0.
    *   Nếu là OR: Chỉ cần 1 biến bằng 1, cả biểu thức bằng 1.

---

### PHẦN E: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Trong đại số Boole, phép toán nào tương ứng với cách mắc các chuyển mạch song song?
A. Phép nhân logic (AND)
B. Phép cộng logic (OR)
C. Phép đảo (NOT)
D. Phép so sánh (XOR)

> **Đáp án: B.**
> *Giải thích:* Song song = Nhiều lối đi = Hoặc đi đường này, hoặc đi đường kia = OR (Cộng).

**Câu 2:** Cho hàm chuyển mạch $F = A.B.C$. Giá trị của F sẽ bằng 1 khi nào?
A. Khi A=1, B=0, C=1
B. Khi có ít nhất một biến bằng 1
C. Khi tất cả các biến A, B, C đều bằng 1
D. Khi tất cả các biến A, B, C đều bằng 0

> **Đáp án: C.**
> *Giải thích:* Đây là phép nhân (AND). Chỉ bằng 1 khi **tất cả** đầu vào là 1.

**Câu 3:** Xét mạch điện thực hiện hàm NOT (như Hình 2-4 trong giáo trình). Khi khóa K đóng (trạng thái 1), bóng đèn sẽ:
A. Sáng, vì mạch kín.
B. Tắt, vì bị ngắn mạch (dòng điện đi qua khóa K thay vì qua đèn).
C. Sáng nhấp nháy.
D. Cháy bóng đèn do quá tải.

> **Đáp án: B.**
> *Giải thích:* Đây là cơ chế đặc biệt của mạch NOT dùng relay/công tắc. Khóa K nối song song với đèn, khi đóng sẽ "cướp" hết dòng điện.

**Câu 4:** Biểu thức nào sau đây thể hiện mối quan hệ "Hấp thụ" trong các định lý cơ bản (mục 2.2 bảng 2.1 - *Hỏi sớm một chút để test tư duy logic cơ bản*)?
A. $A . 1 = A$
B. $A + A = A$
C. $A + A.B = A$
D. $A + \bar{A} = 1$

> **Đáp án: C.**
> *Giải thích:*
> *   $A=1 \to 1 + 1.B = 1 + B = 1$ (Đúng bằng A).
> *   $A=0 \to 0 + 0.B = 0 + 0 = 0$ (Đúng bằng A).
> *   Tư duy: Khi đã có A (lớn), việc cộng thêm một phần nhỏ của A (là A.B) không làm thay đổi giá trị tổng thể.

---
Chào bạn, đây là tài liệu ôn tập cho **Mục 2.2: Một số định lý cơ bản trong đại số Boole**.

Đây là phần **"ngữ pháp"** của môn học. Nếu không nắm vững phần này, bạn sẽ không thể làm được các bài tập rút gọn mạch (Mục 2.3) sau này. Trong thi trắc nghiệm, các câu hỏi thường yêu cầu bạn biến đổi nhanh một biểu thức hoặc nhận diện định lý được áp dụng.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: ĐỊNH LÝ BOOLE & QUY TẮC BIẾN ĐỔI
**(Phạm vi: Mục 2.2 - Chương 2)**

### PHẦN A: CÁC ĐỊNH LÝ "SỐNG CÒN" (Cần hiểu bản chất)

Đừng học vẹt. Hãy tư duy theo logic "Công tắc" và "Tập hợp" để nhớ lâu.

#### 1. Nhóm định lý đơn giản (Dễ nhớ)
*   **Đồng nhất & Phần tử 0/1:**
    *   $A . 1 = A$ (Nối tiếp với dây dẫn $\to$ phụ thuộc vào A).
    *   $A + 0 = A$ (Song song với chỗ hở $\to$ phụ thuộc vào A).
    *   $A . 0 = 0$ (Nối tiếp với chỗ hở $\to$ Mất điện luôn).
    *   $A + 1 = 1$ (Song song với dây dẫn $\to$ Điện luôn đi qua dây dẫn $\to$ Luôn Sáng).
*   **Bất biến (Idempotent):**
    *   $A . A = A$
    *   $A + A = A$
    *   *(Ý nghĩa: Mắc 2 công tắc A giống hệt nhau thì cũng chỉ bằng 1 cái A thôi. $1+1=1$, không phải bằng 2).*
*   **Bù (Complementarity):**
    *   $A . \bar{A} = 0$ (Cái này đóng thì cái kia mở $\to$ Mạch nối tiếp luôn hở).
    *   $A + \bar{A} = 1$ (Luôn có 1 cái đóng $\to$ Mạch song song luôn kín).

#### 2. Định lý Hấp thụ (Absorption) - **Cực kỳ quan trọng để rút gọn**
Đây là công cụ mạnh nhất để làm gọn biểu thức.
*   **Công thức:** $A + A.B = A$
*   **Giải thích sâu:**
    *   Logic học: Nếu $A=1$, thì biểu thức ($1 + 1.B$) luôn bằng 1 (bất chấp B là gì). Nếu $A=0$, thì biểu thức ($0 + 0.B$) luôn bằng 0.
    *   $\rightarrow$ Giá trị của B không ảnh hưởng gì cả. B bị A "nuốt chửng" (hấp thụ).
*   **Mở rộng (Thi hay bẫy):** $A . (A + B) = A$.

#### 3. Định lý DeMorgan - "Thần chú" bẻ gạch
Đây là định lý nổi tiếng nhất, dùng để chuyển đổi giữa phép NHÂN (AND) và phép CỘNG (OR).

*   **Quy tắc:** "Bẻ gạch (đảo), đổi dấu".
    *   Đang Nhân thành Cộng: $\overline{A . B} = \bar{A} + \bar{B}$
    *   Đang Cộng thành Nhân: $\overline{A + B} = \bar{A} . \bar{B}$
*   **Ứng dụng:** Dùng để biến đổi mạch toàn NAND hoặc toàn NOR (Mục 2.4).

---

### PHẦN B: CÁC ĐỊNH LUẬT & ĐẲNG THỨC ĐẶC BIỆT (Phần khó)

Phần này chứa những quy tắc khác hẳn với toán học đại số thông thường.

#### 1. Luật Phân Phối (Distributive) - Cẩn thận bị lừa!
*   Dạng 1 (Giống đại số thường): $A.(B+C) = A.B + A.C$ $\to$ Dễ.
*   **Dạng 2 (KHÁC đại số thường):**
    $$A + (B . C) = (A + B) . (A + C)$$
    *   *Tại sao?* Hãy thử nhân bung vế phải ra: $(A+B)(A+C) = A.A + A.C + B.A + B.C = A + A(C+B) + BC = A(1+...) + BC = A + BC$.
    *   *Lưu ý:* Trong đại số thường $2 + (3.4) \neq (2+3).(2+4)$. Nhưng trong Boole thì **ĐÚNG**. Đây là câu hỏi bẫy kinh điển.

#### 2. Quy tắc Tìm đảo hàm số (Complement) vs. Quy tắc Đối ngẫu (Dual)
Sinh viên rất hay nhầm lẫn hai khái niệm này. Hãy phân biệt kỹ:

| Tiêu chí | **Tìm hàm Đảo ($\bar{F}$)** | **Tìm hàm Đối ngẫu ($F'$ hoặc $F^D$)** |
| :--- | :--- | :--- |
| **Mục đích** | Tìm hàm phủ định (NOT F) | Tìm hàm có cấu trúc đối xứng |
| **Phép toán** | AND $\leftrightarrow$ OR | AND $\leftrightarrow$ OR |
| **Hằng số** | $0 \leftrightarrow 1$ | $0 \leftrightarrow 1$ |
| **Biến số** | **Biến đổi ($\bar{A} \leftrightarrow A$)** | **GIỮ NGUYÊN ($A$ vẫn là $A$)** |
| **Ví dụ** | $F = A.B + 0$ | $F = A.B + 0$ |
| **Kết quả** | $\bar{F} = (\bar{A} + \bar{B}) . 1$ | $F^D = (A + B) . 1$ |

> **Điểm mấu chốt:**
> *   Tìm đảo: Thay đổi **TẤT CẢ** (Phép tính, Hằng số, Biến số).
> *   Đối ngẫu: Thay đổi **CẤU TRÚC** (Chỉ Phép tính và Hằng số), **không động vào biến**.

---

### PHẦN C: CHIẾN THUẬT LÀM BÀI TRẮC NGHIỆM (Cheat Codes)

Khi gặp một biểu thức dài ngoằng và hỏi "Rút gọn biểu thức sau?", nếu bạn quên công thức, hãy dùng phương pháp **"Thử giá trị" (Substitution)**.

1.  **Bước 1:** Chọn giá trị cho A, B (ví dụ A=1, B=0).
2.  **Bước 2:** Tính giá trị biểu thức gốc.
3.  **Bước 3:** Tính giá trị 4 đáp án A, B, C, D.
4.  **Kết luận:** Đáp án nào cho kết quả trùng với biểu thức gốc thì đó là đáp án đúng (hoặc ít nhất loại trừ được các đáp án sai).

*Ví dụ:* Rút gọn $F = (A+B)(A+C)$.
*   Thử A=0, B=1, C=0 $\to$ $F = (0+1)(0+0) = 1.0 = 0$.
*   Thử đáp án:
    *   A. $A + BC \to 0 + 1.0 = 0$ (Khớp).
    *   B. $A(B+C) \to 0(1+0) = 0$ (Khớp).
    *   (Nếu có nhiều cái khớp, thử thêm bộ số khác, ví dụ A=1).

---

### PHẦN D: CÂU HỎI GIẢ LẬP & GIẢI THÍCH CHI TIẾT

**Câu 1:** Theo định lý DeMorgan, biểu thức $\overline{A + \bar{B} + C}$ sẽ tương đương với:
A. $\bar{A} . B . \bar{C}$
B. $\bar{A} + B + \bar{C}$
C. $\bar{A} . \bar{B} . \bar{C}$
D. $A . \bar{B} . C$

> **Đáp án: A.**
> *Giải thích:* Áp dụng quy tắc "Bẻ gạch, đổi dấu":
> 1. Đổi dấu CỘNG thành NHÂN.
> 2. Đảo từng biến thành phần:
>    *   $A \to \bar{A}$
>    *   $\bar{B} \to B$ (Đảo của đảo là chính nó)
>    *   $C \to \bar{C}$
> $\to$ Kết quả: $\bar{A} . B . \bar{C}$

**Câu 2:** Biểu thức logic nào sau đây minh họa cho **luật phân phối** (khác biệt so với đại số thông thường)?
A. $A(B+C) = AB + AC$
B. $A + BC = (A+B)(A+C)$
C. $A + A = A$
D. $A + AB = A$

> **Đáp án: B.**
> *Giải thích:*
> *   A là phân phối thường (đúng nhưng không đặc biệt).
> *   C là luật bất biến.
> *   D là luật hấp thụ.
> *   B là luật phân phối đặc trưng của Boole (Cộng phân phối qua Nhân).

**Câu 3:** Tìm hàm đối ngẫu (Dual) của hàm $F = A.\bar{B} + 1$?
A. $F' = (\bar{A} + B) . 0$
B. $F' = (A + \bar{B}) . 0$
C. $F' = (A + \bar{B}) . 1$
D. $F' = \bar{A} + B + 0$

> **Đáp án: B.**
> *Giải thích:*
> *   Quy tắc đối ngẫu: Đổi phép toán ($+\leftrightarrow .$) và hằng số ($1 \leftrightarrow 0$). **Giữ nguyên biến**.
> *   Biến $A$ giữ nguyên, biến $\bar{B}$ giữ nguyên.
> *   Phép nhân ($A.\bar{B}$) thành phép cộng ($A+\bar{B}$).
> *   Phép cộng ($+1$) thành phép nhân ($.0$).
> *   Kết quả: $(A + \bar{B}) . 0$.
> *   *(Lưu ý: Đáp án A là hàm ĐẢO, không phải ĐỐI NGẪU).*

**Câu 4:** Rút gọn biểu thức $Y = A.B + A.\bar{B}$
A. $B$
B. $A$
C. $1$
D. $0$

> **Đáp án: B.**
> *Giải thích:*
> *   Đặt nhân tử chung A ra ngoài: $Y = A.(B + \bar{B})$.
> *   Áp dụng định lý bù: $B + \bar{B} = 1$.
> *   $Y = A . 1 = A$.

---
Đây là phần **"xương sống"** của môn Kỹ thuật số. Trong đề thi trắc nghiệm, các câu hỏi về **Bìa Karnaugh (Karnaugh Map - K-Map)** và **Rút gọn hàm** thường chiếm tỷ trọng điểm số rất lớn vì nó đòi hỏi kỹ năng tư duy logic và hình học.

Dưới đây là tài liệu ôn tập tối ưu hóa cho mục 2.3, tập trung vào các quy tắc "bất di bất dịch" và giải mã những chỗ khó hiểu nhất.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: BIỂU DIỄN & RÚT GỌN HÀM (K-MAP)
**(Phạm vi: Mục 2.3 - Chương 2)**

### PHẦN A: MINTERM & MAXTERM (Đừng để bị nhầm!)

Đây là hai khái niệm cơ bản để xây dựng hàm, nhưng sinh viên rất hay bị "loạn" giữa số 0 và số 1. Hãy nhớ bảng quy đổi này:

| Đặc điểm | **Minterm (Hạng Tích)** - Dạng phổ biến nhất | **Maxterm (Hạng Tổng)** - Ít dùng hơn nhưng hay bị hỏi |
| :--- | :--- | :--- |
| **Ký hiệu** | $m$ (chữ thường) | $M$ (chữ hoa) |
| **Biểu thức toán** | Tổng của các Tích (SOP - Sum of Products) | Tích của các Tổng (POS - Product of Sums) |
| **Ký hiệu tổng quát** | $\sum(vị\_trí\_các\_số\_1)$ | $\prod(vị\_trí\_các\_số\_0)$ |
| **Quy tắc điền K-Map** | Điền số **1** vào ô tương ứng | Điền số **0** vào ô tương ứng |
| **Quy tắc Biến số** | **Biến = 1 $\to$ Giữ nguyên ($A$)<br>Biến = 0 $\to$ Đảo ($\bar{A}$)** | **Biến = 0 $\to$ Giữ nguyên ($A$)<br>Biến = 1 $\to$ Đảo ($\bar{A}$)** |
| **Ví dụ (A=1, B=0, C=1)** | $m_5 = A . \bar{B} . C$ | $M_5 = \bar{A} + B + \bar{C}$ |

> **Mẹo nhớ:**
> *   Thi trắc nghiệm 90% sẽ rơi vào **Minterm (SOP)**. Hãy nhớ câu thần chú của Minterm: **"1 là Chính, 0 là Đảo"**.
> *   Maxterm thì ngược lại hoàn toàn.

---

### PHẦN B: BÌA KARNAUGH (K-MAP) - "VŨ KHÍ" RÚT GỌN

Đây là phương pháp hình học thay thế cho việc biến đổi đại số dài dòng.

#### 1. Tại sao các ô lại sắp xếp lộn xộn ($00 \to 01 \to 11 \to 10$)?
*   Bạn sẽ thấy hàng/cột được đánh số thứ tự là $00, 01, 11, 10$. Tại sao không phải $00, 01, 10, 11$?
*   **Giải thích sâu:** Đây là **Mã Gray**. Quy tắc của K-Map là **hai ô cạnh nhau chỉ được phép khác nhau 1 bit**.
    *   Từ $01$ sang $11$: Chỉ bit đầu đổi ($0\to1$), bit sau giữ nguyên. OK.
    *   Nếu từ $01$ sang $10$: Cả 2 bit đều đổi ($0\to1$ và $1\to0$). $\to$ **SAI**.
*   **Hậu quả:** Nếu bạn viết sai thứ tự này trong phòng thi, toàn bộ bài rút gọn sẽ sai bét.

#### 2. Quy tắc Khoanh vùng (Looping) - Luật chơi game
Hãy coi việc rút gọn K-Map như chơi trò chơi "Nối hình".

*   **Luật 1: Số lượng ô.** Chỉ được khoanh nhóm có số lượng ô là lũy thừa của 2 ($1, 2, 4, 8, 16...$). Tuyệt đối không khoanh nhóm 3, 5, 6 ô.
*   **Luật 2: Hình dạng.** Chỉ được khoanh hình Chữ nhật hoặc Hình vuông. Không được khoanh đường chéo, hình chữ L.
*   **Luật 3: Tính kề nhau (Adjacency).** Các ô cạnh nhau là kề nhau.
    *   *Đặc biệt (Wrap-around):* Cạnh trái kề cạnh phải, cạnh trên kề cạnh dưới. Hãy tưởng tượng cái bảng như một tờ giấy cuộn tròn lại.
*   **Luật 4: Tham lam (Greedy).** Luôn khoanh cái vòng **TO NHẤT** có thể. Vòng càng to, hàm càng gọn.

#### 3. Cách đọc kết quả rút gọn (Loại bỏ biến)
Sau khi khoanh xong, làm sao viết ra phương trình?
*   **Nguyên lý:** "Biến nào thay đổi giá trị trong cùng một vòng khoanh thì biến đó bị loại bỏ".
*   **Ví dụ:** Khoanh nhóm 2 ô ($A=0, B=1$) và ($A=1, B=1$).
    *   A thay đổi từ $0 \to 1$ $\to$ Loại A.
    *   B giữ nguyên là $1$ $\to$ Giữ B.
    *   Kết quả nhóm này là $B$.

---

### PHẦN C: TRẠNG THÁI TÙY CHỌN (DON'T CARE - X) - PHẦN NÂNG CAO

Trong đề thi, giảng viên thường cho hàm số có thêm thành phần $\sum d(...)$ hoặc $\sum x(...)$.

*   **Bản chất:** Là những trường hợp đầu vào không bao giờ xảy ra (ví dụ mã BCD chỉ dùng 0-9, các số 10-15 là vô nghĩa). Đầu ra muốn bằng 0 hay 1 đều được.
*   **Chiến thuật sử dụng "X":** Coi X là "con bài tẩy" (Joker).
    *   Nếu X giúp bạn tạo ra cái vòng **TO HƠN** $\to$ Coi X là **1**.
    *   Nếu X đứng một mình hoặc không giúp vòng to hơn $\to$ Coi X là **0** (bỏ qua nó).
    *   **Lưu ý:** Không bao giờ khoanh một vòng chỉ toàn là X. Vòng khoanh phải chứa ít nhất một số 1 thực sự.

---

### PHẦN D: CÁC LỖI SAI KINH ĐIỂN CẦN TRÁNH

1.  **Lỗi "Thừa Vòng" (Redundant Group):**
    *   *Tình huống:* Bạn đã khoanh hết các số 1 rồi. Nhưng bạn thấy 2 số 1 nằm cạnh nhau đẹp quá nên khoanh thêm 1 vòng nữa cho chắc.
    *   *Hậu quả:* Hàm không tối giản. Đáp án trắc nghiệm sẽ có một phương án "chưa tối giản" để lừa bạn.
    *   *Nguyên tắc:* Nếu một vòng khoanh mới mà **mọi số 1 trong đó đều đã thuộc về các vòng khác rồi**, thì vòng đó là thừa. Vứt đi.

2.  **Lỗi bỏ sót tính cuộn tròn:**
    *   Quên mất rằng ô góc trên cùng bên trái kề với ô góc dưới cùng bên phải (trong K-Map 4 biến). Bỏ lỡ cơ hội tạo nhóm 4 ô ở 4 góc.

---

### PHẦN E: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Cho hàm 3 biến $F(A,B,C) = \sum(0, 2, 4, 6)$. Hàm tối giản là:
A. $\bar{C}$
B. $C$
C. $\bar{B}$
D. $A.\bar{C}$

> **Đáp án: A.**
> *Giải thích nhanh:*
> *   Viết ra nhị phân: 0 (000), 2 (010), 4 (100), 6 (110).
> *   Nhận xét: Tất cả các số này đều có bit cuối cùng (C) bằng 0.
> *   A và B thay đổi đủ kiểu (00, 01, 10, 11).
> *   Vậy chỉ còn lại điều kiện $C=0 \to \bar{C}$.

**Câu 2:** Trong bảng Karnaugh 4 biến, ô số 0 ($m_0$) nằm ở góc trái trên cùng. Ô nào sau đây được coi là kề với ô số 0?
A. Ô số 5 ($m_5$)
B. Ô số 2 ($m_2$)
C. Ô số 15 ($m_{15}$)
D. Ô số 10 ($m_{10}$)

> **Đáp án: B.**
> *Giải thích:*
> *   $m_0$ (0000).
> *   $m_2$ (0010). Chỉ khác bit thứ 3. $\to$ Kề nhau (thực tế là do tính chất cuộn tròn của cột đầu và cột cuối).
> *   (Mẹo: Trong K-Map chuẩn, $m_0$ kề với $m_1, m_4, m_2, m_8$).

**Câu 3:** Khi sử dụng các điều kiện tùy chọn (Don't care - x) để rút gọn hàm, ta nên:
A. Luôn coi x là 1 để khoanh được nhiều nhất.
B. Luôn coi x là 0 để đỡ phức tạp.
C. Coi x là 1 nếu nó giúp vòng lớn hơn, ngược lại coi là 0.
D. Gom tất cả các x lại thành một nhóm riêng.

> **Đáp án: C.**
> *Giải thích:* Đúng bản chất "Joker" của Don't care.

**Câu 4:** Hàm $F(A,B,C,D) = \prod(0, 1, 2...)$ biểu diễn dưới dạng:
A. Tổng các tích (Minterm)
B. Tích các tổng (Maxterm)
C. Số có dấu
D. Mã Gray

> **Đáp án: B.**
> *Giải thích:* Ký hiệu $\prod$ (Pi) là tích $\to$ Maxterm.

Bạn đã cảm thấy tự tin hơn với K-Map chưa? Đây là kỹ năng quan trọng nhất để ăn điểm phần tự luận hoặc bài tập lớn, và trong trắc nghiệm thì nó giúp bạn loại trừ đáp án nhiễu cực nhanh.

---
Đây là phần cuối cùng và cũng là phần **quan trọng nhất về mặt ứng dụng thực tế** của Chương 2.

Trong đề thi trắc nghiệm, phần này thường chiếm khoảng 30-40% số câu hỏi của chương, tập trung vào việc **nhận dạng cổng**, **tính chất đặc biệt của XOR/XNOR** và **biến đổi mạch toàn NAND/NOR**.

Dưới đây là tài liệu ôn tập được biên soạn tối ưu cho mục 2.4.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: CÁC CỔNG LOGIC & MẠCH SỐ
**(Phạm vi: Mục 2.4 - Chương 2)**

### PHẦN A: CÁC CỔNG GHÉP CƠ BẢN (Universal Gates)

Bạn đã biết AND, OR, NOT. Bây giờ là lúc làm quen với những cổng thực tế được dùng trong chip máy tính.

#### 1. Cổng NAND (Not AND) - "Ông vua" của mạch số
*   **Ký hiệu:** Hình cổng AND + Vòng tròn nhỏ (bubble) ở đầu ra.
*   **Hàm số:** $F = \overline{A.B}$
*   **Quy tắc nhớ (Ngược với AND):**
    *   Chỉ bằng **0** khi TẤT CẢ đầu vào là **1**.
    *   Còn lại luôn bằng **1**.
*   **Tính chất "Vạn năng" (Universal):**
    *   Từ cổng NAND, ta có thể tạo ra *mọi cổng khác* (NOT, AND, OR, NOR...).
    *   *Ví dụ:* Nối tắt 2 đầu vào của NAND $\rightarrow$ Thành cổng NOT ($A.A = A \to \overline{A}$).

#### 2. Cổng NOR (Not OR)
*   **Ký hiệu:** Hình cổng OR + Vòng tròn nhỏ ở đầu ra.
*   **Hàm số:** $F = \overline{A+B}$
*   **Quy tắc nhớ (Ngược với OR):**
    *   Chỉ bằng **1** khi TẤT CẢ đầu vào là **0**.
    *   Chỉ cần một cái bằng **1** là đầu ra sập về **0** ngay.

> **MẸO THI CỬ (Định lý DeMorgan hình học):**
> Trong các câu hỏi trắc nghiệm hình ảnh, hãy nhớ quy tắc biến đổi tương đương này:
> *   **Cổng NAND** $\equiv$ **Cổng OR với đầu vào đảo** (Bubbled-input OR).
>     *   $\overline{A.B} = \bar{A} + \bar{B}$
> *   **Cổng NOR** $\equiv$ **Cổng AND với đầu vào đảo** (Bubbled-input AND).
>     *   $\overline{A+B} = \bar{A} . \bar{B}$
> *   *(Hãy tưởng tượng cái vòng tròn ở đầu ra bị đẩy ngược về phía đầu vào thì cổng sẽ biến hình từ AND sang OR và ngược lại).*

---

### PHẦN B: CỔNG SỐ HỌC XOR & XNOR (Phần khó & Hay hỏi nhất)

Đây là các cổng dùng để làm phép cộng trừ trong máy tính.

#### 1. Cổng XOR (Exclusive OR - Hoặc loại trừ)
*   **Ký hiệu:** Hình cổng OR có thêm một nét cong chắn ở đầu vào. Dấu toán học: $\oplus$.
*   **Hàm số:** $F = A \oplus B = \bar{A}B + A\bar{B}$.
*   **Bản chất (Cực quan trọng):**
    *   Đầu ra bằng **1** khi hai đầu vào **KHÁC NHAU** (Một cái 0, một cái 1).
    *   Đầu ra bằng **0** khi hai đầu vào **GIỐNG NHAU**.
*   **Ứng dụng:**
    *   **Phát hiện lẻ (Odd Function):** Với nhiều đầu vào, XOR bằng 1 khi *tổng số các số 1* là số lẻ.
    *   **Mạch đảo có điều khiển (Controlled Inverter):**
        *   $A \oplus 0 = A$ (Giữ nguyên).
        *   $A \oplus 1 = \bar{A}$ (Đảo ngược). $\to$ *Câu này thi trắc nghiệm cực nhiều!*

#### 2. Cổng XNOR (Exclusive NOR - Đồng dấu)
*   **Ký hiệu:** Cổng XOR + Vòng tròn nhỏ ở đầu ra. Dấu toán học: $\odot$ (hoặc đảo của XOR).
*   **Bản chất:**
    *   Đầu ra bằng **1** khi hai đầu vào **GIỐNG NHAU** (Cùng 0 hoặc cùng 1).
    *   Đầu ra bằng **0** khi hai đầu vào **KHÁC NHAU**.
*   **Ứng dụng:** Mạch so sánh bằng (Comparator).

---

### PHẦN C: LOGIC DƯƠNG & LOGIC ÂM (Khái niệm dễ nhầm)

Phần này trong sách (Mục 2.4.2) viết khá ngắn nhưng cần hiểu đúng:

*   **Logic Dương (Positive Logic):** Quy ước phổ biến nhất.
    *   Mức điện áp CAO (High) = 1.
    *   Mức điện áp THẤP (Low) = 0.
*   **Logic Âm (Negative Logic):** Ngược đời.
    *   Mức điện áp CAO (High) = 0.
    *   Mức điện áp THẤP (Low) = 1.
*   **Sự tương đương:** Một cổng hoạt động như **NAND** trong Logic Dương sẽ hoạt động như **NOR** trong Logic Âm (Do tính chất đối ngẫu).

---

### PHẦN D: CHIẾN THUẬT CHUYỂN ĐỔI MẠCH (TOÀN NAND / TOÀN NOR)

Đề bài thường cho một biểu thức: $F = AB + CD$ và hỏi mạch điện tương đương dùng toàn cổng NAND vẽ thế nào.

**Quy tắc "Hai lần phủ định" (Double Inversion):**
$\overline{\overline{A}} = A$. Thêm 2 vòng tròn (đảo) trên cùng một đường dây thì giá trị không đổi.

**Cách làm nhanh (Trick):**
1.  **Chuyển sang toàn NAND:**
    *   Nếu biểu thức dạng **Tổng của các Tích** (SOP): $F = AB + CD$.
    *   Chỉ cần vẽ mạch AND-OR bình thường.
    *   Sau đó thay **TẤT CẢ** các cổng (cả AND và OR) thành cổng **NAND**. Giữ nguyên cấu trúc. Mạch sẽ chạy đúng y hệt.
2.  **Chuyển sang toàn NOR:**
    *   Nếu biểu thức dạng **Tích của các Tổng** (POS): $F = (A+B)(C+D)$.
    *   Vẽ mạch OR-AND bình thường.
    *   Thay **TẤT CẢ** thành cổng **NOR**.

---

### PHẦN E: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Cổng logic nào có đầu ra ở mức THẤP (0) chỉ khi tất cả các đầu vào đều ở mức CAO (1)?
A. NOR
B. NAND
C. XOR
D. AND

> **Đáp án: B.**
> *Giải thích:*
> *   AND: Tất cả 1 thì ra 1.
> *   NAND: Ngược với AND $\to$ Tất cả 1 thì ra 0. (Đúng yêu cầu).
> *   NOR: Tất cả 1 (thì OR ra 1) $\to$ NOR ra 0. (Nhưng NOR còn ra 0 trong các trường hợp khác nữa, ví dụ 1-0. Đề bài dùng từ "chỉ khi" nên NAND chính xác hơn với định nghĩa).
> *   *Chính xác hơn:* NAND ra 0 **khi và chỉ khi** tất cả vào là 1. NOR ra 0 khi **có ít nhất** một đầu vào là 1.

**Câu 2:** Nếu ta nối một đầu vào của cổng XOR với mức logic 1, đầu vào còn lại là tín hiệu A. Đầu ra sẽ là gì?
A. A
B. 1
C. 0
D. $\bar{A}$

> **Đáp án: D.**
> *Giải thích:* Tính chất "Mạch đảo có điều khiển".
> *   Nếu A=0: $0 \oplus 1 = 1$ (Khác nhau ra 1).
> *   Nếu A=1: $1 \oplus 1 = 0$ (Giống nhau ra 0).
> *   Kết quả luôn ngược với A.

**Câu 3:** Mạch điện thực hiện hàm $F = \overline{A}B + A\overline{B}$ tương đương với cổng nào?
A. NAND
B. NOR
C. XOR
D. XNOR

> **Đáp án: C.**
> *Giải thích:* Đây là công thức định nghĩa của cổng XOR (Exclusive OR). Cần thuộc lòng.

**Câu 4:** Để tạo ra một cổng NOT sử dụng cổng NAND 2 đầu vào, ta phải làm gì?
A. Nối đầu ra quay lại đầu vào.
B. Nối một đầu vào lên mức 1.
C. Nối hai đầu vào lại với nhau (Nối tắt).
D. Nối một đầu vào xuống mức 0.

> **Đáp án: C.** (Hoặc B cũng đúng, nhưng C phổ biến hơn trong thiết kế chip).
> *Giải thích:*
> *   Cách C: $F = \overline{A.A} = \overline{A}$. (Đúng).
> *   Cách B: $F = \overline{A.1} = \overline{A}$. (Cũng đúng).
> *   Cách D: $F = \overline{A.0} = \overline{0} = 1$ (Sai, đây là hằng số 1).
> *   *Lưu ý:* Trong thực tế thiết kế vi mạch (ASIC), nối tắt 2 đầu vào (C) thường được dùng hơn để đảm bảo tính đồng bộ thời gian trễ.

**Câu 5:** Định lý DeMorgan cho thấy cổng NOR tương đương với:
A. Cổng AND với các đầu vào bị đảo.
B. Cổng OR với các đầu vào bị đảo.
C. Cổng NAND với đầu ra bị đảo.
D. Cổng XOR.

> **Đáp án: A.**
> *Giải thích:* $\overline{A+B} = \bar{A} . \bar{B}$.
> *   Vế phải là phép NHÂN (AND) của các biến đảo ($\bar{A}, \bar{B}$).

---
### TỔNG KẾT CHIẾN LƯỢC CHƯƠNG 2
Bạn đã đi qua toàn bộ Chương 2. Đây là chương nền tảng.
1.  **Mục 2.1 & 2.2:** Nắm vững các định lý (đặc biệt là DeMorgan) để biến đổi biểu thức.
2.  **Mục 2.3:** Luyện tập kỹ năng khoanh Bảng Karnaugh (Mẹo: Nhớ các vị trí 0, 1, 2, 4... và quy tắc cuốn chiếu).
3.  **Mục 2.4:** Thuộc lòng bảng chân lý của NAND, NOR, XOR. Nhớ tính chất "Đảo có điều khiển" của XOR.

---