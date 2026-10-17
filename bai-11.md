[⬅️ Quay lại Trang chủ Mục lục](README.md)

# 📘 CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN
# 🌟 BÀI 11: ƯỚC CHUNG. ƯỚC CHUNG LỚN NHẤT
* **Môn học:** Toán học 6 (Tập 1) — *Bộ sách Kết nối tri thức với cuộc sống*
* **Thời lượng tự học:** 60 phút
* **Hình thức:** Học liệu số tương tác (Lý thuyết trực quan + Trò chơi vận dụng)

---

> [!NOTE]
> ### 🎯 MỤC TIÊU CẦN ĐẠT SAU BÀI HỌC
> 1. **Nhận biết** được khái niệm **ước chung (ƯC)** và **ước chung lớn nhất (ƯCLN)** của hai hay nhiều số tự nhiên.
> 2. **Thực hiện thành thạo quy trình 3 bước** tìm ƯCLN bằng cách phân tích các số ra thừa số nguyên tố, từ đó tìm được tập hợp ƯC thông qua ƯCLN.
> 3. **Hiểu và nhận diện** được khái niệm **hai số nguyên tố cùng nhau** và **phân số tối giản**.
> 4. **Vận dụng linh hoạt** ƯCLN để rút gọn phân số về tối giản và giải quyết các bài toán chia phần đều nhau trong thực tiễn.

---

## 🚀 KHỞI ĐỘNG: BÀI TOÁN CHIA QUÀ TÌNH NGUYỆN
**Tình huống:** Trong đợt quyên góp ủng hộ học sinh vùng cao, lớp 6A chuẩn bị được **24 quyển vở** và **36 chiếc bút bi**. Cô giáo muốn chia đều toàn bộ số vở và bút này vào các túi quà sao cho số quyển vở ở mỗi túi đều bằng nhau, và số chiếc bút ở mỗi túi cũng đều bằng nhau (không bị thừa ra quyển vở hay chiếc bút nào).

❓ **Câu hỏi tư duy:** *Cô giáo có thể chia được vào **nhiều nhất** là bao nhiêu túi quà? Khi chia vào số túi nhiều nhất đó, mỗi túi quà sẽ có mấy quyển vở và mấy chiếc bút?*

➔ Để giải quyết nhanh gọn bài toán chia đều "nhiều nhất" như thế này, Toán học cung cấp cho chúng ta công cụ **Ước chung và Ước chung lớn nhất**! Hãy cùng khám phá ngay dưới đây.

---

## 📖 NỘI DUNG 1: ƯỚC CHUNG VÀ ƯỚC CHUNG LỚN NHẤT

### 1.1. Khái niệm Ước chung (ƯC) và Ước chung lớn nhất (ƯCLN)
🔍 **Hoạt động khám phá 1:** Hãy liệt kê tập hợp các ước của `24` và `36`, sau đó tìm những số xuất hiện ở cả hai tập hợp:
* Tập hợp các ước của 24: **`Ư(24) = {1; 2; 3; 4; 6; 8; 12; 24}`**
* Tập hợp các ước của 36: **`Ư(36) = {1; 2; 3; 4; 6; 9; 12; 18; 36}`**
* Các số vừa là ước của 24, vừa là ước của 36 là: **`1; 2; 3; 4; 6; 12`**.

> [!IMPORTANT]
> ### 📌 ĐỊNH NGHĨA VÀ KÍ HIỆU TRỌNG TÂM
> * 🟢 **Ước chung** của hai hay nhiều số là **ước của tất cả** các số đó. Tập hợp các ước chung của *a* và *b* kí hiệu là **`ƯC(a, b)`**.
>   * **Quy tắc kiểm tra:** **`x ∈ ƯC(a, b)`** khi và chỉ khi đồng thời **`a ⋮ x`** và **`b ⋮ x`**.
> * 🟠 **Ước chung lớn nhất** của hai hay nhiều số là **số lớn nhất** trong tập hợp các ước chung của các số đó. Kí hiệu ước chung lớn nhất của *a* và *b* là **`ƯCLN(a, b)`**.

**Từ hoạt động khám phá trên, ta viết được:**
* Tập hợp ước chung: **`ƯC(24, 36) = {1; 2; 3; 4; 6; 12}`**.
* Số lớn nhất trong tập hợp này là `12`, nên: **`ƯCLN(24, 36) = 12`**.

---

### 1.2. Mối liên hệ đặc biệt giữa ƯC và ƯCLN
Quan sát kĩ tập hợp `ƯC(24, 36) = {1; 2; 3; 4; 6; 12}` và số `ƯCLN(24, 36) = 12`, ta nhận thấy một quy luật cực kỳ thú vị:

> [!TIP]
> ### 💡 NHẬN XÉT VÀNG
> * Tất cả các **ước chung** của hai hay nhiều số đều là **ước của ƯCLN** của các số đó!
> * **Trường hợp đặc biệt với số 1:** Với mọi số tự nhiên *a* và *b*, ta luôn có:
>   **`ƯCLN(a, 1) = 1`** và **`ƯCLN(a, b, 1) = 1`**.
> * **Trường hợp chia hết:** Nếu số *a* chia hết cho số *b* (`a ⋮ b` với *b ≠ 0*) thì **`ƯCLN(a, b) = b`** *(chính là số nhỏ hơn)!*
>   *(Ví dụ: Vì `45 ⋮ 15` nên không cần tính toán, kết luận ngay `ƯCLN(45, 15) = 15`)*.

#### 📝 Trạm dừng thực hành số 1
1. Biết **`ƯCLN(a, b) = 15`**. Không cần biết *a* và *b* là hai số nào, hãy tìm ngay tập hợp **`ƯC(a, b)`**.
2. Tìm nhanh: **`ƯCLN(32, 8)`** và **`ƯCLN(2026, 1)`**.

<details>
<summary>👉 <b>NHẤN VÀO ĐÂY ĐỂ XEM ĐÁP ÁN & LỜI GIẢI CHI TIẾT</b></summary>
<br>

* **Câu 1:** Vì ước chung của *a* và *b* chính là các ước của `ƯCLN(a, b)`, nên `ƯC(a, b) = Ư(15) = {1; 3; 5; 15}`. 🟢
* **Câu 2:** 
  * Vì `32 ⋮ 8` nên **`ƯCLN(32, 8) = 8`**. 🟢
  * Áp dụng tính chất số 1, ta có **`ƯCLN(2026, 1) = 1`**. 🟢

</details>

---

## 📖 NỘI DUNG 2: CÁCH TÌM ƯỚC CHUNG LỚN NHẤT (ƯCLN)

Khi gặp các số lớn như `84` và `180`, việc liệt kê từng ước sẽ rất mất thời gian và dễ sót nghiệm. Hãy sử dụng **Quy trình 3 bước bằng thừa số nguyên tố** dưới đây:

> [!IMPORTANT]
> ### 🌟 QUY TRÌNH 3 BƯỚC TÌM ƯCLN CỦA HAI HAY NHIỀU SỐ LỚN HƠN 1
> * **Bước 1 (Phân tích):** Phân tích mỗi số ra **thừa số nguyên tố**.
> * **Bước 2 (Chọn thừa số CHUNG):** Chọn ra các thừa số nguyên tố **CHUNG** (xuất hiện ở tất cả các số).
> * **Bước 3 (Lập tích với mũ NHỎ NHẤT):** Lập tích các thừa số đã chọn, mỗi thừa số lấy với **số mũ nhỏ nhất** của nó. Tích đó chính là **ƯCLN** phải tìm.

---

### Ví dụ mẫu chuẩn trình bày: Tìm `ƯCLN(84, 180)` và `ƯC(84, 180)`

| Các bước thực hiện | Trình bày chi tiết | Giải thích tư duy |
| :--- | :--- | :--- |
| **Bước 1: Phân tích ra TSNT** | • `84 = 2^2 . 3 . 7`<br>• `180 = 2^2 . 3^2 . 5` | Viết gọn dưới dạng lũy thừa và xếp từ nhỏ đến lớn. |
| **Bước 2: Chọn TSNT chung** | Thừa số nguyên tố chung là: **`2`** và **`3`** | *(Số 5 và 7 chỉ xuất hiện ở một bên nên loại bỏ)*. |
| **Bước 3: Lấy số mũ nhỏ nhất** | **`ƯCLN(84, 180) = 2^2 . 3^1 = 4 . 3 = 12`** | • Với cơ số `2`: Số mũ nhỏ nhất là `2` (`2^2`).<br>• Với cơ số `3`: Giữa `3^1` và `3^2`, lấy mũ nhỏ nhất là `3^1`. |
| **Bước mở rộng: Tìm ƯC** | **`ƯC(84, 180) = Ư(12) = {1; 2; 3; 4; 6; 12}`** | Lấy tất cả các ước của ƯCLN (12) thay vì tìm từng số! |

> [!WARNING]
> ### ⚡ MẸO GHI NHỚ NHANH (TRÁNH NHẦM LẪN VỚI BÀI 12)
> Khi tìm **ƯCLN** (dù tên gọi có chữ *"Lớn nhất"*), nhưng ở Bước 2 và Bước 3 ta lại lấy:
> **"Thừa số CHUNG — Số mũ NHỎ NHẤT"**!

#### 📝 Trạm dừng thực hành số 2 (Giải quyết bài toán Khởi động)
Quay lại bài toán đầu bài: Lớp 6A có **24 quyển vở** và **36 chiếc bút bi** chia đều vào các túi quà. Tìm số túi quà nhiều nhất có thể chia được và số vở, bút trong mỗi túi khi đó?

<details>
<summary>👉 <b>NHẤN VÀO ĐÂY ĐỂ XEM LỜI GIẢI KHOA HỌC</b></summary>
<br>

* **Bước 1:** Gọi số túi quà chia được là *x* (túi) (*x ∈ ℕ\**).
* **Bước 2:** Vì 24 quyển vở và 36 chiếc bút được chia đều vào *x* túi nên `24 ⋮ x` và `36 ⋮ x`. Do *x* là số túi **nhiều nhất** nên **`x = ƯCLN(24, 36)`**.
* **Bước 3:** Ta có `24 = 2^3 . 3` và `36 = 2^2 . 3^2`. Suy ra **`x = ƯCLN(24, 36) = 2^2 . 3 = 12` (túi)**.
* **Bước 4:** Khi chia thành 12 túi quà, mỗi túi sẽ có:
  * Số quyển vở là: `24 : 12 = 2` (quyển vở).
  * Số chiếc bút là: `36 : 12 = 3` (chiếc bút). 🟢

</details>

---

## 📖 NỘI DUNG 3: HAI SỐ NGUYÊN TỐ CÙNG NHAU & RÚT GỌN PHÂN SỐ

### 3.1. Hai số nguyên tố cùng nhau là gì?
Đôi khi phân tích hai số ra thừa số nguyên tố, ta không tìm thấy bất kỳ thừa số nguyên tố chung nào (ví dụ `8 = 2^3` và `9 = 3^2`). Khi đó `ƯCLN(8, 9) = 1`.

> [!IMPORTANT]
> ### 📌 ĐỊNH NGHĨA HAI SỐ NGUYÊN TỐ CÙNG NHAU
> * Hai số có **ƯCLN bằng 1** được gọi là **hai số nguyên tố cùng nhau**.
> * **Ví dụ:** `8` và `9` đều là hợp số, nhưng vì **`ƯCLN(8, 9) = 1`** nên `8` và `9` được gọi là **hai số nguyên tố cùng nhau**! Tương tự, hai số tự nhiên liên tiếp bất kỳ (như `14` và `15`) luôn nguyên tố cùng nhau.

---

### 3.2. Ứng dụng tìm ƯCLN để rút gọn về Phân số tối giản
* **Phân số tối giản** là phân số mà tử và mẫu chỉ có ước chung là `1` (tức là tử và mẫu là **hai số nguyên tố cùng nhau**: **`ƯCLN(a, b) = 1`**).
* **Quy tắc rút gọn 1 bước về tối giản:** Để rút gọn một phân số `a/b` về phân số tối giản ngay lập tức, ta chỉ cần **chia cả tử và mẫu cho `ƯCLN(a, b)`**!

**Ví dụ minh họa:** Rút gọn phân số **`84 / 180`** về phân số tối giản:
* Theo ví dụ trên, ta đã tìm được **`ƯCLN(84, 180) = 12`**.
* Chia cả tử và mẫu cho 12: **`84 / 180 = (84 : 12) / (180 : 12) = 7 / 15`**.
* Vì `ƯCLN(7, 15) = 1` nên **`7 / 15`** là phân số tối giản!

---

## 🎮 ĐẤU TRƯỜNG TRÍ TUỆ: THỬ THÁCH NHÀ TOÁN HỌC TRẺ
*(Phần ôn tập tương tác — Học sinh tự làm và click trực tiếp vào phương án mình chọn để mở khóa kết quả!)*

---

### 🏆 VÒNG 1: KHỞI ĐỘNG NHANH (10 Điểm / Câu)

**Câu 1:** Cho hai số đã được phân tích ra thừa số nguyên tố là **`a = 2^3 . 3^2 . 5`** và **`b = 2^2 . 3 . 7`**. Khi đó **`ƯCLN(a, b)`** bằng:
<details>
<summary>🔘 <b>Phương án A: 2^3 . 3^2 . 5 . 7</b></summary>
❌ <b>Nhầm quy tắc rồi!</b> Bạn đang lấy cả thừa số riêng và số mũ lớn nhất mất rồi. Với ƯCLN, chỉ được chọn thừa số <b>CHUNG</b> với số mũ <b>NHỎ NHẤT</b> thôi nhé!
</details>
<details>
<summary>🔘 <b>Phương án B: 2^2 . 3 = 12</b></summary>
🎉 <b>CHÍNH XÁC TUYỆT ĐỐI! (+10 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Thừa số nguyên tố chung của <i>a</i> và <i>b</i> là <b>2</b> và <b>3</b> (loại 5 và 7). Số mũ nhỏ nhất của 2 là `2^2`, của 3 là `3^1`. Vậy `ƯCLN(a, b) = 2^2 . 3 = 12`!
</details>
<details>
<summary>🔘 <b>Phương án C: 2^3 . 3^2 = 72</b></summary>
❌ <b>Sai rồi!</b> Bạn đã chọn đúng thừa số chung là 2 và 3, nhưng lại lấy số mũ lớn nhất. Phải lấy số mũ <b>nhỏ nhất</b> nhé!
</details>

<br>

**Câu 2:** Cặp số nào dưới đây là **hai số nguyên tố cùng nhau**?
<details>
<summary>🔘 <b>Phương án A: 9 và 15</b></summary>
❌ <b>Chưa đúng!</b> Cả 9 và 15 đều chia hết cho 3 nên `ƯCLN(9, 15) = 3 ≠ 1`. Chúng không nguyên tố cùng nhau.
</details>
<details>
<summary>🔘 <b>Phương án B: 14 và 21</b></summary>
❌ <b>Chưa đúng!</b> Cả 14 và 21 đều chia hết cho 7 nên `ƯCLN(14, 21) = 7 ≠ 1`.
</details>
<details>
<summary>🔘 <b>Phương án C: 15 và 16</b></summary>
🎉 <b>XUẤT SẮC! (+10 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Ta có `15 = 3 . 5` và `16 = 2^4`. Hai số này không có thừa số nguyên tố chung nào nên `ƯCLN(15, 16) = 1`. Vậy 15 và 16 là hai số nguyên tố cùng nhau!
</details>

---

### 🔥 VÒNG 2: TĂNG TỐC SUY LUẬN (20 Điểm / Câu)

**Câu 3:** Trong các phân số sau: **`12/20 ; 17/51 ; 25/36 ; 39/65`**, phân số nào là **phân số tối giản**?
<details>
<summary>🔘 <b>Phương án A: 17/51</b></summary>
❌ <b>Cẩn thận bị lừa!</b> Số 17 là số nguyên tố, nhưng `51 = 17 . 3` nên `51 ⋮ 17`! Phân số này rút gọn được cho 17 thành `1/3` nhé.
</details>
<details>
<summary>🔘 <b>Phương án B: 25/36</b></summary>
🎉 <b>ĐỈNH CAO TƯ DUY! (+20 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Ta có `25 = 5^2` và `36 = 2^2 . 3^2`. Vì tử và mẫu không có thừa số nguyên tố chung nào nên `ƯCLN(25, 36) = 1`. Do đó <b>25/36</b> là phân số tối giản! (Còn `12/20` rút gọn cho 4; `39/65` rút gọn cho 13).
</details>
<details>
<summary>🔘 <b>Phương án C: 39/65</b></summary>
❌ <b>Chưa đúng!</b> Cả 39 và 65 đều chia hết cho 13 (`39 = 13 . 3` và `65 = 13 . 5`) nên phân số này chưa tối giản.
</details>

<br>

**Câu 4:** Tìm số tự nhiên **`x`** lớn nhất, biết rằng **`70 ⋮ x`**, **`84 ⋮ x`** và **`140 ⋮ x`**:
<details>
<summary>🔘 <b>Phương án A: x = 7</b></summary>
❌ <b>Chưa chính xác!</b> Số 7 đúng là ước chung của 3 số trên, nhưng đề bài yêu cầu tìm số <i>x</i> <b>lớn nhất</b>!
</details>
<details>
<summary>🔘 <b>Phương án B: x = 14</b></summary>
🎉 <b>CHÍNH XÁC TUYỆT ĐỐI! (+20 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Vì `70 ⋮ x`, `84 ⋮ x`, `140 ⋮ x` và <i>x</i> lớn nhất nên `x = ƯCLN(70, 84, 140)`.<br>
Ta phân tích: `70 = 2 . 5 . 7`; `84 = 2^2 . 3 . 7`; `140 = 2^2 . 5 . 7`.<br>
Thừa số chung của cả 3 số là <b>2</b> và <b>7</b> với mũ nhỏ nhất là 1. Vậy <b>x = 2 . 7 = 14</b>!
</details>
<details>
<summary>🔘 <b>Phương án C: x = 28</b></summary>
❌ <b>Sai rồi!</b> Số 70 không chia hết cho 28 nhé!
</details>

---

### 👑 VÒNG 3: CHINH PHỤC TỰ LUẬN & TOÁN THỰC TẾ (40 Điểm)
*(Hoàn thành 3 bài tập chuẩn SGK vào vở, sau đó mở khóa đáp án để tự chấm điểm)*

* **Bài tập 1 (Tìm tập hợp ƯC thông qua ƯCLN có điều kiện):**
  Tìm số tự nhiên *a*, biết rằng **`90 ⋮ a`**, **`150 ⋮ a`** và **`5 < a < 30`**.

* **Bài tập 2 (Bài toán thực tế chia tổ bác sĩ - SGK Toán 6):**
  Một đội y tế tình nguyện có **24 bác sĩ** và **108 y tá**. Có thể chia đội y tế đó nhiều nhất thành mấy tổ để số bác sĩ cũng như số y tá được chia đều vào mỗi tổ? Khi đó, mỗi tổ có bao nhiêu bác sĩ và bao nhiêu y tá?

* **Bài tập 3 (Thử thách nâng cao dành cho học sinh giỏi):**
  Chứng minh rằng với mọi số tự nhiên *n*, phân số **`(2n + 3) / (3n + 4)`** luôn là phân số tối giản.

<details>
<summary>🔓 <b>MỞ KHÓA HƯỚNG DẪN GIẢI VÀ THANG ĐIỂM TỰ CHẤM (VÒNG 3)</b></summary>
<br>

#### ✅ Lời giải Bài tập 1 (15 Điểm):
* Vì `90 ⋮ a` và `150 ⋮ a` nên **`a ∈ ƯC(90, 150)`**.
* **Tìm ƯCLN(90, 150):**
  * Phân tích ra thừa số nguyên tố: `90 = 2 . 3^2 . 5` và `150 = 2 . 3 . 5^2`.
  * Suy ra **`ƯCLN(90, 150) = 2 . 3 . 5 = 30`**.
* **Tìm tập hợp ƯC(90, 150):**
  `ƯC(90, 150) = Ư(30) = {1; 2; 3; 5; 6; 10; 15; 30}`.
* Kết hợp với điều kiện **`5 < a < 30`**, ta chọn được các giá trị thỏa mãn:
  **`a ∈ {6; 10; 15}`**.

---

#### ✅ Lời giải Bài tập 2 (15 Điểm):
* Gọi số tổ có thể chia được nhiều nhất là *x* (tổ) (*x ∈ ℕ\**).
* Vì 24 bác sĩ và 108 y tá được chia đều vào *x* tổ và *x* là lớn nhất nên:
  **`x = ƯCLN(24, 108)`**.
* Ta phân tích ra thừa số nguyên tố:
  * `24 = 2^3 . 3`
  * `108 = 2^2 . 3^3`
  * Suy ra **`x = ƯCLN(24, 108) = 2^2 . 3 = 12`**.
* **Kết luận:** Có thể chia đội y tế nhiều nhất thành **12 tổ**. Khi đó, mỗi tổ có:
  * Số bác sĩ là: `24 : 12 =` **2 bác sĩ**.
  * Số y tá là: `108 : 12 =` **9 y tá**.

---

#### ✅ Lời giải Bài tập 3 - Nâng cao (10 Điểm):
* Để chứng minh phân số `(2n + 3) / (3n + 4)` tối giản, ta cần chứng minh tử và mẫu là hai số nguyên tố cùng nhau, tức là **`ƯCLN(2n + 3, 3n + 4) = 1`**.
* Gọi **`d = ƯCLN(2n + 3, 3n + 4)`** (*d ∈ ℕ\**).
* Khi đó ta có:
  * `(2n + 3) ⋮ d` ➔ Nhân với 3 ta được: **`3.(2n + 3) = (6n + 9) ⋮ d`** *(1)*.
  * `(3n + 4) ⋮ d` ➔ Nhân với 2 ta được: **`2.(3n + 4) = (6n + 8) ⋮ d`** *(2)*.
* Từ *(1)* và *(2)*, áp dụng tính chất chia hết của một hiệu, ta lấy hiệu hai biểu thức:
  **`[(6n + 9) - (6n + 8)] ⋮ d`** ➔ **`1 ⋮ d`**.
* Vì `1 ⋮ d` và *d ∈ ℕ\** nên bắt buộc **`d = 1`**.
* **Kết luận:** Vậy `ƯCLN(2n + 3, 3n + 4) = 1`, suy ra phân số **`(2n + 3) / (3n + 4)` luôn tối giản** với mọi số tự nhiên *n* (Điều phải chứng minh)!

</details>

---

## 🗺️ SƠ ĐỒ TỔNG KẾT KIẾN THỨC CỐT LÕI (DÀNH CHO ÔN THI)

| <div align="center">🎯 <b>TRỌNG TÂM BÀI 11: ƯỚC CHUNG & ƯỚC CHUNG LỚN NHẤT</b></div> |
| :--- |
| **🟠 NHÁNH 1: KHÁI NIỆM & QUY TRÌNH 3 BƯỚC TÌM ƯCLN** |
| • **Điều kiện Ước chung:** `x ∈ ƯC(a, b)` ⟺ `a ⋮ x` và `b ⋮ x`.<br>• **3 Bước tìm ƯCLN(a, b):**<br>  1. Phân tích mỗi số ra **thừa số nguyên tố**.<br>  2. Chọn các thừa số nguyên tố **CHUNG**.<br>  3. Nhân các thừa số đã chọn với **số mũ NHỎ NHẤT**.<br>• **Tìm ƯC từ ƯCLN:** Tập hợp `ƯC(a, b)` chính là tập hợp tất cả các **ước của `ƯCLN(a, b)`**. |
| **🔵 NHÁNH 2: NGUYÊN TỐ CÙNG NHAU & RÚT GỌN PHÂN SỐ** |
| • **Hai số nguyên tố cùng nhau:** Là hai số có **`ƯCLN(a, b) = 1`**.<br>• **Phân số tối giản:** Phân số `a/b` tối giản khi `ƯCLN(a, b) = 1`. Nếu chưa tối giản, chia cả tử và mẫu cho `ƯCLN(a, b)` sẽ được ngay phân số tối giản.<br>• **Dấu hiệu nhận biết bài toán thực tế dùng ƯCLN:** Đề bài yêu cầu *"chia đều"*, *"xếp đều"* các vật vào các nhóm/túi/tổ sao cho số nhóm/túi/tổ là **"nhiều nhất"** (hoặc *"lớn nhất"*). |

---
[⬅️ Quay lại Trang chủ Mục lục](README.md)
