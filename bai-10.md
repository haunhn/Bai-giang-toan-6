[⬅️ Quay lại Trang chủ Mục lục](README.md)

# 📘 CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN
# 🌟 BÀI 10: SỐ NGUYÊN TỐ
* **Môn học:** Toán học 6 (Tập 1) — *Bộ sách Kết nối tri thức với cuộc sống*
* **Thời lượng tự học:** 60 phút
* **Hình thức:** Học liệu số tương tác (Lý thuyết trực quan + Trò chơi vận dụng)

---

> [!NOTE]
> ### 🎯 MỤC TIÊU CẦN ĐẠT SAU BÀI HỌC
> 1. **Nhận biết và phân biệt** được khái niệm **số nguyên tố** và **hợp số** trong tập hợp số tự nhiên.
> 2. **Ghi nhớ** được các số nguyên tố nhỏ hơn 20 và các trường hợp đặc biệt của số `0`, số `1`, số `2`.
> 3. **Thực hiện thành thạo** việc phân tích một số tự nhiên lớn hơn 1 ra **thừa số nguyên tố** bằng hai phương pháp: *Sơ đồ cây* và *Sơ đồ cột dọc*, đồng thời viết gọn kết quả dưới dạng lũy thừa.
> 4. **Vận dụng** kiến thức về số nguyên tố và phân tích thừa số nguyên tố để giải quyết các bài toán tìm ước và bài toán thực tiễn.

---

## 🚀 KHỞI ĐỘNG: NHỮNG "VIÊN GẠCH" XÂY DỰNG NÊN THẾ GIỚI SỐ
**Tình huống:** Cô giáo giao cho hai bạn Nam và Mai mỗi người một số lượng hình vuông nhỏ bằng nhau để xếp thành các hình chữ nhật (sao cho không bị lẻ ô vuông nào):
* Bạn **Mai** nhận được **6 hình vuông**: Mai dễ dàng xếp được 2 kiểu hình chữ nhật khác nhau là `1 × 6` (1 hàng 6 cột) và `2 × 3` (2 hàng 3 cột).
* Bạn **Nam** nhận được **7 hình vuông**: Dù xoay sở thế nào, Nam cũng chỉ xếp được duy nhất 1 kiểu hình chữ nhật là `1 × 7` (1 hàng 7 cột).

❓ **Câu hỏi tư duy:** *Tại sao cùng là các con số tự nhiên lớn hơn 1, nhưng có những số (như số 6) lại có thể tách thành tích của nhiều số nhỏ hơn, trong khi có những số (như số 7) lại "cứng đầu" không thể tách được ngoài 1 và chính nó?*

➔ Trong Toán học, những con số "không thể tách nhỏ hơn" như số 7 được gọi là **Số nguyên tố** — những viên gạch nguyên bản cấu tạo nên mọi con số khác! Hãy cùng khám phá ngay dưới đây.

---

## 📖 NỘI DUNG 1: SỐ NGUYÊN TỐ VÀ HỢP SỐ

### 1.1. Khám phá số lượng ước của các số tự nhiên lớn hơn 1
🔍 **Hoạt động khám phá 1:** Hãy liệt kê tất cả các ước của các số tự nhiên từ `2` đến `9` và quan sát số lượng ước của chúng trong bảng sau:

| Số tự nhiên *a* | Tập hợp các ước Ư(*a*) | Số lượng ước | Phân loại nhóm |
| :---: | :--- | :---: | :--- |
| **2** | `{1; 2}` | **2 ước** | 🟢 Chỉ có 2 ước (1 và chính nó) |
| **3** | `{1; 3}` | **2 ước** | 🟢 Chỉ có 2 ước (1 và chính nó) |
| **4** | `{1; 2; 4}` | **3 ước** | 🟠 Có nhiều hơn 2 ước |
| **5** | `{1; 5}` | **2 ước** | 🟢 Chỉ có 2 ước (1 và chính nó) |
| **6** | `{1; 2; 3; 6}` | **4 ước** | 🟠 Có nhiều hơn 2 ước |
| **7** | `{1; 7}` | **2 ước** | 🟢 Chỉ có 2 ước (1 và chính nó) |
| **8** | `{1; 2; 4; 8}` | **4 ước** | 🟠 Có nhiều hơn 2 ước |
| **9** | `{1; 3; 9}` | **3 ước** | 🟠 Có nhiều hơn 2 ước |

> [!IMPORTANT]
> ### 📌 ĐỊNH NGHĨA SỐ NGUYÊN TỐ VÀ HỢP SỐ
> * 🟢 **Số nguyên tố** là số tự nhiên **lớn hơn 1**, chỉ có **hai ước** là `1` và `chính nó`. *(Ví dụ: 2, 3, 5, 7, 11, 13, 17, 19...)*
> * 🟠 **Hợp số** là số tự nhiên **lớn hơn 1**, có **nhiều hơn hai ước**. *(Ví dụ: 4, 6, 8, 9, 10, 12, 14, 15...)*

---

### 1.2. Các quy tắc "Vàng" cần khắc cốt ghi tâm

> [!WARNING]
> ### ⚡ 3 LƯU Ý ĐẶC BIỆT (RẤT HAY GẶP TRONG ĐỀ THI)
> 1. **Số `0` và số `1`:** **KHÔNG là số nguyên tố** và cũng **KHÔNG là hợp số** *(vì định nghĩa chỉ xét các số tự nhiên lớn hơn 1)*.
> 2. **Số `2`:** Là **số nguyên tố nhỏ nhất**, và cũng là **số nguyên tố CHẴN duy nhất** trong toán học! *(Tất cả các số chẵn lớn hơn 2 như 4, 6, 8, 10... đều chia hết cho 2 nên đều là hợp số)*.
> 3. **Cách chứng minh một số là Hợp số:** Để chứng minh một số tự nhiên *a* (*a* > 1) là hợp số, ta chỉ cần **chỉ ra thêm ít nhất MỘT ước nữa** của *a* khác `1` và khác `*a*` *(thường dựa vào dấu hiệu chia hết cho 2, 5, 3, 9 ở Bài 9)*.

> [!TIP]
> ### 💡 BẢNG 10 SỐ NGUYÊN TỐ ĐẦU TIÊN (NÊN THUỘC LÒNG)
> Để làm bài tập siêu tốc, các em hãy ghi nhớ 10 số nguyên tố đầu tiên (nhỏ hơn 30):
> **`2;  3;  5;  7;  11;  13;  17;  19;  23;  29`**

#### 📝 Trạm dừng thực hành số 1
Trong các số sau: **`0;  1;  17;  29;  95;  312;  2 025`**, số nào là số nguyên tố, số nào là hợp số? Vì sao?

<details>
<summary>👉 <b>NHẤN VÀO ĐÂY ĐỂ XEM ĐÁP ÁN & LỜI GIẢI CHI TIẾT</b></summary>
<br>

* **Số `0` và `1`:** Không là số nguyên tố, cũng không là hợp số. ⚪
* **Các số nguyên tố:** **`17`** và **`29`** *(vì chúng lớn hơn 1 và chỉ có hai ước là 1 và chính nó)*. 🟢
* **Các hợp số:** **`95; 312; 2 025`** *(vì các số này đều lớn hơn 1 và ngoài 1 với chính nó, ta thấy: `95 ⋮ 5`; `312 ⋮ 2`; `2 025 ⋮ 5` nên chúng có nhiều hơn 2 ước)*. 🟠

</details>

---

## 📖 NỘI DUNG 2: PHÂN TÍCH MỘT SỐ RA THỪA SỐ NGUYÊN TỐ

### 2.1. Thế nào là phân tích một số ra thừa số nguyên tố?
Mọi hợp số đều được tạo thành từ việc nhân các "viên gạch" số nguyên tố lại với nhau.

> [!IMPORTANT]
> ### 🌟 KHÁI NIỆM TRỌNG TÂM
> * **Phân tích một số tự nhiên lớn hơn 1 ra thừa số nguyên tố** là viết số đó dưới dạng **một tích các thừa số nguyên tố**.
> * **Chú ý:** 
>   1. Dạng phân tích ra thừa số nguyên tố của mỗi số nguyên tố là **chính số đó**.
>   2. Khi viết kết quả cuối cùng, ta thường **sắp xếp các thừa số nguyên tố theo thứ tự từ nhỏ đến lớn** và dùng **lũy thừa** để thu gọn các thừa số giống nhau.

**Ví dụ kiểm tra nhanh:** Để phân tích số `12` ra thừa số nguyên tố:
* Bạn An viết: `12 = 3 . 4` ➔ ❌ **SAI** *(vì thừa số `4` là hợp số, chưa phải là số nguyên tố)*.
* Bạn Bình viết: `12 = 2 . 2 . 3 = 2^2 . 3` ➔ ✅ **ĐÚNG** *(vì `2` và `3` đều là các số nguyên tố)*.

---

### 2.2. Hai phương pháp phân tích một số ra thừa số nguyên tố
Hãy cùng phân tích số **`24`** ra thừa số nguyên tố bằng 2 cách trình bày chuẩn SGK:

| 🌳 PHƯƠNG PHÁP 1: SƠ ĐỒ CÂY (Tách nhánh tự do) | 📏 PHƯƠNG PHÁP 2: SƠ ĐỒ CỘT DỌC (Chia liên tiếp) |
| :--- | :--- |
| **Cách làm:** Tách số `24` thành tích của 2 thừa số bất kỳ lớn hơn 1. Tiếp tục tách các nhánh hợp số cho đến khi mọi nhánh tận cùng đều là **số nguyên tố**.<br><br>**Minh họa với số 24:**<br>• Tách bước 1: `24 = 4 × 6` *(cả 4 và 6 đều là hợp số)*<br>• Tách nhánh số 4: `4 = 2 × 2` *(2 là số nguyên tố ➔ Dừng)*<br>• Tách nhánh số 6: `6 = 2 × 3` *(2 và 3 là số nguyên tố ➔ Dừng)*<br><br>➔ Gom các nhánh tận cùng lại: **`24 = 2 . 2 . 2 . 3 = 2^3 . 3`** | **Cách làm:** Chia số `24` lần lượt cho các số nguyên tố từ nhỏ đến lớn (`2, 3, 5, 7...`). Chia cho đến khi thương bằng `1` thì dừng lại.<br><br>**Minh họa phép chia cột dọc số 24:**<br>• Lấy `24 : 2` được thương là **`12`** *(viết 2 bên phải)*<br>• Lấy `12 : 2` được thương là **`6`** *(viết 2 bên phải)*<br>• Lấy `6 : 2` được thương là **`3`** *(viết 2 bên phải)*<br>• Lấy `3 : 3` được thương là **`1`** *(viết 3 bên phải ➔ Dừng)*<br><br>➔ Nhân cột bên phải lại: **`24 = 2 . 2 . 2 . 3 = 2^3 . 3`** |

> [!TIP]
> ### 💡 NHẬN XÉT QUAN TRỌNG
> Dù các em dùng **Sơ đồ cây** (tách theo kiểu `24 = 4 . 6` hay `24 = 3 . 8`) hay dùng **Sơ đồ cột dọc**, khi thu gọn dưới dạng lũy thừa thì **kết quả cuối cùng luôn luôn duy nhất**: **`24 = 2^3 . 3`**!

#### 📝 Trạm dừng thực hành số 2
Hãy tự lấy nháp phân tích hai số sau ra thừa số nguyên tố và viết kết quả dưới dạng lũy thừa:
1. Số **`60`**
2. Số **`135`**

<details>
<summary>👉 <b>NHẤN VÀO ĐÂY ĐỂ XEM ĐÁP ÁN & LỜI GIẢI CHI TIẾT</b></summary>
<br>

* **Câu 1 (Phân tích số 60):**
  * Ta thấy `60 = 6 . 10 = (2 . 3) . (2 . 5) = 2 . 2 . 3 . 5`.
  * Viết gọn bằng lũy thừa theo thứ tự tăng dần: **`60 = 2^2 . 3 . 5`**. 🟢
* **Câu 2 (Phân tích số 135 theo cột dọc):**
  * `135` không chia hết cho 2; xét sang số nguyên tố `3`: `135 : 3 = 45`.
  * `45 : 3 = 15`.
  * `15 : 3 = 5`.
  * `5 : 5 = 1` *(Dừng lại)*.
  * Vậy kết quả chuẩn xác là: **`135 = 3 . 3 . 3 . 5 = 3^3 . 5`**. 🟢

</details>

---

## 🎮 ĐẤU TRƯỜNG TRÍ TUỆ: THỬ THÁCH NHÀ TOÁN HỌC TRẺ
*(Phần ôn tập tương tác — Học sinh tự làm và click trực tiếp vào phương án mình chọn để mở khóa kết quả!)*

---

### 🏆 VÒNG 1: NHẬN DIỆN NGUYÊN TỐ (10 Điểm / Câu)

**Câu 1:** Khẳng định nào dưới đây là **ĐÚNG**?
<details>
<summary>🔘 <b>Phương án A: Mọi số nguyên tố đều là số lẻ.</b></summary>
❌ <b>Bị lừa rồi!</b> Số <b>2</b> là số nguyên tố nhưng lại là số chẵn! (Câu đúng phải là: <i>Mọi số nguyên tố lớn hơn 2 đều là số lẻ</i>).
</details>
<details>
<summary>🔘 <b>Phương án B: Số 1 là số nguyên tố nhỏ nhất.</b></summary>
❌ <b>Sai rồi!</b> Số 1 chỉ có duy nhất 1 ước là chính nó, nên số 1 <b>không phải là số nguyên tố</b>. Số nguyên tố nhỏ nhất phải là số <b>2</b>!
</details>
<details>
<summary>🔘 <b>Phương án C: Có duy nhất một số nguyên tố chẵn là số 2.</b></summary>
🎉 <b>CHÍNH XÁC TUYỆT ĐỐI! (+10 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Số 2 chỉ có hai ước là 1 và 2 nên là số nguyên tố. Mọi số chẵn lớn hơn 2 đều chia hết cho 2 (có ít nhất 3 ước là 1, 2 và chính nó) nên đều là hợp số!
</details>

<br>

**Câu 2:** Kết quả phân tích số **`120`** ra thừa số nguyên tố nào dưới đây là **ĐÚNG CHUẨN**?
<details>
<summary>🔘 <b>Phương án A: 120 = 2^3 . 15</b></summary>
❌ <b>Chưa xong!</b> Số <b>15</b> vẫn là hợp số (`15 = 3 . 5`), bạn chưa phân tích triệt để ra thừa số nguyên tố rồi!
</details>
<details>
<summary>🔘 <b>Phương án B: 120 = 2 . 3 . 4 . 5</b></summary>
❌ <b>Sai rồi!</b> Trong tích này có số <b>4</b> là hợp số chứ không phải số nguyên tố.
</details>
<details>
<summary>🔘 <b>Phương án C: 120 = 2^3 . 3 . 5</b></summary>
🎉 <b>XUẤT SẮC! (+10 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Cả ba cơ số 2, 3, 5 đều là các số nguyên tố và ta có `2^3 . 3 . 5 = 8 . 3 . 5 = 120` hoàn toàn chuẩn xác!
</details>

---

### 🔥 VÒNG 2: TĂNG TỐC SUY LUẬN (20 Điểm / Câu)

**Câu 3:** Không cần tính giá trị của biểu thức, hãy cho biết biểu thức **`M = 5 . 7 . 11 + 13 . 17 . 19`** là **số nguyên tố** hay **hợp số**?
<details>
<summary>🔘 <b>Phương án A: M là số nguyên tố</b></summary>
❌ <b>Chưa chính xác!</b> Đừng thấy toàn các số nguyên tố ghép lại mà vội kết luận nhé! Hãy xét tính chẵn lẻ của hai tích xem sao.
</details>
<details>
<summary>🔘 <b>Phương án B: M là hợp số</b></summary>
🎉 <b>ĐỈNH CAO TƯ DUY! (+20 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> 
• Tích thứ nhất `5 . 7 . 11` là tích của các số lẻ nên kết quả là một <b>số lẻ</b>.<br>
• Tích thứ hai `13 . 17 . 19` cũng là tích của các số lẻ nên kết quả là một <b>số lẻ</b>.<br>
• Mà <b>Số lẻ + Số lẻ = Số chẵn</b>! Do đó tổng `M` là một số chẵn lớn hơn 2 (tức là `M ⋮ 2`). Ngoài ước là 1 và M, nó còn có ước là 2 nên <b>M chắc chắn là HỢP SỐ</b>!
</details>

<br>

**Câu 4:** Biết số tự nhiên `A` được phân tích ra thừa số nguyên tố có dạng **`A = 2^2 . 3 . 5`**. Hỏi trong các số sau, số nào **KHÔNG PHẢI** là ước của `A`?
<details>
<summary>🔘 <b>Phương án A: Số 12</b></summary>
❌ <b>Chưa đúng!</b> Ta có `12 = 2^2 . 3`, mà trong phân tích của A có chứa cả `2^2 . 3` (`A = (2^2 . 3) . 5 = 12 . 5`), nên 12 là một ước của A!
</details>
<details>
<summary>🔘 <b>Phương án B: Số 15</b></summary>
❌ <b>Chưa đúng!</b> Ta có `15 = 3 . 5`, mà `A = 2^2 . (3 . 5) = 4 . 15`, nên 15 cũng là một ước của A!
</details>
<details>
<summary>🔘 <b>Phương án C: Số 8</b></summary>
🎉 <b>CHÍNH XÁC TUYỆT ĐỐI! (+20 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Ta biết `8 = 2^3` (cần tới 3 thừa số 2 nhân với nhau), trong khi phân tích của A chỉ có tối đa `2^2` (2 thừa số 2). Do đó A (bằng 60) không chia hết cho 8, hay <b>8 không phải là ước của A</b>!
</details>

---

### 👑 VÒNG 3: CHINH PHỤC TỰ LUẬN & TOÁN THỰC TẾ (40 Điểm)
*(Hoàn thành 3 bài tập chuẩn SGK vào vở, sau đó mở khóa đáp án để tự chấm điểm)*

* **Bài tập 1 (Phân tích thừa số nguyên tố và tìm tập hợp ước):**
  Phân tích số **`70`** ra thừa số nguyên tố, từ đó hãy liệt kê **tất cả các ước** của 70.

* **Bài tập 2 (Bài toán thực tế xếp đội hình - SGK Toán 6):**
  Một đoàn nghi lễ của trường có **36 bạn** học sinh. Cô tổng phụ trách muốn xếp đoàn thành các hàng có số người ở mỗi hàng như nhau (mỗi hàng có từ **4 đến 12 bạn**). Bằng cách phân tích số 36 ra thừa số nguyên tố để tìm các ước của 36, em hãy tính xem cô tổng phụ trách có mấy cách xếp đội hình?

* **Bài tập 3 (Thử thách nâng cao dành cho học sinh giỏi):**
  Tìm số nguyên tố **`p`** sao cho cả **`p + 2`** và **`p + 4`** cũng đều là các số nguyên tố.

<details>
<summary>🔓 <b>MỞ KHÓA HƯỚNG DẪN GIẢI VÀ THANG ĐIỂM TỰ CHẤM (VÒNG 3)</b></summary>
<br>

#### ✅ Lời giải Bài tập 1 (15 Điểm):
* **Bước 1 (Phân tích số 70 ra thừa số nguyên tố):**
  Ta có: `70 = 7 . 10 = 7 . 2 . 5`. Sắp xếp từ nhỏ đến lớn: **`70 = 2 . 5 . 7`**.
* **Bước 2 (Tìm tất cả các ước của 70 từ các thừa số nguyên tố):**
  * Ước là 1 và các thừa số nguyên tố đơn lẻ: `1; 2; 5; 7`.
  * Ước là tích của 2 thừa số nguyên tố: `2.5 = 10`; `2.7 = 14`; `5.7 = 35`.
  * Ước là tích của cả 3 thừa số nguyên tố: `2.5.7 = 70`.
  * **Kết luận:** Tập hợp các ước của 70 là: **`Ư(70) = {1; 2; 5; 7; 10; 14; 35; 70}`**.

---

#### ✅ Lời giải Bài tập 2 (15 Điểm):
* Gọi số học sinh trong mỗi hàng là *x* (bạn), điều kiện: *x ∈ ℕ\** và **`4 ≤ x ≤ 12`**.
* Vì 36 bạn được xếp đều vào các hàng nên *x* là ước của 36 (`x ∈ Ư(36)`).
* Phân tích 36 ra thừa số nguyên tố: **`36 = 2^2 . 3^2`**.
* Từ đó suy ra tập hợp các ước của 36 là: **`Ư(36) = {1; 2; 3; 4; 6; 9; 12; 18; 36}`**.
* Đối chiếu với điều kiện **`4 ≤ x ≤ 12`**, ta tìm được các giá trị thỏa mãn là: **`x ∈ {4; 6; 9; 12}`**.
* **Kết luận:** Vậy cô tổng phụ trách có **4 cách xếp đội hình**:
  1. Xếp mỗi hàng **4 bạn** (được 9 hàng).
  2. Xếp mỗi hàng **6 bạn** (được 6 hàng).
  3. Xếp mỗi hàng **9 bạn** (được 4 hàng).
  4. Xếp mỗi hàng **12 bạn** (được 3 hàng).

---

#### ✅ Lời giải Bài tập 3 - Nâng cao (10 Điểm):
* **Xét trường hợp 1: `p = 2`**
  Khi đó `p + 2 = 2 + 2 = 4` (là hợp số, loại).
* **Xét trường hợp 2: `p = 3`**
  Khi đó:
  * `p + 2 = 3 + 2 = 5` (là số nguyên tố).
  * `p + 4 = 3 + 4 = 7` (là số nguyên tố).
  ➔ Vậy **`p = 3`** hoàn toàn thỏa mãn đề bài!
* **Xét trường hợp 3: `p > 3`**
  Vì *p* là số nguyên tố lớn hơn 3 nên *p* không chia hết cho 3. Khi chia *p* cho 3 chỉ có thể xảy ra 2 trường hợp về số dư:
  * *Nếu p chia 3 dư 1* (`p = 3k + 1`): Khi đó `p + 2 = (3k + 1) + 2 = 3k + 3 ⋮ 3`. Vì `p + 2 > 3` và chia hết cho 3 nên `p + 2` là hợp số (loại).
  * *Nếu p chia 3 dư 2* (`p = 3k + 2`): Khi đó `p + 4 = (3k + 2) + 4 = 3k + 6 ⋮ 3`. Vì `p + 4 > 3` và chia hết cho 3 nên `p + 4` là hợp số (loại).
* **Kết luận:** Vậy chỉ có duy nhất một số nguyên tố thỏa mãn bài toán là **`p = 3`**.

</details>

---

## 🗺️ SƠ ĐỒ TỔNG KẾT KIẾN THỨC CỐT LÕI (DÀNH CHO ÔN THI)

| <div align="center">🎯 <b>TRỌNG TÂM BÀI 10: SỐ NGUYÊN TỐ & HỢP SỐ</b></div> |
| :--- |
| **🟠 NHÁNH 1: PHÂN LOẠI CÁC SỐ TỰ NHIÊN (ℕ)** |
| • **Nhóm đặc biệt (`0` và `1`):** **KHÔNG** là số nguyên tố, **KHÔNG** là hợp số.<br>• **Số nguyên tố (*a* > 1):** Chỉ có đúng **2 ước** là `1` và `chính nó`. *(Số `2` là số nguyên tố nhỏ nhất và chẵn duy nhất)*.<br>• **Hợp số (*a* > 1):** Có **nhiều hơn 2 ước** *(tức là có thêm ít nhất 1 ước khác 1 và chính nó)*. |
| **🔵 NHÁNH 2: PHÂN TÍCH MỘT SỐ RA THỪA SỐ NGUYÊN TỐ** |
| • **Bản chất:** Viết một số tự nhiên lớn hơn 1 dưới dạng **tích của các thừa số nguyên tố**.<br>• **Hai cách làm:** Dùng **Sơ đồ cây** (tách nhánh nhân) hoặc **Sơ đồ cột dọc** (chia liên tiếp cho 2, 3, 5, 7...).<br>• **Quy tắc trình bày:** Luôn thu gọn các thừa số giống nhau bằng **lũy thừa** và sắp xếp cơ số từ nhỏ đến lớn *(Ví dụ: `72 = 2^3 . 3^2`)*. |

---
[⬅️ Quay lại Trang chủ Mục lục](README.md)
