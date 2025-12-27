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

Chào bạn, chúng ta bắt đầu vào **Chương 3: Mạch Logic Tổ Hợp**. Đây là chương "xương sống" của môn học vì nó chuyển hóa các cổng logic rời rạc (Chương 2) thành các hệ thống có chức năng cụ thể.

Mục 3.1 - 3.3 là phần nền tảng về tư duy thiết kế. Trong thi trắc nghiệm, phần này thường không hỏi tính toán quá phức tạp nhưng lại hay đánh lừa về **định nghĩa** và **quy trình**.

Dưới đây là tài liệu ôn tập tối ưu.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: TỔNG QUAN & THIẾT KẾ MẠCH TỔ HỢP
**(Phạm vi: Mục 3.1, 3.2, 3.3 - Chương 3)**

### PHẦN A: KHÁI NIỆM "BẤT DI BẤT DỊCH" (Mục 3.1)

Câu hỏi lý thuyết thường xoay quanh việc phân biệt giữa **Mạch Tổ Hợp (Combinational)** và **Mạch Tuần Tự (Sequential - Chương 4)**.

| Đặc điểm | **Mạch Tổ Hợp (Chương 3)** | Mạch Tuần Tự (Chương 4 - Để so sánh) |
| :--- | :--- | :--- |
| **Định nghĩa** | Đầu ra chỉ phụ thuộc vào đầu vào **HIỆN TẠI**. | Đầu ra phụ thuộc vào đầu vào hiện tại + **QUÁ KHỨ** (Trạng thái cũ). |
| **Bộ nhớ** | **KHÔNG** có bộ nhớ (No Memory). | **CÓ** bộ nhớ (Memory/Flip-flop). |
| **Yếu tố thời gian** | Không phụ thuộc vào "lịch sử" trước đó. | Phụ thuộc vào lịch sử/xung nhịp (Clock). |
| **Cấu trúc** | Chỉ gồm các cổng logic (AND, OR, NOT...). | Cổng logic + Phần tử nhớ. |
| **Ví dụ** | Bộ cộng, Bộ giải mã, Bộ so sánh. | Bộ đếm, Thanh ghi, RAM. |

> **Mẹo nhớ:** Mạch tổ hợp giống như cái máy tính bỏ túi cơ bản: Bạn nhập 1+1, nó ra 2. Nó không quan tâm hôm qua bạn đã tính cái gì.

---

### PHẦN B: QUY TRÌNH PHÂN TÍCH & THIẾT KẾ (Mục 3.2 & 3.3)

#### 1. Phân tích mạch (Analysis)
*   **Mục tiêu:** Cho sơ đồ mạch $\rightarrow$ Tìm ra chức năng (Hàm F).
*   **Quy trình:** Sơ đồ $\rightarrow$ Biểu thức Logic $\rightarrow$ Rút gọn $\rightarrow$ Bảng chân lý.
*   **Mẹo thi trắc nghiệm:**
    *   Khi đề bài cho một hình vẽ rối rắm và hỏi hàm F, đừng hoảng. Hãy viết hàm cho từng cổng từ trái sang phải.
    *   Áp dụng DeMorgan ngay trên hình vẽ nếu gặp các cổng NAND/NOR nối tiếp nhau.

#### 2. Thiết kế mạch (Design)
*   **Mục tiêu:** Cho yêu cầu bài toán (Lời văn) $\rightarrow$ Vẽ sơ đồ mạch.
*   **Quy trình 4 bước chuẩn:**
    1.  **Phân tích:** Xác định số đầu vào, đầu ra.
    2.  **Bảng trạng thái:** Liệt kê tất cả trường hợp (0/1).
    3.  **Tối thiểu hóa:** Dùng Bìa Karnaugh (để mạch đơn giản nhất, tiết kiệm tiền nhất).
    4.  **Vẽ mạch:** Dùng cổng logic.

---

### PHẦN C: CÁC VẤN ĐỀ KHÓ & CHUYÊN SÂU (Giải thích kỹ)

Phần này giảng viên rất thích ra đề để phân loại sinh viên giỏi, đặc biệt là bài toán "Cầu thang" và "Chuyển đổi mạch".

#### 1. Bài toán Công tắc cầu thang (Ví dụ kinh điển trong sách)
*   **Đề bài:** Một đèn ở cầu thang được điều khiển bởi 2 công tắc (tầng 1 và tầng 2). Tác động vào bất kỳ công tắc nào cũng làm thay đổi trạng thái đèn (đang tắt thành bật, đang bật thành tắt).
*   **Phân tích Logic:**
    *   Gọi 2 công tắc là A và B. Đèn là F.
    *   Nếu 2 công tắc cùng vị trí (ví dụ cùng gạt lên: 1-1, hoặc cùng gạt xuống: 0-0) $\rightarrow$ Đèn TẮT (0).
    *   Nếu 2 công tắc khác vị trí (một lên, một xuống: 0-1 hoặc 1-0) $\rightarrow$ Đèn SÁNG (1).
*   **Kết luận:** Đây chính là **Cổng XOR** ($F = A \oplus B$).
*   *Câu hỏi thi:* "Mạch logic nào thực hiện chức năng điều khiển đèn cầu thang?" $\rightarrow$ Chọn **XOR**.

#### 2. Kỹ thuật chuyển đổi về "Toàn NAND" hoặc "Toàn NOR"
Tại sao phải làm việc này? Vì trong thực tế sản xuất chip (IC), việc chỉ dùng một loại cổng (như NAND 7400) rẻ và dễ chế tạo hơn là dùng lẫn lộn AND/OR/NOT.

**a) Quy tắc chuyển mạch AND-OR sang Toàn NAND:**
*   Hàm dạng tổng các tích (SOP): Ví dụ $F = AB + CD$.
*   *Bước 1:* Vẽ mạch gốc (2 cổng AND nối vào 1 cổng OR).
*   *Bước 2:* Thay **TẤT CẢ** các cổng đó bằng cổng **NAND**.
*   *Tại sao đúng?*
    *   $F = AB + CD$.
    *   Thêm 2 dấu gạch đầu (đảo 2 lần): $F = \overline{\overline{AB + CD}}$.
    *   Áp dụng DeMorgan cho gạch dưới: $F = \overline{\overline{AB} . \overline{CD}}$.
    *   Phân tích: $\overline{AB}$ là cổng NAND. $\overline{CD}$ là cổng NAND. Và cả cụm lớn là một cổng NAND nữa.
*   **Kết luận:** Cấu trúc giữ nguyên, chỉ thay hình dạng cổng.

**b) Quy tắc chuyển mạch OR-AND sang Toàn NOR:**
*   Hàm dạng tích các tổng (POS): Ví dụ $F = (A+B)(C+D)$.
*   *Cách làm:* Thay **TẤT CẢ** cổng (OR và AND) thành cổng **NOR**. Cấu trúc giữ nguyên.

---

### PHẦN D: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Đặc điểm nào sau đây **KHÔNG** phải của mạch logic tổ hợp?
A. Trạng thái đầu ra phụ thuộc vào tổ hợp các biến đầu vào.
B. Mạch không có khả năng lưu trữ thông tin (không có bộ nhớ).
C. Trạng thái đầu ra phụ thuộc vào trạng thái trước đó của mạch.
D. Được cấu tạo từ các cổng logic cơ bản.

> **Đáp án: C.**
> *Giải thích:* Phụ thuộc vào trạng thái trước đó là đặc điểm của Mạch tuần tự (Chương 4). Mạch tổ hợp "không có ký ức".

**Câu 2:** Một mạch tổ hợp có 3 đầu vào (A, B, C) và 1 đầu ra (Y). Số lượng ô trong bảng Karnaugh cần thiết để tối thiểu hóa hàm này là bao nhiêu?
A. 4
B. 8
C. 16
D. 9

> **Đáp án: B.**
> *Giải thích:* Số ô = $2^n$ (với n là số biến đầu vào). $2^3 = 8$.

**Câu 3:** Hàm logic $F = AB + BC$ có thể được thực hiện hoàn toàn bằng loại cổng nào sau đây mà không thay đổi cấu trúc mạch (số lượng cổng và cách nối)?
A. NOR
B. XOR
C. NAND
D. NOT

> **Đáp án: C.**
> *Giải thích:* Hàm $F = AB + BC$ là dạng SOP (Tổng của các tích: AND rồi mới OR). Dạng này tương thích trực tiếp với cấu trúc toàn **NAND**. (Nếu là dạng $(A+B)(B+C)$ thì mới dùng toàn NOR).

**Câu 4:** Quy trình thiết kế mạch tổ hợp nào sau đây là đúng trình tự nhất?
A. Vẽ mạch -> Rút gọn -> Bảng trạng thái.
B. Bảng trạng thái -> Rút gọn (K-Map) -> Viết hàm -> Vẽ mạch.
C. Viết hàm -> Vẽ mạch -> Rút gọn.
D. Rút gọn -> Bảng trạng thái -> Vẽ mạch.

> **Đáp án: B.**
> *Giải thích:* Phải hiểu yêu cầu (Bảng trạng thái) trước, rồi mới tìm cách làm cho nó rẻ nhất (Rút gọn), cuối cùng mới thi công (Vẽ mạch).

**Câu 5:** Mạch logic kiểm tra tính chẵn lẻ (Parity) thuộc loại mạch nào?
A. Mạch tuần tự.
B. Mạch tổ hợp.
C. Mạch ghi nhớ.
D. Mạch dao động.

> **Đáp án: B.**
> *Giải thích:* Nó chỉ đếm số lượng bit 1 hiện có để báo chẵn/lẻ, không cần nhớ quá khứ $\rightarrow$ Mạch tổ hợp.

---

Đây là tài liệu ôn tập cho **Mục 3.4: Mạch Mã hóa và Giải mã**.

Trong thi trắc nghiệm, phần này có số lượng câu hỏi rất lớn vì nó liên quan đến các loại mã số (Code) và các IC thực tế. Ba "bẫy" lớn nhất ở đây là: **Nhầm lẫn giữa Mã hóa/Giải mã**, **Tính toán mã Gray**, và **Logic tích cực thấp của LED 7 đoạn**.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: MÃ HÓA & GIẢI MÃ
**(Phạm vi: Mục 3.4 - Chương 3)**

### PHẦN A: CÁC LOẠI MÃ SỐ (Codes) - Cần thuộc tính chất

Trước khi vào mạch, phải hiểu "ngôn ngữ" mà mạch xử lý.

#### 1. Mã BCD (Binary Coded Decimal)
Là cách dùng 4 bit nhị phân để biểu diễn **1 chữ số thập phân** (0-9).
*   **BCD 8421 (Mã tự nhiên):** Phổ biến nhất. Tính tổng trọng số như nhị phân thường ($8, 4, 2, 1$).
    *   *Lưu ý:* Các tổ hợp từ **1010 đến 1111** (10-15) là **Dư thừa (Forbidden/Invalid)**.
*   **BCD 2421 (Mã Aiken):** Trọng số là 2-4-2-1.
    *   *Đặc điểm:* Có tính đối xứng (Bù 9). Dùng để thực hiện phép trừ dễ dàng hơn.
*   **Mã Dư-3 (Excess-3):** Lấy mã BCD 8421 cộng thêm 3 ($0011_2$).
    *   *Đặc điểm:* Không có trọng số. Cũng có tính đối xứng. Không bao giờ có trường hợp toàn số 0 ($0000$), giúp phát hiện lỗi mất tín hiệu.

#### 2. Mã Gray (Mã cách 1) - **Cực quan trọng**
*   **Định nghĩa:** Hai từ mã kế tiếp nhau chỉ khác nhau đúng **1 bit**.
*   **Tính chất:** **Không có trọng số**.
*   **Ứng dụng:** Dùng trong cảm biến vị trí, mã hóa góc quay (để tránh sai số khi chuyển trạng thái).

---

### PHẦN B: MẠCH MÃ HÓA (ENCODER)

Hãy nhớ quy tắc: **ENCODER = NÉN LẠI** (Nhiều vào $\to$ Ít ra).

#### 1. Nguyên lý
*   **Chức năng:** Chuyển đổi tín hiệu con người hiểu (Thập phân, Phím bấm) sang ngôn ngữ máy (Nhị phân, BCD).
*   **Tỷ lệ:** $2^n$ đầu vào $\to$ $n$ đầu ra. (Ví dụ: 8 vào $\to$ 3 ra; 10 vào $\to$ 4 ra).

#### 2. Mạch Mã hóa Ưu tiên (Priority Encoder) - Phần Khó
Mạch mã hóa thường sẽ bị lỗi nếu bạn ấn 2 phím cùng lúc. Mạch ưu tiên giải quyết việc này.

*   **Cơ chế:** Nếu có nhiều đầu vào cùng kích hoạt (mức 1), mạch sẽ chỉ mã hóa đầu vào có **độ ưu tiên cao nhất** (thường là số lớn nhất).
*   **Ví dụ (Mã hóa thập phân sang BCD):**
    *   Bạn ấn phím 5 và phím 9 cùng lúc.
    *   Mạch thông thường: Sẽ ra kết quả sai (loạn xạ).
    *   Mạch ưu tiên: Sẽ bỏ qua số 5, chỉ mã hóa số 9 $\to$ Đầu ra là $1001$.
*   **Bảng chân lý (Vết tích "X"):** Trong bảng trạng thái, các ô ghi chữ **X (Don't care)** ở các dòng dưới thể hiện rằng: "Khi số lớn đã được ấn, thì các số nhỏ hơn bằng 0 hay 1 đều không quan trọng".

---

### PHẦN C: MẠCH GIẢI MÃ (DECODER)

Hãy nhớ quy tắc: **DECODER = BUNG RA** (Ít vào $\to$ Nhiều ra).

#### 1. Nguyên lý
*   **Chức năng:** Chuyển từ mã máy (Nhị phân) sang tín hiệu điều khiển cụ thể (Chọn địa chỉ, Bật đèn LED).
*   **Tỷ lệ:** $n$ đầu vào $\to$ $2^n$ đầu ra. (Ví dụ: 3 vào $\to$ 8 ra; 4 vào $\to$ 16 ra).

#### 2. Tín hiệu cho phép (Enable - E hoặc G)
Hầu hết IC giải mã đều có chân Enable.
*   Nếu chân này không được kích hoạt đúng mức $\to$ IC "ngủ đông" (Tất cả đầu ra đều tắt), bất chấp đầu vào là gì.
*   Dùng để ghép nhiều IC nhỏ thành IC lớn (Ví dụ: Ghép 2 con "3 sang 8" thành 1 con "4 sang 16").

#### 3. Mạch giải mã LED 7 đoạn (Phần thi hay hỏi nhất)
Biến mã BCD (4 bit) thành tín hiệu điều khiển 7 thanh LED (a, b, c, d, e, f, g) để hiện số.

*   **Phân loại LED:**
    *   **Anốt chung (Common Anode):** Chân dương nối chung lên nguồn ($+5V$). Muốn đèn sáng phải cấp **0** (Mức thấp). $\to$ IC giải mã phải có đầu ra **tích cực THẤP**.
    *   **Catốt chung (Common Cathode):** Chân âm nối chung xuống đất ($GND$). Muốn đèn sáng phải cấp **1** (Mức cao). $\to$ IC giải mã phải có đầu ra **tích cực CAO**.
*   **Chân chức năng đặc biệt (RBI, RBO - Ripple Blanking):**
    *   Dùng để **xóa số 0 vô nghĩa** (Leading Zero Suppression).
    *   *Ví dụ:* Số thực là `007`. Nếu không xóa sẽ hiện `007`. Nếu dùng RBI/RBO, mạch sẽ tự tắt 2 số 0 đầu, chỉ hiện `7`.

---

### PHẦN D: CÔNG THỨC CHUYỂN ĐỔI GRAY $\leftrightarrow$ NHỊ PHÂN

Đây là phần bài tập tính toán "gỡ điểm", nhưng rất dễ nhầm lẫn cách cộng. Phép tính sử dụng là **XOR** (Giống nhau bằng 0, Khác nhau bằng 1).

#### 1. Nhị phân sang Gray (Binary to Gray)
*   **Quy tắc:** "Giữ đầu, Cộng kế".
    *   Bit đầu (MSB): Giữ nguyên.
    *   Các bit sau: Lấy bit nhị phân tại vị trí đó **XOR** với bit nhị phân **đứng ngay trước nó**.
    *   $G_i = B_i \oplus B_{i+1}$
*   **Ví dụ:** Đổi $1101_2$ sang Gray.
    1.  Hạ 1 xuống $\to$ 1
    2.  $1 \oplus 1 = 0$
    3.  $1 \oplus 0 = 1$
    4.  $0 \oplus 1 = 1$
    *   Kết quả: **1011**.

#### 2. Gray sang Nhị phân (Gray to Binary)
*   **Quy tắc:** "Giữ đầu, Chéo xuống".
    *   Bit đầu (MSB): Giữ nguyên.
    *   Các bit sau: Lấy kết quả nhị phân vừa tìm được **XOR** với bit Gray tiếp theo.
    *   $B_i = B_{i+1} \oplus G_i$
*   **Ví dụ:** Đổi Gray **1011** về Nhị phân.
    1.  Hạ 1 xuống $\to$ **1** (Bit B3)
    2.  Lấy **1** (B3) $\oplus$ 0 (G2) $\to$ **1** (Bit B2)
    3.  Lấy **1** (B2) $\oplus$ 1 (G1) $\to$ **0** (Bit B1)
    4.  Lấy **0** (B1) $\oplus$ 1 (G0) $\to$ **1** (Bit B0)
    *   Kết quả: **1101**.

---

### PHẦN E: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Mạch nào sau đây có chức năng chuyển đổi thông tin từ $2^n$ đường vào thành mã nhị phân $n$ bit ở đầu ra?
A. Bộ giải mã (Decoder)
B. Bộ mã hóa (Encoder)
C. Bộ hợp kênh (Multiplexer)
D. Bộ so sánh (Comparator)

> **Đáp án: B.**
> *Giải thích:* $2^n \to n$ là NÉN lại $\to$ Encoder.

**Câu 2:** Ưu điểm chính của mã Gray so với mã nhị phân truyền thống là gì?
A. Dễ thực hiện phép tính cộng trừ.
B. Có trọng số xác định (8421).
C. Hai từ mã kế tiếp chỉ khác nhau 1 bit, giảm thiểu lỗi khi chuyển đổi.
D. Có khả năng phát hiện lỗi sai chẵn lẻ.

> **Đáp án: C.**
> *Giải thích:* Đây là định nghĩa cốt lõi của mã Gray.

**Câu 3:** Khi sử dụng LED 7 đoạn loại **Anốt chung (Common Anode)**, để làm sáng một đoạn LED, đầu ra của IC giải mã phải ở mức logic nào?
A. Mức cao (1)
B. Mức thấp (0)
C. Trạng thái trở kháng cao (Z)
D. Xung nhịp (Clock)

> **Đáp án: B.**
> *Giải thích:* Anốt chung là nối lên nguồn dương (+). Muốn có dòng điện chạy qua thì đầu kia phải nối đất (mức 0).

**Câu 4:** Chuyển đổi số nhị phân $B = 1010$ sang mã Gray.
A. 1111
B. 1100
C. 1011
D. 1110

> **Đáp án: A.**
> *Giải thích:*
> *   Bit đầu: 1.
> *   $1 \oplus 0 = 1$.
> *   $0 \oplus 1 = 1$.
> *   $1 \oplus 0 = 1$.
> *   Kết quả: 1111.

**Câu 5:** Trong mạch mã hóa ưu tiên (Priority Encoder) 10 đường (0-9), nếu cả đầu vào số 2 và số 8 đều ở mức tích cực, đầu ra sẽ là mã của số nào?
A. Số 2
B. Số 8
C. Số 10 (Tổng 2+8)
D. Không xác định (Lỗi)

> **Đáp án: B.**
> *Giải thích:* Mạch ưu tiên luôn chọn số lớn nhất (hoặc số có độ ưu tiên cao nhất được quy định).

---

Chào bạn, chúng ta sẽ đi vào **Mục 3.5: Bộ Hợp kênh (MUX) và Phân kênh (DMUX)**.

Đây là một trong những phần thú vị nhất và có tính ứng dụng cao nhất trong thiết kế mạch số. Trong đề thi trắc nghiệm, các câu hỏi về MUX thường chiếm tỷ trọng lớn vì nó có thể thay thế cho cả một bảng chân lý phức tạp.

Dưới đây là tài liệu ôn tập được thiết kế để bạn "nhìn là ra đáp án".

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: MUX & DMUX
**(Phạm vi: Mục 3.5 - Chương 3)**

### PHẦN A: BẢN CHẤT CỐT LÕI (Đừng nhầm lẫn)

Hãy tưởng tượng hệ thống đường ray tàu hỏa để nhớ hai khái niệm này:

| Đặc điểm | **Bộ Hợp kênh (MUX)** | **Bộ Phân kênh (DMUX)** |
| :--- | :--- | :--- |
| **Tên tiếng Anh** | Multiplexer / Data Selector | Demultiplexer / Data Distributor |
| **Biệt danh** | **"Bộ chọn dữ liệu"** | **"Bộ phân phối dữ liệu"** |
| **Mô hình** | **Nhiều vào $\to$ 1 ra** | **1 vào $\to$ Nhiều ra** |
| **Cấu trúc** | $2^n$ đầu vào dữ liệu<br>$n$ đầu vào điều khiển (Select)<br>1 đầu ra | 1 đầu vào dữ liệu<br>$n$ đầu vào điều khiển (Select)<br>$2^n$ đầu ra |
| **Hàm toán học** | $Y = \sum (D_i \cdot \text{Minterm}_i)$ | $Y_i = D \cdot \text{Minterm}_i$ |
| **Ứng dụng chính** | Chuyển Song song $\to$ Nối tiếp<br>Tạo hàm logic bất kỳ | Chuyển Nối tiếp $\to$ Song song<br>Giải mã địa chỉ |

> **Quy tắc số mũ:** Luôn nhớ mối quan hệ **$n$ và $2^n$**.
> *   Nếu có **3** dây điều khiển $\to$ Có **8** kênh ($2^3$).
> *   Nếu có **4** dây điều khiển $\to$ Có **16** kênh ($2^4$).

---

### PHẦN B: BỘ HỢP KÊNH (MUX) - TRỌNG TÂM THI CỬ

Giảng viên rất thích hỏi về MUX vì nó được ví như "IC vạn năng".

#### 1. Nguyên lý hoạt động
*   MUX giống như một cái **công tắc xoay**.
*   Các chân điều khiển (Select - A, B, C...) đóng vai trò là "người chỉnh công tắc".
*   Nếu mã điều khiển là `00` $\to$ Nối ngõ vào $D_0$ ra $Y$.
*   Nếu mã điều khiển là `11` $\to$ Nối ngõ vào $D_3$ ra $Y$.

#### 2. Thiết kế hàm Logic bằng MUX (Phần Khó & Hay hỏi nhất)
Thay vì dùng hàng tá cổng AND, OR, NOT để lắp mạch, ta có thể dùng **duy nhất 1 con MUX** để thực hiện mọi hàm logic.

**Dạng 1: Số đầu vào điều khiển = Số biến của hàm ($n$ biến dùng MUX $2^n \to 1$)**
*   *Cách làm:*
    1.  Viết bảng chân lý của hàm.
    2.  Nối các chân điều khiển của MUX vào các biến (A, B, C).
    3.  Nhìn bảng chân lý:
        *   Dòng nào hàm bằng **1** $\to$ Nối chân dữ liệu tương ứng lên nguồn ($+5V$).
        *   Dòng nào hàm bằng **0** $\to$ Nối chân dữ liệu tương ứng xuống đất ($GND$).
*   *Ví dụ:* Hàm $F(A,B) = \sum(0, 3)$. Dùng MUX 4-1.
    *   $m_0$ và $m_3$ bằng 1.
    *   Nối chân $D_0, D_3$ lên mức 1.
    *   Nối chân $D_1, D_2$ xuống mức 0.

**Dạng 2: Số đầu vào điều khiển < Số biến của hàm (Kỹ thuật gấp/Folding - Rất hay thi)**
*   *Đề bài:* Hàm 3 biến $F(A,B,C)$ nhưng bắt dùng MUX 4-1 (chỉ có 2 chân điều khiển) để thiết kế.
*   *Giải thích:*
    *   Ta dùng 2 biến cao (A, B) nối vào chân điều khiển (Select).
    *   Biến còn lại (C) sẽ được nối vào các chân dữ liệu ($D_0 \dots D_3$).
    *   Tại mỗi chân D, ta so sánh giá trị của hàm F với biến C:
        *   Nếu F luôn bằng 0 $\to$ Nối D vào 0.
        *   Nếu F luôn bằng 1 $\to$ Nối D vào 1.
        *   Nếu F giống hệt C $\to$ Nối D vào C.
        *   Nếu F ngược với C $\to$ Nối D vào $\bar{C}$.

#### 3. Mở rộng MUX (Cascading)
*   Làm sao để tạo ra MUX 8-1 từ các MUX 4-1?
*   **Cách làm:** Dùng 2 con MUX 4-1 nối song song.
    *   Đầu ra của 2 con này đi vào 1 cổng OR (hoặc 1 con MUX 2-1 khác).
    *   Chân điều khiển thứ 3 (bit cao nhất) dùng để chọn xem con MUX nào được hoạt động (thông qua chân Enable/Strobe).

---

### PHẦN C: BỘ PHÂN KÊNH (DMUX) & MỐI QUAN HỆ VỚI DECODER

Đây là một bí mật nhỏ: **DMUX và DECODER thực chất là cùng một mạch!**

#### 1. Sự chuyển đổi thân phận
Hãy nhìn vào IC 74138 (Decoder 3 sang 8). Nó có 3 đầu vào địa chỉ, 1 đầu vào cho phép (Enable), và 8 đầu ra.

*   **Khi dùng làm DECODER:**
    *   Chân Enable = Đóng vai trò công tắc nguồn (ON/OFF).
    *   Chân Địa chỉ = Chọn đầu ra nào sáng.
*   **Khi dùng làm DMUX:**
    *   Chân Enable = Đóng vai trò **Đầu vào dữ liệu (Data Input)**. (Dữ liệu đi vào đường này).
    *   Chân Địa chỉ = Chọn xem dữ liệu đó sẽ chui ra ở cổng nào.
    *   Các đầu ra còn lại (không được chọn) sẽ ở trạng thái nghỉ.

#### 2. Ứng dụng chuyển đổi Song song / Nối tiếp
*   **MUX:** Chuyển đổi **Song song sang Nối tiếp (P2S)**.
    *   Ví dụ: Bạn có 8 bit dữ liệu nằm im một chỗ (Song song). Bạn dùng MUX quét lần lượt từng chân một $\to$ Đầu ra sẽ là một chuỗi bit chạy nối đuôi nhau (Nối tiếp).
*   **DMUX:** Chuyển đổi **Nối tiếp sang Song song (S2P)**.
    *   Ví dụ: Nhận một chuỗi bit nối đuôi nhau vào, DMUX sẽ phân phối từng bit vào các ô nhớ riêng biệt.

---

### PHẦN D: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Một bộ hợp kênh (MUX) có 16 đường vào dữ liệu ($D_0 - D_{15}$). Cần bao nhiêu đường điều khiển (Select lines)?
A. 2
B. 4
C. 8
D. 16

> **Đáp án: B.**
> *Giải thích:* $2^n = 16 \to n = 4$.

**Câu 2:** Hàm logic $F(A,B,C) = \sum(1, 3, 5, 7)$ được thực hiện bằng một bộ MUX 8-1. Các đầu vào dữ liệu ($D_0 - D_7$) sẽ được nối lần lượt như thế nào?
A. 0, 1, 0, 1, 0, 1, 0, 1
B. 1, 0, 1, 0, 1, 0, 1, 0
C. 0, 0, 0, 0, 1, 1, 1, 1
D. 1, 1, 1, 1, 0, 0, 0, 0

> **Đáp án: A.**
> *Giải thích:*
> *   Vị trí 1, 3, 5, 7 (các số lẻ) có hàm bằng 1 $\to$ Nối $D_1, D_3, D_5, D_7$ lên mức 1.
> *   Vị trí 0, 2, 4, 6 (các số chẵn) có hàm bằng 0 $\to$ Nối $D_0, D_2, D_4, D_6$ xuống mức 0.
> *   Thứ tự từ $D_0 \to D_7$ là: 0, 1, 0, 1, 0, 1, 0, 1.

**Câu 3:** IC 74138 là bộ giải mã 3 sang 8. Nếu ta dùng nó làm bộ phân kênh (DMUX), thì tín hiệu dữ liệu đầu vào sẽ được đưa vào chân nào?
A. Chân đầu ra $Y_0$.
B. Một trong các chân địa chỉ (A, B, C).
C. Chân cho phép (Enable / Strobe).
D. Chân nguồn Vcc.

> **Đáp án: C.**
> *Giải thích:* Như đã giải thích ở phần C, chân Enable biến thành chân Data Input khi dùng chế độ DMUX.

**Câu 4:** Để chuyển đổi dữ liệu từ dạng song song sang dạng nối tiếp, ta sử dụng mạch nào?
A. Encoder
B. Decoder
C. Multiplexer (MUX)
D. Demultiplexer (DMUX)

> **Đáp án: C.**
> *Giải thích:* MUX lấy nhiều đầu vào (song song) và lần lượt đưa ra 1 đường (nối tiếp).

**Câu 5 (Câu hỏi khó):** Muốn thiết kế một bộ MUX 16-1 bằng cách sử dụng các bộ MUX 4-1, ta cần ít nhất bao nhiêu bộ MUX 4-1?
A. 4
B. 5
C. 3
D. 2

> **Đáp án: B.**
> *Giải thích:*
> *   Tầng 1: Cần 4 bộ MUX 4-1 để nhận hết 16 đầu vào (4x4=16). Lúc này ta có 4 đầu ra trung gian.
> *   Tầng 2: Cần thêm 1 bộ MUX 4-1 nữa để nhận 4 đầu ra trung gian đó và gom lại thành 1 đầu ra duy nhất.
> *   Tổng cộng: 4 + 1 = 5 bộ.

---

Chào bạn, chúng ta đã đến phần cuối cùng và cũng là phần "trí tuệ" nhất của Chương 3: **Mục 3.6 - Mạch Số Học**.

Đây là nơi các cổng logic (AND, OR, XOR...) được lắp ghép lại để thực hiện các phép tính cộng, trừ, nhân, chia. Trong thi trắc nghiệm, phần này có 2 mảng câu hỏi chính: **Nhớ công thức hàm logic** (của HA, FA) và **Hiểu nguyên lý mạch cộng/trừ kết hợp (Bù 2)**.

Dưới đây là tài liệu ôn tập tối ưu cho mục 3.6.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: MẠCH SỐ HỌC (ADDER/SUBTRACTOR)
**(Phạm vi: Mục 3.6 - Chương 3)**

### PHẦN A: BỘ CỘNG (ADDER) - NỀN TẢNG CỐT LÕI

Phải phân biệt rạch ròi giữa "Bán phần" và "Toàn phần".

#### 1. Bộ cộng Bán phần (HA - Half Adder)
*   **Định nghĩa:** Cộng 2 bit nhị phân ($A, B$), **KHÔNG** quan tâm đến bit nhớ từ hàng trước đưa tới.
*   **Đầu vào:** 2 (A, B).
*   **Đầu ra:** 2 (Tổng $S$, Nhớ $C$).
*   **Công thức (Thuộc lòng):**
    *   Tổng $S = A \oplus B$ (Dùng cổng **XOR**).
    *   Nhớ $C = A . B$ (Dùng cổng **AND**).
*   *Hạn chế:* Không thể dùng để cộng các số nhị phân nhiều bit (vì nó không xử lý được bit nhớ dư ra từ cột bên phải).

#### 2. Bộ cộng Toàn phần (FA - Full Adder)
*   **Định nghĩa:** Cộng 2 bit nhị phân ($A, B$) VÀ **CÓ** cộng thêm bit nhớ từ hàng trước ($C_{in}$).
*   **Đầu vào:** 3 ($A, B, C_{in}$).
*   **Đầu ra:** 2 (Tổng $S$, Nhớ $C_{out}$).
*   **Cấu tạo từ HA (Câu hỏi thi kinh điển):**
    *   **1 FA = 2 HA + 1 cổng OR.**
*   **Công thức:**
    *   Tổng $S = A \oplus B \oplus C_{in}$ (XOR 3 tham số).
    *   Nhớ $C_{out} = AB + C_{in}(A \oplus B)$ (Hoặc $AB + BC_{in} + AC_{in}$ - Luật đa số).

#### 3. Bộ cộng song song nhiều bit & Vấn đề Trễ (Ripple Carry)
*   Để cộng số 4 bit, ta ghép 4 con FA nối tiếp nhau.
*   **Vấn đề:** Bit nhớ ($C_{out}$) của con thứ nhất phải chạy sang con thứ 2, rồi con 2 sang con 3... Giống như sóng lan truyền.
*   **Hậu quả:** Gây ra **Độ trễ truyền dẫn (Propagation Delay)**. Mạch chạy chậm.
*   **Giải pháp (Từ khóa):** Dùng **Bộ cộng nhìn trước (Carry Look-ahead Adder)** để tăng tốc độ.

---

### PHẦN B: BỘ TRỪ (SUBTRACTOR) - "ANH EM SINH ĐÔI" VỚI BỘ CỘNG

Mạch trừ rất giống mạch cộng, chỉ khác một chút ở cổng logic.

#### 1. Bộ trừ Bán phần (HS - Half Subtractor)
*   Thực hiện $A - B$.
*   **Hiệu (Difference - D):** $D = A \oplus B$ (Giống hệt mạch cộng!).
*   **Mượn (Borrow - B):** $B = \overline{A} . B$ (Lưu ý: Phải có cổng **NOT** ở A).
    *   *Mẹo nhớ:* Tại sao lại đảo A? Vì muốn mượn thì số bị trừ (A) phải nhỏ hơn số trừ (B) (ví dụ 0 - 1). Tức là A=0, B=1. Khi đó $\overline{A}.B = 1.1 = 1$ (Có mượn).

#### 2. Bộ trừ Toàn phần (FS - Full Subtractor)
*   Tương tự FA, nó trừ 2 bit và trừ cả bit mượn từ hàng trước.
*   **1 FS = 2 HS + 1 cổng OR.**

---

### PHẦN C: MẠCH CỘNG/TRỪ KẾT HỢP (PHẦN KHÓ & HAY NHẤT)

Làm sao để một con chip vừa biết cộng, vừa biết trừ? Người ta không lắp riêng 2 mạch, mà dùng kỹ thuật **Bù 2**.

#### 1. Bản chất toán học
Phép trừ $A - B$ thực chất là: $A + (\text{Bù 2 của B})$.
Mả: $\text{Bù 2 của B} = (\text{Đảo B}) + 1$.
$\Rightarrow A - B = A + \overline{B} + 1$.

#### 2. Cơ chế mạch điện (IC 7483 + XOR)
Để thiết kế mạch này, người ta dùng 1 chân điều khiển $M$ (Mode):
*   Nếu $M=0$: Phép Cộng.
*   Nếu $M=1$: Phép Trừ.

**Vai trò thần thánh của cổng XOR (Cổng đảo có điều khiển):**
*   Ta cho bit $B$ đi qua cổng XOR với chân $M$.
    *   Nếu $M=0$: $B \oplus 0 = B$ (Giữ nguyên B).
    *   Nếu $M=1$: $B \oplus 1 = \overline{B}$ (Đảo B - Tạo ra Bù 1).

**Vai trò của chân $C_{in}$ (Bit nhớ đầu vào):**
*   Nối chân $M$ vào thẳng chân $C_{in}$ đầu tiên của bộ cộng.
    *   Nếu $M=0$: $C_{in} = 0$ (Cộng bình thường: $A + B + 0$).
    *   Nếu $M=1$: $C_{in} = 1$ (Thực hiện bước "Cộng 1" trong quy tắc bù 2: $A + \overline{B} + 1$).

> **TÓM LẠI (Cần nhớ để thi):**
> Trong mạch cộng/trừ kết hợp 4 bit:
> *   Dùng **4 bộ cộng toàn phần (FA)**.
> *   Dùng **4 cổng XOR** ở đầu vào B để đảo bit.
> *   Tín hiệu điều khiển **M** nối vào 1 chân của XOR và nối vào **$C_0$ (Carry in)**.

---

### PHẦN D: MẠCH SO SÁNH (COMPARATOR)

#### 1. So sánh bằng (=)
*   Dùng cổng **XNOR** (Đồng dấu).
*   Hai bit giống nhau thì XNOR ra 1.
*   Để so sánh 2 số 4 bit ($A_3A_2A_1A_0$ và $B_3B_2B_1B_0$), ta XNOR từng cặp bit tương ứng, rồi đưa tất cả vào cổng **AND**. Nếu tất cả đều khớp (đều ra 1) thì cổng AND ra 1 (Hai số bằng nhau).

#### 2. So sánh lớn hơn/nhỏ hơn (Magnitude)
*   Dùng IC chuyên dụng (7485).
*   **Nguyên tắc xếp tầng (Cascading):** Khi so sánh số lớn (ví dụ 8 bit) bằng cách ghép 2 con IC 4 bit:
    *   Ta nối các đầu ra $>, <, =$ của con "trọng số thấp" (LSB) vào đầu vào xếp tầng của con "trọng số cao" (MSB).
    *   Con MSB sẽ quyết định trước. Nếu MSB bằng nhau thì mới "hỏi" ý kiến của con LSB.

---

### PHẦN E: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Một bộ cộng bán phần (Half Adder) bao gồm những cổng logic nào?
A. 1 cổng AND và 1 cổng OR.
B. 1 cổng XOR và 1 cổng AND.
C. 2 cổng NAND.
D. 1 cổng XOR và 1 cổng OR.

> **Đáp án: B.**
> *Giải thích:* $S = A \oplus B$ (XOR), $C = A.B$ (AND).

**Câu 2:** Biểu thức logic cho bit "Mượn" (Borrow Output) của bộ trừ bán phần ($A - B$) là gì?
A. $A . B$
B. $A . \overline{B}$
C. $\overline{A} . B$
D. $A \oplus B$

> **Đáp án: C.**
> *Giải thích:* Mượn xảy ra khi số bị trừ nhỏ hơn số trừ ($A=0, B=1$). $\to \overline{0}.1 = 1$.

**Câu 3:** Để thực hiện phép trừ $A - B$ bằng mạch cộng, ta cần thực hiện thao tác nào đối với B?
A. Đảo bit B (Bù 1)
B. Giữ nguyên B và đặt $C_{in} = 1$
C. Lấy bù 2 của B (Đảo B và đặt $C_{in}=1$)
D. Đặt B = 0

> **Đáp án: C.**
> *Giải thích:* Quy tắc $A - B = A + (-B)$. Trong máy tính $-B$ là bù 2 của B.

**Câu 4:** Trong mạch cộng/trừ 4 bit có điều khiển M ($M=0$ là cộng, $M=1$ là trừ). Tín hiệu M được nối vào đâu để tạo ra phép cộng thêm 1 cho Bù 2?
A. Đầu vào dữ liệu A.
B. Đầu vào dữ liệu B.
C. Đầu vào nhớ $C_0$ (Carry In) của bit thấp nhất.
D. Đầu ra nhớ $C_4$.

> **Đáp án: C.**
> *Giải thích:* Khi $M=1$, $C_0$ nhận mức 1, tương đương với việc cộng thêm 1 vào tổng $\to$ Hoàn tất phép lấy Bù 2.

**Câu 5:** Một bộ cộng toàn phần (Full Adder) có thể được cấu tạo từ:
A. 2 bộ cộng bán phần (HA) và 1 cổng OR.
B. 2 bộ cộng bán phần (HA) và 1 cổng AND.
C. 1 bộ cộng bán phần (HA) và 1 cổng XOR.
D. 3 bộ cộng bán phần.

> **Đáp án: A.**
> *Giải thích:* Đây là cấu trúc chuẩn trong giáo trình.

---
### TỔNG KẾT TOÀN BỘ CHƯƠNG 3

Bạn đã hoàn thành chương dài nhất và quan trọng nhất. Hãy nhìn lại lộ trình:
1.  **Phân tích/Thiết kế:** Nhớ quy trình 4 bước và K-Map.
2.  **Mã hóa/Giải mã:** Nhớ BCD, Gray, LED 7 đoạn và Anốt/Catốt chung.
3.  **MUX/DMUX:** Nhớ MUX là "tạo hàm logic", DMUX là "Decoder có data in".
4.  **Số học:** Nhớ HA/FA và cơ chế Bù 2 dùng cổng XOR.

---

Chào bạn, chúng ta chính thức bước sang **Chương 4: Mạch Logic Tuần Tự**. Đây là bước ngoặt lớn của môn học: từ những mạch "không có trí nhớ" (Chương 3) sang những mạch "có trí nhớ" (như RAM, CPU).

Mục 4.1 và 4.2 giới thiệu về **Flip-Flop (Trigơ)** - phần tử cơ bản nhất của bộ nhớ. Trong thi trắc nghiệm, phần này cực kỳ quan trọng vì nếu không hiểu bản chất của Flip-Flop, bạn sẽ mất gốc hoàn toàn ở phần Bộ đếm và Thanh ghi sau này.

Dưới đây là tài liệu ôn tập tối ưu.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: KHÁI NIỆM & PHẦN TỬ NHỚ (FLIP-FLOP)
**(Phạm vi: Mục 4.1 & 4.2 - Chương 4)**

### PHẦN A: BẢN CHẤT MẠCH TUẦN TỰ (Mục 4.1)

Câu hỏi lý thuyết sẽ xoay quanh sự khác biệt với mạch tổ hợp.

1.  **Định nghĩa:**
    *   **Mạch Tuần Tự (Sequential):** Đầu ra phụ thuộc vào đầu vào hiện tại + **Trạng thái cũ (Quá khứ)**.
    *   **Từ khóa:** "Có nhớ" (Memory), "Hồi tiếp" (Feedback), "Trạng thái trong" ($Q$).
2.  **Mô hình toán học (Cần nhớ):**
    *   $Z = f(X, Q)$ (Đầu ra phụ thuộc vào Vào $X$ và Trạng thái $Q$).
    *   $Q^{n+1} = f(X, Q^n)$ (Trạng thái kế tiếp phụ thuộc vào Vào $X$ và Trạng thái hiện tại $Q^n$).

---

### PHẦN B: CÁC LOẠI TRIGƠ (FLIP-FLOP) - "LINH HỒN" CỦA CHƯƠNG (Mục 4.2)

Đây là phần thi nhiều nhất. Bạn cần thuộc lòng **Bảng hoạt động** và **Phương trình đặc trưng** của 4 loại FF chính.

#### 1. Trigơ RS (Reset-Set) - "Ông tổ" sơ khai
*   **Nguyên lý:** Có 2 ngõ vào: **S** (Set - Đặt lên 1) và **R** (Reset - Xóa về 0).
*   **Hoạt động:**
    *   $S=1, R=0 \to Q=1$ (Lập).
    *   $S=0, R=1 \to Q=0$ (Xóa).
    *   $S=0, R=0 \to Q_{giữ nguyên}$ (Nhớ).
    *   **$S=1, R=1 \to$ CẤM (Forbidden)**. (Đây là điểm yếu chết người của RS, thi rất hay hỏi).
*   **Phương trình đặc trưng:** $Q^{n+1} = S + \bar{R}Q^n$ (Điều kiện $SR=0$).

#### 2. Trigơ JK - "Phiên bản hoàn hảo" của RS
Khắc phục nhược điểm của RS. Đây là loại FF đa năng nhất.
*   **Nguyên lý:** Giống RS ($J \approx S, K \approx R$), nhưng xử lý được trạng thái "1-1".
*   **Hoạt động:**
    *   $J=1, K=0 \to Q=1$ (Set).
    *   $J=0, K=1 \to Q=0$ (Reset).
    *   $J=0, K=0 \to Q_{giữ nguyên}$ (Nhớ).
    *   **$J=1, K=1 \to$ LẬT TRẠNG THÁI (Toggle)**. (Đang 0 thành 1, đang 1 thành 0). $\to$ *Tính chất quan trọng nhất!*
*   **Phương trình đặc trưng:** $Q^{n+1} = J\bar{Q}^n + \bar{K}Q^n$.

#### 3. Trigơ D (Delay/Data) - "Dùng để lưu dữ liệu"
*   **Nguyên lý:** Chỉ có 1 ngõ vào D.
*   **Hoạt động:** Đầu ra bám theo đầu vào.
    *   $D=1 \to Q^{n+1}=1$.
    *   $D=0 \to Q^{n+1}=0$.
*   **Ứng dụng:** Dùng làm thanh ghi, bộ nhớ đệm.
*   **Phương trình:** $Q^{n+1} = D$.

#### 4. Trigơ T (Toggle) - "Chuyên gia chia tần số"
*   **Nguyên lý:** Chỉ có 1 ngõ vào T.
*   **Hoạt động:**
    *   $T=0 \to Q$ giữ nguyên.
    *   $T=1 \to Q$ lật trạng thái (Toggle).
*   **Phương trình:** $Q^{n+1} = T \oplus Q^n$.

---

### PHẦN C: CÁC VẤN ĐỀ KHÓ & CHUYÊN SÂU (Giải thích kỹ)

Phần này giúp bạn hiểu sâu để trả lời các câu hỏi khó về thiết kế mạch.

#### 1. Trigơ Chủ - Tớ (Master-Slave Flip-Flop)
*   **Vấn đề:** Các Trigơ thông thường dễ bị nhiễu hoặc thay đổi trạng thái liên tục khi xung Clock đang ở mức cao (Hiện tượng *Racing*).
*   **Giải pháp:** Cấu tạo gồm 2 con Trigơ mắc nối tiếp (Con chủ - Master và con tớ - Slave).
    *   *Master:* Hoạt động khi Clock = 1 (nhận dữ liệu vào).
    *   *Slave:* Hoạt động khi Clock = 0 (đưa dữ liệu ra).
    *   Hai con này không bao giờ mở cùng lúc.
*   **Kết quả:** Dữ liệu chỉ thay đổi ở **Sườn Xung** (Cạnh lên hoặc cạnh xuống), giúp mạch hoạt động cực kỳ ổn định.

#### 2. Các ngõ vào KHÔNG ĐỒNG BỘ (Preset & Clear) - *Hay bị lừa*
Ngoài các chân J, K, D, Clock... Trigơ thực tế (như IC 7476) còn có chân **PRE (Set)** và **CLR (Reset)**.
*   **Đặc điểm:** Chúng là các "đại ca", có quyền lực tối cao.
*   **Quy tắc:**
    *   Nếu chân **PRE/CLR kích hoạt**, Trigơ lập tức chuyển về 1 hoặc 0 **BẤT CHẤP** xung Clock hay các chân J, K đang là gì.
    *   Chỉ khi PRE và CLR không kích hoạt thì Trigơ mới hoạt động theo Clock.
*   *Lưu ý:* Thường các chân này tích cực THẤP (có dấu tròn). Tức là nối đất (0) thì nó mới hoạt động.

#### 3. Chuyển đổi giữa các loại Trigơ (Mục 4.2.3)
Làm sao biến con JK thành con D? Hoặc D thành T?
*   **Nguyên tắc:** Dùng phương trình đặc trưng để so sánh.
*   *Ví dụ:* Biến JK thành D.
    *   PT của JK: $Q^{n+1} = J\bar{Q} + \bar{K}Q$.
    *   PT của D: $Q^{n+1} = D = D(1) = D(\bar{Q} + Q) = D\bar{Q} + DQ$.
    *   Đồng nhất hệ số: $J = D$ và $\bar{K} = D \Rightarrow K = \bar{D}$.
    *   **Kết luận:** Nối chân J vào D, chân K vào cổng NOT của D.

---

### PHẦN D: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Trigơ nào sau đây có trạng thái "cấm" (không xác định) khi cả hai đầu vào điều khiển đều ở mức logic 1?
A. Trigơ D
B. Trigơ JK
C. Trigơ T
D. Trigơ RS

> **Đáp án: D.**
> *Giải thích:* Đặc điểm yếu nhất của RS là khi $R=1, S=1$ thì trạng thái đầu ra không xác định.

**Câu 2:** Phương trình đặc trưng $Q^{n+1} = J\bar{Q}^n + \bar{K}Q^n$ mô tả hoạt động của loại Trigơ nào?
A. RS
B. JK
C. D
D. T

> **Đáp án: B.**
> *Giải thích:* Đây là công thức chuẩn của JK. Nhớ mẹo: Có chữ J và chữ K trong công thức.

**Câu 3:** Khi chân Preset (PRE) và Clear (CLR) của một Trigơ tích cực thấp đều được nối lên mức logic 1 (High), Trigơ sẽ hoạt động như thế nào?
A. Luôn ở trạng thái 1 (Set).
B. Luôn ở trạng thái 0 (Reset).
C. Hoạt động bình thường theo xung Clock và các ngõ vào điều khiển.
D. Rơi vào trạng thái cấm.

> **Đáp án: C.**
> *Giải thích:* Vì tích cực thấp (Low), nên mức 1 (High) nghĩa là **KHÔNG kích hoạt**. Khi 2 chân này "ngủ", Trigơ mới làm việc bình thường theo Clock.

**Câu 4:** Để chuyển đổi một Trigơ JK thành Trigơ T, ta cần thực hiện kết nối nào?
A. Nối J với T, K với mức 0.
B. Nối J với T, K với mức 1.
C. Nối J và K lại với nhau và nối vào tín hiệu T.
D. Nối J vào T, K vào đảo của T.

> **Đáp án: C.**
> *Giải thích:*
> *   Nếu $J=K=0 \to$ Giữ nguyên (T=0).
> *   Nếu $J=K=1 \to$ Lật trạng thái (T=1).
> *   Đúng với bản chất của Trigơ T.

**Câu 5:** Đặc điểm quan trọng nhất của cấu trúc Trigơ Master-Slave là gì?
A. Tăng tốc độ chuyển mạch.
B. Loại bỏ hiện tượng đua (racing) và chỉ thay đổi trạng thái ở sườn xung clock.
C. Giảm số lượng cổng logic cần dùng.
D. Cho phép hoạt động ở cả mức 0 và mức 1 của xung clock cùng lúc.

> **Đáp án: B.**
> *Giải thích:* Master-Slave tách biệt quá trình nhận và xuất dữ liệu, giúp mạch ổn định, tránh việc đầu ra thay đổi lung tung trong một chu kỳ xung.

---
### TỔNG KẾT CHIẾN LƯỢC
1.  **Học thuộc 4 phương trình đặc trưng** (RS, JK, D, T).
2.  **Nhớ đặc điểm "độc":** RS có trạng thái cấm, JK có trạng thái lật, T là chuyên gia lật, D là sao chép.
3.  **Lưu ý Async:** Chân Preset/Clear luôn ưu tiên cao nhất (đè lệnh Clock).

---

Chào bạn, chúng ta đang đi vào phần **"Giải phẫu mạch"** (Mục 4.3).

Nếu như mục 4.1-4.2 là học về "từng viên gạch" (Flip-Flop), thì mục 4.3 là học cách nhìn vào một "bức tường" (sơ đồ mạch hoàn chỉnh) và hiểu nó hoạt động như thế nào.

Trong thi trắc nghiệm, phần này thường xuất hiện dưới dạng: **Cho một hình vẽ sơ đồ mạch $\to$ Hỏi phương trình trạng thái, bảng trạng thái hoặc giản đồ xung.**

Dưới đây là tài liệu ôn tập được thiết kế để bạn phân tích mạch nhanh và chính xác nhất.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: PHÂN TÍCH MẠCH TUẦN TỰ
**(Phạm vi: Mục 4.3 - Chương 4)**

### PHẦN A: NHẬN DIỆN LOẠI MẠCH (Bước đầu tiên phải làm)

Trước khi tính toán, bạn phải nhìn sơ đồ và trả lời ngay: Đây là mạch **ĐỒNG BỘ** hay **KHÔNG ĐỒNG BỘ**? Vì cách tính của chúng khác hẳn nhau.

| Đặc điểm | **Mạch Đồng bộ (Synchronous)** | **Mạch Không đồng bộ (Asynchronous)** |
| :--- | :--- | :--- |
| **Dấu hiệu nhận biết** | Tất cả chân Clock (CK/CLK) của các Trigơ đều nối chung vào **MỘT nguồn xung nhịp duy nhất**. | Chân Clock của Trigơ này được nối vào **ĐẦU RA (Q)** của Trigơ khác. |
| **Thời điểm đổi trạng thái** | Tất cả Trigơ thay đổi **CÙNG LÚC** (tại sườn xung nhịp). | Các Trigơ thay đổi **LẦN LƯỢT** (kiểu dây chuyền/ripple). |
| **Độ khó tính toán** | Dễ hơn (dùng chung phương trình). | Khó hơn (phải xét thời điểm kích từng con). |

> **Mẹo thi trắc nghiệm:** Nhìn vào đường dây Clock. Nếu thấy nó rẽ nhánh đi vào tất cả các Trigơ $\to$ Đồng bộ. Nếu thấy nó đi kiểu "nối đuôi" $\to$ Không đồng bộ.

---

### PHẦN B: QUY TRÌNH PHÂN TÍCH (5 Bước chuẩn)

Dù mạch rối rắm thế nào, hãy tuân thủ đúng 5 bước này để không bị lạc:

1.  **Viết Phương trình Kích (Excitation Equations):**
    *   Nhìn vào các chân điều khiển ($J, K, D, T$) của từng Trigơ xem nó nối với cái gì.
    *   *Ví dụ:* Chân J của Trigơ 1 nối với đầu ra $\bar{Q}_2$ $\to$ Viết: $J_1 = \bar{Q}_2$.

2.  **Viết Phương trình Đặc trưng (Characteristic Equations) - QUAN TRỌNG:**
    *   Nhớ lại kiến thức Mục 4.2.
    *   JK: $Q^{n+1} = J\bar{Q}^n + \bar{K}Q^n$
    *   D: $Q^{n+1} = D$
    *   T: $Q^{n+1} = T \oplus Q^n$

3.  **Thay thế (Substitution) - Phần khó nhất:**
    *   Lấy phương trình Kích (Bước 1) thay vào phương trình Đặc trưng (Bước 2) để ra **Phương trình Chuyển đổi trạng thái**.
    *   *Mục đích:* Tìm xem trạng thái tiếp theo ($Q^{n+1}$) phụ thuộc thế nào vào trạng thái hiện tại ($Q^n$).

4.  **Lập Bảng Trạng thái (State Table):**
    *   Kẻ bảng liệt kê hiện tại ($Q^n$) và tính ra tương lai ($Q^{n+1}$).

5.  **Vẽ Đồ hình Trạng thái (State Diagram):**
    *   Các vòng tròn (State) và mũi tên chuyển hướng.

---

### PHẦN C: GIẢI THÍCH SÂU VỀ CÁCH TÍNH TOÁN (Deep Dive)

Đây là chỗ sinh viên hay sai nhất: **Làm sao để tính ra trạng thái tiếp theo?**

Giả sử đề bài cho mạch dùng **Trigơ JK**.
*   Đầu vào kích nhìn thấy trên sơ đồ: $J = 1$, $K = Q$.
*   Hỏi: Trạng thái tiếp theo ($Q^{n+1}$) là gì?

**Cách tư duy:**
1.  Đừng đoán mò. Hãy dùng công thức gốc của JK:
    $$Q^{n+1} = J \cdot \bar{Q}^n + \bar{K} \cdot Q^n$$
2.  Thay $J=1$ và $K=Q$ vào:
    $$Q^{n+1} = 1 \cdot \bar{Q}^n + \overline{(Q^n)} \cdot Q^n$$
3.  Rút gọn:
    *   $1 \cdot \bar{Q}^n = \bar{Q}^n$
    *   $\bar{Q}^n \cdot Q^n = 0$ (Định lý: A nhân đảo A luôn bằng 0).
4.  Kết quả cuối cùng: $Q^{n+1} = \bar{Q}^n + 0 = \bar{Q}^n$.
    $\to$ **Kết luận:** Mạch này sẽ **lật trạng thái** liên tục (Toggle).

> **Lưu ý với mạch Không đồng bộ (Asynchronous):**
> Bạn không thể áp dụng công thức trên cho tất cả Trigơ cùng lúc.
> *   Phải xem Trigơ đầu tiên đổi trạng thái trước.
> *   Nếu Trigơ 1 đổi từ $1 \to 0$ (sườn xuống) $\to$ Nó mới kích Trigơ 2 hoạt động.
> *   Nếu Trigơ 1 đổi từ $0 \to 1$ (sườn lên) $\to$ Trigơ 2 đứng im (nếu dùng kích sườn âm).
> $\to$ *Phần này thường được hỏi kỹ hơn ở bài "Bộ đếm" (Mục 4.4).*

---

### PHẦN D: ĐỒ HÌNH TRẠNG THÁI (STATE DIAGRAM)

Trong trắc nghiệm, người ta thường cho một cái hình có các vòng tròn và mũi tên, rồi hỏi: **"Đây là mạch đếm mod bao nhiêu?"** hoặc **"Chu trình hoạt động của mạch là gì?"**.

*   **Cách đọc:**
    *   Mỗi vòng tròn là một con số (trạng thái). Ví dụ: `00`, `01`, `10`...
    *   Mũi tên chỉ hướng đi tiếp theo khi có xung Clock.
*   **Mod (Hệ số đếm):** Đếm số lượng vòng tròn trong vòng lặp chính.
    *   Ví dụ: $00 \to 01 \to 10 \to 00$. Có 3 vòng tròn $\to$ Mod 3.
*   **Tự khởi động (Self-correcting):**
    *   Nếu có các trạng thái thừa (ví dụ mạch 2 bit có 4 trạng thái, nhưng chỉ dùng 3), bạn phải xem các mũi tên từ trạng thái thừa đó có trỏ về vòng lặp chính không.
    *   Nếu có $\to$ Mạch tự khởi động (Tốt).
    *   Nếu nó tạo thành vòng lặp riêng hoặc đi vào ngõ cụt $\to$ Mạch bị treo ("Chết").

---

### PHẦN E: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Để phân tích một mạch tuần tự đồng bộ, bước đầu tiên cần làm là gì?
A. Lập bảng trạng thái.
B. Viết phương trình các hàm kích (đầu vào) cho các Trigơ.
C. Vẽ giản đồ xung.
D. Tối thiểu hóa mạch dùng bảng Karnaugh.

> **Đáp án: B.**
> *Giải thích:* Phải biết đầu vào ($J, K, D...$) là gì thì mới tính được cái khác.

**Câu 2:** Cho một Trigơ D có phương trình đầu vào là $D = \bar{Q}$. Phương trình trạng thái kế tiếp $Q^{n+1}$ sẽ là:
A. $Q^n$
B. $\bar{Q}^n$
C. 1
D. 0

> **Đáp án: B.**
> *Giải thích:* Phương trình gốc của Trigơ D là $Q^{n+1} = D$. Thay $D = \bar{Q}$ vào $\to Q^{n+1} = \bar{Q}^n$. (Đây là mạch chia đôi tần số).

**Câu 3:** Một mạch tuần tự có 3 Trigơ ($Q_1, Q_2, Q_3$). Số trạng thái tối đa mà mạch này có thể có là bao nhiêu?
A. 3
B. 6
C. 8
D. 9

> **Đáp án: C.**
> *Giải thích:* Số trạng thái tối đa = $2^n$ (với n là số Trigơ). $2^3 = 8$.

**Câu 4:** Sự khác biệt cơ bản nhất trong quy trình phân tích mạch "Không đồng bộ" so với "Đồng bộ" là gì?
A. Không cần viết phương trình kích.
B. Phải xác định điều kiện kích (sườn xung) của từng Trigơ riêng biệt.
C. Không sử dụng bảng trạng thái.
D. Luôn dùng Trigơ RS thay vì JK.

> **Đáp án: B.**
> *Giải thích:* Trong mạch không đồng bộ, Clock không gõ nhịp chung, nên phải xem con này lật xong có kích con kia lật không.

**Câu 5:** Đồ hình trạng thái của một mạch đếm là: $00 \to 01 \to 11 \to 10 \to 00$. Đây là bộ đếm mã gì?
A. Nhị phân tự nhiên (Binary).
B. Mã Gray.
C. Mã BCD.
D. Mã Johnson.

> **Đáp án: B.**
> *Giải thích:*
> *   Nhị phân: $00 \to 01 \to 10 \to 11$.
> *   Chuỗi đề bài: $00 \to 01 \to 11 \to 10$. Nhận thấy các số kế nhau chỉ thay đổi 1 bit (01 sang 11 đổi bit đầu, 11 sang 10 đổi bit sau). Đây là đặc trưng của **Mã Gray**.

---
Chào bạn, chúng ta đang bước vào phần **"nặng ký" nhất của Chương 4: MỤC 4.4 - BỘ ĐẾM (COUNTERS)**.

Trong đề thi trắc nghiệm, đây là phần chiếm nhiều câu hỏi tính toán và suy luận logic nhất. Bạn sẽ gặp các dạng bài như: *Xác định dung lượng đếm, Tính tần số đầu ra, Nhận biết sơ đồ mạch (Đếm lên hay xuống), và Thiết kế bộ đếm Mod N.*

Dưới đây là tài liệu ôn tập được thiết kế để bạn "nhìn sơ đồ - ra đáp án".

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: BỘ ĐẾM (COUNTERS)
**(Phạm vi: Mục 4.4 - Chương 4)**

### PHẦN A: CÁC THAM SỐ CỐT LÕI (Phải thuộc nằm lòng)

Trước khi phân tích mạch, bạn cần nắm chắc các định nghĩa này để không bị lừa về mặt thuật ngữ.

1.  **Dung lượng đếm (Modulus - $M$ hoặc $N$):**
    *   Là số trạng thái tối đa mà bộ đếm có thể trải qua trước khi quay vòng.
    *   Ví dụ: Đếm từ 0 đến 9 $\to$ Có 10 số $\to$ **Mod 10**.
    *   **Công thức liên hệ số Trigơ ($n$):**
        $$2^{n-1} < M \le 2^n$$
    *   *Ví dụ:* Muốn đếm Mod 12, cần bao nhiêu Flip-Flop?
        *   $2^3 = 8$ (Thiếu).
        *   $2^4 = 16$ (Đủ). $\to$ Cần **4 Trigơ**.

2.  **Chức năng Chia tần số (Frequency Division):**
    *   Bộ đếm còn là bộ chia tần số.
    *   **Công thức:** $f_{out} = \frac{f_{in}}{M}$
    *   *Ví dụ:* Xung nhịp vào 100Hz, qua bộ đếm Mod 5 $\to$ Đầu ra dao động với tần số $20Hz$.

---

### PHẦN B: PHÂN LOẠI & SO SÁNH (ĐỒNG BỘ vs. KHÔNG ĐỒNG BỘ)

Đây là câu hỏi lý thuyết kinh điển.

| Đặc điểm | **Bộ đếm KHÔNG ĐỒNG BỘ (Asynchronous / Ripple)** | **Bộ đếm ĐỒNG BỘ (Synchronous / Parallel)** |
| :--- | :--- | :--- |
| **Cấu trúc Clock** | Xung Clock chỉ vào Trigơ đầu tiên (LSB). Các Trigơ sau lấy Clock từ đầu ra của Trigơ trước. | Xung Clock đi vào **TẤT CẢ** Trigơ cùng một lúc. |
| **Tốc độ** | **CHẬM**. Do độ trễ lan truyền dồn tích (Trigơ 1 lật xong mới kích Trigơ 2...). | **NHANH**. Vì tất cả lật cùng lúc. |
| **Độ phức tạp** | Đơn giản, ít cổng logic phụ. | Phức tạp, cần nhiều cổng logic để điều khiển J, K, T. |
| **Tên gọi khác** | Bộ đếm nối tiếp (Serial Counter). | Bộ đếm song song (Parallel Counter). |
| **Nhược điểm** | Gây ra **Gai nhiễu (Glitches)** khi giải mã trạng thái (do các bit lật không đều). | Khó thiết kế với số bit lớn. |

---

### PHẦN C: GIẢI MÃ SƠ ĐỒ MẠCH (Phần khó nhất - Deep Dive)

Làm sao nhìn vào sơ đồ mà biết nó đếm LÊN hay đếm XUỐNG? Hãy dùng "Bảng Chân Lý Rút Gọn" dưới đây.

#### 1. Nguyên tắc cho Bộ đếm KHÔNG ĐỒNG BỘ (Ripple Counter)
Mạch này thường dùng Trigơ T hoặc JK (treo mức 1). Quy luật đếm phụ thuộc vào 2 yếu tố:
1.  **Loại sườn xung kích:** Sườn Âm ($\downarrow$ - có vòng tròn) hay Sườn Dương ($\uparrow$ - không vòng tròn).
2.  **Điểm lấy xung:** Lấy từ $Q$ hay đảo $\bar{Q}$ của tầng trước nối vào Clock tầng sau.

**QUY TẮC "CÙNG-XUỐNG, KHÁC-LÊN" (Mẹo nhớ nhanh):**
*   Coi Sườn Âm ($\downarrow$) và Đầu ra $Q$ là "Cùng phe" (Phe Âm/Thường).
*   Coi Sườn Dương ($\uparrow$) và Đầu ra $\bar{Q}$ là "Cùng phe" (Phe Dương/Đảo).

| Sườn xung kích (Clock) | Nối từ đầu ra nào của tầng trước? | Kết quả đếm |
| :---: | :---: | :---: |
| Âm ($\downarrow$) | $Q$ | **LÊN (UP)** |
| Âm ($\downarrow$) | $\bar{Q}$ | **XUỐNG (DOWN)** |
| Dương ($\uparrow$) | $Q$ | **XUỐNG (DOWN)** |
| Dương ($\uparrow$) | $\bar{Q}$ | **LÊN (UP)** |

> **Phân tích kỹ:** Tại sao Âm + Q lại là Đếm Lên?
> *   Giả sử Trigơ A (LSB) đang là 1, chuẩn bị về 0 (sườn xuống).
> *   Sườn xuống của $Q_A$ kích vào Clock của Trigơ B.
> *   Trigơ B lật trạng thái (0 lên 1).
> *   Kết quả: `01` $\to$ `10` (Số 1 thành số 2 $\to$ Tăng $\to$ Đếm lên).

#### 2. Nguyên tắc cho Bộ đếm Mod N (Bất kỳ)
Làm sao để đếm Mod 6 (0 đến 5) hoặc Mod 10 (0 đến 9) từ một bộ đếm 4 bit (Mod 16)?
*   **Cơ chế:** Dùng chân **RESET (Xóa)**.
*   **Cách làm:**
    1.  Cho bộ đếm chạy bình thường.
    2.  Khi nó nhảy đến số $N$ (Số cần giới hạn), mạch logic sẽ phát hiện và lập tức Reset bộ đếm về 0.
    3.  *Ví dụ:* Đếm Mod 6 (0,1,2,3,4,5).
        *   Khi số nhảy sang **6** (Nhị phân: $110_2$ tức là $Q_3=0, Q_2=1, Q_1=1$).
        *   Ta dùng cổng NAND nối $Q_2$ và $Q_1$ vào chân Reset (CLR).
        *   Vừa chớm sang số 6, mạch bị Reset về 0 ngay lập tức.
    *   **Lưu ý thi trắc nghiệm:** Mạch Reset ở số $N$ (ví dụ số 6), nhưng trạng thái số 6 chỉ tồn tại trong tích tắc (vài nano giây) rồi biến mất. Người quan sát chỉ thấy đếm từ 0 đến 5.

---

### PHẦN D: CÁC BỘ ĐẾM ĐẶC BIỆT

#### 1. Bộ đếm BCD (Thập phân - Mod 10)
*   Đếm từ `0000` đến `1001` (0-9).
*   **IC tiêu biểu:** 7490 (Chia 2 và Chia 5).
    *   Muốn đếm 10: Nối đầu ra của bộ chia 2 vào đầu vào bộ chia 5.

#### 2. Bộ đếm Vòng (Ring Counter) - Mục 4.5 (Liên quan đến 4.4)
*   **Cấu tạo:** Dùng thanh ghi dịch, nối đầu ra $Q$ cuối cùng quay lại đầu vào $D$ đầu tiên.
*   **Hoạt động:** Chỉ có **duy nhất 1 bit mức 1** chạy vòng tròn.
    *   `1000` $\to$ `0100` $\to$ `0010` $\to$ `0001` $\to$ `1000`...
*   **Mod đếm:** $N$ trigơ đếm được $N$ trạng thái. (Hiệu suất thấp).
*   **Không tự khởi động:** Nếu rơi vào trạng thái `0000` hoặc `1100`, nó sẽ chạy sai mãi mãi. Cần mạch khởi tạo.

#### 3. Bộ đếm Vòng xoắn (Johnson Counter)
*   **Cấu tạo:** Nối đầu ra đảo $\bar{Q}$ cuối cùng quay lại đầu vào $D$ đầu tiên.
*   **Mod đếm:** $N$ trigơ đếm được $2N$ trạng thái. (Hiệu suất tốt hơn Ring).
*   **Giải mã:** Cần mạch giải mã để biết trạng thái.

---

### PHẦN E: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Để thiết kế một bộ đếm Mod 60 (đếm giây đồng hồ), ta cần tối thiểu bao nhiêu Flip-Flop?
A. 5
B. 6
C. 60
D. 12

> **Đáp án: B.**
> *Giải thích:* $2^5 = 32$ (Thiếu), $2^6 = 64$ (Đủ). Vậy cần 6 FF.

**Câu 2:** Một bộ đếm không đồng bộ (Ripple Counter) 4-bit đếm lên, sử dụng Trigơ JK có xung Clock kích hoạt sườn âm ($\downarrow$). Đầu vào Clock của Trigơ thứ 2 ($Q_1$) được nối với:
A. Đầu ra $Q_0$ của Trigơ trước đó.
B. Đầu ra $\bar{Q}_0$ của Trigơ trước đó.
C. Nguồn xung Clock chính hệ thống.
D. Mức logic 1.

> **Đáp án: A.**
> *Giải thích:* Quy tắc "Cùng-Xuống, Khác-Lên".
> *   Đếm LÊN (UP).
> *   Sườn ÂM ($\downarrow$).
> *   $\to$ Phải nối vào **Q** (Cùng phe âm/thường).

**Câu 3:** Tần số xung nhịp đầu vào của một bộ đếm Mod 12 là 12kHz. Tần số của xung tại đầu ra cuối cùng (MSB) là bao nhiêu? (Giả sử chu kỳ nhiệm vụ 50% ở đầu ra Mod 12 chuẩn).
A. 144 kHz
B. 12 kHz
C. 1 kHz
D. 6 kHz

> **Đáp án: C.**
> *Giải thích:* $f_{out} = 12kHz / 12 = 1 kHz$.

**Câu 4:** Trong một bộ đếm Mod 10 (BCD) không đồng bộ, cổng logic Reset được kết nối để xóa mạch về 0 khi bộ đếm đạt đến trạng thái nhị phân nào?
A. 1001 (Số 9)
B. 1010 (Số 10)
C. 1111 (Số 15)
D. 1000 (Số 8)

> **Đáp án: B.**
> *Giải thích:* Muốn đếm 0-9, thì ngay khi chạm số **10 ($1010_2$)**, mạch phải bị Reset ngay lập tức. (Nếu Reset ở 9 thì chỉ đếm được đến 8).

**Câu 5:** Nhược điểm lớn nhất của bộ đếm không đồng bộ (Ripple) so với bộ đếm đồng bộ là gì?
A. Cấu trúc phức tạp hơn.
B. Tiêu thụ nhiều năng lượng hơn.
C. Tốc độ chậm do trễ lan truyền tích lũy qua các tầng.
D. Khó thiết kế số Mod bất kỳ.

> **Đáp án: C.**
> *Giải thích:* Đây là đặc điểm "chết người" của mạch Ripple. Trigơ cuối cùng phải đợi tất cả các Trigơ trước lật xong thì mới đến lượt nó.

---
Chào bạn, chúng ta đã đi đến chặng cuối cùng của môn Kỹ thuật số: **Bộ Ghi Dịch (4.5)** và **Thanh Chốt (4.6)**.

Đây là hai thành phần không thể thiếu để xây dựng nên một hệ thống máy tính thực thụ (CPU, RAM, Bus dữ liệu). Trong thi trắc nghiệm, phần này không quá khó về toán học nhưng lại rất dễ nhầm lẫn về **cơ chế hoạt động (Sườn xung vs. Mức điện áp)**.

Dưới đây là tài liệu ôn tập chốt hạ cho chương trình.

---

# TÀI LIỆU ÔN TẬP TRẮC NGHIỆM: GHI DỊCH & THANH CHỐT
**(Phạm vi: Mục 4.5 & 4.6 - Chương 4)**

### PHẦN A: BỘ GHI DỊCH (SHIFT REGISTER) - MỤC 4.5

Hãy tưởng tượng Bộ ghi dịch giống như một hàng người xếp hàng truyền tay nhau những quả bóng. Mỗi khi có tiếng còi (Clock), người này chuyền quả bóng sang người bên cạnh.

#### 1. Phân loại 4 chế độ hoạt động (Cần nhớ tên viết tắt)
Đề thi thường dùng tên tiếng Anh viết tắt, bạn cần phản xạ ngay:

| Tên viết tắt | Tiếng Anh | Tiếng Việt | Đặc điểm & Ứng dụng |
| :--- | :--- | :--- | :--- |
| **SISO** | Serial In - Serial Out | Vào nối tiếp - Ra nối tiếp | **Tạo trễ (Delay)**. Dữ liệu đi vào đầu này, một lúc sau mới chui ra đầu kia. |
| **SIPO** | Serial In - Parallel Out | Vào nối tiếp - Ra song song | **Nhận dữ liệu truyền tin**. Nhận từng bit một, khi đủ thì xuất ra cả cụm cho CPU xử lý. |
| **PISO** | Parallel In - Serial Out | Vào song song - Ra nối tiếp | **Phát dữ liệu**. CPU gửi cả cụm dữ liệu ra, mạch này "băm" nhỏ để gửi đi xa từng bit. |
| **PIPO** | Parallel In - Parallel Out | Vào song song - Ra song song | **Lưu trữ tạm thời**. Giống như một ngăn nhớ đệm. |

#### 2. Cơ chế tạo trễ (Time Delay) - Công thức thi
*   Nếu bạn đưa 1 bit vào bộ ghi dịch SISO gồm **N** tầng (N trigơ).
*   Sau bao lâu bit đó sẽ xuất hiện ở đầu ra?
*   **Công thức:** $\Delta t = N \times T_{clk} = \frac{N}{f_{clk}}$
*   *Ví dụ:* Bộ ghi dịch 4 bit, xung nhịp 1MHz ($T=1\mu s$).
    *   Độ trễ = $4 \times 1\mu s = 4\mu s$.

#### 3. Bộ đếm Vòng & Vòng Xoắn (Ứng dụng của Ghi dịch)
Phần này đã nhắc ở mục 4.4, nhưng ở đây chúng ta chốt lại sự khác biệt về **Hiệu suất**:

| Loại | **Bộ đếm Vòng (Ring Counter)** | **Bộ đếm Vòng Xoắn (Johnson Counter)** |
| :--- | :--- | :--- |
| **Cấu tạo** | Nối đầu ra $Q_{cuối}$ quay về đầu vào $D_{đầu}$. | Nối đầu ra đảo $\overline{Q}_{cuối}$ quay về đầu vào $D_{đầu}$. |
| **Số trạng thái (Mod)** | **N** (Dùng N trigơ đếm được N số). | **2N** (Dùng N trigơ đếm được 2N số). |
| **Hiệu suất** | Kém. | Tốt gấp đôi. |
| **Giải mã** | Không cần (Mỗi trạng thái chỉ có 1 bit 1 duy nhất). | Cần mạch giải mã. |

---

### PHẦN B: THANH CHỐT (LATCH) vs. FLIP-FLOP - MỤC 4.6 (Phần dễ sai nhất)

Sinh viên thường coi Latch và Flip-Flop là một. **SAI HOÀN TOÀN**. Trong thi trắc nghiệm, đây là cái bẫy lớn nhất.

#### 1. Sự khác biệt cốt lõi (Deep Dive)

*   **Flip-Flop (Trigơ - Ví dụ IC 74374):**
    *   Hoạt động theo **SƯỜN XUNG** (Edge-triggered).
    *   *Ví dụ:* Chỉ khi xung Clock chuyển từ 0 lên 1 (tích tắc), nó mới chụp ảnh dữ liệu. Thời gian còn lại, đầu vào thay đổi thế nào nó cũng mặc kệ.
    *   *Ứng dụng:* Dùng trong các mạch đếm, mạch tuần tự chính xác.

*   **Latch (Chốt - Ví dụ IC 74373):**
    *   Hoạt động theo **MỨC ĐIỆN ÁP** (Level-triggered).
    *   *Ví dụ:* Khi chân cho phép (LE - Latch Enable) ở mức cao (1), cổng mở toang. Dữ liệu vào thay đổi $\to$ Đầu ra thay đổi theo ngay lập tức (Xuyên suốt - Transparent).
    *   Khi LE xuống mức thấp (0), nó đóng sập cửa lại, giữ nguyên giá trị cuối cùng.
    *   *Ứng dụng:* Dùng để bắt lấy dữ liệu từ Bus (đường truyền) khi nó đã ổn định.

#### 2. Trạng thái Trở kháng cao (High-Z)
Các IC chốt (như 74373) thường có chân **OE (Output Enable)**.
*   Nếu OE tích cực: IC xuất dữ liệu ra bình thường (0 hoặc 1).
*   Nếu OE không tích cực (Cấm): Đầu ra rơi vào trạng thái **Trở kháng cao (High-Z)**.
    *   *Nghĩa là gì?* Nghĩa là chân IC như bị "cắt đứt" khỏi mạch điện. Nó không là 0, cũng không là 1.
    *   *Tại sao cần?* Để nhiều con chip có thể nối chung vào một đường dây (Bus) mà không gây chập mạch. Con nào không dùng thì ngắt mình ra (High-Z).

---

### PHẦN C: CÂU HỎI GIẢ LẬP (MOCK TEST)

**Câu 1:** Để chuyển đổi dữ liệu từ dạng nối tiếp sang song song (ví dụ nhận dữ liệu từ bàn phím vào máy tính), ta sử dụng loại thanh ghi dịch nào?
A. PISO
B. SISO
C. SIPO
D. PIPO

> **Đáp án: C.**
> *Giải thích:* Serial In (từ bàn phím) $\to$ Parallel Out (vào bus máy tính).

**Câu 2:** Một bộ ghi dịch 8-bit hoạt động với tần số xung nhịp 2 MHz. Thời gian trễ từ đầu vào đến đầu ra nối tiếp là bao nhiêu?
A. $4 \mu s$
B. $2 \mu s$
C. $0.5 \mu s$
D. $16 \mu s$

> **Đáp án: A.**
> *Giải thích:* $f = 2MHz \to T = 0.5 \mu s$.
> Độ trễ = $8 \times 0.5 \mu s = 4 \mu s$.

**Câu 3:** Điểm khác biệt lớn nhất giữa Latch (Chốt) và Flip-Flop (Trigơ) là gì?
A. Latch không có khả năng lưu trữ dữ liệu.
B. Latch nhạy với mức điện áp (Level), còn Flip-Flop nhạy với sườn xung (Edge).
C. Flip-Flop cấu tạo đơn giản hơn Latch.
D. Latch chỉ hoạt động với tín hiệu Analog.

> **Đáp án: B.**
> *Giải thích:* Đây là định nghĩa phân biệt quan trọng nhất.

**Câu 4:** Bộ đếm Johnson 4 bit (Mod 8) có các trạng thái hợp lệ nào sau đây?
A. 0000, 0001, 0010, 0011... (Mã nhị phân)
B. 1000, 0100, 0010, 0001 (Mã 1 nóng)
C. 0000, 1000, 1100, 1110, 1111, 0111... (Mã Johnson)
D. 0000, 0001, 0011, 0111, 1111 (Mã Gray)

> **Đáp án: C.**
> *Giải thích:* Đặc điểm của Johnson là bit 1 sẽ tràn dần vào (1000 $\to$ 1100) rồi sau đó bit 0 lại tràn dần vào. Đáp án B là Ring Counter.

**Câu 5:** Chân $\overline{OE}$ (Output Enable - tích cực thấp) của IC chốt 74373 được nối lên mức cao (Logic 1). Trạng thái đầu ra của IC sẽ là:
A. Luôn bằng 1.
B. Luôn bằng 0.
C. Bằng với đầu vào D.
D. Trạng thái trở kháng cao (High-Z).

> **Đáp án: D.**
> *Giải thích:* Tích cực thấp mà nối lên cao $\to$ Bị Cấm (Disable) $\to$ Ngắt kết nối (High-Z).

---

### TỔNG KẾT TOÀN BỘ KHÓA HỌC

Chúc mừng bạn! Chúng ta đã rà soát xong toàn bộ 4 chương của môn Kỹ thuật số. Dưới đây là "Bản đồ tư duy" rút gọn để bạn mang vào phòng thi (trong đầu):

1.  **Chương 1 (Hệ đếm):**
    *   Nhớ các phép đổi cơ số (chia lấy dư, nhân lấy nguyên).
    *   **Bù 2:** Đảo bit + 1. Phạm vi số có dấu.

2.  **Chương 2 (Cổng Logic):**
    *   **DeMorgan:** Bẻ gạch đổi dấu.
    *   **K-Map:** Khoanh vùng số 1 to nhất có thể ($2^n$).
    *   **NAND/NOR:** Cổng vạn năng.

3.  **Chương 3 (Mạch Tổ Hợp):**
    *   **Decoder:** Giải mã địa chỉ.
    *   **MUX:** Chọn kênh dữ liệu / Tạo hàm logic.
    *   **Adder:** HA, FA và mạch cộng/trừ bù 2 (XOR).

4.  **Chương 4 (Mạch Tuần Tự):**
    *   **FF:** Thuộc 4 phương trình JK, D, T, RS.
    *   **Bộ đếm:** Mod $N$, quy tắc nối $Q$ hay $\bar{Q}$ để đếm Lên/Xuống.
    *   **Latch vs FF:** Mức vs Sườn.

**Lời khuyên cuối cùng:** Trong phòng thi trắc nghiệm, nếu gặp câu tính toán mạch phức tạp, hãy thử **thay giá trị (0 hoặc 1)** vào đầu vào và nhẩm trong đầu xem đầu ra là gì, sau đó loại trừ đáp án. Cách này nhanh hơn việc viết phương trình rất nhiều.

Chúc bạn có một kỳ thi đạt điểm A! Nếu cần hỗ trợ giải đề thi thử sau này, hãy cứ quay lại đây.