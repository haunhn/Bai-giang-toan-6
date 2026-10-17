[⬅️ Quay lại Trang chủ Mục lục](README.md)

# 📘 CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN
# 🌟 BÀI 12: BỘI CHUNG. BỘI CHUNG NHỎ NHẤT
* **Môn học:** Toán học 6 (Tập 1) — *Bộ sách Kết nối tri thức với cuộc sống*
* **Thời lượng tự học:** 60 phút
* **Hình thức:** Học liệu số tương tác (Lý thuyết trực quan + Trò chơi vận dụng)

---

> [!NOTE]
> ### 🎯 MỤC TIÊU CẦN ĐẠT SAU BÀI HỌC
> 1. **Nhận biết** được khái niệm **bội chung (BC)** và **bội chung nhỏ nhất (BCNN)** của hai hay nhiều số tự nhiên.
> 2. **Thực hiện thành thạo quy trình 3 bước** tìm BCNN bằng cách phân tích các số ra thừa số nguyên tố, từ đó tìm được tập hợp BC thông qua BCNN.
> 3. **Phân biệt sắc bén** sự đối lập giữa cách tìm **ƯCLN** và **BCNN** để không bao giờ bị nhầm lẫn khi làm bài thi.
> 4. **Vận dụng linh hoạt** BCNN để quy đồng mẫu các phân số và giải quyết các bài toán thực tiễn có tính chu kỳ lặp lại.

---

## 🚀 KHỞI ĐỘNG: BÀI TOÁN NHỊP ĐÈN NHẤP NHÁY
**Tình huống:** Trên một biển quảng cáo điện tử có hai dây đèn LED màu xanh và màu đỏ:
* Dây đèn màu **xanh** cứ sau mỗi **4 giây** lại phát sáng một lần.
* Dây đèn màu **đỏ** cứ sau mỗi **6 giây** lại phát sáng một lần.

Giả sử tại thời điểm bắt đầu bấm giờ (`0` giây), cả hai dây đèn cùng phát sáng một lúc.

❓ **Câu hỏi tư duy:** *Sau ít nhất bao nhiêu giây nữa kể từ lúc bấm giờ thì cả hai dây đèn lại **cùng phát sáng một lúc** lần tiếp theo? Và trong vòng 1 phút (60 giây), có tất cả bao nhiêu lần hai dây đèn cùng phát sáng?*

➔ Những bài toán tìm thời điểm lặp lại trùng nhau sớm nhất như thế này chính là ứng dụng tiêu biểu của **Bội chung và Bội chung nhỏ nhất**! Hãy cùng khám phá ngay dưới đây.

---

## 📖 NỘI DUNG 1: BỘI CHUNG VÀ BỘI CHUNG NHỎ NHẤT

### 1.1. Khái niệm Bội chung (BC) và Bội chung nhỏ nhất (BCNN)
🔍 **Hoạt động khám phá 1:** Hãy liệt kê các bội của `4` và các bội của `6`, sau đó tìm các số xuất hiện ở cả hai tập hợp:
* Tập hợp các bội của 4: **`B(4) = {0; 4; 8; 12; 16; 20; 24; 28; 32; 36; ...}`**
* Tập hợp các bội của 6: **`B(6) = {0; 6; 12; 18; 24; 30; 36; 42; ...}`**
* Các số vừa là bội của 4, vừa là bội của 6 là: **`0; 12; 24; 36; ...`**

> [!IMPORTANT]
> ### 📌 ĐỊNH NGHĨA VÀ KÍ HIỆU TRỌNG TÂM
> * 🟢 **Bội chung** của hai hay nhiều số là **bội của tất cả** các số đó. Tập hợp các bội chung của *a* và *b* kí hiệu là **`BC(a, b)`**.
>   * **Quy tắc kiểm tra:** **`x ∈ BC(a, b)`** khi và chỉ khi đồng thời **`x ⋮ a`** và **`x ⋮ b`**.
> * 🟠 **Bội chung nhỏ nhất** của hai hay nhiều số là **số nhỏ nhất khác `0`** trong tập hợp các bội chung của các số đó. Kí hiệu bội chung nhỏ nhất của *a* và *b* là **`BCNN(a, b)`**.

**Từ hoạt động khám phá trên, ta viết được:**
* Tập hợp bội chung: **`BC(4, 6) = {0; 12; 24; 36; ...}`**.
* Số nhỏ nhất **khác 0** trong tập hợp này là `12`, nên: **`BCNN(4, 6) = 12`**.

> [!CAUTION]
> ### 🚨 CẢNH BÁO "BẪY" SỐ 0!
> Số **`0`** luôn nằm trong tập hợp bội chung của mọi số tự nhiên (`0 ∈ BC(a, b)`). Tuy nhiên, khi tìm **Bội chung nhỏ nhất (BCNN)**, định nghĩa bắt buộc phải lấy **số nhỏ nhất KHÁC 0**! Tuyệt đối không bao giờ kết luận `BCNN(a, b) = 0` nhé!

---

### 1.2. Mối liên hệ đặc biệt giữa BC và BCNN
Quan sát tập hợp `BC(4, 6) = {0; 12; 24; 36; ...}` và số `BCNN(4, 6) = 12`, ta thấy `0, 12, 24, 36...` chính là kết quả khi nhân `12` lần lượt với `0, 1, 2, 3...`!

> [!TIP]
> ### 💡 NHẬN XÉT VÀNG
> * Tất cả các **bội chung** của hai hay nhiều số đều là **bội của BCNN** của các số đó! Do đó, để tìm tập hợp `BC(a, b)`, ta chỉ cần tìm `BCNN(a, b)`, rồi nhân số đó lần lượt với `0, 1, 2, 3, ...`
> * **Trường hợp đặc biệt với số 1:** Với mọi số tự nhiên *a* và *b* khác 0, ta luôn có:
>   **`BCNN(a, 1) = a`** và **`BCNN(a, b, 1) = BCNN(a, b)`**.
> * **Trường hợp chia hết:** Nếu số *a* chia hết cho số *b* (`a ⋮ b`) thì **`BCNN(a, b) = a`** *(chính là số lớn hơn)!*
>   *(Ví dụ: Vì `45 ⋮ 15` nên không cần tính toán, kết luận ngay `BCNN(45, 15) = 45`)*.

#### 📝 Trạm dừng thực hành số 1
1. Biết **`BCNN(a, b) = 30`**. Hãy tìm tập hợp **`BC(a, b)`** gồm các số nhỏ hơn 100.
2. Tìm nhanh: **`BCNN(18, 6)`** và **`BCNN(25, 1)`**.

<details>
<summary>👉 <b>NHẤN VÀO ĐÂY ĐỂ XEM ĐÁP ÁN & LỜI GIẢI CHI TIẾT</b></summary>
<br>

* **Câu 1:** Vì `BC(a, b) = B(30)`, ta nhân 30 lần lượt với `0, 1, 2, 3, ...` Các bội chung nhỏ hơn 100 là: **`{0; 30; 60; 90}`**. 🟢
* **Câu 2:** 
  * Vì `18 ⋮ 6` nên **`BCNN(18, 6) = 18`** (lấy số lớn hơn). 🟢
  * Áp dụng tính chất số 1, ta có **`BCNN(25, 1) = 25`**. 🟢

</details>

---

## 📖 NỘI DUNG 2: CÁCH TÌM BỘI CHUNG NHỎ NHẤT (BCNN)

> [!IMPORTANT]
> ### 🌟 QUY TRÌNH 3 BƯỚC TÌM BCNN CỦA HAI HAY NHIỀU SỐ LỚN HƠN 1
> * **Bước 1 (Phân tích):** Phân tích mỗi số ra **thừa số nguyên tố**.
> * **Bước 2 (Chọn thừa số CHUNG và RIÊNG):** Chọn ra tất cả các thừa số nguyên tố **CHUNG và RIÊNG** (mặt số nguyên tố nào xuất hiện cũng phải lấy hết).
> * **Bước 3 (Lập tích với mũ LỚN NHẤT):** Lập tích các thừa số đã chọn, mỗi thừa số lấy với **số mũ lớn nhất** của nó. Tích đó chính là **BCNN** phải tìm.

---

### Ví dụ mẫu chuẩn trình bày: Tìm `BCNN(12, 18, 30)` và `BC(12, 18, 30)`

| Các bước thực hiện | Trình bày chi tiết | Giải thích tư duy |
| :--- | :--- | :--- |
| **Bước 1: Phân tích ra TSNT** | • `12 = 2^2 . 3`<br>• `18 = 2 . 3^2`<br>• `30 = 2 . 3 . 5` | Viết gọn dưới dạng lũy thừa và xếp từ nhỏ đến lớn. |
| **Bước 2: Chọn TSNT chung & riêng** | Thừa số nguyên tố chung và riêng là: **`2`**, **`3`** và **`5`** | *(Lấy cả 2, 3 là thừa số chung và lấy cả 5 là thừa số riêng)*. |
| **Bước 3: Lấy số mũ lớn nhất** | **`BCNN(12, 18, 30) = 2^2 . 3^2 . 5 = 4 . 9 . 5 = 180`** | • Với cơ số `2`: Số mũ lớn nhất là `2^2`.<br>• Với cơ số `3`: Số mũ lớn nhất là `3^2`.<br>• Với cơ số `5`: Số mũ lớn nhất là `5^1`. |
| **Bước mở rộng: Tìm BC** | **`BC(12, 18, 30) = B(180) = {0; 180; 360; 540; ...}`** | Nhân `BCNN` (180) lần lượt với `0, 1, 2, 3...` |

---

### ⚖️ BẢNG ĐỐI CHIẾU "VÀNG": PHÂN BIỆT ƯCLN VÀ BCNN (TRÁNH NHẦM LẪN)
Hai khái niệm **ƯCLN** (Bài 11) và **BCNN** (Bài 12) có quy tắc tìm **ngược nhau hoàn toàn**. Hãy nhìn bảng so sánh này để nhớ suốt đời:

| Tiêu chí so sánh | 🟠 ƯỚC CHUNG LỚN NHẤT — `ƯCLN(a, b)` | 🔵 BỘI CHUNG NHỎ NHẤT — `BCNN(a, b)` |
| :--- | :--- | :--- |
| **Kí hiệu chia hết** | `a ⋮ x` và `b ⋮ x` *(Số cần tìm **x nằm ở bên phải** dấu chia hết - là số chia)* | `x ⋮ a` và `x ⋮ b` *(Số cần tìm **x nằm ở bên trái** dấu chia hết - là số bị chia)* |
| **Bước 2: Chọn thừa số** | Chỉ chọn thừa số nguyên tố **CHUNG** | Chọn thừa số nguyên tố **CHUNG và RIÊNG** |
| **Bước 3: Chọn số mũ** | Lấy số mũ **NHỎ NHẤT** | Lấy số mũ **LỚN NHẤT** |
| **Khi `a ⋮ b`** | `ƯCLN(a, b) = b` *(Lấy **số nhỏ**)* | `BCNN(a, b) = a` *(Lấy **số lớn**)* |
| **Khi `a, b` nguyên tố cùng nhau** | `ƯCLN(a, b) = 1` | `BCNN(a, b) = a . b` *(Bằng tích hai số)* |
| **Từ khóa bài toán thực tế** | *"Chia đều vào các túi/tổ/nhóm"*, *"Số nhóm **nhiều nhất / lớn nhất**"* | *"Cùng lặp lại / cùng trực nhật"*, *"Xếp vừa đủ không thừa"*, *"Số lượng **ít nhất / nhỏ nhất**"* |

---

## 📖 NỘI DUNG 3: ỨNG DỤNG BCNN ĐỂ QUY ĐỒNG MẪU CÁC PHÂN SỐ

Ở Tiểu học, khi quy đồng mẫu hai phân số, ta thường lấy hai mẫu nhân với nhau khiến mẫu chung rất lớn. Với công cụ **BCNN**, ta sẽ tìm được **Mẫu số chung nhỏ nhất**!

> [!IMPORTANT]
> ### 📌 QUY TRÌNH 3 BƯỚC QUY ĐỒNG MẪU NHIỀU PHÂN SỐ
> * **Bước 1 (Tìm mẫu chung):** Tìm một bội chung của các mẫu (thường chọn là **BCNN** của các mẫu) để làm **mẫu chung**.
> * **Bước 2 (Tìm thừa số phụ):** Tìm **thừa số phụ** của mỗi mẫu bằng cách lấy **mẫu chung chia cho từng mẫu riêng**.
> * **Bước 3 (Nhân cả tử và mẫu):** Nhân cả tử và mẫu của mỗi phân số với thừa số phụ tương ứng của nó.

**Ví dụ minh họa:** Quy đồng mẫu hai phân số **`5 / 12`** và **`7 / 18`**:
* **Bước 1 (Tìm mẫu chung):** Ta có `12 = 2^2 . 3` và `18 = 2 . 3^2`.
  ➔ Mẫu chung là **`BCNN(12, 18) = 2^2 . 3^2 = 36`**.
* **Bước 2 (Tìm thừa số phụ):**
  * Thừa số phụ của mẫu 12 là: `36 : 12 =` **`3`**.
  * Thừa số phụ của mẫu 18 là: `36 : 18 =` **`2`**.
* **Bước 3 (Nhân tử và mẫu với thừa số phụ):**
  * **`5 / 12 = (5 . 3) / (12 . 3) = 15 / 36`**
  * **`7 / 18 = (7 . 2) / (18 . 2) = 14 / 36`**

---

## 🎮 ĐẤU TRƯỜNG TRÍ TUỆ: THỬ THÁCH NHÀ TOÁN HỌC TRẺ
*(Phần ôn tập tương tác — Học sinh tự làm và click trực tiếp vào phương án mình chọn để mở khóa kết quả!)*

---

### 🏆 VÒNG 1: KHỞI ĐỘNG NHANH (10 Điểm / Câu)

**Câu 1:** Cho hai số đã được phân tích ra thừa số nguyên tố là **`a = 2^2 . 3 . 5`** và **`b = 2 . 3^3 . 7`**. Khi đó **`BCNN(a, b)`** bằng:
<details>
<summary>🔘 <b>Phương án A: 2 . 3</b></summary>
❌ <b>Nhầm sang ƯCLN rồi!</b> `2 . 3` là thừa số chung với mũ nhỏ nhất (đây là ƯCLN). Để tìm BCNN, bạn phải lấy cả thừa số <b>chung và riêng</b> với số mũ <b>lớn nhất</b> nhé!
</details>
<details>
<summary>🔘 <b>Phương án B: 2^2 . 3^3 . 5 . 7</b></summary>
🎉 <b>CHÍNH XÁC TUYỆT ĐỐI! (+10 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Các thừa số nguyên tố chung và riêng của <i>a</i> và <i>b</i> là <b>2, 3, 5, 7</b>. Số mũ lớn nhất của 2 là `2^2`, của 3 là `3^3`, của 5 là `5^1`, của 7 là `7^1`. Vậy `BCNN(a, b) = 2^2 . 3^3 . 5 . 7`!
</details>
<details>
<summary>🔘 <b>Phương án C: 2^2 . 3^3</b></summary>
❌ <b>Thiếu thừa số riêng rồi!</b> Bạn đã lấy đúng số mũ lớn nhất của 2 và 3, nhưng lại bỏ quên hai thừa số nguyên tố riêng là <b>5</b> và <b>7</b>!
</details>

<br>

**Câu 2:** Giá trị của **`BCNN(15, 45, 1)`** bằng bao nhiêu?
<details>
<summary>🔘 <b>Phương án A: 1</b></summary>
❌ <b>Bị lừa rồi!</b> `ƯCLN(15, 45, 1)` mới bằng 1, còn đây là <b>BCNN</b> (Bội chung nhỏ nhất) nhé!
</details>
<details>
<summary>🔘 <b>Phương án B: 15</b></summary>
❌ <b>Chưa đúng!</b> Số 15 không chia hết cho 45 nên 15 không thể là bội của 45 được.
</details>
<details>
<summary>🔘 <b>Phương án C: 45</b></summary>
🎉 <b>XUẤT SẮC! (+10 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Ta có `BCNN(15, 45, 1) = BCNN(15, 45)`. Vì `45 ⋮ 15` nên trong hai số này, số lớn hơn là <b>45</b> chính là BCNN!
</details>

---

### 🔥 VÒNG 2: TĂNG TỐC SUY LUẬN (20 Điểm / Câu)

**Câu 3:** Tìm số tự nhiên **`x`** nhỏ nhất khác 0, biết rằng **`x ⋮ 8`**, **`x ⋮ 12`** và **`x ⋮ 15`**:
<details>
<summary>🔘 <b>Phương án A: x = 60</b></summary>
❌ <b>Chưa đúng!</b> Số 60 chia hết cho 12 và 15, nhưng `60 ∤ 8` (60 chia 8 được 7 dư 4).
</details>
<details>
<summary>🔘 <b>Phương án B: x = 120</b></summary>
🎉 <b>ĐỈNH CAO TƯ DUY! (+20 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Vì `x ⋮ 8`, `x ⋮ 12`, `x ⋮ 15` và <i>x</i> nhỏ nhất khác 0 nên `x = BCNN(8, 12, 15)`.<br>
Ta phân tích: `8 = 2^3`; `12 = 2^2 . 3`; `15 = 3 . 5`.<br>
Lấy các thừa số chung và riêng (2, 3, 5) với mũ lớn nhất: <b>x = 2^3 . 3 . 5 = 8 . 3 . 5 = 120</b>!
</details>
<details>
<summary>🔘 <b>Phương án C: x = 240</b></summary>
❌ <b>Chưa chính xác!</b> Số 240 đúng là bội chung của 8, 12, 15 nhưng chưa phải là số <b>nhỏ nhất</b> khác 0!
</details>

<br>

**Câu 4:** Khi quy đồng mẫu ba phân số **`3/8 ; 5/12 ; 7/18`**, mẫu số chung nhỏ nhất của ba phân số này là:
<details>
<summary>🔘 <b>Phương án A: 36</b></summary>
❌ <b>Chưa đúng!</b> 36 chia hết cho 12 và 18, nhưng `36 ∤ 8` nên không làm mẫu chung cho phân số `3/8` được.
</details>
<details>
<summary>🔘 <b>Phương án B: 72</b></summary>
🎉 <b>CHÍNH XÁC TUYỆT ĐỐI! (+20 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Mẫu chung nhỏ nhất chính là `BCNN(8, 12, 18)`. Ta có `8 = 2^3`; `12 = 2^2 . 3`; `18 = 2 . 3^2`. Suy ra `BCNN(8, 12, 18) = 2^3 . 3^2 = 8 . 9 =` <b>72</b>!
</details>
<details>
<summary>🔘 <b>Phương án C: 144</b></summary>
❌ <b>Chưa tối ưu!</b> 144 là một bội chung của 8, 12, 18 nhưng chưa phải là mẫu số chung <b>nhỏ nhất</b>.
</details>

---

### 👑 VÒNG 3: CHINH PHỤC TỰ LUẬN & TOÁN THỰC TẾ (40 Điểm)
*(Hoàn thành 3 bài tập chuẩn SGK vào vở, sau đó mở khóa đáp án để tự chấm điểm)*

* **Bài tập 1 (Tìm tập hợp BC thông qua BCNN có điều kiện):**
  Tìm số tự nhiên *x*, biết rằng **`x ⋮ 10`**, **`x ⋮ 12`**, **`x ⋮ 15`** và **`100 < x < 250`**.

* **Bài tập 2 (Bài toán thực tế xếp hàng đồng diễn - SGK Toán 6):**
  Học sinh khối 6 của một trường THCS khi xếp thành **12 hàng**, **15 hàng** hoặc **18 hàng** để tập đồng diễn thể dục thì đều **vừa đủ hàng** (không thừa bạn nào). Tính số học sinh khối 6 của trường đó, biết rằng số học sinh trong khoảng từ **300 đến 400 em**.

* **Bài tập 3 (Thử thách nâng cao — Bài toán chia có cùng số dư):**
  Tìm số tự nhiên *a* nhỏ nhất khác 2, biết rằng khi chia *a* cho **5**, cho **7** và cho **9** thì đều có **số dư là 2**.

<details>
<summary>🔓 <b>MỞ KHÓA HƯỚNG DẪN GIẢI VÀ THANG ĐIỂM TỰ CHẤM (VÒNG 3)</b></summary>
<br>

#### ✅ Lời giải Bài tập 1 (15 Điểm):
* Vì `x ⋮ 10`, `x ⋮ 12` và `x ⋮ 15` nên **`x ∈ BC(10, 12, 15)`**.
* **Tìm BCNN(10, 12, 15):**
  * Phân tích ra thừa số nguyên tố: `10 = 2 . 5`; `12 = 2^2 . 3`; `15 = 3 . 5`.
  * Suy ra **`BCNN(10, 12, 15) = 2^2 . 3 . 5 = 60`**.
* **Tìm tập hợp BC(10, 12, 15):**
  `BC(10, 12, 15) = B(60) = {0; 60; 120; 180; 240; 300; ...}`.
* Kết hợp với điều kiện **`100 < x < 250`**, ta chọn được các giá trị thỏa mãn:
  **`x ∈ {120; 180; 240}`**.

---

#### ✅ Lời giải Bài tập 2 (15 Điểm):
* Gọi số học sinh khối 6 của trường là *x* (học sinh), điều kiện: *x ∈ ℕ\** và **`300 ≤ x ≤ 400`**.
* Vì khi xếp thành 12 hàng, 15 hàng hoặc 18 hàng đều vừa đủ nên `x ⋮ 12`, `x ⋮ 15` và `x ⋮ 18`. Suy ra **`x ∈ BC(12, 15, 18)`**.
* **Tìm BCNN(12, 15, 18):**
  * Ta có: `12 = 2^2 . 3`; `15 = 3 . 5`; `18 = 2 . 3^2`.
  * Suy ra **`BCNN(12, 15, 18) = 2^2 . 3^2 . 5 = 4 . 9 . 5 = 180`**.
* Do đó: **`x ∈ BC(12, 15, 18) = B(180) = {0; 180; 360; 540; ...}`**.
* Vì **`300 ≤ x ≤ 400`** nên ta chọn được giá trị duy nhất thỏa mãn là **`x = 360`**.
* **Kết luận:** Vậy khối 6 của trường đó có **360 học sinh**.

---

#### ✅ Lời giải Bài tập 3 - Nâng cao (10 Điểm):
* Vì số tự nhiên *a* khi chia cho 5, cho 7 và cho 9 đều dư 2, nên nếu ta bớt *a* đi 2 đơn vị thì số **`(a - 2)` sẽ chia hết cho cả 5, 7 và 9**:
  * `(a - 2) ⋮ 5`
  * `(a - 2) ⋮ 7`
  * `(a - 2) ⋮ 9`
  ➔ Suy ra **`(a - 2) ∈ BC(5, 7, 9)`**.
* Để *a* là số tự nhiên nhỏ nhất khác 2 (tức là `a - 2 > 0` và `a - 2` nhỏ nhất), thì **`(a - 2)` phải bằng `BCNN(5, 7, 9)`**.
* Vì ba số `5`, `7` và `9 = 3^2` đôi một nguyên tố cùng nhau (không có thừa số nguyên tố chung nào), nên:
  **`BCNN(5, 7, 9) = 5 . 7 . 9 = 315`**.
* Từ `a - 2 = 315` ➔ `a = 315 + 2 = 317`.
* **Kết luận:** Vậy số tự nhiên cần tìm là **`a = 317`**.

</details>

---

## 🗺️ SƠ ĐỒ TỔNG KẾT KIẾN THỨC CỐT LÕI (DÀNH CHO ÔN THI)

| <div align="center">🎯 <b>TRỌNG TÂM BÀI 12: BỘI CHUNG & BỘI CHUNG NHỎ NHẤT</b></div> |
| :--- |
| **🟠 NHÁNH 1: KHÁI NIỆM & QUY TRÌNH 3 BƯỚC TÌM BCNN** |
| • **Điều kiện Bội chung:** `x ∈ BC(a, b)` ⟺ `x ⋮ a` và `x ⋮ b`.<br>• **3 Bước tìm BCNN(a, b):**<br>  1. Phân tích mỗi số ra **thừa số nguyên tố**.<br>  2. Chọn các thừa số nguyên tố **CHUNG và RIÊNG**.<br>  3. Nhân các thừa số đã chọn với **số mũ LỚN NHẤT**.<br>• **Tìm BC từ BCNN:** Tập hợp `BC(a, b)` chính là tập hợp các **bội của `BCNN(a, b)`** *(nhân BCNN với 0, 1, 2, 3...)*. |
| **🔵 NHÁNH 2: QUY ĐỒNG MẪU SỐ & BÀI TOÁN THỰC TẾ** |
| • **Quy đồng mẫu nhiều phân số:** Chọn mẫu chung là **BCNN** của các mẫu riêng ➔ Tìm thừa số phụ (Lấy mẫu chung chia mẫu riêng) ➔ Nhân cả tử và mẫu với thừa số phụ.<br>• **Dấu hiệu bài toán thực tế dùng BCNN:** Đề bài có từ khóa *"xếp hàng/chia nhóm vừa đủ"*, *"cùng lặp lại công việc sau một khoảng thời gian"*, và yêu cầu tìm số lượng trong một khoảng cho trước hoặc tìm giá trị **"ít nhất / nhỏ nhất"**. |

---
[⬅️ Quay lại Trang chủ Mục lục](README.md)
