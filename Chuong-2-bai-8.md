# 📘 CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN
# 🌟 BÀI 8: QUAN HỆ CHIA HẾT VÀ TÍNH CHẤT
* **Môn học:** Toán học 6 (Tập 1) — *Bộ sách Kết nối tri thức với cuộc sống*
* **Thời lượng tự học:** 45 – 60 phút
* **Hình thức:** Học liệu số tương tác (Lý thuyết trực quan + Trò chơi vận dụng)

---

> [!NOTE]
> ### 🎯 MỤC TIÊU CẦN ĐẠT SAU BÀI HỌC
> 1. **Nhận biết** được quan hệ chia hết, khái niệm **ước** và **bội** trong tập hợp các số tự nhiên.
> 2. **Sử dụng chuẩn xác** các kí hiệu toán học: chia hết (**⋮**), không chia hết (**∤**), thuộc (**∈**), không thuộc (**∉**).
> 3. **Thiết lập được quy trình** tìm tập hợp các ước **Ư(a)** và tập hợp các bội **B(b)** của một số tự nhiên.
> 4. **Vận dụng linh hoạt** hai tính chất chia hết của một tổng (hoặc một hiệu) để xét tính chia hết mà không cần tính giá trị biểu thức, đồng thời giải quyết các bài toán thực tiễn.

---

## 🚀 KHỞI ĐỘNG: BÀI TOÁN THỰC TIỄN
**Tình huống:** Nhân dịp sinh nhật, mẹ chuẩn bị cho Việt **12 gói kẹo** để liên hoan cùng các bạn, mỗi gói có **35 cái kẹo**. Việt dự định chia đều tổng số kẹo đó cho **5 bạn** trong nhóm học tập.

❓ **Câu hỏi tư duy:** *Không cần đặt phép tính nhân `12 . 35` rồi chia cho `5`, làm thế nào để khẳng định ngay lập tức rằng Việt hoàn toàn có thể chia đều số kẹo đó mà không bị lẻ cái nào? Và nếu Việt cất bớt đi 2 gói kẹo, số kẹo còn lại có chia đều được cho 5 bạn nữa không?*

➔ Hãy cùng khám phá cơ sở toán học đằng sau tình huống này qua 2 nội dung trọng tâm dưới đây!

---

## 📖 NỘI DUNG 1: QUAN HỆ CHIA HẾT VÀ KHÁI NIỆM ƯỚC – BỘI

### 1.1. Khi nào số tự nhiên *a* chia hết cho số tự nhiên *b*?
🔍 **Hoạt động khám phá 1:** Thực hiện hai phép chia sau và quan sát số dư:
* **Phép chia 1:** `15 : 3` ➔ Thương là **5**, số dư bằng **0** *(vì 15 = 3 . 5)*.
* **Phép chia 2:** `16 : 3` ➔ Thương là **5**, số dư bằng **1** *(vì 16 = 3 . 5 + 1)*.

> [!IMPORTANT]
> ### 📌 ĐỊNH NGHĨA QUAN HỆ CHIA HẾT
> Cho hai số tự nhiên *a* và *b* (với điều kiện ***b* ≠ 0**):
> * 🟢 Nếu có số tự nhiên *k* sao cho **a = b . k** thì ta nói ***a* chia hết cho *b*** và kí hiệu là: **`a ⋮ b`**
> * 🔴 Nếu *a* không chia hết cho *b* (phép chia có số dư *r* với *0 < r < b*), ta kí hiệu là: **`a ∤ b`**

---

### 1.2. Khái niệm Ước và Bội
Khi có quan hệ chia hết **`a ⋮ b`**, hai số *a* và *b* được định danh như sau:

* 🔵 Số ***a*** (số bị chia) được gọi là **BỘI** của *b*. Tập hợp các bội của *b* kí hiệu là **`B(b)`**.
* 🟠 Số ***b*** (số chia) được gọi là **ƯỚC** của *a*. Tập hợp các ước của *a* kí hiệu là **`Ư(a)`**.

**Ví dụ minh họa 1:** 
Xét phép tính `24 = 8 . 3`. Ta thấy **24 ⋮ 8**, do đó:
* **24** là **bội** của 8 *(viết dưới dạng kí hiệu tập hợp: **24 ∈ B(8)**)*.
* **8** là **ước** của 24 *(viết dưới dạng kí hiệu tập hợp: **8 ∈ Ư(24)**)*.
* Tương tự, vì `24 ⋮ 3` nên **3** cũng là một **ước** của 24 và **24** cũng là một **bội** của 3.

> [!WARNING]
> ### ⚡ CÁC TRƯỜNG HỢP ĐẶC BIỆT CỦA SỐ 0 VÀ SỐ 1
> * **Số 0:** Là **bội** của mọi số tự nhiên khác 0 *(vì `0 ⋮ b` với mọi `b ≠ 0`)*. Tuy nhiên, số 0 **không phải là ước** của bất kì số tự nhiên nào *(vì không có phép chia cho 0)*.
> * **Số 1:** Chỉ có duy nhất một ước là chính nó (`Ư(1) = {1}`), nhưng số 1 lại là **ước của mọi số tự nhiên** *(vì `a ⋮ 1` với mọi số tự nhiên `a`)*.
> * **Mọi số tự nhiên *a* (*a* ≠ 0)** luôn là ước của chính nó và là bội của chính nó.

---

### 1.3. Quy trình tìm Ước và Bội của một số tự nhiên
Làm thế nào để liệt kê đầy đủ các ước và bội mà không bị sót nghiệm? Hãy đối chiếu qua bảng quy tắc chuẩn dưới đây:

| Tiêu chí so sánh | 🟠 QUY TẮC TÌM ƯỚC CỦA SỐ *a* (*a* > 1) | 🔵 QUY TẮC TÌM BỘI CỦA SỐ *b* (*b* ≠ 0) |
| :--- | :--- | :--- |
| **Phương pháp thực hiện** | Lần lượt **chia *a*** cho các số tự nhiên từ `1` đến `*a*`. Phép chia nào chia hết thì số chia đó là **ước** của *a*. | Lần lượt **nhân *b*** với các số tự nhiên `0, 1, 2, 3, 4, ...` Các kết quả thu được đều là **bội** của *b*. |
| **Số lượng phần tử** | **Hữu hạn** phần tử. Luôn bắt đầu bằng `1` và kết thúc bằng chính số `*a*`. | **Vô số** phần tử. Luôn bắt đầu bằng số `0` và phải có dấu ba chấm `...` ở cuối tập hợp. |
| **Ví dụ thực hành** | **Tìm tập hợp Ư(18):**<br>Chia 18 lần lượt cho 1, 2, ..., 18.<br>➔ **`Ư(18) = {1; 2; 3; 6; 9; 18}`** | **Tìm tập hợp B(6):**<br>Nhân 6 lần lượt với 0, 1, 2, 3, 4, ...<br>➔ **`B(6) = {0; 6; 12; 18; 24; ...}`** |

> [!TIP]
> ### 💡 MẸO TƯ DUY NHANH: PHƯƠNG PHÁP "CẶP THỪA SỐ ĐỐI XỨNG" KHI TÌM ƯỚC
> Khi tìm ước của một số lớn (ví dụ tìm `Ư(36)`), thay vì thực hiện 36 phép chia từ 1 đến 36, ta chỉ cần tìm các cặp số nhân với nhau bằng 36 từ ngoài vào trong:
> * `1 . 36 = 36` ➔ Có cặp ước: **1** và **36**
> * `2 . 18 = 36` ➔ Có cặp ước: **2** và **18**
> * `3 . 12 = 36` ➔ Có cặp ước: **3** và **12**
> * `4 . 9 = 36` ➔ Có cặp ước: **4** và **9**
> * `6 . 6 = 36` ➔ Hai thừa số chạm nhau tại số **6** (dừng lại!).
> 
> ➔ Sắp xếp theo thứ tự tăng dần, ta thu được ngay: **`Ư(36) = {1; 2; 3; 4; 6; 9; 12; 18; 36}`**.

#### 📝 Trạm dừng thực hành số 1
Hãy tự nháp ra giấy câu trả lời trước khi nhấn vào thanh bên dưới để kiểm tra:
1. Tìm tập hợp **Ư(20)**.
2. Tìm tập hợp *A* gồm các số tự nhiên *x* sao cho **x ∈ B(8)** và **x < 40**.

<details>
<summary>👉 <b>NHẤN VÀO ĐÂY ĐỂ XEM ĐÁP ÁN & LỜI GIẢI CHI TIẾT</b></summary>
<br>

* **Câu 1:** Ta tách cặp nhân: `20 = 1 . 20 = 2 . 10 = 4 . 5`.
  ➔ Tập hợp các ước của 20 là: **`Ư(20) = {1; 2; 4; 5; 10; 20}`**. 🟢
* **Câu 2:** Nhân 8 lần lượt với 0, 1, 2, 3, 4 ta được: `0, 8, 16, 24, 32`. Nếu nhân tiếp với 5 thì `8 . 5 = 40` (không thỏa mãn điều kiện *x < 40*).
  ➔ Vậy tập hợp cần tìm là: **`A = {0; 8; 16; 24; 32}`**. 🟢

</details>

---

## 📖 NỘI DUNG 2: TÍNH CHẤT CHIA HẾT CỦA MỘT TỔNG (VÀ HIỆU)

Làm sao để biết một tổng lớn như `120 + 360 + 45` có chia hết cho 15 hay không mà không cần đặt tính cộng? Hai tính chất dưới đây là công cụ giúp ta giải quyết bài toán này trong 3 giây.

### 2.1. Tính chất 1: Trường hợp CHIA HẾT
🔍 **Hoạt động khám phá 2:** Lấy hai số đều chia hết cho 5 là `15` và `25`. Xét tổng của chúng: `15 + 25 = 40`. Ta thấy `40 ⋮ 5`.

> [!IMPORTANT]
> ### 🌟 TÍNH CHẤT 1 (CÙNG CHIA HẾT ➔ TỔNG CHIA HẾT)
> Nếu **tất cả các số hạng** của một tổng đều chia hết cho cùng một số thì **tổng đó chia hết** cho số đó.
> * **Công thức tổng quát:** Với *a, b, m ∈ ℕ* và *m ≠ 0*:
>   Nếu **`a ⋮ m`** và **`b ⋮ m`** thì **`(a + b) ⋮ m`**

📌 **Mở rộng Tính chất 1:**
* **Đối với phép trừ** *(điều kiện a ≥ b)*: Nếu **`a ⋮ m`** và **`b ⋮ m`** thì **`(a - b) ⋮ m`**.
* **Đối với nhiều số hạng:** Nếu **`a ⋮ m`**, **`b ⋮ m`** và **`c ⋮ m`** thì **`(a + b + c) ⋮ m`**.

**Ví dụ minh họa 2:** Không thực hiện phép tính, xét xem biểu thức `A = 48 + 12 - 36` có chia hết cho 6 không?
* **Phân tích:** Ta thấy `48 ⋮ 6` *(vì 48 = 6 . 8)*, `12 ⋮ 6` *(vì 12 = 6 . 2)* và `36 ⋮ 6` *(vì 36 = 6 . 6)*.
* **Kết luận:** Vì tất cả các thành phần trong biểu thức đều chia hết cho 6, nên theo Tính chất 1 mở rộng, **`(48 + 12 - 36) ⋮ 6`**.

---

### 2.2. Tính chất 2: Trường hợp KHÔNG CHIA HẾT
🔍 **Hoạt động khám phá 3:** Lấy một số chia hết cho 5 là `20` và một số không chia hết cho 5 là `12`. Xét tổng của chúng: `20 + 12 = 32`. Ta thấy `32 ∤ 5`.

> [!IMPORTANT]
> ### ⚠️ TÍNH CHẤT 2 (MỘT SỐ LẺ LOI KHÔNG CHIA HẾT ➔ TỔNG KHÔNG CHIA HẾT)
> Nếu **chỉ có duy nhất một số hạng** của tổng không chia hết cho một số, còn **tất cả các số hạng khác đều chia hết** cho số đó thì **tổng đó KHÔNG chia hết** cho số đó.
> * **Công thức tổng quát:** Với *a, b, m ∈ ℕ* và *m ≠ 0*:
>   Nếu **`a ⋮ m`** và **`b ∤ m`** thì **`(a + b) ∤ m`**

📌 **Mở rộng Tính chất 2:**
* **Đối với phép trừ** *(điều kiện a > b)*: Nếu **`a ⋮ m`** và **`b ∤ m`** thì **`(a - b) ∤ m`** *(hoặc ngược lại nếu `a ∤ m` và `b ⋮ m` thì `(a - b) ∤ m`)*.
* **Đối với nhiều số hạng:** Nếu **`a ⋮ m`**, **`b ⋮ m`** nhưng **`c ∤ m`** thì **`(a + b + c) ∤ m`**.

> [!CAUTION]
> ### 🚨 CẢNH BÁO "BẪY" TOÁN HỌC THƯỜNG GẶP NHẤT!
> Tính chất 2 chỉ đúng khi có **DUY NHẤT MỘT** số hạng không chia hết. 
> Nếu trong một tổng có **từ HAI số hạng trở lên không chia hết** cho *m*, ta **TUYỆT ĐỐI KHÔNG ĐƯỢC** kết luận ngay là tổng đó không chia hết cho *m*! Khi đó, các số dư của chúng có thể bù trừ cho nhau để tạo thành một số chia hết.
> 
> * **Ví dụ chứng minh:** Xét tổng `S = 16 + 13 + 7` với số chia là `4`.
>   * Ta có: `16 ⋮ 4`, nhưng `13 ∤ 4` (dư 1) và `7 ∤ 4` (dư 3) ➔ Có tới **2 số hạng** không chia hết cho 4.
>   * Nếu vội vàng kết luận `S ∤ 4` là **SAI**!
>   * **Cách làm đúng:** Nhóm hai số không chia hết lại với nhau: `S = 16 + (13 + 7) = 16 + 20`. Vì `16 ⋮ 4` và `20 ⋮ 4` nên tổng **`(16 + 13 + 7) ⋮ 4`**!

#### 📝 Trạm dừng thực hành số 2 (Giải quyết bài toán Khởi động)
Quay lại câu hỏi của bạn Việt ở đầu bài: Mẹ cho **12 gói kẹo**, mỗi gói **35 cái**. Việt lấy ra **2 gói kẹo** cất đi. Hỏi số kẹo còn lại có chia đều được cho **5 bạn** không?

<details>
<summary>👉 <b>NHẤN VÀO ĐÂY ĐỂ XEM LỜI GIẢI KHOA HỌC</b></summary>
<br>

* **Bước 1:** Tổng số kẹo ban đầu là `12 . 35`. Vì thừa số `35 ⋮ 5` nên tích `(12 . 35) ⋮ 5`.
* **Bước 2:** Số kẹo Việt lấy ra cất đi là `2 . 35`. Vì `35 ⋮ 5` nên tích `(2 . 35) ⋮ 5`.
* **Bước 3:** Số kẹo còn lại là hiệu: **`(12 . 35) - (2 . 35)`**. Vì cả số bị trừ và số trừ đều chia hết cho 5, nên theo Tính chất 1 mở rộng, hiệu này **chia hết cho 5**.
* **Kết luận:** Số kẹo còn lại **hoàn toàn chia đều được cho 5 bạn** mà không cần tính tổng số kẹo! 🟢

</details>

---

## 🎮 ĐẤU TRƯỜNG TRÍ TUỆ: THỬ THÁCH NHÀ TOÁN HỌC TRẺ
*(Phần ôn tập tương tác — Học sinh tự làm và click trực tiếp vào phương án mình chọn để mở khóa kết quả!)*

---

### 🏆 VÒNG 1: KHỞI ĐỘNG NHANH (10 Điểm / Câu)

**Câu 1:** Khẳng định nào dưới đây sử dụng **SAI** kí hiệu toán học?
<details>
<summary>🔘 <b>Phương án A: 42 ⋮ 6</b></summary>
❌ <b>Chưa đúng!</b> Vì 42 = 6 . 7 nên 42 ⋮ 6 là một khẳng định <b>ĐÚNG</b>. Hãy tìm câu sai nhé!
</details>
<details>
<summary>🔘 <b>Phương án B: 5 ∈ Ư(25)</b></summary>
❌ <b>Chưa đúng!</b> Vì 25 chia hết cho 5 nên 5 là một phần tử thuộc tập hợp ước của 25. Khẳng định này <b>ĐÚNG</b>.
</details>
<details>
<summary>🔘 <b>Phương án C: 0 ∈ Ư(15)</b></summary>
🎉 <b>CHÍNH XÁC! (+10 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Khẳng định này <b>SAI</b> vì không có phép chia cho số 0, do đó số 0 không bao giờ là ước của bất kì số tự nhiên nào! (Số 0 chỉ là bội của 15: `0 ∈ B(15)`).
</details>

<br>

**Câu 2:** Tập hợp tất cả các số tự nhiên *y* thỏa mãn **`y ∈ Ư(50)`** và **`y > 5`** là:
<details>
<summary>🔘 <b>Phương án A: {5; 10; 25; 50}</b></summary>
❌ <b>Bị lừa rồi!</b> Đề bài yêu cầu <i>y > 5</i> (lớn hơn hẳn 5) nên không được lấy số 5 vào tập hợp nhé!
</details>
<details>
<summary>🔘 <b>Phương án B: {10; 25; 50}</b></summary>
🎉 <b>XUẤT SẮC! (+10 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Ta có Ư(50) = {1; 2; 5; 10; 25; 50}. Lọc các phần tử lớn hơn 5, ta thu được tập hợp chuẩn xác là <b>{10; 25; 50}</b>.
</details>
<details>
<summary>🔘 <b>Phương án C: {10; 20; 25; 50}</b></summary>
❌ <b>Sai rồi!</b> Số 20 không phải là ước của 50 vì 50 chia 20 được 2 dư 10 (50 ∤ 20).
</details>

---

### 🔥 VÒNG 2: TĂNG TỐC SUY LUẬN (20 Điểm / Câu)

**Câu 3:** Không thực hiện phép tính, hãy cho biết trong các tổng/hiệu sau, biểu thức nào **CHIA HẾT CHO 8**?
* `Biểu thức M = 80 + 16 + 28`
* `Biểu thức N = 100 - 40`
* `Biểu thức P = 64 + 32 + 19 + 5`

<details>
<summary>🔘 <b>Phương án A: Chỉ có biểu thức M</b></summary>
❌ <b>Sai rồi!</b> Trong biểu thức M có 80 ⋮ 8, 16 ⋮ 8 nhưng 28 ∤ 8 (dư 4). Theo Tính chất 2, M không chia hết cho 8.
</details>
<details>
<summary>🔘 <b>Phương án B: Chỉ có biểu thức N</b></summary>
❌ <b>Chưa chính xác!</b> Trong biểu thức N có 40 ⋮ 8 nhưng 100 ∤ 8 (100 = 8 . 12 + 4). Vậy (100 - 40) ∤ 8.
</details>
<details>
<summary>🔘 <b>Phương án C: Chỉ có biểu thức P</b></summary>
🎉 <b>ĐỈNH CAO TƯ DUY! (+20 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Bạn đã không bị mắc bẫy! Trong biểu thức P = 64 + 32 + 19 + 5, mặc dù 19 ∤ 8 và 5 ∤ 8, nhưng khi nhóm hai số này lại ta có <b>(19 + 5) = 24</b> mà <b>24 ⋮ 8</b>. Vì 64 ⋮ 8, 32 ⋮ 8 và 24 ⋮ 8 nên tổng <b>P chia hết cho 8</b>!
</details>

<br>

**Câu 4:** Cho tổng **`S = 35 + x`**. Tìm điều kiện của số tự nhiên *x* thuộc tập hợp `{7; 14; 18; 21}` để **`S ∤ 7`** *(S không chia hết cho 7)*:
<details>
<summary>🔘 <b>Phương án A: x ∈ {7; 14; 21}</b></summary>
❌ <b>Đọc kĩ đề nhé!</b> Đề bài yêu cầu tìm <i>x</i> để tổng S <b>KHÔNG chia hết</b> cho 7 (S ∤ 7). Với x ∈ {7; 14; 21} thì tổng S sẽ chia hết cho 7 mất rồi!
</details>
<details>
<summary>🔘 <b>Phương án B: x = 18</b></summary>
🎉 <b>CHÍNH XÁC TUYỆT ĐỐI! (+20 Điểm)</b> 🟢<br>
<b>Giải thích khoa học:</b> Ta có 35 ⋮ 7. Theo Tính chất 2, để tổng (35 + x) ∤ 7 thì số hạng <i>x</i> phải không chia hết cho 7 (x ∤ 7). Trong tập hợp đã cho, chỉ có duy nhất <b>18 ∤ 7</b>. Vậy <b>x = 18</b>.
</details>

---

### 👑 VÒNG 3: CHINH PHỤC TỰ LUẬN & TOÁN THỰC TẾ (40 Điểm)
*(Hoàn thành 3 bài tập chuẩn SGK trang 33 vào vở, sau đó mở khóa đáp án để tự chấm điểm)*

* **Bài tập 1 (Nhận diện tính chất trong biểu thức chứa tích):**
  Xét xem các khẳng định sau là Đúng hay Sai và giải thích rõ lí do:
  * a) `(219 . 7 + 8)` chia hết cho 7.
  * b) `(8 . 12 + 9)` chia hết cho 3.

* **Bài tập 2 (Bài toán chia nhóm dự án - SGK Toán 6):**
  Một lớp học có **40 học sinh**. Giáo viên muốn chia lớp thành các nhóm có số người như nhau để thực hiện dự án học tập. Biết rằng mỗi nhóm phải có **nhiều hơn 3 người** và **ít hơn 15 người**. Hỏi có thể chia lớp thành mấy nhóm và mỗi nhóm có bao nhiêu học sinh?

* **Bài tập 3 (Thử thách nâng cao dành cho học sinh giỏi):**
  Tìm tất cả các số tự nhiên *n* sao cho **`(n + 8) ⋮ (n + 3)`**.

<details>
<summary>🔓 <b>MỞ KHÓA HƯỚNG DẪN GIẢI VÀ THANG ĐIỂM TỰ CHẤM (VÒNG 3)</b></summary>
<br>

#### ✅ Lời giải Bài tập 1 (10 Điểm):
* **a) Khẳng định SAI.** 
  * *Lí giải:* Vì `7 ⋮ 7` nên tích `(219 . 7) ⋮ 7`. Tuy nhiên, số hạng thứ hai là `8 ∤ 7`. Theo Tính chất 2, tổng **`(219 . 7 + 8) ∤ 7`**.
* **b) Khẳng định ĐÚNG.**
  * *Lí giải:* Trong tích `(8 . 12)` có thừa số `12 ⋮ 3` nên tích `(8 . 12) ⋮ 3`. Mặt khác, số hạng thứ hai là `9 ⋮ 3`. Theo Tính chất 1, tổng **`(8 . 12 + 9) ⋮ 3`**.

---

#### ✅ Lời giải Bài tập 2 (15 Điểm):
* Gọi số học sinh trong mỗi nhóm là *x* (điều kiện: *x ∈ ℕ\** và **3 < *x* < 15**).
* Vì 40 học sinh được chia đều vào các nhóm không dư bạn nào nên `40 ⋮ x`, suy ra **`x ∈ Ư(40)`**.
* Ta tìm tập hợp các ước của 40 bằng phương pháp cặp nhân:
  **`Ư(40) = {1; 2; 4; 5; 8; 10; 20; 40}`**.
* Kết hợp với điều kiện **3 < *x* < 15**, ta chọn được các giá trị thỏa mãn là: **`x ∈ {4; 5; 8; 10}`**.
* **Bảng kết luận các phương án chia nhóm:**

| Phương án | Số học sinh mỗi nhóm (*x*) | Số nhóm tương ứng (40 : *x*) |
| :---: | :---: | :---: |
| **Cách 1** | **4** học sinh | `40 : 4` = **10 nhóm** |
| **Cách 2** | **5** học sinh | `40 : 5` = **8 nhóm** |
| **Cách 3** | **8** học sinh | `40 : 8` = **5 nhóm** |
| **Cách 4** | **10** học sinh | `40 : 10` = **4 nhóm** |

---

#### ✅ Lời giải Bài tập 3 - Nâng cao (15 Điểm):
* **Phương pháp tách số:** Ta biến đổi biểu thức bị chia `(n + 8)` sao cho xuất hiện biểu thức chia `(n + 3)`:
  Ta có: **`n + 8 = (n + 3) + 5`**.
* Vì bản thân số hạng **`(n + 3) ⋮ (n + 3)`** với mọi số tự nhiên *n*, nên theo Tính chất 1 và 2, để tổng `[(n + 3) + 5] ⋮ (n + 3)` thì số hạng còn lại là **5 phải chia hết cho `(n + 3)`**, tức là:
  **`5 ⋮ (n + 3)`** hay **`(n + 3) ∈ Ư(5)`**.
* Mà **`Ư(5) = {1; 5}`**. Vì *n* là số tự nhiên (*n ≥ 0*) nên `n + 3 ≥ 3`.
* Đối chiếu với tập hợp `Ư(5)`, chỉ có giá trị **`n + 3 = 5`** thỏa mãn (loại trường hợp `n + 3 = 1`).
* Từ `n + 3 = 5`, suy ra `n = 5 - 3 = 2`.
* **Kết luận:** Vậy **`n = 2`** *(Thử lại: với n = 2 thì n + 8 = 10, n + 3 = 5, ta có 10 ⋮ 5 — hoàn toàn chính xác!)*.

</details>

---

## 🗺️ SƠ ĐỒ TỔNG KẾT KIẾN THỨC CỐT LÕI (DÀNH CHO ÔN THI)

| <div align="center">🎯 <b>TRỌNG TÂM: QUAN HỆ CHIA HẾT</b><br><code>a = b . k</code> <i>(với a, b ∈ ℕ; b ≠ 0)</i> ➔ <b><code>a ⋮ b</code></b></div> |
| :--- |
| **🟠 NHÁNH 1: KHÁI NIỆM ƯỚC & BỘI** |
| • **a là BỘI của b** — Kí hiệu: **`B(b)`**<br>  ➔ *Cách tìm:* Nhân *b* lần lượt với `0, 1, 2, 3, ...` (Tập hợp vô hạn).<br><br>• **b là ƯỚC của a** — Kí hiệu: **`Ư(a)`**<br>  ➔ *Cách tìm:* Chia *a* lần lượt cho `1, 2, ..., a` (Tập hợp hữu hạn).<br>  *(Mẹo: Dùng phương pháp ghép cặp nhân đối xứng từ ngoài vào trong để không bao giờ bị sót nghiệm).* |
| **🔵 NHÁNH 2: TÍNH CHẤT CHIA HẾT CỦA TỔNG VÀ HIỆU** |
| • **Tính chất 1 (Trường hợp cùng chia hết):**<br>  Nếu **`a ⋮ m`** và **`b ⋮ m`** thì:<br>  ➔ **`(a + b) ⋮ m`** và **`(a - b) ⋮ m`** *(với điều kiện a ≥ b)*.<br><br>• **Tính chất 2 (Trường hợp chỉ có một số không chia hết):**<br>  Nếu **`a ⋮ m`** và **`b ∤ m`** thì:<br>  ➔ **`(a + b) ∤ m`** và **`(a - b) ∤ m`** *(với điều kiện a > b)*.<br>  *(⚠️ Cảnh báo: Nếu có từ 2 số hạng trở lên không chia hết, tuyệt đối không dùng tính chất 2).* |
