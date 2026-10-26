<style>
  /* Ẩn tiêu đề mặc định Bai-giang-toan-6 của GitHub Pages và mở rộng khung nhìn */
  .markdown-body > h1:first-child { display: none !important; }
  .container-lg, .markdown-body { max-width: 980px !important; margin: 0 auto !important; padding: 16px !important; font-family: 'Segoe UI', system-ui, -apple-system, sans-serif !important; color: #0f172a !important; background-color: #f0f9ff !important; }
  body { background-color: #f0f9ff !important; }

  /* Thanh điều khiển cố định */
  .sky-topbar { position: sticky; top: 10px; z-index: 999; background: #ffffff; border: 2px solid #0284c7; border-radius: 12px; padding: 12px 20px; margin-bottom: 24px; display: flex; justify-content: space-between; align-items: center; box-shadow: 0 8px 20px rgba(2, 132, 199, 0.15); flex-wrap: wrap; gap: 10px; }
  .sky-topbar-title { font-weight: 800; color: #0c4a6e; font-size: 1rem; letter-spacing: 0.3px; }
  .sky-topbar-actions { display: flex; align-items: center; gap: 12px; }
  .sky-score { background: #e0f2fe; color: #0369a1; border: 1.5px solid #0284c7; padding: 6px 16px; border-radius: 99px; font-weight: 800; font-size: 0.95rem; }
  .sky-sound-btn { background: #0284c7; color: #ffffff; border: none; padding: 8px 16px; border-radius: 8px; font-weight: 700; cursor: pointer; font-size: 0.9rem; transition: 0.2s; }
  .sky-sound-btn:hover { background: #0369a1; }

  /* Khung Banner mở đầu */
  .sky-hero { background: linear-gradient(135deg, #0284c7 0%, #0369a1 100%); color: #ffffff; border-radius: 16px; padding: 32px 24px; text-align: center; margin-bottom: 28px; box-shadow: 0 10px 25px rgba(2, 132, 199, 0.2); border: 2px solid #38bdf8; }
  .sky-hero-tag { display: inline-block; background: #e0f2fe; color: #0c4a6e; font-weight: 800; font-size: 0.85rem; padding: 6px 18px; border-radius: 99px; text-transform: uppercase; letter-spacing: 0.8px; margin-bottom: 14px; }
  .sky-hero-title { color: #ffffff !important; font-size: 2rem !important; font-weight: 800 !important; margin: 0 0 18px 0 !important; border: none !important; padding: 0 !important; line-height: 1.3 !important; }
  .sky-meta-list { display: flex; justify-content: center; flex-wrap: wrap; gap: 12px; }
  .sky-meta-chip { background: rgba(255, 255, 255, 0.15); border: 1px solid rgba(255, 255, 255, 0.4); color: #ffffff; padding: 6px 16px; border-radius: 8px; font-size: 0.92rem; font-weight: 600; backdrop-filter: blur(4px); }

  /* Khung từng phần bài giảng (Section Card) */
  .sky-card { background: #ffffff; border: 2px solid #7dd3fc; border-radius: 16px; margin-bottom: 28px; overflow: hidden; box-shadow: 0 6px 18px rgba(2, 132, 199, 0.08); }
  .sky-card-header { background: linear-gradient(90deg, #e0f2fe 0%, #bae6fd 100%); border-bottom: 2px solid #7dd3fc; padding: 16px 24px; color: #0c4a6e; font-size: 1.25rem; font-weight: 800; text-transform: uppercase; letter-spacing: 0.4px; }
  .sky-card-body { padding: 24px; line-height: 1.75; font-size: 1.02rem; }

  /* Khung con (Sub-box) */
  .sky-subbox { background: #f8fafc; border: 1.5px solid #bae6fd; border-radius: 12px; padding: 20px; margin-bottom: 22px; }
  .sky-subbox:last-child { margin-bottom: 0; }
  .sky-sub-heading { color: #0284c7; font-size: 1.15rem; font-weight: 800; margin-bottom: 12px; padding-bottom: 8px; border-bottom: 2px solid #e0f2fe; }

  /* Khung Ghi nhớ, Định nghĩa, Cảnh báo (Thay thế hoàn toàn chữ xám xấu xí) */
  .sky-alert { background: #e0f2fe; border-left: 6px solid #0284c7; border-radius: 10px; padding: 16px 20px; margin: 16px 0; color: #0c4a6e; }
  .sky-alert-title { font-weight: 800; font-size: 1rem; margin-bottom: 8px; text-transform: uppercase; color: #0369a1; }
  .sky-alert-warn { background: #fef9c3; border-left: 6px solid #eab308; color: #713f12; }
  .sky-alert-warn .sky-alert-title { color: #a16207; }
  .sky-alert-danger { background: #ffe4e6; border-left: 6px solid #e11d48; color: #881337; }
  .sky-alert-danger .sky-alert-title { color: #be123c; }

  /* Kí hiệu toán học nổi bật */
  .m-tag { background: #e0f2fe; color: #0369a1; border: 1px solid #7dd3fc; padding: 2px 8px; border-radius: 6px; font-family: 'Consolas', monospace; font-weight: 700; font-size: 0.96em; display: inline-block; }

  /* Bảng chuẩn đẹp */
  .sky-table { width: 100%; border-collapse: collapse; margin: 16px 0; border-radius: 10px; overflow: hidden; border: 1.5px solid #7dd3fc; }
  .sky-table th { background: #0284c7 !important; color: #ffffff !important; padding: 12px 16px !important; text-align: left; font-weight: 700; border: 1px solid #0369a1 !important; }
  .sky-table td { padding: 12px 16px !important; border: 1px solid #bae6fd !important; background: #ffffff !important; color: #0f172a !important; vertical-align: top; }
  .sky-table tr:nth-child(even) td { background: #f0f9ff !important; }

  /* Nút mở lời giải */
  details.sky-details { background: #ffffff; border: 2px solid #0284c7; border-radius: 10px; margin-top: 14px; overflow: hidden; }
  details.sky-details summary { background: #e0f2fe; color: #0c4a6e; padding: 12px 18px; font-weight: 800; cursor: pointer; list-style: none; user-select: none; transition: 0.2s; }
  details.sky-details summary:hover { background: #bae6fd; }
  .sky-details-body { padding: 18px; border-top: 1.5px solid #bae6fd; background: #ffffff; }

  /* Trò chơi Nối cặp (Matching Game) */
  .match-container { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-top: 16px; }
  .match-col-head { background: #0284c7; color: #ffffff; text-align: center; padding: 10px; border-radius: 8px; font-weight: 800; margin-bottom: 12px; }
  .match-box { background: #f0f9ff; border: 2px solid #7dd3fc; border-radius: 10px; padding: 14px 16px; margin-bottom: 12px; font-weight: 700; color: #0c4a6e; cursor: pointer; transition: 0.2s; display: flex; justify-content: space-between; align-items: center; user-select: none; }
  .match-box:hover:not(.matched) { background: #e0f2fe; border-color: #0284c7; transform: translateY(-2px); }
  .match-box.selected { background: #0284c7; color: #ffffff; border-color: #0c4a6e; box-shadow: 0 0 0 4px rgba(2, 132, 199, 0.25); }
  .match-box.matched { background: #dcfce7; border-color: #16a34a; color: #166534; cursor: default; }
  .match-box.wrong { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .match-tag { font-size: 0.8rem; background: #16a34a; color: #fff; padding: 2px 8px; border-radius: 10px; display: none; }
  .match-box.matched .match-tag { display: inline-block; }

  /* Trò chơi Trắc nghiệm */
  .quiz-box { background: #f0f9ff; border: 1.5px solid #7dd3fc; border-radius: 12px; padding: 18px; margin-bottom: 18px; }
  .quiz-title { font-weight: 800; color: #0c4a6e; margin-bottom: 12px; font-size: 1.05rem; }
  .quiz-list { display: grid; gap: 10px; }
  .quiz-opt { text-align: left; background: #ffffff; border: 2px solid #bae6fd; padding: 12px 16px; border-radius: 8px; font-weight: 700; color: #0f172a; cursor: pointer; font-size: 0.96rem; transition: 0.2s; }
  .quiz-opt:hover:not(:disabled) { background: #e0f2fe; border-color: #0284c7; }
  .quiz-opt.ok { background: #dcfce7; border-color: #16a34a; color: #166534; }
  .quiz-opt.err { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .quiz-msg { display: none; margin-top: 12px; padding: 12px 16px; border-radius: 8px; font-weight: 600; font-size: 0.95rem; }
  .btn-replay { background: #0284c7; color: #ffffff; border: none; padding: 10px 20px; border-radius: 8px; font-weight: 700; cursor: pointer; margin-top: 10px; }
  .btn-replay:hover { background: #0369a1; }

  @media (max-width: 680px) {
    .match-container { grid-template-columns: 1fr; }
  }
</style>

<!-- THANH ĐIỀU KHIỂN CỐ ĐỊNH -->
<div class="sky-topbar">
  <div class="sky-topbar-title">TOÁN 6 — BÀI 8: QUAN HỆ CHIA HẾT VÀ TÍNH CHẤT</div>
  <div class="sky-topbar-actions">
    <div class="sky-score">ĐIỂM SỐ: <span id="scoreVal">0</span> / 100</div>
    <button class="sky-sound-btn" id="btnAudio" onclick="switchSound()">Âm thanh: ĐANG BẬT</button>
  </div>
</div>

<!-- KHUNG TIÊU ĐỀ BÀI GIẢNG -->
<div class="sky-hero">
  <div class="sky-hero-tag">CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN</div>
  <h1 class="sky-hero-title">BÀI 8: QUAN HỆ CHIA HẾT VÀ TÍNH CHẤT</h1>
  <div class="sky-meta-list">
    <div class="sky-meta-chip">Môn học: Toán 6 (Tập 1) — Kết nối tri thức với cuộc sống</div>
    <div class="sky-meta-chip">Thời lượng tự học: 45 – 60 phút</div>
    <div class="sky-meta-chip">Hình thức: Học liệu số tương tác</div>
  </div>
</div>

<!-- KHUNG 1: MỤC TIÊU CẦN ĐẠT -->
<div class="sky-card">
  <div class="sky-card-header">MỤC TIÊU CẦN ĐẠT SAU BÀI HỌC</div>
  <div class="sky-card-body">
    <ol>
      <li><b>Nhận biết</b> được quan hệ chia hết, khái niệm <b>ước</b> và <b>bội</b> trong tập hợp các số tự nhiên.</li>
      <li><b>Sử dụng chuẩn xác</b> các kí hiệu toán học: chia hết (<span class="m-tag">⋮</span>), không chia hết (<span class="m-tag">∤</span>), thuộc (<span class="m-tag">∈</span>), không thuộc (<span class="m-tag">∉</span>).</li>
      <li><b>Thiết lập được quy trình</b> tìm tập hợp các ước <span class="m-tag">Ư(a)</span> và tập hợp các bội <span class="m-tag">B(b)</span> của một số tự nhiên.</li>
      <li><b>Vận dụng linh hoạt</b> hai tính chất chia hết của một tổng (hoặc một hiệu) để xét tính chia hết mà không cần tính giá trị biểu thức, đồng thời giải quyết các bài toán thực tiễn.</li>
    </ol>
  </div>
</div>

<!-- KHUNG 2: KHỞI ĐỘNG -->
<div class="sky-card">
  <div class="sky-card-header">KHỞI ĐỘNG: BÀI TOÁN THỰC TIỄN</div>
  <div class="sky-card-body">
    <p><b>Tình huống:</b> Nhân dịp sinh nhật, mẹ chuẩn bị cho Việt <b>12 gói kẹo</b> để liên hoan cùng các bạn, mỗi gói có <b>35 cái kẹo</b>. Việt dự định chia đều tổng số kẹo đó cho <b>5 bạn</b> trong nhóm học tập.</p>
    <div class="sky-alert">
      <div class="sky-alert-title">CÂU HỎI TƯ DUY</div>
      Không cần đặt phép tính nhân <span class="m-tag">12 . 35</span> rồi chia cho <span class="m-tag">5</span>, làm thế nào để khẳng định ngay lập tức rằng Việt hoàn toàn có thể chia đều số kẹo đó mà không bị lẻ cái nào? Và nếu Việt cất bớt đi 2 gói kẹo, số kẹo còn lại có chia đều được cho 5 bạn nữa không?
    </div>
    <p>Hãy cùng khám phá cơ sở toán học đằng sau tình huống này qua 2 nội dung trọng tâm dưới đây.</p>
  </div>
</div>

<!-- KHUNG 3: NỘI DUNG 1 -->
<div class="sky-card">
  <div class="sky-card-header">NỘI DUNG 1: QUAN HỆ CHIA HẾT VÀ KHÁI NIỆM ƯỚC – BỘI</div>
  <div class="sky-card-body">

    <div class="sky-subbox">
      <div class="sky-sub-heading">1.1. Khi nào số tự nhiên a chia hết cho số tự nhiên b?</div>
      <p><b>Hoạt động khám phá 1:</b> Thực hiện hai phép chia sau và quan sát số dư:</p>
      <ul>
        <li><b>Phép chia 1:</b> <span class="m-tag">15 : 3</span> ➔ Thương là <b>5</b>, số dư bằng <b>0</b> <i>(vì 15 = 3 . 5)</i>.</li>
        <li><b>Phép chia 2:</b> <span class="m-tag">16 : 3</span> ➔ Thương là <b>5</b>, số dư bằng <b>1</b> <i>(vì 16 = 3 . 5 + 1)</i>.</li>
      </ul>
      <div class="sky-alert">
        <div class="sky-alert-title">ĐỊNH NGHĨA QUAN HỆ CHIA HẾT</div>
        Cho hai số tự nhiên <i>a</i> và <i>b</i> (với điều kiện <b><i>b</i> ≠ 0</b>):
        <ul>
          <li>Nếu có số tự nhiên <i>k</i> sao cho <span class="m-tag">a = b . k</span> thì ta nói <b><i>a</i> chia hết cho <i>b</i></b> và kí hiệu là: <span class="m-tag">a ⋮ b</span></li>
          <li>Nếu <i>a</i> không chia hết cho <i>b</i> (phép chia có số dư <i>r</i> với <i>0 &lt; r &lt; b</i>), ta kí hiệu là: <span class="m-tag">a ∤ b</span></li>
        </ul>
      </div>
    </div>

    <div class="sky-subbox">
      <div class="sky-sub-heading">1.2. Khái niệm Ước và Bội</div>
      <p>Khi có quan hệ chia hết <span class="m-tag">a ⋮ b</span>, hai số <i>a</i> và <i>b</i> được định danh như sau:</p>
      <ul>
        <li>Số <b><i>a</i></b> (số bị chia) được gọi là <b>BỘI</b> của <i>b</i>. Tập hợp các bội của <i>b</i> kí hiệu là <span class="m-tag">B(b)</span>.</li>
        <li>Số <b><i>b</i></b> (số chia) được gọi là <b>ƯỚC</b> của <i>a</i>. Tập hợp các ước của <i>a</i> kí hiệu là <span class="m-tag">Ư(a)</span>.</li>
      </ul>
      <p><b>Ví dụ minh họa 1:</b> Xét phép tính <span class="m-tag">24 = 8 . 3</span>. Ta thấy <b>24 ⋮ 8</b>, do đó:</p>
      <ul>
        <li><b>24</b> là <b>bội</b> của 8 <i>(viết dưới dạng kí hiệu tập hợp: <span class="m-tag">24 ∈ B(8)</span>)</i>.</li>
        <li><b>8</b> là <b>ước</b> của 24 <i>(viết dưới dạng kí hiệu tập hợp: <span class="m-tag">8 ∈ Ư(24)</span>)</i>.</li>
        <li>Tương tự, vì <span class="m-tag">24 ⋮ 3</span> nên <b>3</b> cũng là một <b>ước</b> của 24 và <b>24</b> cũng là một <b>bội</b> của 3.</li>
      </ul>
      <div class="sky-alert sky-alert-warn">
        <div class="sky-alert-title">CÁC TRƯỜNG HỢP ĐẶC BIỆT CỦA SỐ 0 VÀ SỐ 1</div>
        <ul>
          <li><b>Số 0:</b> Là <b>bội</b> của mọi số tự nhiên khác 0 <i>(vì <span class="m-tag">0 ⋮ b</span> với mọi <span class="m-tag">b ≠ 0</span>)</i>. Tuy nhiên, số 0 <b>không phải là ước</b> của bất kì số tự nhiên nào <i>(vì không có phép chia cho 0)</i>.</li>
          <li><b>Số 1:</b> Chỉ có duy nhất một ước là chính nó (<span class="m-tag">Ư(1) = {1}</span>), nhưng số 1 lại là <b>ước của mọi số tự nhiên</b> <i>(vì <span class="m-tag">a ⋮ 1</span> với mọi số tự nhiên <span class="m-tag">a</span>)</i>.</li>
          <li><b>Mọi số tự nhiên <i>a</i> (<i>a</i> ≠ 0)</b> luôn là ước của chính nó và là bội của chính nó.</li>
        </ul>
      </div>
    </div>

    <div class="sky-subbox">
      <div class="sky-sub-heading">1.3. Quy trình tìm Ước và Bội của một số tự nhiên</div>
      <p>Làm thế nào để liệt kê đầy đủ các ước và bội mà không bị sót nghiệm? Hãy đối chiếu qua bảng quy tắc chuẩn dưới đây:</p>
      <table class="sky-table">
        <thead>
          <tr>
            <th>Tiêu chí so sánh</th>
            <th>QUY TẮC TÌM ƯỚC CỦA SỐ a (a &gt; 1)</th>
            <th>QUY TẮC TÌM BỘI CỦA SỐ b (b ≠ 0)</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><b>Phương pháp thực hiện</b></td>
            <td>Lần lượt <b>chia <i>a</i></b> cho các số tự nhiên từ <span class="m-tag">1</span> đến <span class="m-tag">a</span>. Phép chia nào chia hết thì số chia đó là <b>ước</b> của <i>a</i>.</td>
            <td>Lần lượt <b>nhân <i>b</i></b> với các số tự nhiên <span class="m-tag">0, 1, 2, 3, 4, ...</span> Các kết quả thu được đều là <b>bội</b> của <i>b</i>.</td>
          </tr>
          <tr>
            <td><b>Số lượng phần tử</b></td>
            <td><b>Hữu hạn</b> phần tử. Luôn bắt đầu bằng <span class="m-tag">1</span> và kết thúc bằng chính số <span class="m-tag">a</span>.</td>
            <td><b>Vô số</b> phần tử. Luôn bắt đầu bằng số <span class="m-tag">0</span> và phải có dấu ba chấm <span class="m-tag">...</span> ở cuối tập hợp.</td>
          </tr>
          <tr>
            <td><b>Ví dụ thực hành</b></td>
            <td><b>Tìm tập hợp Ư(18):</b><br>Chia 18 lần lượt cho 1, 2, ..., 18.<br>➔ <span class="m-tag">Ư(18) = {1; 2; 3; 6; 9; 18}</span></td>
            <td><b>Tìm tập hợp B(6):</b><br>Nhân 6 lần lượt với 0, 1, 2, 3, 4, ...<br>➔ <span class="m-tag">B(6) = {0; 6; 12; 18; 24; ...}</span></td>
          </tr>
        </tbody>
      </table>

      <div class="sky-alert">
        <div class="sky-alert-title">MẸO TƯ DUY NHANH: PHƯƠNG PHÁP "CẶP THỪA SỐ ĐỐI XỨNG" KHI TÌM ƯỚC</div>
        Khi tìm ước của một số lớn (ví dụ tìm <span class="m-tag">Ư(36)</span>), thay vì thực hiện 36 phép chia từ 1 đến 36, ta chỉ cần tìm các cặp số nhân với nhau bằng 36 từ ngoài vào trong:
        <ul>
          <li><span class="m-tag">1 . 36 = 36</span> ➔ Có cặp ước: <b>1</b> và <b>36</b></li>
          <li><span class="m-tag">2 . 18 = 36</span> ➔ Có cặp ước: <b>2</b> và <b>18</b></li>
          <li><span class="m-tag">3 . 12 = 36</span> ➔ Có cặp ước: <b>3</b> và <b>12</b></li>
          <li><span class="m-tag">4 . 9 = 36</span> ➔ Có cặp ước: <b>4</b> và <b>9</b></li>
          <li><span class="m-tag">6 . 6 = 36</span> ➔ Hai thừa số chạm nhau tại số <b>6</b> (dừng lại!).</li>
        </ul>
        ➔ Sắp xếp theo thứ tự tăng dần, ta thu được ngay: <span class="m-tag">Ư(36) = {1; 2; 3; 4; 6; 9; 12; 18; 36}</span>.
      </div>

      <p><b>TRẠM DỪNG THỰC HÀNH SỐ 1:</b> Hãy tự nháp ra giấy câu trả lời trước khi nhấn vào thanh bên dưới để kiểm tra:</p>
      <ol>
        <li>Tìm tập hợp <span class="m-tag">Ư(20)</span>.</li>
        <li>Tìm tập hợp <i>A</i> gồm các số tự nhiên <i>x</i> sao cho <span class="m-tag">x ∈ B(8)</span> và <span class="m-tag">x &lt; 40</span>.</li>
      </ol>

      <details class="sky-details" onclick="sndClick()">
        <summary>[ NHẤN VÀO ĐÂY ĐỂ XEM ĐÁP ÁN & LỜI GIẢI CHI TIẾT ]</summary>
        <div class="sky-details-body">
          <ul>
            <li><b>Câu 1:</b> Ta tách cặp nhân: <span class="m-tag">20 = 1 . 20 = 2 . 10 = 4 . 5</span>.<br>➔ Tập hợp các ước của 20 là: <span class="m-tag">Ư(20) = {1; 2; 4; 5; 10; 20}</span>.</li>
            <li><b>Câu 2:</b> Nhân 8 lần lượt với 0, 1, 2, 3, 4 ta được: <span class="m-tag">0, 8, 16, 24, 32</span>. Nếu nhân tiếp với 5 thì <span class="m-tag">8 . 5 = 40</span> (không thỏa mãn điều kiện <i>x &lt; 40</i>).<br>➔ Vậy tập hợp cần tìm là: <span class="m-tag">A = {0; 8; 16; 24; 32}</span>.</li>
          </ul>
        </div>
      </details>
    </div>

  </div>
</div>

<!-- KHUNG 4: NỘI DUNG 2 -->
<div class="sky-card">
  <div class="sky-card-header">NỘI DUNG 2: TÍNH CHẤT CHIA HẾT CỦA MỘT TỔNG (VÀ HIỆU)</div>
  <div class="sky-card-body">
    <p>Làm sao để biết một tổng lớn như <span class="m-tag">120 + 360 + 45</span> có chia hết cho 15 hay không mà không cần đặt tính cộng? Hai tính chất dưới đây là công cụ giúp ta giải quyết bài toán này trong 3 giây.</p>

    <div class="sky-subbox">
      <div class="sky-sub-heading">2.1. Tính chất 1: Trường hợp CHIA HẾT</div>
      <p><b>Hoạt động khám phá 2:</b> Lấy hai số đều chia hết cho 5 là <span class="m-tag">15</span> và <span class="m-tag">25</span>. Xét tổng của chúng: <span class="m-tag">15 + 25 = 40</span>. Ta thấy <span class="m-tag">40 ⋮ 5</span>.</p>
      <div class="sky-alert">
        <div class="sky-alert-title">TÍNH CHẤT 1 (CÙNG CHIA HẾT ➔ TỔNG CHIA HẾT)</div>
        Nếu <b>tất cả các số hạng</b> của một tổng đều chia hết cho cùng một số thì <b>tổng đó chia hết</b> cho số đó.<br>
        • <b>Công thức tổng quát:</b> Với <i>a, b, m ∈ ℕ</i> và <i>m ≠ 0</i>: Nếu <span class="m-tag">a ⋮ m</span> và <span class="m-tag">b ⋮ m</span> thì <span class="m-tag">(a + b) ⋮ m</span>
      </div>
      <p><b>Mở rộng Tính chất 1:</b></p>
      <ul>
        <li><b>Đối với phép trừ</b> <i>(điều kiện a ≥ b)</i>: Nếu <span class="m-tag">a ⋮ m</span> và <span class="m-tag">b ⋮ m</span> thì <span class="m-tag">(a - b) ⋮ m</span>.</li>
        <li><b>Đối với nhiều số hạng:</b> Nếu <span class="m-tag">a ⋮ m</span>, <span class="m-tag">b ⋮ m</span> và <span class="m-tag">c ⋮ m</span> thì <span class="m-tag">(a + b + c) ⋮ m</span>.</li>
      </ul>
      <p><b>Ví dụ minh họa 2:</b> Không thực hiện phép tính, xét xem biểu thức <span class="m-tag">A = 48 + 12 - 36</span> có chia hết cho 6 không?</p>
      <ul>
        <li><b>Phân tích:</b> Ta thấy <span class="m-tag">48 ⋮ 6</span> <i>(vì 48 = 6 . 8)</i>, <span class="m-tag">12 ⋮ 6</span> <i>(vì 12 = 6 . 2)</i> và <span class="m-tag">36 ⋮ 6</span> <i>(vì 36 = 6 . 6)</i>.</li>
        <li><b>Kết luận:</b> Vì tất cả các thành phần trong biểu thức đều chia hết cho 6, nên theo Tính chất 1 mở rộng, <span class="m-tag">(48 + 12 - 36) ⋮ 6</span>.</li>
      </ul>
    </div>

    <div class="sky-subbox">
      <div class="sky-sub-heading">2.2. Tính chất 2: Trường hợp KHÔNG CHIA HẾT</div>
      <p><b>Hoạt động khám phá 3:</b> Lấy một số chia hết cho 5 là <span class="m-tag">20</span> và một số không chia hết cho 5 là <span class="m-tag">12</span>. Xét tổng của chúng: <span class="m-tag">20 + 12 = 32</span>. Ta thấy <span class="m-tag">32 ∤ 5</span>.</p>
      <div class="sky-alert">
        <div class="sky-alert-title">TÍNH CHẤT 2 (MỘT SỐ LẺ LOI KHÔNG CHIA HẾT ➔ TỔNG KHÔNG CHIA HẾT)</div>
        Nếu <b>chỉ có duy nhất một số hạng</b> của tổng không chia hết cho một số, còn <b>tất cả các số hạng khác đều chia hết</b> cho số đó thì <b>tổng đó KHÔNG chia hết</b> cho số đó.<br>
        • <b>Công thức tổng quát:</b> Với <i>a, b, m ∈ ℕ</i> và <i>m ≠ 0</i>: Nếu <span class="m-tag">a ⋮ m</span> và <span class="m-tag">b ∤ m</span> thì <span class="m-tag">(a + b) ∤ m</span>
      </div>
      <p><b>Mở rộng Tính chất 2:</b></p>
      <ul>
        <li><b>Đối với phép trừ</b> <i>(điều kiện a &gt; b)</i>: Nếu <span class="m-tag">a ⋮ m</span> và <span class="m-tag">b ∤ m</span> thì <span class="m-tag">(a - b) ∤ m</span> <i>(hoặc ngược lại nếu <span class="m-tag">a ∤ m</span> và <span class="m-tag">b ⋮ m</span> thì <span class="m-tag">(a - b) ∤ m</span>)</i>.</li>
        <li><b>Đối với nhiều số hạng:</b> Nếu <span class="m-tag">a ⋮ m</span>, <span class="m-tag">b ⋮ m</span> nhưng <span class="m-tag">c ∤ m</span> thì <span class="m-tag">(a + b + c) ∤ m</span>.</li>
      </ul>

      <div class="sky-alert sky-alert-danger">
        <div class="sky-alert-title">CẢNH BÁO "BẪY" TOÁN HỌC THƯỜNG GẶP NHẤT!</div>
        Tính chất 2 chỉ đúng khi có <b>DUY NHẤT MỘT</b> số hạng không chia hết. Nếu trong một tổng có <b>từ HAI số hạng trở lên không chia hết</b> cho <i>m</i>, ta <b>TUYỆT ĐỐI KHÔNG ĐƯỢC</b> kết luận ngay là tổng đó không chia hết cho <i>m</i>! Khi đó, các số dư của chúng có thể bù trừ cho nhau để tạo thành một số chia hết.
        <ul>
          <li><b>Ví dụ chứng minh:</b> Xét tổng <span class="m-tag">S = 16 + 13 + 7</span> với số chia là <span class="m-tag">4</span>.</li>
          <li>Ta có: <span class="m-tag">16 ⋮ 4</span>, nhưng <span class="m-tag">13 ∤ 4</span> (dư 1) và <span class="m-tag">7 ∤ 4</span> (dư 3) ➔ Có tới <b>2 số hạng</b> không chia hết cho 4.</li>
          <li>Nếu vội vàng kết luận <span class="m-tag">S ∤ 4</span> là <b>SAI</b>!</li>
          <li><b>Cách làm đúng:</b> Nhóm hai số không chia hết lại với nhau: <span class="m-tag">S = 16 + (13 + 7) = 16 + 20</span>. Vì <span class="m-tag">16 ⋮ 4</span> và <span class="m-tag">20 ⋮ 4</span> nên tổng <span class="m-tag">(16 + 13 + 7) ⋮ 4</span>!</li>
        </ul>
      </div>

      <p><b>TRẠM DỪNG THỰC HÀNH SỐ 2 (Giải quyết bài toán Khởi động):</b> Quay lại câu hỏi của bạn Việt ở đầu bài: Mẹ cho <b>12 gói kẹo</b>, mỗi gói <b>35 cái</b>. Việt lấy ra <b>2 gói kẹo</b> cất đi. Hỏi số kẹo còn lại có chia đều được cho <b>5 bạn</b> không?</p>
      <details class="sky-details" onclick="sndClick()">
        <summary>[ NHẤN VÀO ĐÂY ĐỂ XEM LỜI GIẢI KHOA HỌC ]</summary>
        <div class="sky-details-body">
          <ul>
            <li><b>Bước 1:</b> Tổng số kẹo ban đầu là <span class="m-tag">12 . 35</span>. Vì thừa số <span class="m-tag">35 ⋮ 5</span> nên tích <span class="m-tag">(12 . 35) ⋮ 5</span>.</li>
            <li><b>Bước 2:</b> Số kẹo Việt lấy ra cất đi là <span class="m-tag">2 . 35</span>. Vì <span class="m-tag">35 ⋮ 5</span> nên tích <span class="m-tag">(2 . 35) ⋮ 5</span>.</li>
            <li><b>Bước 3:</b> Số kẹo còn lại là hiệu: <span class="m-tag">(12 . 35) - (2 . 35)</span>. Vì cả số bị trừ và số trừ đều chia hết cho 5, nên theo Tính chất 1 mở rộng, hiệu này <b>chia hết cho 5</b>.</li>
            <li><b>Kết luận:</b> Số kẹo còn lại <b>hoàn toàn chia đều được cho 5 bạn</b> mà không cần tính tổng số kẹo!</li>
          </ul>
        </div>
      </details>
    </div>

  </div>
</div>

<!-- KHUNG 5: ĐẤU TRƯỜNG TRÒ CHƠI TƯƠNG TÁC (CÓ ÂM THANH & NỐI CẶP) -->
<div class="sky-card">
  <div class="sky-card-header">ĐẤU TRƯỜNG TRÍ TUỆ: TRÒ CHƠI NỐI CẶP & TRẮC NGHIỆM CÓ ÂM THANH</div>
  <div class="sky-card-body">

    <!-- VÒNG 1: TRÒ CHƠI NỐI CẶP -->
    <div class="sky-subbox">
      <div class="sky-sub-heading">VÒNG 1: TRÒ CHƠI NỐI CẶP TOÁN HỌC (40 ĐIỂM — 10 Điểm / Cặp)</div>
      <p><b>Cách chơi:</b> Nhấn vào một thẻ ở <b>CỘT A</b>, sau đó nhấn vào thẻ kết quả tương ứng ở <b>CỘT B</b> để nối chúng với nhau. Có âm thanh báo đúng/sai ngay lập tức!</p>

      <div class="match-container">
        <div>
          <div class="match-col-head">CỘT A: BIỂU THỨC / TẬP HỢP</div>
          <div class="match-box" data-a="1" onclick="chooseA(this)">
            <span>1. Tập hợp các ước của 18: Ư(18)</span>
            <span class="match-tag" id="tagA-1"></span>
          </div>
          <div class="match-box" data-a="2" onclick="chooseA(this)">
            <span>2. Tập hợp B(8) nhỏ hơn 35</span>
            <span class="match-tag" id="tagA-2"></span>
          </div>
          <div class="match-box" data-a="3" onclick="chooseA(this)">
            <span>3. Biểu thức: 42 + 56 - 14</span>
            <span class="match-tag" id="tagA-3"></span>
          </div>
          <div class="match-box" data-a="4" onclick="chooseA(this)">
            <span>4. Biểu thức: 24 + 36 + 15</span>
            <span class="match-tag" id="tagA-4"></span>
          </div>
        </div>

        <div>
          <div class="match-col-head">CỘT B: KẾT QUẢ TƯƠNG ỨNG</div>
          <div class="match-box" data-b="3" onclick="chooseB(this)">
            <span>a) Chia hết cho 7 (⋮ 7)</span>
            <span class="match-tag" id="tagB-3"></span>
          </div>
          <div class="match-box" data-b="1" onclick="chooseB(this)">
            <span>b) {1; 2; 3; 6; 9; 18}</span>
            <span class="match-tag" id="tagB-1"></span>
          </div>
          <div class="match-box" data-b="4" onclick="chooseB(this)">
            <span>c) Không chia hết cho 6 (∤ 6)</span>
            <span class="match-tag" id="tagB-4"></span>
          </div>
          <div class="match-box" data-b="2" onclick="chooseB(this)">
            <span>d) {0; 8; 16; 24; 32}</span>
            <span class="match-tag" id="tagB-2"></span>
          </div>
        </div>
      </div>

      <div id="matchNotice" style="margin-top: 12px; font-weight: 800; color: #0284c7;"></div>
      <button class="btn-replay" onclick="replayMatch()">Chơi lại Vòng 1 (Nối cặp)</button>
    </div>

    <!-- VÒNG 2: TRẮC NGHIỆM CÓ ÂM THANH -->
    <div class="sky-subbox">
      <div class="sky-sub-heading">VÒNG 2: KHỞI ĐỘNG NHANH & TĂNG TỐC SUY LUẬN (60 ĐIỂM — 15 Điểm / Câu)</div>

      <div class="quiz-box" id="qz-1">
        <div class="quiz-title">Câu 1: Khẳng định nào dưới đây sử dụng SAI kí hiệu toán học?</div>
        <div class="quiz-list">
          <button class="quiz-opt" onclick="pickQuiz(1, this, false, 'Chưa đúng! Vì 42 = 6 . 7 nên 42 ⋮ 6 là một khẳng định ĐÚNG. Hãy tìm câu sai nhé!')">Phương án A: 42 ⋮ 6</button>
          <button class="quiz-opt" onclick="pickQuiz(1, this, false, 'Chưa đúng! Vì 25 chia hết cho 5 nên 5 là một phần tử thuộc tập hợp ước của 25. Khẳng định này ĐÚNG.')">Phương án B: 5 ∈ Ư(25)</button>
          <button class="quiz-opt" onclick="pickQuiz(1, this, true, 'CHÍNH XÁC (+15 Điểm)! Khẳng định này SAI vì không có phép chia cho số 0, do đó số 0 không bao giờ là ước của bất kì số tự nhiên nào! (Số 0 chỉ là bội của 15: 0 ∈ B(15)).')">Phương án C: 0 ∈ Ư(15)</button>
        </div>
        <div class="quiz-msg" id="qmsg-1"></div>
      </div>

      <div class="quiz-box" id="qz-2">
        <div class="quiz-title">Câu 2: Tập hợp tất cả các số tự nhiên y thỏa mãn y ∈ Ư(50) và y &gt; 5 là:</div>
        <div class="quiz-list">
          <button class="quiz-opt" onclick="pickQuiz(2, this, false, 'Bị lừa rồi! Đề bài yêu cầu y > 5 (lớn hơn hẳn 5) nên không được lấy số 5 vào tập hợp nhé!')">Phương án A: {5; 10; 25; 50}</button>
          <button class="quiz-opt" onclick="pickQuiz(2, this, true, 'XUẤT SẮC (+15 Điểm)! Ta có Ư(50) = {1; 2; 5; 10; 25; 50}. Lọc các phần tử lớn hơn 5, ta thu được tập hợp chuẩn xác là {10; 25; 50}.')">Phương án B: {10; 25; 50}</button>
          <button class="quiz-opt" onclick="pickQuiz(2, this, false, 'Sai rồi! Số 20 không phải là ước của 50 vì 50 chia 20 được 2 dư 10 (50 ∤ 20).')">Phương án C: {10; 20; 25; 50}</button>
        </div>
        <div class="quiz-msg" id="qmsg-2"></div>
      </div>

      <div class="quiz-box" id="qz-3">
        <div class="quiz-title">Câu 3: Không thực hiện phép tính, hãy cho biết trong các biểu thức (M = 80 + 16 + 28; N = 100 - 40; P = 64 + 32 + 19 + 5), biểu thức nào CHIA HẾT CHO 8?</div>
        <div class="quiz-list">
          <button class="quiz-opt" onclick="pickQuiz(3, this, false, 'Sai rồi! Trong biểu thức M có 80 ⋮ 8, 16 ⋮ 8 nhưng 28 ∤ 8 (dư 4). Theo Tính chất 2, M không chia hết cho 8.')">Phương án A: Chỉ có biểu thức M</button>
          <button class="quiz-opt" onclick="pickQuiz(3, this, false, 'Chưa chính xác! Trong biểu thức N có 40 ⋮ 8 nhưng 100 ∤ 8 (100 = 8 . 12 + 4). Vậy (100 - 40) ∤ 8.')">Phương án B: Chỉ có biểu thức N</button>
          <button class="quiz-opt" onclick="pickQuiz(3, this, true, 'ĐỈNH CAO TƯ DUY (+15 Điểm)! Trong P = 64 + 32 + 19 + 5, mặc dù 19 ∤ 8 và 5 ∤ 8, nhưng khi nhóm hai số này lại ta có (19 + 5) = 24 mà 24 ⋮ 8. Do đó tổng P chia hết cho 8!')">Phương án C: Chỉ có biểu thức P</button>
        </div>
        <div class="quiz-msg" id="qmsg-3"></div>
      </div>

      <div class="quiz-box" id="qz-4">
        <div class="quiz-title">Câu 4: Cho tổng S = 35 + x. Tìm điều kiện của số tự nhiên x thuộc tập hợp {7; 14; 18; 21} để S ∤ 7 (S không chia hết cho 7):</div>
        <div class="quiz-list">
          <button class="quiz-opt" onclick="pickQuiz(4, this, false, 'Đọc kĩ đề nhé! Đề bài yêu cầu tìm x để tổng S KHÔNG chia hết cho 7 (S ∤ 7). Với x ∈ {7; 14; 21} thì tổng S sẽ chia hết cho 7 mất rồi!')">Phương án A: x ∈ {7; 14; 21}</button>
          <button class="quiz-opt" onclick="pickQuiz(4, this, true, 'CHÍNH XÁC TUYỆT ĐỐI (+15 Điểm)! Ta có 35 ⋮ 7. Theo Tính chất 2, để tổng (35 + x) ∤ 7 thì số hạng x phải không chia hết cho 7 (x ∤ 7). Trong tập hợp đã cho, chỉ có duy nhất 18 ∤ 7. Vậy x = 18.')">Phương án B: x = 18</button>
        </div>
        <div class="quiz-msg" id="qmsg-4"></div>
      </div>
    </div>

    <!-- VÒNG 3: TỰ LUẬN & TOÁN THỰC TẾ -->
    <div class="sky-subbox">
      <div class="sky-sub-heading">VÒNG 3: CHINH PHỤC TỰ LUẬN & TOÁN THỰC TẾ (40 Điểm — Làm vào vở)</div>
      <ul>
        <li><b>Bài tập 1 (Nhận diện tính chất trong biểu thức chứa tích):</b><br>Xét xem các khẳng định sau là Đúng hay Sai và giải thích rõ lí do:<br>a) <span class="m-tag">(219 . 7 + 8)</span> chia hết cho 7.<br>b) <span class="m-tag">(8 . 12 + 9)</span> chia hết cho 3.</li>
        <li><b>Bài tập 2 (Bài toán chia nhóm dự án - SGK Toán 6):</b><br>Một lớp học có <b>40 học sinh</b>. Giáo viên muốn chia lớp thành các nhóm có số người như nhau để thực hiện dự án học tập. Biết rằng mỗi nhóm phải có <b>nhiều hơn 3 người</b> và <b>ít hơn 15 người</b>. Hỏi có thể chia lớp thành mấy nhóm và mỗi nhóm có bao nhiêu học sinh?</li>
        <li><b>Bài tập 3 (Thử thách nâng cao dành cho học sinh giỏi):</b><br>Tìm tất cả các số tự nhiên <i>n</i> sao cho <span class="m-tag">(n + 8) ⋮ (n + 3)</span>.</li>
      </ul>

      <details class="sky-details" onclick="sndClick()">
        <summary>[ MỞ KHÓA HƯỚNG DẪN GIẢI VÀ THANG ĐIỂM TỰ CHẤM VÒNG 3 ]</summary>
        <div class="sky-details-body">
          <p><b>Lời giải Bài tập 1 (10 Điểm):</b></p>
          <ul>
            <li><b>a) Khẳng định SAI.</b> Vì <span class="m-tag">7 ⋮ 7</span> nên tích <span class="m-tag">(219 . 7) ⋮ 7</span>. Tuy nhiên, số hạng thứ hai là <span class="m-tag">8 ∤ 7</span>. Theo Tính chất 2, tổng <span class="m-tag">(219 . 7 + 8) ∤ 7</span>.</li>
            <li><b>b) Khẳng định ĐÚNG.</b> Trong tích <span class="m-tag">(8 . 12)</span> có thừa số <span class="m-tag">12 ⋮ 3</span> nên tích <span class="m-tag">(8 . 12) ⋮ 3</span>. Mặt khác, số hạng thứ hai là <span class="m-tag">9 ⋮ 3</span>. Theo Tính chất 1, tổng <span class="m-tag">(8 . 12 + 9) ⋮ 3</span>.</li>
          </ul>
          <hr>
          <p><b>Lời giải Bài tập 2 (15 Điểm):</b></p>
          <ul>
            <li>Gọi số học sinh trong mỗi nhóm là <i>x</i> (điều kiện: <i>x ∈ ℕ*</i> và <b>3 &lt; <i>x</i> &lt; 15</b>).</li>
            <li>Vì 40 học sinh được chia đều vào các nhóm không dư bạn nào nên <span class="m-tag">40 ⋮ x</span>, suy ra <span class="m-tag">x ∈ Ư(40)</span>.</li>
            <li>Ta tìm tập hợp các ước của 40 bằng phương pháp cặp nhân: <span class="m-tag">Ư(40) = {1; 2; 4; 5; 8; 10; 20; 40}</span>.</li>
            <li>Kết hợp với điều kiện <b>3 &lt; <i>x</i> &lt; 15</b>, ta chọn được các giá trị thỏa mãn là: <span class="m-tag">x ∈ {4; 5; 8; 10}</span>.</li>
          </ul>
          <table class="sky-table">
            <thead>
              <tr>
                <th>Phương án</th>
                <th>Số học sinh mỗi nhóm (x)</th>
                <th>Số nhóm tương ứng (40 : x)</th>
              </tr>
            </thead>
            <tbody>
              <tr><td><b>Cách 1</b></td><td><b>4</b> học sinh</td><td><span class="m-tag">40 : 4</span> = <b>10 nhóm</b></td></tr>
              <tr><td><b>Cách 2</b></td><td><b>5</b> học sinh</td><td><span class="m-tag">40 : 5</span> = <b>8 nhóm</b></td></tr>
              <tr><td><b>Cách 3</b></td><td><b>8</b> học sinh</td><td><span class="m-tag">40 : 8</span> = <b>5 nhóm</b></td></tr>
              <tr><td><b>Cách 4</b></td><td><b>10</b> học sinh</td><td><span class="m-tag">40 : 10</span> = <b>4 nhóm</b></td></tr>
            </tbody>
          </table>
          <hr>
          <p><b>Lời giải Bài tập 3 - Nâng cao (15 Điểm):</b></p>
          <ul>
            <li><b>Phương pháp tách số:</b> Ta biến đổi biểu thức bị chia <span class="m-tag">(n + 8)</span> sao cho xuất hiện biểu thức chia <span class="m-tag">(n + 3)</span>: Ta có <span class="m-tag">n + 8 = (n + 3) + 5</span>.</li>
            <li>Vì bản thân số hạng <span class="m-tag">(n + 3) ⋮ (n + 3)</span> với mọi số tự nhiên <i>n</i>, nên theo Tính chất 1 và 2, để tổng <span class="m-tag">[(n + 3) + 5] ⋮ (n + 3)</span> thì số hạng còn lại là <b>5 phải chia hết cho <span class="m-tag">(n + 3)</span></b>, tức là: <span class="m-tag">5 ⋮ (n + 3)</span> hay <span class="m-tag">(n + 3) ∈ Ư(5)</span>.</li>
            <li>Mà <span class="m-tag">Ư(5) = {1; 5}</span>. Vì <i>n</i> là số tự nhiên (<i>n ≥ 0</i>) nên <span class="m-tag">n + 3 ≥ 3</span>.</li>
            <li>Đối chiếu với tập hợp <span class="m-tag">Ư(5)</span>, chỉ có giá trị <span class="m-tag">n + 3 = 5</span> thỏa mãn (loại trường hợp <span class="m-tag">n + 3 = 1</span>).</li>
            <li>Từ <span class="m-tag">n + 3 = 5</span>, suy ra <span class="m-tag">n = 5 - 3 = 2</span>.</li>
            <li><b>Kết luận:</b> Vậy <span class="m-tag">n = 2</span> <i>(Thử lại: với n = 2 thì n + 8 = 10, n + 3 = 5, ta có 10 ⋮ 5 — hoàn toàn chính xác!)</i>.</li>
          </ul>
        </div>
      </details>
    </div>

  </div>
</div>

<!-- KHUNG 6: SƠ ĐỒ TỔNG KẾT KIẾN THỨC CỐT LÕI -->
<div class="sky-card">
  <div class="sky-card-header">SƠ ĐỒ TỔNG KẾT KIẾN THỨC CỐT LÕI (DÀNH CHO ÔN THI)</div>
  <div class="sky-card-body">
    <table class="sky-table">
      <thead>
        <tr>
          <th colspan="2" style="text-align:center; font-size:1.05rem;">
            TRỌNG TÂM: QUAN HỆ CHIA HẾT — a = b . k (với a, b ∈ ℕ; b ≠ 0) ➔ a ⋮ b
          </th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td width="50%">
            <b>NHÁNH 1: KHÁI NIỆM ƯỚC & BỘI</b>
            <ul>
              <li><b>a là BỘI của b</b> — Kí hiệu: <span class="m-tag">B(b)</span><br>➔ <i>Cách tìm:</i> Nhân <i>b</i> lần lượt với <span class="m-tag">0, 1, 2, 3, ...</span> (Tập hợp vô hạn).</li>
              <li><b>b là ƯỚC của a</b> — Kí hiệu: <span class="m-tag">Ư(a)</span><br>➔ <i>Cách tìm:</i> Chia <i>a</i> lần lượt cho <span class="m-tag">1, 2, ..., a</span> (Tập hợp hữu hạn).<br><i>(Mẹo: Dùng phương pháp ghép cặp nhân đối xứng từ ngoài vào trong để không bao giờ bị sót nghiệm).</i></li>
            </ul>
          </td>
          <td width="50%">
            <b>NHÁNH 2: TÍNH CHẤT CHIA HẾT CỦA TỔNG VÀ HIỆU</b>
            <ul>
              <li><b>Tính chất 1 (Trường hợp cùng chia hết):</b><br>Nếu <span class="m-tag">a ⋮ m</span> và <span class="m-tag">b ⋮ m</span> thì:<br>➔ <span class="m-tag">(a + b) ⋮ m</span> và <span class="m-tag">(a - b) ⋮ m</span> <i>(với điều kiện a ≥ b)</i>.</li>
              <li><b>Tính chất 2 (Trường hợp chỉ có một số không chia hết):</b><br>Nếu <span class="m-tag">a ⋮ m</span> và <span class="m-tag">b ∤ m</span> thì:<br>➔ <span class="m-tag">(a + b) ∤ m</span> và <span class="m-tag">(a - b) ∤ m</span> <i>(với điều kiện a &gt; b)</i>.<br><i>(Cảnh báo: Nếu có từ 2 số hạng trở lên không chia hết, tuyệt đối không dùng tính chất 2).</i></li>
            </ul>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<script>
  // BỘ PHÁT ÂM THANH TỰ ĐỘNG (WEB AUDIO API)
  let isSoundOn = true;
  const AudioCtx = window.AudioContext || window.webkitAudioContext;
  let actx = null;

  function initCtx() {
    if (!actx) actx = new AudioCtx();
    if (actx.state === 'suspended') actx.resume();
  }

  function tone(freq, type, dur, delay = 0) {
    if (!isSoundOn) return;
    initCtx();
    setTimeout(() => {
      const o = actx.createOscillator();
      const g = actx.createGain();
      o.type = type;
      o.frequency.setValueAtTime(freq, actx.currentTime);
      g.gain.setValueAtTime(0.18, actx.currentTime);
      g.gain.exponentialRampToValueAtTime(0.001, actx.currentTime + dur);
      o.connect(g);
      g.connect(actx.destination);
      o.start();
      o.stop(actx.currentTime + dur);
    }, delay);
  }

  function sndClick() { tone(540, 'sine', 0.07); }
  function sndRight() { tone(587.33, 'triangle', 0.14, 0); tone(880, 'triangle', 0.28, 110); }
  function sndWrong() { tone(210, 'sawtooth', 0.16, 0); tone(165, 'sawtooth', 0.24, 140); }
  function sndWin() {
    tone(523.25, 'triangle', 0.14, 0);
    tone(659.25, 'triangle', 0.14, 120);
    tone(783.99, 'triangle', 0.14, 240);
    tone(1046.50, 'triangle', 0.40, 360);
  }

  function switchSound() {
    isSoundOn = !isSoundOn;
    document.getElementById('btnAudio').textContent = isSoundOn ? 'Âm thanh: ĐANG BẬT' : 'Âm thanh: ĐÃ TẮT';
    if (isSoundOn) sndClick();
  }

  let curScore = 0;
  function addPts(pts) {
    curScore += pts;
    document.getElementById('scoreVal').textContent = curScore;
    if (curScore === 100) setTimeout(sndWin, 350);
  }

  // VÒNG 1: NỐI CẶP
  let pickedA = null;
  let matchedPairs = 0;

  function chooseA(el) {
    if (el.classList.contains('matched')) return;
    sndClick();
    document.querySelectorAll('[data-a]').forEach(x => x.classList.remove('selected'));
    el.classList.add('selected');
    pickedA = el;
  }

  function chooseB(el) {
    if (el.classList.contains('matched') || !pickedA) return;
    const aVal = pickedA.getAttribute('data-a');
    const bVal = el.getAttribute('data-b');

    if (aVal === bVal) {
      sndRight();
      pickedA.classList.remove('selected');
      pickedA.classList.add('matched');
      el.classList.add('matched');
      document.getElementById('tagA-' + aVal).textContent = 'Cặp #' + aVal;
      document.getElementById('tagB-' + bVal).textContent = 'Cặp #' + aVal;
      pickedA = null;
      matchedPairs++;
      addPts(10);
      if (matchedPairs === 4) {
        document.getElementById('matchNotice').textContent = 'XUẤT SẮC! Bạn đã nối đúng toàn bộ 4 cặp kiến thức (+40 Điểm)!';
        sndWin();
      }
    } else {
      sndWrong();
      const tmp = pickedA;
      tmp.classList.add('wrong');
      el.classList.add('wrong');
      setTimeout(() => {
        tmp.classList.remove('wrong', 'selected');
        el.classList.remove('wrong');
      }, 400);
      pickedA = null;
    }
  }

  function replayMatch() {
    sndClick();
    addPts(-(matchedPairs * 10));
    matchedPairs = 0;
    pickedA = null;
    document.getElementById('matchNotice').textContent = '';
    document.querySelectorAll('.match-box').forEach(x => x.classList.remove('matched', 'selected', 'wrong'));
  }

  // VÒNG 2: TRẮC NGHIỆM
  const doneQuiz = {};
  function pickQuiz(qNum, btn, isOk, msg) {
    if (doneQuiz[qNum]) return;
    const box = document.getElementById('qmsg-' + qNum);
    box.style.display = 'block';
    box.textContent = msg;

    if (isOk) {
      sndRight();
      btn.classList.add('ok');
      box.style.background = '#dcfce7';
      box.style.color = '#166534';
      box.style.border = '1.5px solid #16a34a';
      doneQuiz[qNum] = true;
      addPts(15);
      document.querySelectorAll('#qz-' + qNum + ' .quiz-opt').forEach(b => b.disabled = true);
    } else {
      sndWrong();
      btn.classList.add('err');
      box.style.background = '#ffe4e6';
      box.style.color = '#9f1239';
      box.style.border = '1.5px solid #e11d48';
    }
  }
</script>
