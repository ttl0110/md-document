Chào bạn, tôi đã phân tích xong file PDF **"Chương 1: Dao Động và Sóng"**. Đây là một chương có khối lượng kiến thức rất lớn, bao trùm cả Cơ học và Điện từ học.

Đối với bài thi trắc nghiệm, giảng viên thường khai thác sự **tương đồng** (analogy) giữa dao động cơ và dao động điện, cũng như các **điều kiện biên** (cực đại, cực tiểu, cộng hưởng).

Dưới đây là tài liệu ôn tập chiến lược dành riêng cho Chương 1:

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 1 (DAO ĐỘNG & SÓNG)

## PHẦN A: "GIẢI PHẪU" TỪ KHÓA & ĐỊNH NGHĨA (THEORY ANATOMY)
*Mẹo: Thấy từ khóa bên trái -> Khoanh ngay đáp án chứa nội dung bên phải.*

### 1. Phân loại Dao động (Cơ & Điện)
| Thuật ngữ | Từ khóa nhận diện (Keywords) | Đặc điểm cốt lõi |
| :--- | :--- | :--- |
| **Dao động điều hòa** | `sin`, `cos`, `không ma sát`, `bỏ qua điện trở` | Năng lượng **bảo toàn** (Cơ năng/Năng lượng điện từ = const). Biên độ $A$ không đổi. |
| **Dao động tắt dần** | `ma sát`, `lực cản`, `điện trở R`, `tỏa nhiệt` | **Biên độ giảm dần** theo hàm mũ ($e^{-\beta t}$). **Năng lượng mất mát** chuyển hóa thành nhiệt. Chu kỳ $T_{tắt} > T_{riêng}$. |
| **Dao động cưỡng bức** | `ngoại lực tuần hoàn`, `nguồn điện xoay chiều`, `ổn định` | Tần số dao động = **Tần số của ngoại lực** ($\Omega$), *không phải* tần số riêng ($\omega_0$). Biên độ không đổi theo thời gian. |
| **Cộng hưởng** | `biên độ cực đại`, `I max`, `hệ số cản nhỏ` | Xảy ra khi: Tần số ngoại lực = Tần số riêng ($\Omega = \omega_0$). Lực cản càng nhỏ, đỉnh cộng hưởng càng cao/nhọn. |

### 2. Sóng Cơ & Sóng Âm
| Loại sóng | Định nghĩa (Hướng dao động vs. Hướng truyền) | Ví dụ điển hình |
| :--- | :--- | :--- |
| **Sóng Ngang** | Vuông góc ($\perp$) | Sóng nước, Sóng trên dây, **Sóng điện từ**. |
| **Sóng Dọc** | Trùng / Song song ($||$) | Dao động lò xo dọc, **Sóng âm** (không khí). |
| **Hạ âm** | $f < 20$ Hz | Tai người không nghe được. |
| **Siêu âm** | $f > 20.000$ Hz | Tai người không nghe được. |
| **Nghe được** | $20$ Hz $\le f \le 20.000$ Hz | Tai người nghe được. |

### 3. Sóng Điện từ
*   **Môi trường:** Truyền được trong chân không (khác sóng cơ). Vận tốc trong chân không là lớn nhất ($c = 3.10^8$ m/s).
*   **Tam diện thuận:** 3 vector $\vec{E}, \vec{H}, \vec{v}$ vuông góc từng đôi một.
*   **Pha dao động:** Tại một điểm, $\vec{E}$ và $\vec{H}$ luôn dao động **CÙNG PHA** (cùng cực đại, cùng cực tiểu). *Lưu ý: Đây là điểm sinh viên hay sai nhất.*

---

## PHẦN B: BẢNG SO SÁNH TƯƠNG TỰ (ANALOGY MAPPING)
*Rất nhiều câu trắc nghiệm hỏi về sự tương quan giữa Cơ và Điện. Học 1 được 2 nhờ bảng này.*

| Đại lượng Dao động Cơ (Con lắc lò xo) | Đại lượng Dao động Điện từ (Mạch LC) | Ghi chú |
| :--- | :--- | :--- |
| Li độ $x$ | Điện tích $q$ | Biến thiên điều hòa |
| Vận tốc $v = x'$ | Dòng điện $i = q'$ | $i$ sớm pha $\pi/2$ so với $q$ |
| Khối lượng $m$ (quán tính) | Độ tự cảm $L$ (quán tính điện từ) | |
| Độ cứng $k$ (lực đàn hồi) | Nghịch đảo điện dung $1/C$ | |
| Lực ma sát/cản $r$ | Điện trở $R$ | Gây tắt dần |
| Động năng $W_đ = \frac{1}{2}mv^2$ | Năng lượng từ trường $W_m = \frac{1}{2}Li^2$ | Tập trung ở cuộn cảm |
| Thế năng $W_t = \frac{1}{2}kx^2$ | Năng lượng điện trường $W_e = \frac{1}{2}\frac{q^2}{C}$ | Tập trung ở tụ điện |

---

## PHẦN C: "BẪY" VÀ NGOẠI LỆ (TRAP DETECTION)
*Những chỗ này giảng viên rất thích ra đề để lừa sinh viên đọc lướt.*

1.  **Bẫy về sự truyền vật chất:**
    *   *Sai:* Sóng truyền các phần tử vật chất đi xa.
    *   *Đúng:* Sóng chỉ truyền **pha dao động** và **năng lượng**. Các phần tử vật chất chỉ dao động tại chỗ quanh vị trí cân bằng.

2.  **Bẫy về Vuông góc vs. Cùng pha trong Sóng điện từ:**
    *   Về **không gian**: $\vec{E}$ vuông góc $\vec{B}$.
    *   Về **thời gian**: $\vec{E}$ và $\vec{B}$ biến thiên **cùng pha** (tỉ lệ thuận với nhau).
    *   *Câu lừa:* "Trong sóng điện từ, điện trường trễ pha $\pi/2$ so với từ trường" -> **SAI**.

3.  **Bẫy về Tổng hợp dao động (Quỹ đạo chuyển động):**
    *   Hai dao động vuông góc ($\Delta\varphi = \pi/2$): Quỹ đạo là **Elip** (hoặc tròn nếu $A_1=A_2$).
    *   Hai dao động cùng pha/ngược pha ($\Delta\varphi = k\pi$): Quỹ đạo là **Đoạn thẳng**.

4.  **Bẫy về Hiệu ứng Doppler (Dấu cộng hay trừ?):**
    *   Nhớ quy tắc: **Lại gần thì Tần số tăng, Đi xa thì Tần số giảm**.
    *   Máy thu lại gần nguồn: $v + u_M$.
    *   Nguồn lại gần máy thu: mẫu số là $v - u_S$ (để phân số tăng lên).

5.  **Bẫy về chu kỳ năng lượng:**
    *   Vật dao động với chu kỳ $T$, thì Động năng và Thế năng biến thiên với chu kỳ **$T' = T/2$** (tần số gấp đôi).

---

## PHẦN D: BỘ CÂU HỎI GIẢ LẬP (MOCK TEST THEORY)
*Thử che đáp án và giải thích tại sao.*

**Câu 1: Điều nào sau đây là SAI khi nói về sóng cơ?**
A. Sóng cơ mang năng lượng.
B. Sóng cơ có thể giao thoa và nhiễu xạ.
C. Sóng cơ truyền được trong chân không.
D. Sóng cơ là quá trình lan truyền dao động.
> **Đáp án C.** Sóng cơ cần môi trường đàn hồi (rắn, lỏng, khí). Chỉ sóng điện từ mới truyền được trong chân không.

**Câu 2: Trong dao động điện từ tắt dần của mạch RLC, nguyên nhân gây tắt dần là:**
A. Do tụ điện phóng điện.
B. Do cuộn cảm sinh ra dòng tự cảm.
C. Do tỏa nhiệt Joule-Lenz trên điện trở R.
D. Do bức xạ sóng điện từ.
> **Đáp án C.** Điện trở R tiêu thụ năng lượng dưới dạng nhiệt ($Q=I^2Rt$), làm năng lượng toàn phần giảm dần.

**Câu 3: Khi tổng hợp hai dao động điều hòa cùng phương, cùng tần số nhưng vuông pha nhau, quỹ đạo của vật là:**
A. Đường thẳng.
B. Đường tròn.
C. Đường Elip.
D. Đường hình sin.
> **Đáp án C.** (Xem lại công thức 1-56 trong PDF). Chỉ là đường tròn khi biên độ bằng nhau ($A_1=A_2$). Tổng quát là Elip.

**Câu 4: Hiện tượng cộng hưởng xảy ra rõ nét nhất (nhọn nhất) khi:**
A. Lực cản môi trường rất lớn.
B. Lực cản môi trường rất nhỏ.
C. Tần số cưỡng bức lớn hơn nhiều tần số riêng.
D. Biên độ ngoại lực nhỏ.
> **Đáp án B.** Lực cản càng nhỏ, năng lượng tiêu hao ít, biên độ cộng hưởng vọt lên càng cao.

**Câu 5: Trong thí nghiệm Hertz, ta phát hiện sóng điện từ dựa trên nguyên lý:**
A. Điện trường biến thiên sinh ra từ trường xoáy.
B. Từ trường biến thiên sinh ra điện trường xoáy.
C. Cả A và B (Thuyết Maxwell).
D. Hiện tượng quang điện.
> **Đáp án C.** Sóng điện từ hình thành do sự lan truyền của điện từ trường biến thiên (liên kết khăng khít giữa E và B).

**Câu 6: Theo hiệu ứng Doppler, khi nguồn âm chuyển động lại gần người quan sát đứng yên, người đó nghe thấy âm có:**
A. Tần số lớn hơn tần số nguồn phát.
B. Tần số nhỏ hơn tần số nguồn phát.
C. Bước sóng dài hơn.
D. Vận tốc truyền âm lớn hơn.
> **Đáp án A.** Lại gần -> Tần số nghe được tăng lên (Tiếng xe hú to và thanh hơn khi lao tới).

**Câu 7: Phát biểu nào đúng về vector cường độ điện trường $\vec{E}$ và cảm ứng từ $\vec{B}$ trong sóng điện từ phẳng?**
A. Vuông góc với nhau và lệch pha $\pi/2$.
B. Song song với nhau và cùng pha.
C. Vuông góc với nhau và cùng pha.
D. Cùng phương truyền sóng.
> **Đáp án C.** Vuông góc về phương (không gian) nhưng cùng pha về thời gian.

---
**Lời khuyên:** Bạn hãy in tài liệu này ra, kẹp vào giáo trình. Khi đọc lại sách, hãy chú ý các đoạn mình đã đánh dấu trong phần "Giải phẫu" và "Bẫy". Đó là nơi điểm số nằm ở đó.

Chào bạn, tôi đã phân tích xong file PDF **"Chương 2: Giao thoa ánh sáng"**. Đây là chương trọng tâm của phần Quang học sóng.

Khác với Chương 1 (thiên về tính toán chu kỳ/tần số), Chương 2 trong đề thi trắc nghiệm thường đánh mạnh vào **bản chất vật lý** (tại sao vân sáng/tối), **điều kiện biên** (phản xạ có đổi pha hay không) và **ứng dụng thực tế**.

Dưới đây là tài liệu ôn tập chiến lược dành riêng cho Chương 2:

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 2 (GIAO THOA ÁNH SÁNG)

## PHẦN A: "GIẢI PHẪU" TỪ KHÓA & ĐỊNH NGHĨA (THEORY ANATOMY)

### 1. Bản chất ánh sáng & Quang lộ
| Thuật ngữ | Từ khóa nhận diện (Keywords) | Đặc điểm cốt lõi (Cần nhớ để chọn đúng) |
| :--- | :--- | :--- |
| **Sóng ánh sáng** | `Sóng điện từ`, `Sóng ngang`, `E vuông góc B` | Là sóng ngang. Vector sáng là vector điện trường $\vec{E}$. Vận tốc trong chân không $c$ là lớn nhất. |
| **Quang lộ ($L$)** | `L = n.d`, `Chân không`, `Thời gian tương ứng` | Là quãng đường ánh sáng đi trong chân không trong cùng khoảng thời gian nó đi đoạn $d$ trong môi trường $n$. **$L = n.d$**. |
| **Định lý Malus** | `Mặt trực giao`, `Vuông góc tia sáng` | Quang lộ giữa hai mặt trực giao (mặt đầu sóng) là bằng nhau. |
| **Nguồn kết hợp** | `Cùng tần số`, `Hiệu pha không đổi` | Hai nguồn độc lập (2 bóng đèn) **không** giao thoa được vì không kết hợp. Phải tách từ 1 nguồn duy nhất. |

### 2. Các loại Giao thoa (Phân loại để không nhầm công thức)
| Loại giao thoa | Cơ chế tạo vân | Hình dạng vân |
| :--- | :--- | :--- |
| **Khe Young** | Chia mặt sóng (Tách 1 chùm thành 2) | Vân thẳng, song song, cách đều. |
| **Bản mỏng song song** | Chia biên độ (Phản xạ 2 mặt) | **Vân cùng độ nghiêng** (các đường tròn đồng tâm tại vô cực/tiêu diện thấu kính). |
| **Nêm không khí** | Chia biên độ (Bề dày $d$ thay đổi) | **Vân cùng độ dày** (các đường thẳng song song cạnh nêm). |
| **Vân tròn Newton** | Chia biên độ (Thấu kính cong + mặt phẳng) | **Vân cùng độ dày** (các vòng tròn đồng tâm). Tâm thường là vân tối. |

---

## PHẦN B: QUY TẮC "NỬA BƯỚC SÓNG" (THE HALF-WAVE RULE) - *Quan trọng nhất*
*Đây là phần sinh viên hay mất điểm nhất trong lý thuyết giao thoa bản mỏng.*

Trong giao thoa bản mỏng (Nêm, Newton, Màng xà phòng), phải luôn tự hỏi: **"Có sự lệch pha $\pi$ (hay cộng thêm $\lambda/2$) không?"**

*   **Quy tắc:** Khi ánh sáng đi từ môi trường chiết suất **nhỏ** sang môi trường chiết suất **lớn** ($n_1 < n_2$) và bị **phản xạ**:
    *   Pha dao động đổi một lượng $\pi$.
    *   Quang lộ cộng thêm một lượng $\lambda/2$.
*   **Ngược lại ($n_1 > n_2$):** Không đổi pha, không cộng quang lộ.

> **Ví dụ áp dụng:**
> *   **Nêm không khí / Newton:** Tia phản xạ ở mặt trên (thủy tinh -> khí) không đổi pha. Tia phản xạ ở mặt dưới (khí -> thủy tinh) **bị đổi pha**. => Hiệu quang lộ phải cộng thêm $\lambda/2$.
> *   **Hệ quả:** Tại vị trí $d=0$ (đỉnh nêm, điểm tiếp xúc thấu kính), hiệu quang lộ = $\lambda/2$ -> Giao thoa triệt tiêu -> **Vân tối**.

---

## PHẦN C: "BẪY" THƯỜNG GẶP (TRAP DETECTION)

1.  **Bẫy về Màu sắc vân trung tâm:**
    *   Chiếu ánh sáng đơn sắc: Vân trung tâm cùng màu.
    *   Chiếu ánh sáng **trắng**: Vân trung tâm là **Vân sáng trắng**.
    *   Các vân sáng bậc 1, 2... bị tán sắc thành dải cầu vồng: **Tím ở trong (gần vân trung tâm), Đỏ ở ngoài**. (Nhớ: $\lambda_{tím} < \lambda_{đỏ} \rightarrow i_{tím} < i_{đỏ}$).

2.  **Bẫy dịch chuyển hệ vân (Thí dụ 1 trong PDF):**
    *   Nếu đặt một bản mỏng (bề dày $e$, chiết suất $n$) chắn trước khe $S_1$:
    *   Quang lộ tia $S_1$ tăng lên -> Hệ vân dịch chuyển về phía **có đặt bản mỏng** (về phía $S_1$).
    *   Công thức dịch chuyển: $x_0 = \frac{D}{a}(n-1)e$.

3.  **Bẫy về ứng dụng (Ai làm gì?):**
    *   **Giao thoa kế Rayleigh:** Đo chiết suất chất khí/lỏng.
    *   **Giao thoa kế Michelson:** Đo độ dài cực nhỏ, độ giãn nở.
    *   **Vân Newton/Nêm:** Kiểm tra độ phẳng, độ cong bề mặt.
    *   **Khử phản xạ (Lớp phủ ống kính):** Dùng giao thoa **triệt tiêu** (Vân tối). Điều kiện: Bề dày màng mỏng $d_{min} = \lambda / 4n$.

4.  **Bẫy về Vân tối/Sáng trong bản mỏng:**
    *   Khe Young: Hiệu quang lộ $k\lambda$ là Sáng.
    *   Nêm không khí/Newton: Do có cộng thêm $\lambda/2$, nên công thức bị đảo ngược.
        *   $2d + \lambda/2 = k\lambda$ -> Vân tối là $2d = k\lambda$ (xấp xỉ).
        *   *Mẹo:* Đừng học vẹt công thức, hãy nhớ bản chất có bị lệch pha hay không.

---

## PHẦN D: BỘ CÂU HỎI GIẢ LẬP LÝ THUYẾT (MOCK TEST)

**Câu 1: Điều kiện để hai sóng ánh sáng có thể giao thoa được với nhau là:**
A. Hai sóng phải cùng biên độ và cùng pha.
B. Hai sóng xuất phát từ hai nguồn khác nhau nhưng cùng màu.
C. Hai sóng phải là sóng kết hợp (cùng tần số và hiệu pha không đổi).
D. Hai sóng phải là sóng điện từ truyền trong chân không.
> **Đáp án C.** Đây là định nghĩa cơ bản.

**Câu 2: Trong thí nghiệm Young dùng ánh sáng trắng, phát biểu nào sau đây là ĐÚNG?**
A. Vân trung tâm là vân tối.
B. Vân trung tâm là vân sáng trắng, hai bên là các dải màu cầu vồng, tím ở trong, đỏ ở ngoài.
C. Vân trung tâm là vân sáng trắng, hai bên là các dải màu cầu vồng, đỏ ở trong, tím ở ngoài.
D. Toàn bộ trường giao thoa là màu trắng.
> **Đáp án B.** Vì bước sóng đỏ lớn hơn tím, nên khoảng vân đỏ lớn hơn ($i = \lambda D/a$), đỏ sẽ nằm xa vân trung tâm hơn.

**Câu 3: Trong hệ vân tròn Newton (cho ánh sáng phản xạ), tại điểm tiếp xúc giữa thấu kính và bản thủy tinh (tâm hệ vân), ta quan sát thấy:**
A. Một điểm sáng.
B. Một điểm tối.
C. Một điểm có màu cầu vồng.
D. Không xác định được.
> **Đáp án B.** Tại điểm tiếp xúc $d=0$, nhưng do phản xạ tại mặt dưới lớp không khí (trên mặt bản thủy tinh) bị đổi pha $\pi$ (thêm quang lộ $\lambda/2$), nên điều kiện trở thành triệt tiêu -> Vân tối.

**Câu 4: Để khử phản xạ cho kính tiềm vọng hoặc ống kính máy ảnh, người ta mạ lên kính một lớp mỏng trong suốt. Hiện tượng này dựa trên nguyên lý:**
A. Khúc xạ ánh sáng.
B. Phản xạ toàn phần.
C. Giao thoa ánh sáng cho vân tối.
D. Giao thoa ánh sáng cho vân sáng.
> **Đáp án C.** Ta muốn triệt tiêu ánh sáng phản xạ đi vào mắt, nên cần tạo ra giao thoa cực tiểu (vân tối).

**Câu 5: Khi chiếu ánh sáng đơn sắc vào một nêm không khí, nếu tăng góc nghiêng của nêm thì:**
A. Khoảng vân không đổi.
B. Các vân sít lại gần nhau hơn (khoảng vân giảm).
C. Các vân giãn ra xa nhau hơn (khoảng vân tăng).
D. Hệ vân biến mất.
> **Đáp án B.** Khoảng vân $i = \lambda / (2\sin\alpha) \approx \lambda / 2\alpha$. Nếu góc $\alpha$ tăng thì $i$ giảm -> Vân xít lại.

**Câu 6: Trong giao thoa kế Michelson, nếu dịch chuyển gương di động một đoạn bằng $\lambda/4$ thì hiệu quang lộ thay đổi bao nhiêu?**
A. $\lambda/4$
B. $\lambda/2$
C. $\lambda$
D. $2\lambda$
> **Đáp án B.** Ánh sáng đi tới gương và phản xạ trở lại, nên quãng đường thay đổi là $2 \times (\text{đoạn dịch chuyển}) = 2 \times (\lambda/4) = \lambda/2$.

**Câu 7: Hiện tượng giao thoa chứng tỏ ánh sáng có tính chất:**
A. Hạt.
B. Sóng.
C. Lưỡng tính sóng hạt.
D. Truyền thẳng.
> **Đáp án B.** Giao thoa là đặc trưng cơ bản nhất để nhận biết sóng. (Chương sau sẽ học về tính chất hạt).

---
**Lời khuyên:** Chương này rất dễ nhầm lẫn giữa các công thức $k\lambda$ và $(k+0.5)\lambda$ trong các trường hợp bản mỏng. Hãy ghi nhớ quy tắc: **Phản xạ trên môi trường chiết quang hơn thì cộng thêm $\lambda/2$ vào quang lộ**. Chúc bạn ôn tập tốt!

Chào bạn, tôi đã phân tích xong file PDF **"Chương 3: Nhiễu xạ ánh sáng"**.

Chương này là "ác mộng" với nhiều sinh viên vì công thức toán học (tích phân) rất phức tạp. Tuy nhiên, **tin vui cho bạn**: Đề thi trắc nghiệm thường **không** yêu cầu tính tích phân, mà chỉ hỏi về **kết quả cuối cùng** và **hiện tượng vật lý**.

Dưới đây là tài liệu ôn tập chiến lược, tập trung vào lý thuyết và các "bẫy" công thức dễ nhầm lẫn.

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 3 (NHIỄU XẠ ÁNH SÁNG)

## PHẦN A: "GIẢI PHẪU" TỪ KHÓA & ĐỊNH NGHĨA
*Nắm chắc các khái niệm này để loại trừ đáp án nhiễu.*

| Thuật ngữ | Đặc điểm cốt lõi (Keywords) | Phân biệt |
| :--- | :--- | :--- |
| **Nhiễu xạ (Diffraction)** | Ánh sáng bị **lệch phương truyền** thẳng khi gặp vật cản/lỗ nhỏ (kích thước ~ bước sóng). | Khác Khúc xạ (đổi môi trường) và Phản xạ (gặp bề mặt). |
| **Nguyên lý Huygens-Fresnel** | Mỗi điểm trên mặt sóng là nguồn **thứ cấp**. Các sóng này **giao thoa** với nhau. | Bổ sung tính chất "Giao thoa" (biên độ & pha) cho nguyên lý Huygens cũ. |
| **Nhiễu xạ Fresnel** | Nhiễu xạ **sóng cầu** (Nguồn và Màn ở **gần** vật cản). | Dùng phương pháp "Đới cầu Fresnel". |
| **Nhiễu xạ Fraunhofer** | Nhiễu xạ **sóng phẳng** (Nguồn và Màn ở **vô cùng** hoặc dùng thấu kính hội tụ). | Thường gặp: 1 khe hẹp, Cách tử. |

---

## PHẦN B: CÁC CÔNG THỨC & KẾT QUẢ CỐT LÕI (THEORY CHEATSHEET)
*Đây là phần quan trọng nhất. Bạn không cần biết chứng minh, chỉ cần nhớ KẾT QUẢ.*

### 1. Nhiễu xạ qua LỖ TRÒN (Fresnel) - Phương pháp đới cầu
*   **Đới cầu:** Chia mặt sóng thành các vòng tròn đồng tâm.
    *   Diện tích các đới: **Bằng nhau** ($\Delta S \approx \pi R b \lambda / (R+b)$).
    *   Bán kính đới thứ k: $r_k \sim \sqrt{k}$ (Tỉ lệ với căn bậc hai số nguyên).
    *   Hai đới kế tiếp: Ngược pha nhau (triệt tiêu nhau).
*   **Biên độ tại tâm M:** $A_M = \frac{A_1}{2} \pm \frac{A_n}{2}$ (+ nếu n lẻ, - nếu n chẵn).
*   **Quy tắc Sáng/Tối tại tâm:**
    *   Lỗ chứa số **LẺ** đới cầu ($n=1, 3, 5...$) $\rightarrow$ Tâm **SÁNG**.
    *   Lỗ chứa số **CHẴN** đới cầu ($n=2, 4, 6...$) $\rightarrow$ Tâm **TỐI**.
    *   **Đặc biệt:** Nếu lỗ chỉ chứa **1 đới cầu** ($n=1$) $\rightarrow$ Sáng nhất ($I = 4I_0$).

### 2. Nhiễu xạ qua ĐĨA TRÒN (Vật cản tròn)
*   Hiện tượng kỳ lạ (nghịch lý): Tại tâm bóng tối hình học của chiếc đĩa tròn chắn sáng **LUÔN CÓ MỘT ĐIỂM SÁNG**.
*   Lý do: Các sóng từ mép đĩa truyền đến tâm đều đi quãng đường bằng nhau $\rightarrow$ Cùng pha $\rightarrow$ Tăng cường.

### 3. Nhiễu xạ qua 1 KHE HẸP (Fraunhofer) - *Cực kỳ hay thi*
*   **Bề rộng khe:** $b$. Góc nhiễu xạ: $\varphi$.
*   **Điều kiện CỰC TIỂU (Tối):**
    $$b \sin \varphi = k\lambda \quad (k = \pm 1, \pm 2...)$$
    *(Lưu ý: Không có k=0)*
*   **Điều kiện CỰC ĐẠI (Sáng):**
    $$b \sin \varphi = (2k+1)\frac{\lambda}{2}$$
*   **Cực đại giữa (Trung tâm):** Nằm tại $\varphi = 0$. Bề rộng góc rộng gấp đôi các cực đại khác.

### 4. Nhiễu xạ qua CÁCH TỬ (Nhiều khe hẹp)
*   **Chu kỳ cách tử:** $d = b + a$ (bề rộng khe + khoảng cách chắn).
*   **Điều kiện CỰC ĐẠI CHÍNH (Sáng):**
    $$d \sin \varphi = m\lambda \quad (m = 0, \pm 1, \pm 2...)$$
*   **Hệ quả:**
    *   Ánh sáng trắng bị tán sắc thành quang phổ.
    *   Góc lệch màu Đỏ > Góc lệch màu Tím (Khác với khúc xạ qua lăng kính).
    *   Số vạch tối đa quan sát được: $|\sin \varphi| \le 1 \Rightarrow |m| \le \frac{d}{\lambda}$.

---

## PHẦN C: "BẪY" VÀ SỰ NHẦM LẪN (TRAP DETECTION)

1.  **Bẫy ngược dấu (Khe hẹp vs. Giao thoa Young):**
    *   Trong giao thoa Young (2 khe): Hiệu quang lộ $= k\lambda$ là **Vân Sáng**.
    *   Trong nhiễu xạ 1 khe: Hiệu quang lộ ($b \sin \varphi$) $= k\lambda$ là **Vân Tối**.
    *   *Mẹo nhớ:* Nhiễu xạ 1 khe là "kẻ nổi loạn", công thức $k\lambda$ cho cực tiểu thay vì cực đại.

2.  **Bẫy về Đĩa tròn vs. Lỗ tròn:**
    *   Lỗ tròn: Tâm có thể Sáng hoặc Tối (tùy số đới cầu).
    *   Đĩa tròn (vật cản): Tâm **LUÔN LUÔN SÁNG** (dù đĩa to hay nhỏ, miễn là còn nhiễu xạ).

3.  **Bẫy về Cách tử (Cực đại bị thiếu):**
    *   Nếu công thức cực đại chính ($d \sin \varphi = m\lambda$) trùng với công thức cực tiểu của 1 khe ($b \sin \varphi = k\lambda$), thì vạch sáng đó sẽ **BIẾN MẤT**.
    *   Ví dụ: Nếu $d = 2b$, các vạch bậc chẵn $m=2, 4, 6...$ sẽ bị mất.

4.  **Bẫy về Nhiễu xạ tinh thể (Tia X):**
    *   Công thức Bragg: $2d \sin \theta = k\lambda$.
    *   *Lưu ý:* $\theta$ ở đây thường là **góc lướt** (góc hợp bởi tia tới và *mặt phẳng* tinh thể), KHÔNG PHẢI góc tới (hợp bởi tia tới và pháp tuyến). Đọc kỹ đề bài.

---

## PHẦN D: CÂU HỎI LÝ THUYẾT GIẢ LẬP (MOCK TEST)

**Câu 1: Điều kiện để quan sát rõ hiện tượng nhiễu xạ ánh sáng là:**
A. Kích thước vật cản lớn hơn nhiều so với bước sóng.
B. Kích thước vật cản nhỏ hơn hoặc tương đương với bước sóng.
C. Ánh sáng phải là ánh sáng trắng.
D. Vật cản phải trong suốt.
> **Đáp án B.** Đây là điều kiện tiên quyết. Nếu vật cản quá lớn, ta chỉ thấy hiện tượng truyền thẳng (bóng tối rõ rệt).

**Câu 2: Trong hiện tượng nhiễu xạ qua một lỗ tròn nhỏ, tâm của ảnh nhiễu xạ sẽ là:**
A. Luôn luôn sáng.
B. Luôn luôn tối.
C. Sáng hoặc tối tùy thuộc vào số đới cầu Fresnel chứa trong lỗ.
D. Có màu cầu vồng.
> **Đáp án C.** (Xem lại Phần B, mục 1).

**Câu 3: Phát biểu nào sau đây ĐÚNG về hiện tượng nhiễu xạ qua một đĩa tròn nhỏ chắn sáng?**
A. Tâm của bóng đen hình học luôn có một điểm sáng.
B. Tâm của bóng đen luôn tối hoàn toàn.
C. Chỉ có điểm sáng nếu đĩa rất nhỏ (< 1mm).
D. Hiện tượng này không xảy ra với ánh sáng đơn sắc.
> **Đáp án A.** Điểm sáng này gọi là điểm Poisson (hoặc Arago).

**Câu 4: Chiếu ánh sáng đơn sắc vào một khe hẹp có bề rộng $b$. Điều kiện để tại điểm M nhìn dưới góc $\varphi$ có CỰC TIỂU nhiễu xạ là:**
A. $b \sin \varphi = k\lambda$
B. $b \sin \varphi = (2k+1)\lambda/2$
C. $d \sin \varphi = k\lambda$
D. $b \sin \varphi = (k+0,5)\lambda$
> **Đáp án A.** Nhớ kỹ: Nhiễu xạ 1 khe, công thức "đẹp" ($k\lambda$) dành cho Cực Tiểu.

**Câu 5: Khi dùng ánh sáng trắng chiếu vào cách tử nhiễu xạ, quang phổ bậc 1 sẽ:**
A. Có màu tím nằm gần vân trung tâm nhất, màu đỏ xa nhất.
B. Có màu đỏ nằm gần vân trung tâm nhất, màu tím xa nhất.
C. Chỉ có một màu trắng.
D. Các màu chồng chập lên nhau hoàn toàn.
> **Đáp án A.** Từ $d \sin \varphi = \lambda$, vì $\lambda_{tím} < \lambda_{đỏ}$ nên $\sin \varphi_{tím} < \sin \varphi_{đỏ}$. Góc lệch màu tím nhỏ hơn nên nằm trong (gần vân trung tâm).

**Câu 6: Giới hạn độ phân giải của quang cụ (như kính thiên văn) bị hạn chế chủ yếu bởi:**
A. Sự tán sắc ánh sáng.
B. Sự khúc xạ ánh sáng.
C. Hiện tượng nhiễu xạ ánh sáng qua lỗ tròn (vật kính).
D. Sai số chế tạo thấu kính.
> **Đáp án C.** Đây là lý do ta không thể nhìn rõ các vật quá nhỏ hoặc quá xa nhau, do ảnh của một điểm sáng không phải là điểm mà là một đĩa nhiễu xạ (đĩa Airy).

---
**Mẹo cuối cùng:** Với Chương 3, nếu gặp bài tập tính toán, hãy ưu tiên dùng công thức **Cách tử** ($d\sin\varphi = k\lambda$) hoặc **Một khe** ($b\sin\varphi = k\lambda$ cho cực tiểu). Đừng sa đà vào tính bán kính đới cầu Fresnel trừ khi đề hỏi lý thuyết trực tiếp. Chúc bạn thi tốt!

Chào bạn, tôi đã hoàn thành việc phân tích file PDF **"Chương 4: Tán sắc, Hấp thụ và Tán xạ ánh sáng"**.

Đây là chương thiên về **Lý thuyết vật lý** và **Giải thích hiện tượng**. Trong đề thi trắc nghiệm, phần này thường chiếm khoảng 10-15% số câu hỏi và là phần "ăn điểm" nếu bạn nắm chắc bản chất, vì ít tính toán phức tạp.

Dưới đây là tài liệu ôn tập tối ưu hóa cho thi trắc nghiệm Chương 4:

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 4 (TƯƠNG TÁC ÁNH SÁNG - MÔI TRƯỜNG)

## PHẦN A: "GIẢI PHẪU" TỪ KHÓA & ĐỊNH NGHĨA (THEORY ANATOMY)

### 1. Tán sắc ánh sáng (Dispersion)
*   **Định nghĩa:** Là sự phụ thuộc của **chiết suất** ($n$) vào **bước sóng** ($\lambda$) (hoặc tần số) của ánh sáng.
*   **Hệ quả:** Chùm ánh sáng trắng qua lăng kính bị tách thành dải màu (Cầu vồng).
*   **Thứ tự lệch:** Tia **Tím** bị lệch nhiều nhất ($n_{tím}$ lớn nhất), tia **Đỏ** bị lệch ít nhất ($n_{đỏ}$ nhỏ nhất).
    *   $\lambda_{đỏ} > \lambda_{tím} \Rightarrow n_{đỏ} < n_{tím} \Rightarrow D_{đỏ} < D_{tím}$ (Góc lệch).
*   **Công thức Cauchy:** $n = A + \frac{B}{\lambda^2} + ...$ (Chiết suất tỉ lệ nghịch với bình phương bước sóng).

### 2. Hấp thụ ánh sáng (Absorption)
*   **Định luật Bouguer-Lambert:** Cường độ sáng giảm theo hàm mũ khi đi qua môi trường.
    *   $I = I_0 e^{-kl}$ ($k$: hệ số hấp thụ).
*   **Định luật Lambert-Beer (cho dung dịch):** $I = I_0 e^{-\alpha C l}$ (phụ thuộc nồng độ $C$).
*   **Màu sắc vật thể:**
    *   Vật trong suốt: Màu của ánh sáng mà nó **truyền qua** (ít hấp thụ nhất).
    *   Vật đục: Màu của ánh sáng mà nó **phản xạ**.
    *   Hấp thụ mọi màu $\rightarrow$ Màu đen.

### 3. Tán xạ ánh sáng (Scattering)
*   **Nguyên nhân:** Do môi trường **không đồng nhất** về mặt quang học (chiết suất không đều).
*   **Định luật Rayleigh (Quan trọng nhất):** Cường độ tán xạ tỉ lệ nghịch với **lũy thừa bậc 4** của bước sóng.
    $$I \sim \frac{1}{\lambda^4}$$
    *   $\lambda$ càng ngắn (Tím/Lam) $\rightarrow$ Tán xạ càng mạnh.
    *   $\lambda$ càng dài (Đỏ/Vàng) $\rightarrow$ Tán xạ càng yếu (xuyên thấu tốt).

---

## PHẦN B: PHÂN LOẠI CÁC LOẠI TÁN XẠ (BẢNG SO SÁNH)
*Đây là phần dễ bị "lừa" nhất trong đề thi. Hãy học kỹ bảng này.*

| Loại Tán Xạ | Nguyên nhân | Tần số (Bước sóng) | Đặc điểm nhận diện |
| :--- | :--- | :--- | :--- |
| **Tyndall** | Môi trường **vẩn đục** (khói, bụi, sương mù - các hạt nhỏ lơ lửng). | **Không đổi** ($\omega' = \omega_0$) | Giải thích màu khói, đèn pha ô tô trong sương mù. |
| **Phân tử** | Môi trường **sạch**. Do **thăng giáng mật độ** (chuyển động nhiệt). | **Không đổi** ($\omega' = \omega_0$) | Giải thích **màu xanh da trời** (ban ngày) và **màu đỏ** (hoàng hôn). |
| **Raman** | Tương tác với **phân tử** (dao động nội tại). | **THAY ĐỔI** ($\omega' \neq \omega_0$) | Có vạch **Stokes** ($\omega < \omega_0$) và **Đối Stokes** ($\omega > \omega_0$). |
| **Mandelstam-Brillouin** | Tương tác với **sóng âm** trong môi trường. | **THAY ĐỔI** ($\omega' = \omega_0 \pm \Omega$) | Liên quan đến sóng âm tần số $\Omega$. |

---

## PHẦN C: "BẪY" VÀ CÁC CÂU HỎI KHÓ (TRAP DETECTION)

1.  **Bẫy về Tán sắc Thường vs. Dị thường:**
    *   **Tán sắc thường:** $\lambda$ tăng $\rightarrow$ $n$ giảm (Phổ biến, thủy tinh, nước...).
    *   **Tán sắc dị thường:** $\lambda$ tăng $\rightarrow$ $n$ **tăng**. (Xảy ra ở miền có đám hấp thụ mạnh).
    *   *Câu hỏi lừa:* "Chiết suất môi trường luôn giảm khi bước sóng tăng?" $\rightarrow$ SAI (vì có tán sắc dị thường).

2.  **Bẫy về Tán xạ Raman (Stokes vs. Anti-Stokes):**
    *   Vạch Stokes (tần số thấp hơn, bước sóng dài hơn): Cường độ **MẠNH**.
    *   Vạch Đối Stokes (tần số cao hơn, bước sóng ngắn hơn): Cường độ **RẤT YẾU**.
    *   Khoảng cách tần số ($\Delta \omega$) phụ thuộc vào **bản chất môi trường**, KHÔNG phụ thuộc ánh sáng tới.

3.  **Bẫy về Màu sắc bầu trời (Tại sao xanh mà không phải Tím?):**
    *   Theo Rayleigh ($1/\lambda^4$), màu Tím tán xạ mạnh nhất.
    *   Nhưng mắt người nhạy cảm với màu Lam/Xanh hơn $\rightarrow$ Ta thấy bầu trời màu Xanh.
    *   Hoàng hôn màu đỏ: Do ánh sáng đi quãng đường dài, màu xanh bị tán xạ hết, chỉ còn màu đỏ (bước sóng dài) truyền tới mắt.

4.  **Bẫy về Cầu vồng:**
    *   **Cầu vồng chính (Bậc 1):** 1 lần phản xạ trong. **Đỏ ở trên, Tím ở dưới**.
    *   **Cầu vồng phụ (Bậc 2):** 2 lần phản xạ trong. **Tím ở trên, Đỏ ở dưới** (Ngược lại).

---

## PHẦN D: BỘ CÂU HỎI LÝ THUYẾT GIẢ LẬP (MOCK TEST)

**Câu 1: Nguyên nhân chính gây ra hiện tượng tán sắc ánh sáng là:**
A. Do ánh sáng bị phản xạ toàn phần trong lăng kính.
B. Do vận tốc (và chiết suất) của ánh sáng trong môi trường phụ thuộc vào bước sóng.
C. Do ánh sáng bị hấp thụ khi đi qua lăng kính.
D. Do lăng kính nhuộm màu ánh sáng.
> **Đáp án B.** Định nghĩa cốt lõi của tán sắc.

**Câu 2: Phát biểu nào sau đây về định luật Rayleigh (tán xạ) là đúng?**
A. Cường độ ánh sáng tán xạ tỉ lệ thuận với bước sóng.
B. Cường độ ánh sáng tán xạ tỉ lệ nghịch với bình phương bước sóng.
C. Cường độ ánh sáng tán xạ tỉ lệ nghịch với lũy thừa bậc 4 của bước sóng.
D. Ánh sáng đỏ bị tán xạ mạnh hơn ánh sáng tím.
> **Đáp án C.** $I \sim 1/\lambda^4$. Do đó Tím/Lam tán xạ mạnh hơn Đỏ.

**Câu 3: Trong quang phổ tán xạ Raman, vạch Stokes có đặc điểm:**
A. Tần số lớn hơn tần số ánh sáng tới.
B. Tần số nhỏ hơn tần số ánh sáng tới.
C. Tần số bằng tần số ánh sáng tới.
D. Cường độ luôn nhỏ hơn vạch đối Stokes.
> **Đáp án B.** Vạch Stokes ứng với việc photon mất năng lượng cho phân tử ($\omega_{Stokes} = \omega_0 - \Delta\omega$).

**Câu 4: Tại sao đèn tín hiệu cảnh báo nguy hiểm (hoặc đèn sương mù) thường có màu đỏ hoặc vàng?**
A. Vì màu đỏ đẹp mắt.
B. Vì màu đỏ có bước sóng dài, ít bị tán xạ, truyền đi được xa trong sương mù.
C. Vì màu đỏ bị tán xạ mạnh nhất nên dễ nhìn thấy.
D. Vì màu đỏ có năng lượng lớn nhất.
> **Đáp án B.** Dựa trên định luật Rayleigh, bước sóng dài ít bị tán xạ bởi hạt bụi/sương nên xuyên thấu tốt nhất.

**Câu 5: Hiện tượng tán sắc "dị thường" xảy ra khi:**
A. Chiết suất giảm khi bước sóng tăng.
B. Chiết suất tăng khi bước sóng tăng.
C. Chiết suất không đổi theo bước sóng.
D. Ánh sáng truyền trong chân không.
> **Đáp án B.** Ngược lại với quy luật thông thường.

**Câu 6: Theo định luật Lambert-Beer, nếu nồng độ dung dịch tăng gấp đôi (độ dày không đổi) thì cường độ ánh sáng truyền qua sẽ:**
A. Giảm đi 2 lần.
B. Giảm đi một nửa.
C. Giảm theo quy luật hàm mũ.
D. Không đổi.
> **Đáp án C.** Công thức $I = I_0 e^{-\alpha C l}$. C nằm trên số mũ nên sự giảm không phải tuyến tính.

**Câu 7: Ánh sáng tán xạ bầu trời bị phân cực mạnh nhất khi quan sát theo phương nào so với tia tới (từ mặt trời)?**
A. 0 độ (cùng phương).
B. 90 độ (vuông góc).
C. 180 độ (ngược chiều).
D. 45 độ.
> **Đáp án B.** Tại phương vuông góc ($\theta = \pi/2$), ánh sáng tán xạ bị phân cực hoàn toàn.

---
**Lời khuyên:** Chương 4 không khó nhưng nhiều lý thuyết vụn vặt. Bạn chỉ cần nhớ kỹ quy tắc **$1/\lambda^4$ (Rayleigh)** và sự khác biệt về **thay đổi tần số (Raman)** là đã giải quyết được 80% câu hỏi trắc nghiệm của chương này. Chúc bạn ôn tập tốt!

Chào bạn, tôi đã hoàn thành việc phân tích file PDF **"Chương 5: Phân cực ánh sáng"**.

Đây là chương chốt lại phần Quang học sóng. Trong đề thi trắc nghiệm, chương này thường có nhiều câu hỏi lý thuyết "đánh lừa" về các khái niệm mặt phẳng và các điều kiện đặc biệt. Điểm mấu chốt là bạn phải phân biệt được **Ánh sáng tự nhiên** vs **Ánh sáng phân cực** và vai trò của các thiết bị.

Dưới đây là tài liệu ôn tập tối ưu hóa cho thi trắc nghiệm Chương 5:

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 5 (PHÂN CỰC ÁNH SÁNG)

## PHẦN A: "GIẢI PHẪU" TỪ KHÓA & ĐỊNH NGHĨA (THEORY ANATOMY)

### 1. Bản chất sự phân cực
| Thuật ngữ | Đặc điểm cốt lõi (Keywords) | Ghi chú quan trọng |
| :--- | :--- | :--- |
| **Sóng ngang** | Vector $\vec{E} \perp$ phương truyền. | Chỉ sóng ngang mới có hiện tượng phân cực. Sóng dọc (âm thanh) không có. |
| **Ánh sáng tự nhiên** | Vector $\vec{E}$ dao động **đều đặn theo mọi phương**. | Đối xứng trục. (Ví dụ: Mặt trời, đèn dây tóc). |
| **Ánh sáng phân cực (thẳng)** | Vector $\vec{E}$ chỉ dao động theo **một phương xác định**. | Thường tạo ra bởi bản Tuamalin, Nicol, Polaroid. |
| **Mặt phẳng dao động** | Chứa tia sáng và vector $\vec{E}$. | |
| **Mặt phẳng phân cực** | Chứa tia sáng và **vuông góc** với mặt phẳng dao động. | *Lưu ý kỹ: Rất hay bị hỏi ngược.* |

### 2. Định luật Malus (Về cường độ sáng)
*   **Mô hình:** Kính phân cực (P) $\rightarrow$ Kính phân tích (A). Góc giữa 2 quang trục là $\alpha$.
*   **Công thức:** $I_2 = I_1 \cos^2 \alpha$.
    *   Nếu $\alpha = 0$ (Song song): $I_2 = I_1$ (Sáng nhất).
    *   Nếu $\alpha = 90^\circ$ (Vuông góc/Bắt chéo): $I_2 = 0$ (Tối hoàn toàn).
*   **Lưu ý:** Nếu chiếu ánh sáng **tự nhiên** ($I_0$) vào kính phân cực đầu tiên, cường độ giảm đi một nửa: $I_1 = 0.5 I_0$.

### 3. Phân cực do Phản xạ (Định luật Brewster)
*   Khi ánh sáng phản xạ trên bề mặt môi trường trong suốt, nó bị phân cực một phần.
*   **Điều kiện phân cực toàn phần (Góc Brewster $i_B$):**
    *   Công thức: $\tan i_B = n_{21} = \frac{n_2}{n_1}$.
    *   Đặc điểm tia sáng: Tia phản xạ **vuông góc** tia khúc xạ ($i + r = 90^\circ$).
    *   Thành phần: Tia phản xạ chỉ chứa vector $\vec{E}$ vuông góc với mặt phẳng tới.

---

## PHẦN B: PHÂN LOẠI LƯỠNG CHIẾT & BẢN MỎNG (QUARTZ & CALCITE)
*Phần này thường gây rối vì nhiều khái niệm tương tự nhau.*

### 1. Hiện tượng Lưỡng chiết (Double Refraction)
Khi chiếu sáng vào tinh thể (Băng lan/Calcite, Thạch anh), tia sáng tách làm 2:
*   **Tia Thường ($o$ - Ordinary):** Tuân theo định luật khúc xạ. $n_o$ không đổi.
*   **Tia Bất thường ($e$ - Extraordinary):** KHÔNG tuân theo định luật khúc xạ. $n_e$ thay đổi theo hướng.
*   **Quang trục:** Phương mà dọc theo đó $v_o = v_e$ (ánh sáng không bị tách đôi).

### 2. Các loại bản mỏng quang học (Wave Plates)
Dựa vào hiệu quang lộ $\Delta L = (n_o - n_e)d$:

| Loại bản | Hiệu quang lộ $\Delta L$ | Hiệu pha $\Delta \varphi$ | Tác dụng (Khi chiếu AS phân cực thẳng vào) |
| :--- | :--- | :--- | :--- |
| **Bản 1/4 bước sóng** | $(k + 0.5)\frac{\lambda}{2}$ hoặc $\frac{\lambda}{4}$ | $\frac{\pi}{2}$ | Biến đổi thành **Elip** hoặc **Tròn** (nếu góc tới $45^\circ$). |
| **Bản 1/2 bước sóng** | $(k + 0.5)\lambda$ hoặc $\frac{\lambda}{2}$ | $\pi$ | Vẫn là phân cực thẳng, nhưng **quay mặt phẳng dao động** một góc $2\alpha$. |
| **Bản 1 bước sóng** | $k\lambda$ | $2\pi$ | Không đổi (Vẫn là phân cực thẳng như cũ). |

### 3. Lăng kính Nicol (Thiết bị tạo AS phân cực)
*   Cấu tạo: Tinh thể Băng lan cắt đôi, dán bằng nhựa Canada ($n=1.55$).
*   Cơ chế:
    *   Tia thường ($n_o = 1.66 > 1.55$): Bị **phản xạ toàn phần** và bị hấp thụ ở sơn đen.
    *   Tia bất thường ($n_e = 1.48 < 1.55$): **Truyền qua** được.
    *   **Kết quả:** Cho ra 1 chùm tia phân cực toàn phần (tia $e$).

---

## PHẦN C: "BẪY" VÀ CÁC CÂU HỎI KHÓ (TRAP DETECTION)

1.  **Bẫy về Cường độ sáng qua hệ kính:**
    *   *Câu hỏi:* Chiếu ánh sáng tự nhiên cường độ $I_0$ qua hệ 2 kính phân cực hợp nhau góc $\alpha$. Cường độ đầu ra là bao nhiêu?
    *   *Sai lầm:* Áp dụng ngay $I_0 \cos^2 \alpha$.
    *   *Đúng:* Qua kính 1 mất 50% $\rightarrow$ $0.5 I_0$. Qua kính 2 mới dùng Malus $\rightarrow$ **$I = 0.5 I_0 \cos^2 \alpha$**.

2.  **Bẫy về Bản 1/4 bước sóng:**
    *   Bản $\lambda/4$ chỉ tạo ra ánh sáng **Phân cực tròn** KHI VÀ CHỈ KHI góc giữa vector sáng tới và quang trục là **$45^\circ$**.
    *   Nếu góc khác $45^\circ$ $\rightarrow$ Phân cực **Elip**.
    *   Nếu góc là $0^\circ$ hoặc $90^\circ$ $\rightarrow$ Vẫn là phân cực **Thẳng**.

3.  **Bẫy về khái niệm "Quang trục":**
    *   Quang trục của tinh thể lưỡng chiết **không phải là một đường thẳng cố định**, mà là một **phương** (hướng). Mọi đường thẳng song song với phương này đều là quang trục.

4.  **Bẫy về Góc Brewster:**
    *   $\tan i_B = n_2/n_1$. Nếu ánh sáng đi từ không khí ($n_1=1$) vào thủy tinh ($n_2=n$), thì $\tan i_B = n$.
    *   Nếu đi từ thủy tinh ra không khí: $\tan i_B = 1/n$. (Đọc kỹ đề bài xem ánh sáng đi từ đâu).

---

## PHẦN D: BỘ CÂU HỎI LÝ THUYẾT GIẢ LẬP (MOCK TEST)

**Câu 1: Hiện tượng phân cực ánh sáng chứng tỏ ánh sáng là:**
A. Sóng dọc.
B. Sóng ngang.
C. Hạt.
D. Sóng cơ học.
> **Đáp án B.** Đây là câu hỏi kinh điển nhất của chương này.

**Câu 2: Trong định luật Malus, nếu quay kính phân tích một góc $360^\circ$ quanh tia sáng thì cường độ sáng sau kính phân tích sẽ:**
A. Không đổi.
B. Triệt tiêu 1 lần.
C. Triệt tiêu 2 lần và cực đại 2 lần.
D. Triệt tiêu 4 lần.
> **Đáp án C.** Hàm $\cos^2 \alpha$ biến thiên tuần hoàn với chu kỳ $\pi$ ($180^\circ$). Trong $360^\circ$ có 2 lần cực đại ($0, 180$) và 2 lần cực tiểu ($90, 270$).

**Câu 3: Khi ánh sáng tự nhiên chiếu tới mặt phân cách giữa hai môi trường dưới góc tới Brewster thì:**
A. Tia khúc xạ bị phân cực toàn phần.
B. Tia phản xạ bị phân cực toàn phần.
C. Cả tia phản xạ và khúc xạ đều phân cực toàn phần.
D. Tia phản xạ biến mất.
> **Đáp án B.** Tia khúc xạ chỉ phân cực một phần (mạnh nhất tại điểm này nhưng chưa toàn phần).

**Câu 4: Bản chất của hiện tượng lưỡng chiết là do:**
A. Sự hấp thụ ánh sáng khác nhau theo các phương.
B. Tinh thể có hai chiết suất khác nhau đối với tia thường và tia bất thường.
C. Sự phản xạ toàn phần bên trong tinh thể.
D. Sự nhiễu xạ ánh sáng qua mạng tinh thể.
> **Đáp án B.** $n_o \neq n_e$ do tính dị hướng của tinh thể. (Câu A là nguyên nhân của bản Tuamalin/Polaroid - tính lưỡng sắc/hấp thụ dị hướng, khác với lưỡng chiết).

**Câu 5: Để biến ánh sáng phân cực thẳng thành ánh sáng phân cực tròn, ta cần dùng:**
A. Bản 1/2 bước sóng.
B. Bản 1/4 bước sóng đặt sao cho quang trục hợp với vector sáng tới góc $45^\circ$.
C. Bản 1/4 bước sóng đặt sao cho quang trục song song với vector sáng tới.
D. Lăng kính Nicol.
> **Đáp án B.** Phải thỏa mãn cả 2 điều kiện: $\lambda/4$ và góc $45^\circ$.

**Câu 6: Chất hoạt quang (như dung dịch đường) có khả năng:**
A. Biến ánh sáng trắng thành đơn sắc.
B. Làm quay mặt phẳng phân cực của ánh sáng truyền qua nó.
C. Tạo ra hiện tượng lưỡng chiết.
D. Hấp thụ hoàn toàn ánh sáng phân cực.
> **Đáp án B.** Ứng dụng trong đường kế (Saccharimeter) để đo nồng độ đường. Góc quay $\varphi = [\alpha]Cd$.

**Câu 7: Trong lăng kính Nicol, tia nào bị loại bỏ (hấp thụ/phản xạ đi) và tia nào ló ra ngoài?**
A. Tia thường ló ra, tia bất thường bị loại.
B. Tia bất thường ló ra, tia thường bị loại.
C. Cả hai tia đều ló ra nhưng lệch phương nhau.
D. Cả hai tia đều bị hấp thụ một phần.
> **Đáp án B.** Nhựa Canada có $n=1.55$, nằm giữa $n_e$ và $n_o$. Tia thường có $n_o > n_{keo}$ nên dễ bị phản xạ toàn phần và bị loại bỏ.

---
**Lời khuyên:** Hãy chú ý đến các bài tập về **Hiệu ứng Kerr** (Lưỡng chiết nhân tạo) và **Đường kế** (Công thức quay mặt phẳng phân cực), đây là những phần lý thuyết ứng dụng hay xuất hiện trong các câu hỏi phân loại điểm cao. Chúc bạn hoàn thành tốt môn học!

Chào bạn, tôi đã nghiên cứu kỹ file PDF **"Chương 6: Thuyết Tương đối hẹp Einstein"**.

Đây là một chương rất đặc thù. Nếu các chương trước (như Giao thoa, Nhiễu xạ) nặng về hiện tượng thực tế, thì chương này nặng về **tư duy trừu tượng** và **thay đổi quan niệm** về không gian - thời gian.

Trong thi trắc nghiệm, các câu hỏi chương này thường "đánh lừa" sinh viên bằng cách dùng các kiến thức của cơ học cổ điển (Newton) để gài bẫy.

Dưới đây là tài liệu ôn tập chiến lược dành riêng cho Chương 6:

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 6 (THUYẾT TƯƠNG ĐỐI HẸP)

## PHẦN A: "GIẢI PHẪU" TỪ KHÓA & TIÊN ĐỀ (THEORY ANATOMY)
*Nắm chắc 2 tiên đề là chìa khóa giải quyết 50% câu hỏi lý thuyết.*

### 1. Cơ sở lý thuyết
*   **Phạm vi áp dụng:**
    *   Cơ học Newton (Cổ điển): Đúng khi vận tốc nhỏ ($v \ll c$).
    *   Thuyết tương đối hẹp: Đúng với **mọi vận tốc**, kể cả vận tốc rất lớn ($v \approx c$).
*   **Không gian & Thời gian:**
    *   Newton: Tuyệt đối, độc lập với vật chất và chuyển động.
    *   Einstein: **Tương đối**, phụ thuộc vào hệ quy chiếu và chuyển động. Không gian và thời gian liên kết với nhau.

### 2. Hai tiên đề Einstein (Cực kỳ quan trọng)
| Tiên đề | Nội dung cốt lõi (Keywords để khoanh) | Ý nghĩa |
| :--- | :--- | :--- |
| **1. Nguyên lý tương đối** | Các định luật vật lý **như nhau** trong mọi hệ quy chiếu **quán tính**. | Không có hệ quán tính nào ưu việt hơn hệ nào. |
| **2. Nguyên lý vận tốc ánh sáng** | Vận tốc ánh sáng trong chân không ($c$) là **bất biến** (hằng số). | $c = 3.10^8$ m/s. Không phụ thuộc vào vận tốc nguồn phát hay người quan sát. |

---

## PHẦN B: CÁC HỆ QUẢ CỦA PHÉP BIẾN ĐỔI LORENTZ (CONSEQUENCES)
*Đây là phần sinh viên hay nhầm lẫn nhất: Cái nào ngắn lại? Cái nào dài ra?*

Quy tắc nhớ nhanh: **"Động ngắn, Tĩnh nhanh"** (Vật chuyển động thì ngắn lại, đồng hồ chuyển động thì chạy chậm đi).

### 1. Sự co ngắn của độ dài (Length Contraction)
*   **Hiện tượng:** Một vật chuyển động dọc theo trục của nó sẽ có chiều dài ngắn hơn khi nó đứng yên.
*   **Công thức:** $\ell = \ell_0 \sqrt{1 - \frac{v^2}{c^2}}$
    *   $\ell_0$: Chiều dài nghỉ (đo trong hệ vật đứng yên) $\rightarrow$ **Dài nhất**.
    *   $\ell$: Chiều dài tương đối tính (đo khi vật chuyển động) $\rightarrow$ Ngắn hơn.
*   **Lưu ý:** Chỉ co ngắn theo **phương chuyển động**. Kích thước theo phương vuông góc không đổi.
    *   *Ví dụ:* Hình cầu chuyển động nhanh $\rightarrow$ Hình elipxoit dẹt.

### 2. Sự giãn của thời gian (Time Dilation)
*   **Hiện tượng:** Đồng hồ chuyển động chạy chậm hơn đồng hồ đứng yên.
*   **Công thức:** $\Delta t' = \Delta t \sqrt{1 - \frac{v^2}{c^2}}$ (Theo ký hiệu trong PDF của bạn).
    *   *Cách hiểu đơn giản:* Thời gian trôi đi trên tàu vũ trụ (hệ chuyển động) sẽ **ít hơn** thời gian trôi đi trên Trái Đất (hệ đứng yên).
    *   Nếu phi hành gia đi 1 năm (theo đồng hồ trên tàu), thì ở Trái Đất đã trôi qua > 1 năm.

### 3. Tính tương đối của sự đồng thời
*   Hai biến cố xảy ra **đồng thời** ở hệ K (đứng yên) thì **KHÔNG đồng thời** ở hệ K' (chuyển động), trừ khi chúng xảy ra tại cùng một vị trí.
*   **Quan hệ nhân quả:** Tuy nhiên, nếu biến cố A là nguyên nhân của biến cố B (A xảy ra trước B), thì trật tự này được **bảo toàn** trong mọi hệ quy chiếu (A luôn trước B).

---

## PHẦN C: ĐỘNG LỰC HỌC TƯƠNG ĐỐI (DYNAMICS)
*Phần này nhiều công thức, cần nhớ sự khác biệt với cơ học Newton.*

### 1. Khối lượng tương đối tính
*   Khối lượng không hằng định mà tăng theo vận tốc.
*   $m = \frac{m_0}{\sqrt{1 - v^2/c^2}}$
    *   $m_0$: Khối lượng nghỉ (khi $v=0$).
    *   Khi $v \to c$ thì $m \to \infty$ (vô cùng). $\Rightarrow$ Không thể gia tốc vật có khối lượng đạt vận tốc ánh sáng.

### 2. Năng lượng (Hệ thức Einstein)
Đây là công thức nổi tiếng nhất, cần nhớ kỹ các dạng biến thể:

| Đại lượng | Công thức | Ghi chú |
| :--- | :--- | :--- |
| **Năng lượng toàn phần** | $E = mc^2$ | Bao gồm cả năng lượng nghỉ và động năng. |
| **Năng lượng nghỉ** | $E_0 = m_0 c^2$ | Năng lượng tiềm ẩn khi vật đứng yên. |
| **Động năng ($E_đ$)** | $E_đ = E - E_0 = (m - m_0)c^2$ | **Tuyệt đối KHÔNG dùng $\frac{1}{2}mv^2$**. |
| **Hệ thức năng lượng - động lượng** | $E^2 = (m_0c^2)^2 + (pc)^2$ | Liên hệ $E$ và $p$. |

---

## PHẦN D: "BẪY" TRẮC NGHIỆM CẦN TRÁNH (TRAP DETECTION)

1.  **Bẫy về cộng vận tốc:**
    *   *Câu lừa:* "Hai xe đi ngược chiều, mỗi xe vận tốc $0.8c$. Vận tốc tương đối là $1.6c$."
    *   *Sự thật:* Sai. Vận tốc tương đối không bao giờ vượt quá $c$. Phải dùng công thức cộng vận tốc Einstein (dù không bắt tính phức tạp, nhưng phải biết $v < c$).

2.  **Bẫy về sự co độ dài:**
    *   *Câu lừa:* "Một thanh thước mét chuyển động ngang trước mặt bạn. Bạn thấy bề ngang của nó nhỏ hơn."
    *   *Sự thật:* Sai. Chỉ co ngắn theo **phương chuyển động**. Bề ngang (vuông góc chuyển động) giữ nguyên.

3.  **Bẫy về Động năng:**
    *   *Câu lừa:* "Tính động năng vật chuyển động với $v=0.8c$ bằng công thức $W_đ = \frac{1}{2}mv^2$."
    *   *Sự thật:* Sai hoàn toàn. Phải dùng $E_đ = mc^2 - m_0c^2$. Công thức $\frac{1}{2}mv^2$ chỉ là trường hợp giới hạn khi $v \ll c$.

4.  **Bẫy về Photon:**
    *   Photon (hạt ánh sáng) có khối lượng nghỉ $m_0 = 0$. Nó luôn chuyển động với vận tốc $c$.

---

## PHẦN E: BỘ CÂU HỎI LÝ THUYẾT GIẢ LẬP (MOCK TEST)

**Câu 1: Theo thuyết tương đối hẹp, phát biểu nào sau đây là ĐÚNG về vận tốc ánh sáng?**
A. Phụ thuộc vào vận tốc của nguồn phát.
B. Phụ thuộc vào phương truyền sóng.
C. Có giá trị $c$ đối với mọi hệ quy chiếu quán tính.
D. Có giá trị vô cùng lớn.
> **Đáp án C.** Đây là tiên đề thứ 2 của Einstein.

**Câu 2: Một vật có khối lượng nghỉ $m_0$. Khi vật chuyển động với vận tốc $v$, khối lượng tương đối tính $m$ của nó sẽ:**
A. Luôn bằng $m_0$.
B. Luôn nhỏ hơn $m_0$.
C. Luôn lớn hơn $m_0$.
D. Bằng 0.
> **Đáp án C.** $m = m_0 / \sqrt{1-v^2/c^2}$. Vì mẫu số < 1 nên $m > m_0$.

**Câu 3: Hệ thức liên hệ giữa năng lượng toàn phần $E$ và khối lượng tương đối tính $m$ là:**
A. $E = \frac{1}{2}mv^2$
B. $E = m_0c^2$
C. $E = mc^2$
D. $E = (m - m_0)c^2$
> **Đáp án C.** Hệ thức Einstein nổi tiếng. (Câu D là động năng).

**Câu 4: Hiện tượng "co ngắn Lorenz" xảy ra theo phương nào?**
A. Mọi phương của vật.
B. Chỉ phương vuông góc với chuyển động.
C. Chỉ phương trùng với phương chuyển động.
D. Không xảy ra, kích thước là tuyệt đối.
> **Đáp án C.**

**Câu 5: Nếu bạn di chuyển với vận tốc gần bằng vận tốc ánh sáng đi xa Trái Đất rồi quay trở về. So với người bạn sinh đôi ở lại Trái Đất, bạn sẽ:**
A. Già hơn.
B. Trẻ hơn.
C. Bằng tuổi nhau.
D. Không so sánh được.
> **Đáp án B.** Do sự giãn thời gian (nghịch lý anh em sinh đôi). Đồng hồ trên tàu chạy chậm hơn đồng hồ Trái Đất.

**Câu 6: Nguyên nhân chính dẫn đến sự ra đời của thuyết tương đối là:**
A. Sự mâu thuẫn giữa cơ học Newton và thuyết điện từ Maxwell về tính bất biến của vận tốc ánh sáng.
B. Sự phát hiện ra sóng hấp dẫn.
C. Sự sai lệch trong tính toán quỹ đạo các hành tinh.
D. Nhu cầu chế tạo bom nguyên tử.
> **Đáp án A.** (Được đề cập ngay phần mở đầu PDF). Cơ học Newton cho rằng vận tốc cộng thêm được, Maxwell bảo $c$ là hằng số.

---
**Lời khuyên:** Chương này rất ngắn gọn trong giáo trình của bạn (chỉ khoảng 15 trang). Hãy đọc kỹ phần **6.3.3 Các hệ quả (Năng lượng)** trong PDF vì đây là nơi tập trung nhiều công thức dễ nhầm lẫn nhất. Chúc bạn ôn thi tốt!

Chào bạn, tôi đã hoàn thành việc phân tích file PDF **"Chương 7: Quang học lượng tử"**.

Đây là chương đánh dấu bước chuyển mình từ Vật lý cổ điển sang Vật lý hiện đại. Đối với thi trắc nghiệm, chương này cực kỳ quan trọng vì nó chứa nhiều định luật, các hệ quả thực nghiệm và các giả thuyết nền tảng.

Dưới đây là tài liệu ôn tập được tối ưu hóa cho thi trắc nghiệm, tập trung sâu vào lý thuyết và các bẫy tư duy thường gặp.

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 7 (QUANG HỌC LƯỢNG TỬ)

## PHẦN A: "GIẢI PHẪU" TỪ KHÓA & ĐỊNH NGHĨA (THEORY ANATOMY)

### 1. Bức xạ nhiệt & Vật đen tuyệt đối
| Thuật ngữ | Đặc điểm cốt lõi (Keywords) | Ghi chú quan trọng |
| :--- | :--- | :--- |
| **Bức xạ nhiệt cân bằng** | Phát xạ = Hấp thụ. Nhiệt độ vật không đổi. | Là trạng thái lý tưởng để áp dụng các định luật. |
| **Hệ số hấp thụ đơn sắc ($a_{\lambda, T}$)** | Tỷ số năng lượng hấp thụ / năng lượng tới. | Luôn $\le 1$. |
| **Vật đen tuyệt đối** | Hấp thụ **toàn bộ** bức xạ chiếu tới ($a_{\lambda, T} = 1$). | Không phụ thuộc bản chất vật, chỉ phụ thuộc nhiệt độ. Mô hình: Cái lỗ nhỏ của bình kín. |
| **Định luật Kirchhoff** | Tỷ số $r_{\lambda, T} / a_{\lambda, T} = f(\lambda, T)$ (Hàm phổ biến). | Vật nào hấp thụ mạnh thì phát xạ mạnh. |

### 2. Các định luật về Vật đen tuyệt đối (Dễ nhầm công thức)
*   **Định luật Stephan-Boltzmann:** Năng suất phát xạ toàn phần tỉ lệ với luỹ thừa 4 của nhiệt độ.
    $$R_T = \sigma T^4$$
    *   *Hệ quả trắc nghiệm:* Nếu $T$ tăng 2 lần $\rightarrow$ Năng lượng phát ra tăng $2^4 = 16$ lần.
*   **Định luật Wien:** Bước sóng mang nhiều năng lượng nhất ($\lambda_{max}$) tỉ lệ nghịch với nhiệt độ.
    $$\lambda_{max} = \frac{b}{T}$$
    *   *Hệ quả trắc nghiệm:* Khi vật nóng lên (T tăng), màu sắc chuyển dần về phía tím (bước sóng ngắn lại).

### 3. Thuyết lượng tử & Photon
*   **Giả thuyết Planck:** Năng lượng trao đổi không liên tục mà ngắt quãng thành các gói (lượng tử) $\varepsilon = h\nu$. $\rightarrow$ Giải quyết "Sự khủng hoảng vùng tử ngoại".
*   **Thuyết Photon (Einstein):**
    *   Ánh sáng là chùm hạt (photon).
    *   Photon luôn chuyển động với vận tốc $c$.
    *   **Khối lượng nghỉ của photon bằng 0**. (Rất hay hỏi).
    *   Năng lượng $\varepsilon = h\nu = hc/\lambda$. Động lượng $p = h/\lambda$.

---

## PHẦN B: HIỆN TƯỢNG QUANG ĐIỆN (TRỌNG TÂM THI)
*Phần này chiếm tỉ trọng lớn nhất trong các câu hỏi trắc nghiệm của chương.*

### 1. Cơ chế và Định luật
*   **Bản chất:** Photon bắn vào $\rightarrow$ Electron bật ra (1 đổi 1).
*   **3 Định luật quang điện:**
    1.  **Về điều kiện:** Phải có $\lambda \le \lambda_0$ (Giới hạn quang điện). $\lambda_0$ chỉ phụ thuộc vào **bản chất kim loại** (Công thoát $A$).
    2.  **Về cường độ dòng:** $I_{bão hòa}$ tỉ lệ thuận với **Cường độ chùm sáng** (số lượng photon).
    3.  **Về động năng ($v_{0max}$):** Động năng ban đầu cực đại **KHÔNG** phụ thuộc cường độ sáng, chỉ phụ thuộc vào **bước sóng (tần số)** ánh sáng tới.

### 2. Phương trình Einstein (Cần nhớ để biện luận)
$$h\nu = A + W_{d(max)} = A + \frac{1}{2}mv_{0max}^2$$
*   Năng lượng photon cung cấp = Công thoát + Động năng bắn ra.
*   **Hiệu điện thế hãm ($U_h$ hoặc $U_c$):** Là hiệu điện thế để triệt tiêu dòng quang điện.
    $$|eU_h| = W_{d(max)}$$

---

## PHẦN C: HIỆU ỨNG COMPTON (TÁN XẠ TIA X)
*Chứng minh hùng hồn nhất cho tính chất HẠT của ánh sáng.*

*   **Hiện tượng:** Tia X va chạm với electron **tự do**.
*   **Kết quả:** Tia X bị tán xạ, bước sóng bị **dài ra** ($\lambda' > \lambda$).
*   **Độ biến thiên ($\Delta \lambda$):**
    $$\Delta \lambda = \lambda' - \lambda = \lambda_c (1 - \cos \theta) = 2\lambda_c \sin^2(\frac{\theta}{2})$$
    *   $\Delta \lambda$ **chỉ phụ thuộc vào góc tán xạ $\theta$**.
    *   **KHÔNG** phụ thuộc vào bước sóng tới.
    *   **KHÔNG** phụ thuộc vào bản chất vật liệu làm bia.
*   **Giải thích:** Va chạm đàn hồi giữa photon và electron (như 2 quả bida). Photon truyền một phần năng lượng cho electron $\rightarrow$ Năng lượng giảm $\rightarrow$ Bước sóng tăng.

---

## PHẦN D: "BẪY" VÀ CÁC CÂU HỎI KHÓ (TRAP DETECTION)

1.  **Bẫy về Cường độ sáng vs. Động năng (Quang điện):**
    *   *Câu lừa:* "Tăng cường độ chùm sáng kích thích thì động năng ban đầu của electron tăng." $\rightarrow$ **SAI**.
    *   *Sự thật:* Tăng cường độ sáng $\rightarrow$ Tăng số lượng photon $\rightarrow$ Tăng số electron bật ra $\rightarrow$ Tăng **dòng quang điện bão hòa**. Động năng **không đổi**.

2.  **Bẫy về Vật đen tuyệt đối:**
    *   *Câu lừa:* "Vật đen tuyệt đối là vật có màu đen." $\rightarrow$ **SAI**.
    *   *Sự thật:* Mặt trời, lò nung, dây tóc bóng đèn đang sáng chói vẫn được coi gần đúng là vật đen tuyệt đối vì chúng hấp thụ hầu hết bức xạ chiếu vào (qua lỗ nhỏ của lò).

3.  **Bẫy về Compton vs. Quang điện:**
    *   Quang điện: Photon biến mất hoàn toàn (bị hấp thụ toàn bộ năng lượng). (Xảy ra với ánh sáng khả kiến/tử ngoại, electron liên kết).
    *   Compton: Photon không mất đi, chỉ đổi hướng và giảm năng lượng. (Xảy ra với tia X/Gamma, electron tự do).

4.  **Bẫy về vận tốc Photon:**
    *   Photon luôn bay với vận tốc $c$ trong chân không. Không có photon đứng yên. Không thể làm chậm photon (chỉ có thể làm giảm năng lượng/tần số).

---

## PHẦN E: BỘ CÂU HỎI LÝ THUYẾT GIẢ LẬP (MOCK TEST)

**Câu 1: Theo định luật Wien, khi nhiệt độ của vật đen tuyệt đối tăng lên thì:**
A. Năng suất phát xạ toàn phần giảm.
B. Bước sóng ứng với năng suất phát xạ cực đại tăng lên.
C. Bước sóng ứng với năng suất phát xạ cực đại giảm đi.
D. Vật chuyển sang màu đỏ sẫm.
> **Đáp án C.** ($\lambda_{max} = b/T$, $T$ tăng thì $\lambda$ giảm - dịch về phía tím/tử ngoại).

**Câu 2: Giới hạn quang điện $\lambda_0$ của một kim loại phụ thuộc vào:**
A. Cường độ chùm sáng kích thích.
B. Bước sóng của ánh sáng kích thích.
C. Bản chất của kim loại đó.
D. Thời gian chiếu sáng.
> **Đáp án C.** $\lambda_0 = hc/A$. $A$ là công thoát, đặc trưng riêng cho từng kim loại.

**Câu 3: Trong hiệu ứng Compton, độ biến thiên bước sóng $\Delta \lambda$ phụ thuộc vào:**
A. Bước sóng của chùm tia tới.
B. Bản chất của vật liệu làm bia tán xạ.
C. Góc tán xạ.
D. Cả A và B.
> **Đáp án C.** (Xem lại công thức Compton trong Phần C).

**Câu 4: Phát biểu nào sau đây SAI khi nói về photon?**
A. Photon mang năng lượng.
B. Photon có khối lượng nghỉ bằng 0.
C. Photon chuyển động với vận tốc ánh sáng.
D. Năng lượng của photon tỉ lệ thuận với bước sóng.
> **Đáp án D.** Sai. Năng lượng tỉ lệ thuận với tần số ($\varepsilon = h\nu$) và **tỉ lệ nghịch** với bước sóng ($\varepsilon = hc/\lambda$).

**Câu 5: Để gây ra hiện tượng quang điện, điều kiện là:**
A. Tần số của ánh sáng kích thích phải nhỏ hơn giới hạn quang điện.
B. Bước sóng của ánh sáng kích thích phải nhỏ hơn hoặc bằng giới hạn quang điện.
C. Cường độ ánh sáng phải đủ lớn.
D. Thời gian chiếu phải đủ lâu.
> **Đáp án B.** Điều kiện $\lambda \le \lambda_0$.

**Câu 6: Tại sao hệ thức Rayleigh-Jeans dẫn đến "Sự khủng hoảng vùng tử ngoại"?**
A. Vì nó dự đoán năng lượng bức xạ tiến tới vô cùng khi bước sóng nhỏ (tần số lớn).
B. Vì nó không áp dụng được cho vùng hồng ngoại.
C. Vì nó sai về đơn vị đo.
D. Vì nó cho rằng năng lượng là gián đoạn.
> **Đáp án A.** Công thức cổ điển dự đoán năng lượng tỉ lệ với $T \nu^2$, khi $\nu \to \infty$ thì năng lượng vô hạn -> Vô lý.

---
**Lời khuyên:** Hãy học thuộc các công thức hệ quả (tỉ lệ thuận/nghịch) của **Wien, Stephan-Boltzmann** và các tính chất của **Hiệu ứng Compton** vì đây là những câu hỏi "cho điểm" nếu nhớ lý thuyết, nhưng rất dễ mất điểm nếu nhớ mang máng. Chúc bạn thi tốt!

Chào bạn, tôi đã hoàn thành việc phân tích file PDF **"Chương 8: Cơ học lượng tử"**.

Đây là chương khó nhất về mặt tư duy vì nó phá vỡ các quan niệm của vật lý cổ điển (Newton). Đối với thi trắc nghiệm, giảng viên thường tập trung vào các **khái niệm mới** (lưỡng tính sóng hạt, xác suất, bất định) và **kết quả của các bài toán ứng dụng** (giếng thế, đường ngầm) thay vì bắt giải phương trình vi phân phức tạp.

Dưới đây là tài liệu ôn tập chiến lược dành riêng cho Chương 8:

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 8 (CƠ HỌC LƯỢNG TỬ)

## PHẦN A: "GIẢI PHẪU" TỪ KHÓA & ĐỊNH NGHĨA (THEORY ANATOMY)

### 1. Giả thuyết De Broglie (Sóng vật chất)
*   **Nội dung:** Mọi vật chất (vi hạt) chuyển động đều có tính chất sóng.
*   **Công thức:** $\lambda = \frac{h}{p} = \frac{h}{mv}$
    *   $\lambda$: Bước sóng De Broglie.
    *   $p$: Động lượng.
*   **Hệ quả trắc nghiệm:**
    *   Khối lượng $m$ càng lớn $\rightarrow$ $\lambda$ càng nhỏ (Vật vĩ mô sóng không đáng kể).
    *   Vận tốc $v$ càng lớn $\rightarrow$ $\lambda$ càng nhỏ.
    *   Thực nghiệm kiểm chứng: **Nhiễu xạ electron** (Thí nghiệm Davisson-Germer).

### 2. Hệ thức bất định Heisenberg
*   **Vị trí - Động lượng:** $\Delta x . \Delta p_x \ge \hbar$ (hoặc $\approx h$)
    *   *Ý nghĩa:* Không thể xác định đồng thời chính xác cả vị trí và động lượng.
    *   *Hệ quả quan trọng:* Trong thế giới vi mô, **KHÔNG CÓ KHÁI NIỆM QUỸ ĐẠO** (Electron không chuyển động theo đường như hành tinh quay quanh mặt trời).
*   **Năng lượng - Thời gian:** $\Delta E . \Delta t \approx h$
    *   *Ý nghĩa:* Trạng thái tồn tại càng ngắn ($\Delta t$ nhỏ) thì năng lượng càng không xác định ($\Delta E$ lớn).
    *   Trạng thái bền (tồn tại lâu) $\rightarrow$ Năng lượng xác định rõ.

### 3. Hàm sóng ($\Psi$) và Ý nghĩa thống kê
*   **Hàm sóng $\Psi$:** Mô tả trạng thái của vi hạt.
*   **Ý nghĩa Max Born (Cực quan trọng):**
    *   Bản thân $\Psi$ không có ý nghĩa vật lý trực tiếp.
    *   Bình phương mô-đun $|\Psi|^2$ là **Mật độ xác suất** tìm thấy hạt tại một điểm.
    *   *Câu lừa:* "$\Psi$ là xác suất" $\rightarrow$ SAI. Phải là $|\Psi|^2$.
*   **Điều kiện của hàm sóng:** Phải Liên tục, Hữu hạn, và Đơn trị.
*   **Điều kiện chuẩn hóa:** $\int |\Psi|^2 dV = 1$ (Xác suất tìm thấy hạt trong toàn vũ trụ là 100%).

---

## PHẦN B: KẾT QUẢ CÁC BÀI TOÁN ỨNG DỤNG (KEY RESULTS)
*Trắc nghiệm sẽ hỏi kết quả, không bắt giải phương trình. Hãy học thuộc các đặc điểm sau:*

### 1. Hạt trong giếng thế năng (1 chiều, thành cao vô hạn)
*   **Năng lượng:** Bị lượng tử hóa (gián đoạn).
    $$E_n = n^2 \frac{\pi^2 \hbar^2}{2ma^2} \quad (n = 1, 2, 3...)$$
    *   Tỉ lệ với bình phương số nguyên $n^2$.
    *   Tỉ lệ nghịch với bình phương bề rộng giếng $a^2$ (Giếng càng hẹp, năng lượng càng cao).
*   **Trạng thái cơ bản ($n=1$):** $E_1 \neq 0$. Hạt không bao giờ đứng yên.
*   **Xác suất tìm thấy hạt:** Không đồng đều.
    *   Tại thành giếng ($x=0, x=a$): Xác suất = 0.
    *   Ở giữa giếng: Có các bụng sóng xác suất.

### 2. Hiệu ứng đường ngầm (Tunneling Effect)
*   **Hiện tượng:** Hạt có năng lượng $E < U_0$ (thấp hơn rào cản) vẫn có xác suất xuyên qua hàng rào thế năng.
*   **Đặc điểm:**
    *   Là hiệu ứng **thuần túy lượng tử** (Cơ học cổ điển cấm điều này).
    *   Xác suất truyền qua ($D$) phụ thuộc vào bề rộng và độ cao của rào thế.
*   **Ứng dụng:** Giải thích hiện tượng **Phân rã Alpha** ($\alpha$), phát xạ electron lạnh.

### 3. Dao động tử điều hòa lượng tử
*   **Năng lượng:** Cách đều nhau.
    $$E_n = (n + \frac{1}{2})\hbar\omega \quad (n = 0, 1, 2...)$$
*   **Năng lượng không (Zero-point energy):**
    *   Khi $n=0 \rightarrow E_0 = \frac{1}{2}\hbar\omega \neq 0$.
    *   *Ý nghĩa:* Tại nhiệt độ tuyệt đối $T=0K$, các hạt vi mô **vẫn dao động**, không bao giờ đứng yên. (Phù hợp với nguyên lý bất định).

---

## PHẦN C: "BẪY" VÀ CÁC CÂU HỎI KHÓ (TRAP DETECTION)

1.  **Bẫy về Quỹ đạo:**
    *   *Câu lừa:* "Theo cơ học lượng tử, electron chuyển động quanh hạt nhân theo quỹ đạo tròn/elip."
    *   *Sự thật:* **SAI**. Do nguyên lý bất định, electron không có quỹ đạo. Ta chỉ biết xác suất tìm thấy nó (đám mây electron).

2.  **Bẫy về Năng lượng liên tục vs. Gián đoạn:**
    *   Hạt tự do: Năng lượng liên tục (bất kỳ).
    *   Hạt trong giếng thế / Dao động tử (bị giam cầm): Năng lượng **gián đoạn** (lượng tử hóa).

3.  **Bẫy về bước sóng De Broglie:**
    *   *Câu hỏi:* "Viên bi bay có sóng De Broglie không?"
    *   *Trả lời:* **CÓ**, nhưng bước sóng quá nhỏ ($< 10^{-30}m$) nên không thể quan sát hiện tượng giao thoa/nhiễu xạ. Tính chất sóng chỉ thể hiện rõ ở **vi hạt** (electron, neutron...).

4.  **Bẫy về Hiệu ứng đường ngầm:**
    *   Nếu năng lượng $E > U_0$ (lớn hơn rào), theo cổ điển hạt chắc chắn qua 100%. Nhưng theo lượng tử, vẫn có xác suất bị **phản xạ** lại.

---

## PHẦN D: BỘ CÂU HỎI LÝ THUYẾT GIẢ LẬP (MOCK TEST)

**Câu 1: Theo giả thuyết De Broglie, một hạt có khối lượng $m$ chuyển động với vận tốc $v$ sẽ có bước sóng:**
A. Tỉ lệ thuận với động lượng.
B. Tỉ lệ nghịch với động lượng.
C. Tỉ lệ thuận với bình phương vận tốc.
D. Không phụ thuộc vào khối lượng.
> **Đáp án B.** ($\lambda = h/p$. $p$ tăng thì $\lambda$ giảm).

**Câu 2: Hệ thức bất định Heisenberg $\Delta x . \Delta p_x \ge \hbar$ khẳng định điều gì?**
A. Ta không thể đo chính xác vị trí của vi hạt.
B. Ta không thể đo chính xác động lượng của vi hạt.
C. Ta không thể xác định đồng thời chính xác cả vị trí và động lượng của vi hạt.
D. Sai số dụng cụ đo trong thế giới vi mô là rất lớn.
> **Đáp án C.** Đây là bản chất của vật chất, không phải do dụng cụ đo.

**Câu 3: Ý nghĩa vật lý của hàm sóng $\Psi$ trong cơ học lượng tử là:**
A. $|\Psi|^2$ cho biết mật độ xác suất tìm thấy hạt tại một điểm.
B. $\Psi$ biểu diễn quỹ đạo chuyển động của hạt.
C. $\Psi$ biểu diễn năng lượng của hạt.
D. $|\Psi|$ cho biết vị trí chính xác của hạt.
> **Đáp án A.** (Theo cách giải thích của Max Born).

**Câu 4: Năng lượng của một hạt trong giếng thế năng sâu vô hạn có đặc điểm:**
A. Có thể nhận bất kỳ giá trị nào (liên tục).
B. Tỉ lệ với số nguyên tử lượng $n$.
C. Tỉ lệ với bình phương số nguyên tử lượng $n^2$.
D. Bằng 0 ở trạng thái cơ bản.
> **Đáp án C.** ($E_n \sim n^2$. Lưu ý: Dao động tử điều hòa mới tỉ lệ với $n$).

**Câu 5: Hiệu ứng đường ngầm (Tunneling) xảy ra khi:**
A. Năng lượng của hạt lớn hơn thế năng của rào.
B. Năng lượng của hạt nhỏ hơn thế năng của rào.
C. Hạt là một vật thể vĩ mô.
D. Hàng rào thế năng rất rộng.
> **Đáp án B.** Hạt "chui" qua rào cản dù không đủ năng lượng để vượt qua đỉnh.

**Câu 6: Năng lượng điểm không ($E_0$) của dao động tử điều hòa lượng tử chứng tỏ:**
A. Tại $0K$, các vi hạt ngừng chuyển động.
B. Tại $0K$, các vi hạt vẫn dao động.
C. Nguyên lý bất định không áp dụng tại $0K$.
D. Năng lượng của hạt bằng 0 ở trạng thái cơ bản.
> **Đáp án B.** $E_0 = \frac{1}{2}\hbar\omega \neq 0$.

**Câu 7: Thí nghiệm nào sau đây xác nhận tính chất sóng của electron?**
A. Thí nghiệm giọt dầu Millikan.
B. Hiệu ứng quang điện.
C. Thí nghiệm tán xạ Compton.
D. Thí nghiệm nhiễu xạ electron trên tinh thể (Davisson-Germer).
> **Đáp án D.** Nhiễu xạ là đặc tính của sóng. (B và C chứng minh tính hạt của ánh sáng).

---
**Lời khuyên:** Hãy học thuộc bảng so sánh giữa **Hạt trong giếng** và **Dao động tử điều hòa** (về công thức năng lượng và mức năng lượng thấp nhất), vì đề thi rất hay hỏi tráo đổi giữa hai mô hình này. Chúc bạn thi tốt!

Chào bạn, tôi đã phân tích kỹ nội dung **Chương 9: Vật lý Nguyên tử** trong tài liệu bạn gửi. Chương này chuyển từ các mô hình bán cổ điển sang mô hình **Cơ học lượng tử** hoàn chỉnh để mô tả nguyên tử.

Đối với thi trắc nghiệm, các câu hỏi sẽ xoay quanh **các số lượng tử**, **quy tắc lựa chọn**, và **sự khác biệt giữa các mô hình**. Dưới đây là tài liệu ôn tập chiến lược dành riêng cho chương này.

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 9 (VẬT LÝ NGUYÊN TỬ)

## PHẦN A: "GIẢI PHẪU" BỘ 4 SỐ LƯỢNG TỬ (THEORY CORE)
*Đây là phần quan trọng nhất, chiếm 40-50% câu hỏi lý thuyết. Bạn cần nhớ kỹ tên gọi, ký hiệu và giá trị cho phép của chúng.*

| Tên số lượng tử | Ký hiệu | Giá trị cho phép | Ý nghĩa vật lý |
| :--- | :---: | :--- | :--- |
| **Chính** | $n$ | $1, 2, 3, ...$ (nguyên dương) | Xác định **năng lượng** (lớp K, L, M...). Kích thước đám mây e. |
| **Orbital (Quỹ đạo)** | $\ell$ | $0, 1, ..., n-1$ | Xác định **mô-men động lượng quỹ đạo** ($L$). Hình dạng đám mây e (s, p, d, f). |
| **Từ** | $m$ | $0, \pm 1, ..., \pm \ell$ | Xác định **hình chiếu của L** lên phương z. Sự định hướng trong không gian. |
| **Spin (Từ riêng)** | $m_s$ | $\pm 1/2$ | Xác định **mô-men động lượng riêng** của electron. |

> **Quy ước ký hiệu phân lớp:**
> *   $\ell = 0 \rightarrow s$
> *   $\ell = 1 \rightarrow p$
> *   $\ell = 2 \rightarrow d$
> *   $\ell = 3 \rightarrow f$

---

## PHẦN B: PHÂN LOẠI & SO SÁNH (KEY COMPARISONS)
*Đề thi rất hay hỏi sự khác nhau giữa H và Kim loại kiềm.*

### 1. Nguyên tử Hiđrô (Hydrogen)
*   **Cấu tạo:** 1 proton + 1 electron.
*   **Năng lượng:** Chỉ phụ thuộc vào **$n$**.
    *   $E_n = -\frac{R_H}{n^2}$ (Luôn âm, $n$ càng lớn $E$ càng gần 0).
*   **Suy biến:** Mức năng lượng $E_n$ có $n^2$ trạng thái (nếu không kể spin) hoặc $2n^2$ trạng thái (nếu kể spin).
*   **Bán kính xác suất cực đại (trạng thái cơ bản):** $r = a_0$ (Bán kính Bohr).

### 2. Nguyên tử Kim loại kiềm (Li, Na, K...)
*   **Cấu tạo:** Lõi (+e) + 1 electron hóa trị ở ngoài cùng.
*   **Năng lượng:** Phụ thuộc vào **$n$ VÀ $\ell$**.
    *   $E_{n,\ell} = -\frac{R_H}{(n + \Delta_\ell)^2}$ ($\Delta_\ell$: số bổ chính Rydberg).
    *   Với cùng $n$, năng lượng mức $s < p < d < f$ (do $\ell$ càng nhỏ, electron càng chui sâu vào gần hạt nhân, liên kết càng chặt).
*   **Quang phổ:** Phức tạp hơn H (do sự phụ thuộc vào $\ell$).

### 3. Mô-men động lượng & Spin
Cần phân biệt công thức tính **Độ lớn** và **Hình chiếu**:

| Đại lượng | Độ lớn (Magnitude) | Hình chiếu lên trục z (Quantization) |
| :--- | :--- | :--- |
| **Orbital ($\vec{L}$)** | $L = \hbar\sqrt{\ell(\ell+1)}$ | $L_z = m\hbar$ |
| **Spin ($\vec{S}$)** | $S = \hbar\sqrt{s(s+1)}$ (với $s=1/2$) | $S_z = m_s\hbar$ (với $m_s=\pm 1/2$) |
| **Toàn phần ($\vec{J}$)**| $J = \hbar\sqrt{j(j+1)}$ | $J_z = m_j\hbar$ |

---

## PHẦN C: "BẪY" VÀ QUY TẮC LỰA CHỌN (TRAP DETECTION)

### 1. Quy tắc lựa chọn (Selection Rules) - *Cực kỳ hay thi*
Electron không thể nhảy tùy tiện giữa các mức năng lượng. Nó phải tuân theo luật:
*   **Biến thiên số lượng tử orbital:** $\Delta \ell = \pm 1$ (Chỉ được nhảy giữa các lớp s-p, p-d... Không được nhảy s-s, s-d).
*   **Biến thiên số lượng tử từ:** $\Delta m = 0, \pm 1$.
*   **Biến thiên số lượng tử toàn phần:** $\Delta j = 0, \pm 1$.

### 2. Hiệu ứng Zeeman
*   Là sự tách vạch quang phổ khi đặt nguyên tử trong **từ trường**.
*   Nguyên nhân: Do sự tương tác giữa mô-men từ của electron và từ trường ngoài.
*   Số vạch tách ra phụ thuộc vào số lượng tử từ $m$.

### 3. Số electron tối đa (Nguyên lý Pauli)
*   **Trong một lớp $n$:** Tối đa $2n^2$ electron.
*   **Trong một phân lớp $\ell$:** Tối đa $2(2\ell + 1)$ electron.
    *   s (l=0): 2e
    *   p (l=1): 6e
    *   d (l=2): 10e
    *   f (l=3): 14e

### 4. Thống kê lượng tử (Boson vs Fermion)
*   **Fermion:** Hạt có spin **bán nguyên** ($1/2, 3/2...$). Tuân theo nguyên lý **Pauli** (không được ở cùng một trạng thái). Ví dụ: Electron, Proton, Neutron. $\rightarrow$ Thống kê Fermi-Dirac.
*   **Boson:** Hạt có spin **nguyên** ($0, 1, 2...$). **Không** tuân theo Pauli (có thể tụ tập ở cùng một mức năng lượng). Ví dụ: Photon. $\rightarrow$ Thống kê Bose-Einstein.

---

## PHẦN D: BỘ CÂU HỎI GIẢ LẬP LÝ THUYẾT (MOCK TEST)

**Câu 1: Trạng thái lượng tử của electron trong nguyên tử được xác định hoàn toàn bởi bộ số lượng tử nào?**
A. $n, \ell$
B. $n, \ell, m$
C. $n, \ell, m, m_s$
D. $n, m, m_s$
> **Đáp án C.** Phải đủ 4 số để xác định duy nhất một electron (theo Pauli).

**Câu 2: Trong nguyên tử Hiđrô, năng lượng của electron ở trạng thái dừng phụ thuộc vào:**
A. Chỉ số lượng tử chính $n$.
B. Số lượng tử chính $n$ và số lượng tử orbital $\ell$.
C. Số lượng tử orbital $\ell$ và số lượng tử từ $m$.
D. Cả 4 số lượng tử.
> **Đáp án A.** Đối với H (chỉ có 1e), năng lượng suy biến, chỉ phụ thuộc $n$. (Lưu ý: Nếu là kim loại kiềm thì đáp án là B).

**Câu 3: Theo cơ học lượng tử, mô-men động lượng orbital $L$ của electron được xác định bởi công thức:**
A. $L = n\hbar$
B. $L = \hbar\sqrt{\ell(\ell+1)}$
C. $L = m\hbar$
D. $L = \ell\hbar$
> **Đáp án B.** Đây là kết quả của cơ học lượng tử giải phương trình Schrodinger.

**Câu 4: Chuyển dời năng lượng nào sau đây là KHÔNG được phép (bị cấm) đối với nguyên tử kim loại kiềm?**
A. $3P \to 2S$ ($\Delta \ell = -1$) - Được.
B. $4F \to 3D$ ($\Delta \ell = -1$) - Được.
C. $3S \to 2S$ ($\Delta \ell = 0$) - Cấm.
D. $3D \to 2P$ ($\Delta \ell = -1$) - Được.
> **Đáp án C.** Vì quy tắc lựa chọn là $\Delta \ell = \pm 1$. Từ S sang S thì $\ell$ không đổi ($\Delta \ell = 0$).

**Câu 5: Hiệu ứng Zeeman là hiện tượng:**
A. Tách vạch quang phổ dưới tác dụng của điện trường.
B. Tách vạch quang phổ dưới tác dụng của từ trường.
C. Tán sắc ánh sáng qua lăng kính.
D. Nhiễu xạ electron trên tinh thể.
> **Đáp án B.**

**Câu 6: Hạt nào sau đây tuân theo nguyên lý loại trừ Pauli?**
A. Photon.
B. Electron.
C. Phonon.
D. Hạt có spin nguyên.
> **Đáp án B.** Electron là Fermion (spin 1/2) nên tuân theo Pauli.

**Câu 7: Số electron tối đa có thể chứa trong lớp M ($n=3$) là:**
A. 8
B. 10
C. 18
D. 32
> **Đáp án C.** Công thức $2n^2 = 2 \times 3^2 = 18$.

---
**Lời khuyên:** Chương này có nhiều ký hiệu ($K, L, M$ hay $s, p, d, f$). Bạn hãy viết ra nháp bảng quy đổi giữa Tên lớp/phân lớp và Giá trị số ($n, \ell$) tương ứng trước khi làm bài để tránh nhầm lẫn. Chúc bạn ôn tập tốt!

Chào bạn, tôi đã hoàn thành việc phân tích file PDF **"Chương 10: Vật lý Chất rắn và Bán dẫn"**.

Đây là chương cuối cùng và mang tính ứng dụng công nghệ cao nhất. Đối với thi trắc nghiệm, chương này **ít bài tập tính toán phức tạp** nhưng lại có **rất nhiều định nghĩa, phân loại và cơ chế vật lý** dễ gây nhầm lẫn.

Dưới đây là tài liệu ôn tập chiến lược dành riêng cho Chương 10:

---

# 📘 CHIẾN LƯỢC ÔN TẬP TRẮC NGHIỆM: CHƯƠNG 10 (CHẤT RẮN & BÁN DẪN)

## PHẦN A: "GIẢI PHẪU" TỪ KHÓA & ĐỊNH NGHĨA (THEORY ANATOMY)

### 1. Cấu trúc & Liên kết trong mạng tinh thể
*   **Mạng tinh thể:** Có tính tuần hoàn.
*   **4 loại liên kết (Cần nhớ đặc điểm để chọn đúng/sai):**
    1.  **Liên kết Nguyên tử (Đồng hóa trị):** Bền vững nhất. (Ví dụ: Kim cương, Silic).
    2.  **Liên kết Kim loại:** Các ion dương ở nút mạng, electron tự do chuyển động chung (khí electron).
    3.  **Liên kết Ion:** Lực hút tĩnh điện giữa ion dương và âm (Ví dụ: NaCl).
    4.  **Liên kết Phân tử (Van der Waals):** Yếu nhất. (Ví dụ: Nước đá, Iot).

### 2. Lý thuyết Vùng năng lượng (Band Theory) - *Trọng tâm*
Cấu trúc vùng quyết định tính chất dẫn điện:
*   **Vùng hóa trị (Valence Band):** Vùng đầy electron liên kết (ở 0K).
*   **Vùng dẫn (Conduction Band):** Vùng trống hoặc chứa electron tự do.
*   **Vùng cấm (Band Gap - $E_g$):** Khoảng cách năng lượng giữa đỉnh vùng hóa trị và đáy vùng dẫn.

**Bảng phân loại (Cực quan trọng):**

| Loại vật liệu | Cấu trúc vùng năng lượng | Độ dẫn điện |
| :--- | :--- | :--- |
| **Kim loại (Dẫn điện)** | Vùng hóa trị và Vùng dẫn **phủ nhau** (Overlap). Hoặc vùng dẫn điền đầy một phần. | Dẫn điện tốt ở mọi nhiệt độ. |
| **Bán dẫn** | Có vùng cấm hẹp ($E_g < 3eV$). | Dẫn điện kém ở thấp độ, tốt ở nhiệt độ cao. |
| **Điện môi (Cách điện)** | Có vùng cấm rộng ($E_g \ge 3eV$). | Không dẫn điện (electron không nhảy lên được). |

---

## PHẦN B: VẬT LÝ BÁN DẪN (SEMICONDUCTORS) - *Phần thi nhiều nhất*

### 1. Phân loại Bán dẫn (Bảng "Thần thánh" cần học thuộc)

| Đặc điểm | Bán dẫn Thuần (Intrinsic) | Bán dẫn loại n (Negative) | Bán dẫn loại p (Positive) |
| :--- | :--- | :--- | :--- |
| **Nguyên liệu** | Si, Ge tinh khiết (Nhóm 4). | Si pha tạp chất **Nhóm 5** (P, As...). | Si pha tạp chất **Nhóm 3** (B, Al...). |
| **Tên tạp chất** | Không có. | **Chất Đô-nô (Cho):** Thừa e, tạo ion dương cố định. | **Chất Axepto (Nhận):** Thiếu e, tạo ion âm cố định. |
| **Hạt tải điện** | Electron = Lỗ trống ($n_e = n_p$). | **Đa số: Electron**. Thiểu số: Lỗ trống. | **Đa số: Lỗ trống**. Thiểu số: Electron. |
| **Mức Fermi ($E_F$)** | Nằm **giữa** vùng cấm. | Lệch về phía **đáy Vùng dẫn**. | Lệch về phía **đỉnh Vùng hóa trị**. |

### 2. Lỗ trống (Hole)
*   **Bản chất:** Là chỗ trống do electron để lại trong vùng hóa trị.
*   **Đặc điểm:** Mang điện tích **Dương (+e)**. Có khối lượng hiệu dụng **Dương ($m^* > 0$)**. Chuyển động cùng chiều điện trường.

---

## PHẦN C: LINH KIỆN BÁN DẪN (DIODE & LASER)

### 1. Lớp chuyển tiếp p-n (p-n Junction)
*   **Sự hình thành:** Do sự khuếch tán hạt tải đa số (e từ n sang p, lỗ trống từ p sang n).
*   **Vùng nghèo (Depletion region):** Lớp tiếp xúc ở giữa, **không có hạt tải điện tự do**, chỉ có ion cố định -> Điện trở rất lớn.
*   **Tính chất chỉnh lưu (Diode):**
    *   **Phân cực thuận (+ vào p, - vào n):** Điện trường ngoài chống lại điện trường tiếp xúc $\rightarrow$ Vùng nghèo thu hẹp $\rightarrow$ **Dòng điện lớn chạy qua**.
    *   **Phân cực ngược (+ vào n, - vào p):** Vùng nghèo mở rộng $\rightarrow$ **Hầu như không có dòng điện**.

### 2. Laser Bán dẫn
*   **Nguyên tắc:** Dựa trên hiện tượng **Phát xạ cảm ứng** (giống mọi loại Laser).
*   **Điều kiện cần:** Phải tạo ra trạng thái **Nghịch đảo mật độ** (số hạt ở mức năng lượng cao nhiều hơn mức thấp).
*   **Cấu tạo:** Dùng chuyển tiếp p-n pha tạp mạnh (suy biến).
*   **Buồng cộng hưởng Fabry-Perot:** Hai mặt bên của tinh thể được mài phẳng song song để phản xạ ánh sáng qua lại, khuếch đại ánh sáng.

---

## PHẦN D: "BẪY" VÀ CÁC CÂU HỎI KHÓ (TRAP DETECTION)

1.  **Bẫy về Điện tích của bán dẫn:**
    *   *Câu lừa:* "Bán dẫn loại n tích điện âm, loại p tích điện dương."
    *   *Sự thật:* **SAI**. Cả hai loại đều **trung hòa về điện**. (Vì số electron tự do + ion âm = số lỗ trống + ion dương).

2.  **Bẫy về Nhiệt độ và Độ dẫn điện:**
    *   **Kim loại:** Nhiệt độ tăng $\rightarrow$ Dao động mạng tinh thể mạnh $\rightarrow$ Cản trở electron $\rightarrow$ **Điện trở tăng (Độ dẫn giảm)**.
    *   **Bán dẫn:** Nhiệt độ tăng $\rightarrow$ Cung cấp năng lượng cho e nhảy lên vùng dẫn $\rightarrow$ Số hạt tải điện tăng mạnh $\rightarrow$ **Điện trở giảm (Độ dẫn tăng)**.

3.  **Bẫy về tạp chất:**
    *   Nhớ quy tắc: **"Dư 5 n, Thiếu 3 p"**.
    *   Si (4) + P (5) $\rightarrow$ Dư 1 electron $\rightarrow$ loại **n**.
    *   Si (4) + B (3) $\rightarrow$ Thiếu 1 electron (sinh ra lỗ trống) $\rightarrow$ loại **p**.

---

## PHẦN E: BỘ CÂU HỎI LÝ THUYẾT GIẢ LẬP (MOCK TEST)

**Câu 1: Sự khác biệt cơ bản giữa chất bán dẫn và chất điện môi (cách điện) theo lý thuyết vùng năng lượng là:**
A. Chất bán dẫn không có vùng cấm.
B. Độ rộng vùng cấm của bán dẫn nhỏ hơn nhiều so với điện môi.
C. Vùng hóa trị của bán dẫn không được lấp đầy.
D. Chất điện môi không có vùng dẫn.
> **Đáp án B.** ($E_g$ bán dẫn < 3eV, điện môi > 3eV).

**Câu 2: Trong bán dẫn loại n, hạt tải điện cơ bản (đa số) là:**
A. Ion dương.
B. Lỗ trống.
C. Electron.
D. Ion âm.
> **Đáp án C.** (n = negative = âm = electron).

**Câu 3: Khi nhiệt độ của một khối bán dẫn tinh khiết tăng lên, thì:**
A. Điện trở của nó tăng lên.
B. Điện trở của nó giảm xuống.
C. Số lượng electron dẫn giảm đi.
D. Số lượng lỗ trống giảm đi.
> **Đáp án B.** Nhiệt độ tăng -> sinh ra nhiều cặp e-lỗ trống -> dẫn điện tốt hơn -> điện trở giảm.

**Câu 4: Để tạo ra bán dẫn loại p từ Silic (nhóm 4), ta cần pha tạp chất là nguyên tố thuộc:**
A. Nhóm 1.
B. Nhóm 3.
C. Nhóm 4.
D. Nhóm 5.
> **Đáp án B.** (Ví dụ: Bo, Nhôm... để tạo lỗ trống nhận electron).

**Câu 5: Nguyên tắc hoạt động của Diode bán dẫn dựa trên:**
A. Tính chất chỉnh lưu của lớp chuyển tiếp p-n.
B. Hiện tượng quang điện trong.
C. Sự phát xạ cảm ứng.
D. Hiệu ứng nhiệt điện.
> **Đáp án A.** Cho dòng đi qua theo 1 chiều (phân cực thuận).

**Câu 6: Trong Laser bán dẫn, buồng cộng hưởng Fabry-Perot có tác dụng gì?**
A. Tạo ra trạng thái nghịch đảo mật độ.
B. Cung cấp năng lượng bơm.
C. Làm lạnh bán dẫn.
D. Phản xạ ánh sáng qua lại để khuếch đại và lọc lựa mode sóng.
> **Đáp án D.**

**Câu 7: Phát biểu nào sau đây SAI về lỗ trống?**
A. Lỗ trống mang điện tích dương +e.
B. Lỗ trống thực chất là chỗ trống liên kết do electron để lại.
C. Lỗ trống có khối lượng hiệu dụng dương.
D. Lỗ trống chuyển động ngược chiều điện trường.
> **Đáp án D.** Lỗ trống mang điện dương nên phải chuyển động **cùng chiều** điện trường.

---
**Lời khuyên:** Chương này lý thuyết rất logic. Bạn chỉ cần nhớ sơ đồ: **Si (4) + [5] = n (thừa e)** và **Si (4) + [3] = p (thừa lỗ)** là suy luận được hầu hết các câu hỏi về tạp chất. Chúc bạn có một kỳ thi đạt điểm tối đa!