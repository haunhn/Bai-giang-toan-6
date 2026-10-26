<style>
  /* Ẩn tiêu đề mặc định của GitHub Pages & Thiết lập nền Xanh Nước Biển Nhạt */
  .markdown-body > h1:first-child { display: none !important; }
  .container-lg, .markdown-body { max-width: 980px !important; margin: 0 auto !important; padding: 16px !important; font-family: 'Segoe UI', system-ui, -apple-system, sans-serif !important; color: #0c4a6e !important; background-color: #f0f9ff !important; }
  body { background-color: #f0f9ff !important; }

  /* Thanh điều khiển cố định (Sticky Bar) */
  .sky-topbar { position: sticky; top: 10px; z-index: 999; background: #ffffff; border: 2px solid #0284c7; border-radius: 12px; padding: 10px 20px; margin-bottom: 24px; display: flex; justify-content: space-between; align-items: center; box-shadow: 0 8px 20px rgba(2, 132, 199, 0.14); flex-wrap: wrap; gap: 10px; }
  .sky-topbar-title { font-weight: 800; color: #075985; font-size: 0.98rem; letter-spacing: 0.3px; }
  .sky-topbar-right { display: flex; align-items: center; gap: 12px; }
  .sky-score-badge { background: #e0f2fe; color: #0369a1; border: 1.5px solid #0284c7; padding: 5px 16px; border-radius: 99px; font-weight: 800; font-size: 0.95rem; }
  .sky-sound-btn { background: #0284c7; color: #ffffff; border: none; padding: 7px 15px; border-radius: 8px; font-weight: 700; cursor: pointer; font-size: 0.88rem; transition: 0.2s; }
  .sky-sound-btn:hover { background: #0369a1; }

  /* Khung Banner chính */
  .sky-hero { background: linear-gradient(135deg, #e0f2fe 0%, #bae6fd 100%); border: 2px solid #0284c7; border-radius: 16px; padding: 30px 24px; text-align: center; margin-bottom: 26px; box-shadow: 0 8px 22px rgba(2, 132, 199, 0.1); }
  .sky-hero-tag { display: inline-block; background: #0284c7; color: #ffffff; font-weight: 800; font-size: 0.82rem; padding: 5px 16px; border-radius: 99px; text-transform: uppercase; letter-spacing: 0.7px; margin-bottom: 10px; }
  .sky-hero-title { color: #0c4a6e !important; font-size: 1.95rem !important; font-weight: 800 !important; margin: 0 0 14px 0 !important; border: none !important; padding: 0 !important; }
  .sky-meta-row { display: flex; justify-content: center; flex-wrap: wrap; gap: 10px; }
  .sky-meta-item { background: #ffffff; border: 1px solid #7dd3fc; color: #0369a1; padding: 5px 14px; border-radius: 8px; font-size: 0.9rem; font-weight: 600; }

  /* Hệ thống Khung bài giảng (Section Frames) */
  .sky-card { background: #ffffff; border: 2px solid #bae6fd; border-radius: 16px; margin-bottom: 28px; overflow: hidden; box-shadow: 0 5px 15px rgba(2, 132, 199, 0.06); }
  .sky-card-head { background: linear-gradient(90deg, #e0f2fe 0%, #bae6fd 100%); border-bottom: 2px solid #7dd3fc; padding: 14px 22px; color: #0c4a6e; font-size: 1.18rem; font-weight: 800; display: flex; justify-content: space-between; align-items: center; }
  .sky-step-tag { background: #0284c7; color: #fff; font-size: 0.78rem; padding: 3px 12px; border-radius: 12px; font-weight: 700; }
  .sky-card-body { padding: 24px; line-height: 1.7; font-size: 1rem; }

  /* Khung Lý thuyết cô đọng (Đặt trước Trạm khám phá) */
  .sky-theory-box { background: #f0f9ff; border: 1.5px solid #7dd3fc; border-left: 6px solid #0284c7; border-radius: 12px; padding: 18px 20px; margin-bottom: 20px; }
  .sky-theory-head { font-weight: 800; color: #0369a1; font-size: 1.05rem; margin-bottom: 12px; text-transform: uppercase; letter-spacing: 0.3px; border-bottom: 1.5px solid #bae6fd; padding-bottom: 6px; }
  .sky-theory-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 14px; margin-top: 10px; }
  .sky-mini-card { background: #ffffff; border: 1px solid #bae6fd; border-radius: 10px; padding: 14px 16px; }
  .sky-mini-title { font-weight: 800; color: #0284c7; margin-bottom: 6px; font-size: 0.98rem; }
  .sky-warn-strip { background: #fef9c3; border: 1px solid #fde047; border-left: 5px solid #eab308; border-radius: 8px; padding: 12px 16px; margin-top: 14px; color: #713f12; font-size: 0.95rem; }
  .sky-danger-strip { background: #ffe4e6; border: 1px solid #fda4af; border-left: 5px solid #e11d48; border-radius: 8px; padding: 12px 16px; margin-top: 14px; color: #881337; font-size: 0.95rem; }

  /* Bảng quy tắc */
  .sky-table { width: 100%; border-collapse: collapse; margin: 12px 0; border-radius: 10px; overflow: hidden; border: 1.5px solid #7dd3fc; }
  .sky-table th { background: #0284c7 !important; color: #ffffff !important; padding: 11px 15px !important; text-align: left; font-weight: 800; border: 1px solid #0369a1 !important; }
  .sky-table td { padding: 11px 15px !important; border: 1px solid #bae6fd !important; background: #ffffff !important; color: #0c4a6e !important; vertical-align: top; }
  .sky-table tr:nth-child(even) td { background: #f0f9ff !important; }

  /* Khung Trạm khám phá tương tác */
  .sky-quest-box { background: #f8fafc; border: 2px dashed #0284c7; border-radius: 12px; padding: 18px 20px; margin-bottom: 10px; }
  .sky-quest-title { font-weight: 800; color: #0369a1; margin-bottom: 10px; font-size: 1.03rem; text-transform: uppercase; }

  /* Nút chọn số (Number Chips) */
  .chip-grid { display: flex; flex-wrap: wrap; gap: 10px; margin: 12px 0; }
  .num-chip { background: #ffffff; border: 2px solid #7dd3fc; color: #0c4a6e; padding: 9px 16px; border-radius: 10px; font-weight: 800; font-size: 1rem; cursor: pointer; transition: 0.2s; user-select: none; text-align: center; min-width: 68px; }
  .num-chip:hover { background: #e0f2fe; border-color: #0284c7; transform: translateY(-2px); }
  .num-chip.correct { background: #0284c7; border-color: #075985; color: #ffffff; }
  .num-chip.wrong { background: #ffe4e6; border-color: #e11d48; color: #9f1239; text-decoration: line-through; opacity: 0.75; }

  /* Phòng thí nghiệm nhập số tương tác */
  .lab-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 16px; margin: 14px 0; }
  .lab-box { background: #ffffff; border: 1.5px solid #bae6fd; border-radius: 12px; padding: 16px; }
  .lab-row-inp { display: flex; align-items: center; gap: 8px; margin-top: 10px; flex-wrap: wrap; }
  .sky-input { width: 68px; padding: 6px 8px; border: 2px solid #0284c7; border-radius: 8px; font-weight: 800; text-align: center; font-size: 0.98rem; color: #0c4a6e; background: #f0f9ff; outline: none; }
  .sky-input:focus { border-color: #075985; background: #ffffff; }
  .sky-btn { background: #0284c7; color: #ffffff; border: none; padding: 8px 16px; border-radius: 8px; font-weight: 700; cursor: pointer; transition: 0.2s; }
  .sky-btn:hover { background: #0369a1; }
  .lab-msg { font-size: 0.92rem; font-weight: 700; margin-top: 8px; min-height: 22px; }

  /* Bảng phân loại tương tác (Trạm 3) */
  .sort-item { background: #ffffff; border: 1.5px solid #bae6fd; border-radius: 10px; padding: 12px 16px; margin-bottom: 12px; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 10px; }
  .sort-expr { font-weight: 800; font-size: 1.02rem; color: #0c4a6e; }
  .sort-btns { display: flex; gap: 8px; }
  .s-btn { background: #f0f9ff; border: 2px solid #7dd3fc; color: #0369a1; padding: 6px 14px; border-radius: 8px; font-weight: 800; cursor: pointer; transition: 0.2s; }
  .s-btn:hover:not(:disabled) { background: #e0f2fe; border-color: #0284c7; }
  .s-btn.ok { background: #dcfce7; border-color: #16a34a; color: #166534; }
  .s-btn.err { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .sort-fb { width: 100%; font-size: 0.9rem; font-weight: 600; margin-top: 4px; display: none; padding: 8px 12px; border-radius: 6px; }

  .s-tag { background: #ffffff; color: #0369a1; border: 1px solid #7dd3fc; padding: 1px 8px; border-radius: 6px; font-family: 'Consolas', monospace; font-weight: 800; font-size: 0.95em; display: inline-block; }

  /* Trò chơi Nối cặp (Matching Game) */
  .match-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; margin-top: 14px; }
  .match-head { background: #0284c7; color: #ffffff; text-align: center; padding: 9px; border-radius: 8px; font-weight: 800; margin-bottom: 10px; }
  .m-card { background: #ffffff; border: 2px solid #7dd3fc; border-radius: 10px; padding: 13px 15px; margin-bottom: 10px; font-weight: 700; color: #0c4a6e; cursor: pointer; transition: 0.2s; display: flex; justify-content: space-between; align-items: center; user-select: none; }
  .m-card:hover:not(.matched) { background: #e0f2fe; border-color: #0284c7; transform: translateY(-2px); }
  .m-card.selected { background: #0284c7; color: #ffffff; border-color: #075985; box-shadow: 0 0 0 4px rgba(2, 132, 199, 0.25); }
  .m-card.matched { background: #dcfce7; border-color: #16a34a; color: #166534; cursor: default; }
  .m-card.wrong { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .m-badge { font-size: 0.78rem; background: #16a34a; color: #fff; padding: 2px 8px; border-radius: 10px; display: none; }
  .m-card.matched .m-badge { display: inline-block; }

  /* Trắc nghiệm tốc độ */
  .q-card { background: #ffffff; border: 1.5px solid #7dd3fc; border-radius: 12px; padding: 16px; margin-bottom: 14px; }
  .q-title { font-weight: 800; color: #0c4a6e; margin-bottom: 10px; }
  .q-opts { display: grid; grid-template-columns: repeat(auto-fit, minmax(210px, 1fr)); gap: 10px; }
  .q-btn { background: #f0f9ff; border: 2px solid #bae6fd; padding: 10px 14px; border-radius: 8px; font-weight: 700; color: #0c4a6e; cursor: pointer; text-align: left; transition: 0.2s; }
  .q-btn:hover:not(:disabled) { background: #e0f2fe; border-color: #0284c7; }
  .q-btn.ok { background: #dcfce7; border-color: #16a34a; color: #166534; }
  .q-btn.err { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .q-exp { display: none; margin-top: 10px; padding: 10px 14px; border-radius: 8px; font-weight: 600; font-size: 0.92rem; }

  /* Nút mở lời giải tự luận */
  details.sky-details { background: #ffffff; border: 2px solid #0284c7; border-radius: 10px; margin-top: 14px; overflow: hidden; }
  details.sky-details summary { background: #e0f2fe; color: #0c4a6e; padding: 12px 18px; font-weight: 800; cursor: pointer; list-style: none; user-select: none; transition: 0.2s; }
  details.sky-details summary:hover { background: #bae6fd; }
  .sky-details-body { padding: 18px; border-top: 1.5px solid #bae6fd; background: #ffffff; }

  @media (max-width: 680px) {
    .match-grid { grid-template-columns: 1fr; }
  }
</style>

<!-- THANH ĐIỀU KHIỂN CỐ ĐỊNH -->
<div class="sky-topbar">
  <div class="sky-topbar-title">TOÁN 6 — BÀI 8: QUAN HỆ CHIA HẾT VÀ TÍNH CHẤT</div>
  <div class="sky-topbar-right">
    <div class="sky-score-badge">ĐIỂM KHÁM PHÁ: <span id="ptsVal">0</span> / 100</div>
    <button class="sky-sound-btn" id="btnSound" onclick="toggleSound()">Âm thanh: ĐANG BẬT</button>
  </div>
</div>

<!-- BANNER MỞ ĐẦU -->
<div class="sky-hero">
  <div class="sky-hero-tag">CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN</div>
  <h1 class="sky-hero-title">BÀI 8: QUAN HỆ CHIA HẾT VÀ TÍNH CHẤT</h1>
  <div class="sky-meta-row">
    <div class="sky-meta-item">Toán 6 (Tập 1) — Kết nối tri thức với cuộc sống</div>
    <div class="sky-meta-item">Thời lượng: 45 – 60 phút (Lý thuyết cô đọng + Tương tác + Trò chơi)</div>
  </div>
</div>

<!-- NỘI DUNG 1: QUAN HỆ CHIA HẾT & KHÁI NIỆM ƯỚC - BỘI -->
<div class="sky-card">
  <div class="sky-card-head">
    <span>NỘI DUNG 1: QUAN HỆ CHIA HẾT & KHÁI NIỆM ƯỚC – BỘI</span>
    <span class="sky-step-tag">Phần 1 / 4</span>
  </div>
  <div class="sky-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="sky-theory-box">
      <div class="sky-theory-head">1. LÝ THUYẾT CỐT LÕI CẦN NHỚ</div>
      <div class="sky-theory-grid">
        <div class="sky-mini-card">
          <div class="sky-mini-title">QUAN HỆ CHIA HẾT</div>
          Cho hai số tự nhiên <i>a</i> và <i>b</i> (<span class="s-tag">b ≠ 0</span>):<br>
          • Nếu có số tự nhiên <i>k</i> sao cho <span class="s-tag">a = b . k</span> thì ta nói <b><i>a</i> chia hết cho <i>b</i></b>, kí hiệu: <span class="s-tag">a ⋮ b</span>.<br>
          • Nếu <i>a</i> không chia hết cho <i>b</i> (phép chia có dư), kí hiệu: <span class="s-tag">a ∤ b</span>.
        </div>
        <div class="sky-mini-card">
          <div class="sky-mini-title">TÊN GỌI ƯỚC VÀ BỘI</div>
          Khi <span class="s-tag">a ⋮ b</span>, ta định danh:<br>
          • Số bị chia <b><i>a</i></b> là <b>BỘI</b> của <i>b</i> ➔ Kí hiệu tập hợp: <span class="s-tag">B(b)</span>.<br>
          • Số chia <b><i>b</i></b> là <b>ƯỚC</b> của <i>a</i> ➔ Kí hiệu tập hợp: <span class="s-tag">Ư(a)</span>.<br>
          • <i>Ví dụ:</i> Vì <span class="s-tag">24 ⋮ 8</span> nên <span class="s-tag">24 ∈ B(8)</span> và <span class="s-tag">8 ∈ Ư(24)</span>.
        </div>
      </div>
      <div class="sky-warn-strip">
        <b>Các trường hợp đặc biệt của số 0 và số 1:</b><br>
        • <b>Số 0:</b> Là <b>bội</b> của mọi số tự nhiên khác 0, nhưng <b>không phải là ước</b> của bất kì số tự nhiên nào.<br>
        • <b>Số 1:</b> Chỉ có 1 ước là chính nó (<span class="s-tag">Ư(1) = {1}</span>), nhưng lại là <b>ước của mọi số tự nhiên</b>.<br>
        • Mọi số tự nhiên <span class="s-tag">a ≠ 0</span> luôn là ước của chính nó và là bội của chính nó.
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ 1 -->
    <div class="sky-quest-box">
      <div class="sky-quest-title">TRẠM KHÁM PHÁ 1: SĂN TÌM TẬP HỢP CÁC ƯỚC CỦA 18 (+15 ĐIỂM)</div>
      <p><b>Nhiệm vụ:</b> Số 18 chia hết cho những số nào dưới đây? Hãy <b>bấm chọn đúng 6 ước của 18</b> để hoàn thành tập hợp <span class="s-tag">Ư(18)</span>:</p>
      <div class="chip-grid" id="u18Grid">
        <div class="num-chip" onclick="pickU18(this, false, 'Cảnh báo bẫy! Không có phép chia cho 0 nên số 0 không bao giờ là ước của bất kì số nào!')">Số 0</div>
        <div class="num-chip" onclick="pickU18(this, true, 'Chính xác! 18 = 1 . 18 nên 1 và 18 là cặp ước đầu tiên.')">Số 1</div>
        <div class="num-chip" onclick="pickU18(this, true, 'Chính xác! 18 = 2 . 9 nên 2 là ước của 18.')">Số 2</div>
        <div class="num-chip" onclick="pickU18(this, true, 'Chính xác! 18 = 3 . 6 nên 3 là ước của 18.')">Số 3</div>
        <div class="num-chip" onclick="pickU18(this, false, 'Sai rồi! 18 chia 4 được 4 dư 2 (18 ∤ 4).')">Số 4</div>
        <div class="num-chip" onclick="pickU18(this, true, 'Chính xác! 18 ⋮ 6 (cặp đối xứng với số 3).')">Số 6</div>
        <div class="num-chip" onclick="pickU18(this, false, 'Sai rồi! 18 chia 8 được 2 dư 2 (18 ∤ 8).')">Số 8</div>
        <div class="num-chip" onclick="pickU18(this, true, 'Chính xác! 18 ⋮ 9 (cặp đối xứng với số 2).')">Số 9</div>
        <div class="num-chip" onclick="pickU18(this, true, 'Xuất sắc! Mọi số tự nhiên khác 0 luôn có ước lớn nhất là chính nó (18).')">Số 18</div>
      </div>
      <div id="msgU18" style="font-weight:700; color:#0369a1; font-size:0.93rem; min-height:22px;"></div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 2: QUY TRÌNH TÌM ƯỚC VÀ BỘI -->
<div class="sky-card">
  <div class="sky-card-head">
    <span>NỘI DUNG 2: QUY TRÌNH TÌM TẬP HỢP ƯỚC VÀ BỘI</span>
    <span class="sky-step-tag">Phần 2 / 4</span>
  </div>
  <div class="sky-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="sky-theory-box">
      <div class="sky-theory-head">2. BẢNG QUY TẮC TÌM ƯỚC VÀ BỘI CHUẨN XÁC</div>
      <table class="sky-table">
        <thead>
          <tr>
            <th width="22%">Tiêu chí</th>
            <th width="39%">QUY TẮC TÌM ƯỚC CỦA SỐ a (a &gt; 1)</th>
            <th width="39%">QUY TẮC TÌM BỘI CỦA SỐ b (b ≠ 0)</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><b>Cách thực hiện</b></td>
            <td>Lần lượt <b>chia <i>a</i></b> cho các số tự nhiên từ <span class="s-tag">1</span> đến <span class="s-tag">a</span>. Phép chia nào chia hết thì số chia đó là <b>ước</b> của <i>a</i>.</td>
            <td>Lần lượt <b>nhân <i>b</i></b> với <span class="s-tag">0, 1, 2, 3, 4, ...</span> Các kết quả thu được đều là <b>bội</b> của <i>b</i>.</td>
          </tr>
          <tr>
            <td><b>Số lượng phần tử</b></td>
            <td><b>Hữu hạn</b> phần tử. Bắt đầu bằng <span class="s-tag">1</span> và kết thúc bằng chính số <span class="s-tag">a</span>.</td>
            <td><b>Vô số</b> phần tử. Bắt đầu bằng số <span class="s-tag">0</span> và có dấu <span class="s-tag">...</span> ở cuối tập hợp.</td>
          </tr>
        </tbody>
      </table>
      <div class="sky-warn-strip">
        <b>Mẹo "Cặp thừa số đối xứng" khi tìm Ước của số lớn (như Ư(36)):</b><br>
        Thay vì chia lần lượt từ 1 đến 36, ta tìm các cặp số nhân với nhau bằng 36 từ ngoài vào trong:<br>
        • <span class="s-tag">36 = 1 . 36 = 2 . 18 = 3 . 12 = 4 . 9 = 6 . 6</span> (hai thừa số chạm nhau tại 6 thì dừng lại!).<br>
        ➔ Sắp xếp tăng dần: <span class="s-tag">Ư(36) = {1; 2; 3; 4; 6; 9; 12; 18; 36}</span> (không bao giờ sót nghiệm!).
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ 2 -->
    <div class="sky-quest-box">
      <div class="sky-quest-title">TRẠM KHÁM PHÁ 2: PHÒNG THÍ NGHIỆM CẶP ƯỚC & BỘI CÓ ĐIỀU KIỆN (+20 ĐIỂM)</div>
      <div class="lab-grid">
        <div class="lab-box">
          <b>Thí nghiệm A: Tìm cặp ước đối xứng của 20</b><br>
          Ta tách: <span class="s-tag">20 = 1 . 20 = 2 . 10 = 4 . ?</span><br>
          Do đó <span class="s-tag">Ư(20) = {1; 2; 4; ?; 10; 20}</span>. Số còn thiếu ở dấu <span class="s-tag">?</span> là bao nhiêu?
          <div class="lab-row-inp">
            <span>Ước còn thiếu = </span>
            <input type="number" id="inpLab1" class="sky-input" placeholder="?">
            <button class="sky-btn" onclick="checkLab(1, 5, 'Chính xác! Cặp nhân cuối cùng là 4 . 5 = 20 ➔ Ư(20) = {1; 2; 4; 5; 10; 20}!')">Kiểm tra</button>
          </div>
          <div class="lab-msg" id="msgLab1"></div>
        </div>

        <div class="lab-box">
          <b>Thí nghiệm B: Tìm bội thỏa mãn điều kiện</b><br>
          Tìm số tự nhiên <span class="s-tag">x</span> lớn nhất sao cho <span class="s-tag">x ∈ B(8)</span> và <span class="s-tag">x &lt; 40</span>.<br>
          <i>(Gợi ý: Nhân 8 với 0, 1, 2, 3, 4... nhưng phải nhỏ hơn hẳn 40)</i>.
          <div class="lab-row-inp">
            <span>Giá trị x lớn nhất = </span>
            <input type="number" id="inpLab2" class="sky-input" placeholder="x = ?">
            <button class="sky-btn" onclick="checkLab(2, 32, 'Tuyệt vời! Các bội nhỏ hơn 40 của 8 là {0; 8; 16; 24; 32} (không lấy 40 vì x < 40).')">Kiểm tra</button>
          </div>
          <div class="lab-msg" id="msgLab2"></div>
        </div>
      </div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 3: TÍNH CHẤT CHIA HẾT CỦA MỘT TỔNG (VÀ HIỆU) -->
<div class="sky-card">
  <div class="sky-card-head">
    <span>NỘI DUNG 3: TÍNH CHẤT CHIA HẾT CỦA MỘT TỔNG (VÀ HIỆU)</span>
    <span class="sky-step-tag">Phần 3 / 4</span>
  </div>
  <div class="sky-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="sky-theory-box">
      <div class="sky-theory-head">3. HAI TÍNH CHẤT CHIA HẾT TRỌNG TÂM</div>
      <div class="sky-theory-grid">
        <div class="sky-mini-card">
          <div class="sky-mini-title">TÍNH CHẤT 1 (CÙNG CHIA HẾT ➔ CHIA HẾT)</div>
          Nếu <b>tất cả các số hạng</b> của một tổng đều chia hết cho cùng một số thì <b>tổng đó chia hết</b> cho số đó:<br>
          • <span class="s-tag">a ⋮ m</span> và <span class="s-tag">b ⋮ m</span> ➔ <span class="s-tag">(a + b) ⋮ m</span>.<br>
          • <i>Mở rộng cho hiệu (a ≥ b) và nhiều số hạng:</i> Nếu <span class="s-tag">a ⋮ m, b ⋮ m, c ⋮ m</span> thì <span class="s-tag">(a + b - c) ⋮ m</span>.
        </div>
        <div class="sky-mini-card">
          <div class="sky-mini-title">TÍNH CHẤT 2 (MỘT SỐ KHÔNG CHIA HẾT ➔ KHÔNG CHIA HẾT)</div>
          Nếu <b>chỉ có duy nhất một số hạng</b> của tổng không chia hết cho một số, còn các số hạng khác đều chia hết thì <b>tổng đó KHÔNG chia hết</b>:<br>
          • <span class="s-tag">a ⋮ m</span> và <span class="s-tag">b ∤ m</span> ➔ <span class="s-tag">(a + b) ∤ m</span>.<br>
          • <i>Mở rộng:</i> <span class="s-tag">a ⋮ m, b ⋮ m</span> nhưng <span class="s-tag">c ∤ m</span> ➔ <span class="s-tag">(a + b + c) ∤ m</span>.
        </div>
      </div>
      <div class="sky-danger-strip">
        <b>CẢNH BÁO "BẪY" TOÁN HỌC THƯỜNG GẶP NHẤT:</b><br>
        Tính chất 2 chỉ đúng khi có <b>DUY NHẤT MỘT</b> số hạng không chia hết. Nếu trong tổng có <b>từ HAI số hạng trở lên không chia hết</b> cho <i>m</i>, ta <b>TUYỆT ĐỐI KHÔNG ĐƯỢC</b> vội kết luận tổng không chia hết, mà phải <b>nhóm các số không chia hết lại với nhau</b>!<br>
        • <i>Ví dụ:</i> Xét <span class="s-tag">S = 16 + 13 + 7</span> với số chia <span class="s-tag">4</span>. Tuy <span class="s-tag">13 ∤ 4</span> và <span class="s-tag">7 ∤ 4</span>, nhưng khi nhóm <span class="s-tag">(13 + 7) = 20 ⋮ 4</span>, kết hợp với <span class="s-tag">16 ⋮ 4</span> nên tổng <span class="s-tag">(16 + 13 + 7) ⋮ 4</span>!
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ 3 -->
    <div class="sky-quest-box">
      <div class="sky-quest-title">TRẠM KHÁM PHÁ 3: PHÂN LOẠI NHANH BIỂU THỨC TRONG 3 GIÂY (+15 ĐIỂM)</div>
      <p><b>Nhiệm vụ:</b> Không cần tính tổng, hãy bấm chọn khẳng định <b>Chia hết</b> hoặc <b>Không chia hết</b> cho mỗi biểu thức dưới đây:</p>

      <div class="sort-item" id="sbox-1">
        <div class="sort-expr">1) Biểu thức A = 48 + 12 - 36 (Xét với số 6)</div>
        <div class="sort-btns">
          <button class="s-btn" onclick="sortCheck(1, this, true, 'Chính xác (+5 Điểm)! Vì 48 ⋮ 6, 12 ⋮ 6 và 36 ⋮ 6 nên theo Tính chất 1 mở rộng, A ⋮ 6.')">Chia hết (⋮ 6)</button>
          <button class="s-btn" onclick="sortCheck(1, this, false, 'Nhầm rồi! Cả 3 số 48, 12, 36 đều chia hết cho 6 nên biểu thức A phải chia hết cho 6.')">Không chia hết (∤ 6)</button>
        </div>
        <div class="sort-fb" id="sfb-1"></div>
      </div>

      <div class="sort-item" id="sbox-2">
        <div class="sort-expr">2) Biểu thức B = 80 + 16 + 28 (Xét với số 8)</div>
        <div class="sort-btns">
          <button class="s-btn" onclick="sortCheck(2, this, false, 'Sai rồi! Có 80 ⋮ 8 và 16 ⋮ 8, nhưng duy nhất số 28 ∤ 8 (dư 4) nên B không chia hết cho 8.')">Chia hết (⋮ 8)</button>
          <button class="s-btn" onclick="sortCheck(2, this, true, 'Chính xác (+5 Điểm)! Vì 80 ⋮ 8, 16 ⋮ 8 nhưng chỉ có duy nhất 28 ∤ 8 nên theo Tính chất 2, B ∤ 8.')">Không chia hết (∤ 8)</button>
        </div>
        <div class="sort-fb" id="sfb-2"></div>
      </div>

      <div class="sort-item" id="sbox-3" style="margin-bottom:0;">
        <div class="sort-expr">3) Biểu thức P = 64 + 32 + 19 + 5 (Xét với số 8)</div>
        <div class="sort-btns">
          <button class="s-btn" onclick="sortCheck(3, this, true, 'ĐỈNH CAO (+5 Điểm)! Bạn đã vượt qua bẫy! Nhóm hai số không chia hết lại: (19 + 5) = 24 ⋮ 8. Do đó P ⋮ 8!')">Chia hết (⋮ 8)</button>
          <button class="s-btn" onclick="sortCheck(3, this, false, 'Mắc bẫy rồi! Có tới 2 số không chia hết cho 8 là 19 và 5. Khi nhóm (19 + 5) = 24 lại chia hết cho 8 đấy!')">Không chia hết (∤ 8)</button>
        </div>
        <div class="sort-fb" id="sfb-3"></div>
      </div>

    </div>

  </div>
</div>

<!-- NỘI DUNG 4: ĐẤU TRƯỜNG TRÍ TUỆ & BÀI TOÁN THỰC TIỄN -->
<div class="sky-card">
  <div class="sky-card-head">
    <span>NỘI DUNG 4: ĐẤU TRƯỜNG NỐI CẶP, TRẮC NGHIỆM & TOÁN THỰC TẾ</span>
    <span class="sky-step-tag">Phần 4 / 4</span>
  </div>
  <div class="sky-card-body">

    <!-- VÒNG 1: TRÒ CHƠI NỐI CẶP (20 ĐIỂM) -->
    <div class="sky-quest-box" style="margin-bottom:20px;">
      <div class="sky-quest-title">VÒNG 1: GHÉP NỐI TỐC ĐỘ (20 ĐIỂM — 5 Điểm / Cặp)</div>
      <p><b>Cách chơi:</b> Nhấn chọn một biểu thức hoặc tập hợp ở <b>CỘT A</b>, sau đó nhấn chọn kết quả tương ứng ở <b>CỘT B</b> để nối chúng lại với nhau.</p>

      <div class="match-grid">
        <div>
          <div class="match-head">CỘT A: MỆNH ĐỀ / TẬP HỢP</div>
          <div class="m-card" data-a="1" onclick="selA(this)">
            <span>1. Tập hợp các ước của 12: Ư(12)</span>
            <span class="m-badge" id="bA-1"></span>
          </div>
          <div class="m-card" data-a="2" onclick="selA(this)">
            <span>2. Tập hợp B(9) nhỏ hơn 30</span>
            <span class="m-badge" id="bA-2"></span>
          </div>
          <div class="m-card" data-a="3" onclick="selA(this)">
            <span>3. Tổng (219 . 7 + 8)</span>
            <span class="m-badge" id="bA-3"></span>
          </div>
          <div class="m-card" data-a="4" onclick="selA(this)">
            <span>4. Tổng (8 . 12 + 9)</span>
            <span class="m-badge" id="bA-4"></span>
          </div>
        </div>

        <div>
          <div class="match-head">CỘT B: KẾT QUẢ TƯƠNG ỨNG</div>
          <div class="m-card" data-b="3" onclick="selB(this)">
            <span>a) Không chia hết cho 7 (vì 8 ∤ 7)</span>
            <span class="m-badge" id="bB-3"></span>
          </div>
          <div class="m-card" data-b="1" onclick="selB(this)">
            <span>b) {1; 2; 3; 4; 6; 12}</span>
            <span class="m-badge" id="bB-1"></span>
          </div>
          <div class="m-card" data-b="4" onclick="selB(this)">
            <span>c) Chia hết cho 3 (vì 12 ⋮ 3 và 9 ⋮ 3)</span>
            <span class="m-badge" id="bB-4"></span>
          </div>
          <div class="m-card" data-b="2" onclick="selB(this)">
            <span>d) {0; 9; 18; 27}</span>
            <span class="m-badge" id="bB-2"></span>
          </div>
        </div>
      </div>

      <div id="matchMsg" style="margin-top:8px; font-weight:800; color:#0369a1;"></div>
      <button class="sky-btn" style="margin-top:8px;" onclick="resetMatching()">Chơi lại Vòng 1</button>
    </div>

    <!-- VÒNG 2: TRẮC NGHIỆM PHẢN XẠ (30 ĐIỂM) -->
    <div class="sky-quest-box" style="margin-bottom:20px;">
      <div class="sky-quest-title">VÒNG 2: TĂNG TỐC SUY LUẬN (30 ĐIỂM — 10 Điểm / Câu)</div>

      <div class="q-card" id="qc-1">
        <div class="q-title">Câu 1: Khẳng định nào dưới đây sử dụng SAI kí hiệu toán học?</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Chưa đúng! Vì 42 = 6 . 7 nên 42 ⋮ 6 là một khẳng định ĐÚNG. Hãy tìm câu sai nhé!')">A. 42 ⋮ 6</button>
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Chưa đúng! Vì 25 chia hết cho 5 nên 5 ∈ Ư(25) là một khẳng định ĐÚNG.')">B. 5 ∈ Ư(25)</button>
          <button class="q-btn" onclick="ansQuiz(1, this, true, 'CHÍNH XÁC (+10 Điểm)! Khẳng định này SAI vì không có phép chia cho 0, do đó số 0 không bao giờ là ước của bất kì số tự nhiên nào!')">C. 0 ∈ Ư(15)</button>
        </div>
        <div class="q-exp" id="qexp-1"></div>
      </div>

      <div class="q-card" id="qc-2">
        <div class="q-title">Câu 2: Tập hợp tất cả các số tự nhiên y thỏa mãn y ∈ Ư(50) và y &gt; 5 là:</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Bị lừa rồi! Đề bài yêu cầu y > 5 (lớn hơn hẳn 5) nên không được lấy số 5 vào tập hợp nhé!')">A. {5; 10; 25; 50}</button>
          <button class="q-btn" onclick="ansQuiz(2, this, true, 'XUẤT SẮC (+10 Điểm)! Ta có Ư(50) = {1; 2; 5; 10; 25; 50}. Lọc các phần tử lớn hơn 5 ta được {10; 25; 50}.')">B. {10; 25; 50}</button>
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Sai rồi! Số 20 không phải là ước của 50 vì 50 chia 20 được 2 dư 10.')">C. {10; 20; 25; 50}</button>
        </div>
        <div class="q-exp" id="qexp-2"></div>
      </div>

      <div class="q-card" id="qc-3" style="margin-bottom:0;">
        <div class="q-title">Câu 3: Cho tổng S = 35 + x. Tìm giá trị của x thuộc tập hợp {7; 14; 18; 21} để S ∤ 7 (S không chia hết cho 7):</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(3, this, false, 'Đọc kĩ đề nhé! Đề yêu cầu tìm x để S KHÔNG chia hết cho 7. Với x ∈ {7; 14; 21} thì S chia hết cho 7 mất rồi!')">A. x ∈ {7; 14; 21}</button>
          <button class="q-btn" onclick="ansQuiz(3, this, true, 'CHÍNH XÁC TUYỆT ĐỐI (+10 Điểm)! Vì 35 ⋮ 7 nên để (35 + x) ∤ 7 thì x phải không chia hết cho 7. Chỉ có 18 ∤ 7.')">B. x = 18</button>
          <button class="q-btn" onclick="ansQuiz(3, this, false, 'Sai rồi! Số 14 chia hết cho 7 nên 35 + 14 chia hết cho 7.')">C. x = 14</button>
        </div>
        <div class="q-exp" id="qexp-3"></div>
      </div>
    </div>

    <!-- VÒNG 3: BÀI TOÁN TỰ LUẬN & THỰC TIỄN -->
    <div class="sky-quest-box" style="margin-bottom:0;">
      <div class="sky-quest-title">VÒNG 3: CHINH PHỤC TOÁN THỰC TIỄN & NÂNG CAO (LÀM VÀO VỞ)</div>
      <ul>
        <li><b>Bài toán 1 (Bài toán gói kẹo thực tiễn):</b> Nhân dịp sinh nhật, mẹ chuẩn bị cho Việt <b>12 gói kẹo</b>, mỗi gói có <b>35 cái kẹo</b>. Việt lấy ra <b>2 gói kẹo</b> cất đi. Không tính tổng số kẹo, hãy giải thích vì sao số kẹo còn lại hoàn toàn chia đều được cho <b>5 bạn</b>?</li>
        <li><b>Bài toán 2 (Chia nhóm dự án - SGK trang 33):</b> Một lớp học có <b>40 học sinh</b>. Cô giáo muốn chia lớp thành các nhóm có số người như nhau để làm dự án. Biết mỗi nhóm phải có <b>nhiều hơn 3 người</b> và <b>ít hơn 15 người</b>. Hỏi mỗi nhóm có thể có bao nhiêu học sinh?</li>
        <li><b>Bài toán 3 (Thử thách nâng cao):</b> Tìm tất cả các số tự nhiên <i>n</i> sao cho <span class="s-tag">(n + 8) ⋮ (n + 3)</span>.</li>
      </ul>

      <details class="sky-details" onclick="sfxClick()">
        <summary>[ NHẤN ĐỂ MỞ KHÓA LỜI GIẢI TRÌNH BÀY MẪU VÒNG 3 ]</summary>
        <div class="sky-details-body">
          <p><b>Lời giải Bài toán 1:</b></p>
          <ul>
            <li>Tổng số kẹo ban đầu là <span class="s-tag">12 . 35</span>. Vì <span class="s-tag">35 ⋮ 5</span> nên tích <span class="s-tag">(12 . 35) ⋮ 5</span>.</li>
            <li>Số kẹo Việt cất đi là <span class="s-tag">2 . 35</span>. Vì <span class="s-tag">35 ⋮ 5</span> nên tích <span class="s-tag">(2 . 35) ⋮ 5</span>.</li>
            <li>Số kẹo còn lại là hiệu <span class="s-tag">(12 . 35) - (2 . 35)</span>. Theo Tính chất 1 mở rộng, hiệu này <b>chia hết cho 5</b> nên chia đều được cho 5 bạn!</li>
          </ul>
          <hr style="margin:12px 0; border:0; border-top:1px solid #bae6fd;">
          <p><b>Lời giải Bài toán 2:</b></p>
          <ul>
            <li>Gọi số học sinh trong mỗi nhóm là <i>x</i> (điều kiện: <span class="s-tag">x ∈ ℕ*</span> và <span class="s-tag">3 &lt; x &lt; 15</span>).</li>
            <li>Vì 40 học sinh chia đều vào các nhóm nên <span class="s-tag">40 ⋮ x</span>, suy ra <span class="s-tag">x ∈ Ư(40) = {1; 2; 4; 5; 8; 10; 20; 40}</span>.</li>
            <li>Kết hợp điều kiện <span class="s-tag">3 &lt; x &lt; 15</span>, ta tìm được 4 phương án cho số học sinh mỗi nhóm là: <span class="s-tag">x ∈ {4; 5; 8; 10}</span> (tương ứng với 10 nhóm, 8 nhóm, 5 nhóm hoặc 4 nhóm).</li>
          </ul>
          <hr style="margin:12px 0; border:0; border-top:1px solid #bae6fd;">
          <p><b>Lời giải Bài toán 3 (Nâng cao):</b></p>
          <ul>
            <li>Tách số bị chia: <span class="s-tag">n + 8 = (n + 3) + 5</span>.</li>
            <li>Vì <span class="s-tag">(n + 3) ⋮ (n + 3)</span> nên để tổng <span class="s-tag">[(n + 3) + 5] ⋮ (n + 3)</span> thì <span class="s-tag">5 ⋮ (n + 3)</span> hay <span class="s-tag">(n + 3) ∈ Ư(5) = {1; 5}</span>.</li>
            <li>Do <span class="s-tag">n ≥ 0</span> nên <span class="s-tag">n + 3 ≥ 3</span> ➔ Chọn <span class="s-tag">n + 3 = 5</span>, suy ra <span class="s-tag">n = 2</span>.</li>
          </ul>
        </div>
      </details>
    </div>

  </div>
</div>

<!-- BẢNG TÓM TẮT CỐT LÕI BÀI 8 -->
<div class="sky-card" style="margin-bottom:0;">
  <div class="sky-card-head">
    <span>SƠ ĐỒ TỔNG KẾT KIẾN THỨC CỐT LÕI BÀI 8</span>
    <span class="sky-step-tag">Ôn tập nhanh</span>
  </div>
  <div class="sky-card-body">
    <table class="sky-table">
      <thead>
        <tr>
          <th width="50%">NHÁNH 1: KHÁI NIỆM ƯỚC & BỘI (<span class="s-tag">a = b . k ➔ a ⋮ b</span>)</th>
          <th width="50%">NHÁNH 2: TÍNH CHẤT CHIA HẾT CỦA TỔNG & HIỆU</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>
            • <b><i>a</i> là BỘI của <i>b</i></b> — Kí hiệu: <span class="s-tag">B(b)</span><br>
            ➔ <i>Cách tìm:</i> Nhân <i>b</i> lần lượt với <span class="s-tag">0, 1, 2, 3, ...</span> (Tập hợp vô hạn).<br><br>
            • <b><i>b</i> là ƯỚC của <i>a</i></b> — Kí hiệu: <span class="s-tag">Ư(a)</span><br>
            ➔ <i>Cách tìm:</i> Chia <i>a</i> lần lượt cho <span class="s-tag">1, 2, ..., a</span> hoặc ghép cặp nhân đối xứng (Tập hợp hữu hạn).
          </td>
          <td>
            • <b>Tính chất 1 (Cùng chia hết):</b><br>
            Nếu <span class="s-tag">a ⋮ m</span> và <span class="s-tag">b ⋮ m</span> thì <span class="s-tag">(a + b) ⋮ m</span> và <span class="s-tag">(a - b) ⋮ m</span>.<br><br>
            • <b>Tính chất 2 (Duy nhất 1 số không chia hết):</b><br>
            Nếu <span class="s-tag">a ⋮ m</span> và <span class="s-tag">b ∤ m</span> thì <span class="s-tag">(a + b) ∤ m</span> và <span class="s-tag">(a - b) ∤ m</span>.<br>
            <i>(Lưu ý: Có từ 2 số hạng không chia hết trở lên thì phải nhóm lại, không dùng Tính chất 2).</i>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<script>
  // HỆ THỐNG ÂM THANH TỰ ĐỘNG (WEB AUDIO API)
  let soundOn = true;
  const AudioCtx = window.AudioContext || window.webkitAudioContext;
  let actx = null;

  function initAudio() {
    if (!actx) actx = new AudioCtx();
    if (actx.state === 'suspended') actx.resume();
  }

  function playNote(freq, type, dur, delay = 0) {
    if (!soundOn) return;
    initAudio();
    setTimeout(() => {
      const osc = actx.createOscillator();
      const gain = actx.createGain();
      osc.type = type;
      osc.frequency.setValueAtTime(freq, actx.currentTime);
      gain.gain.setValueAtTime(0.18, actx.currentTime);
      gain.gain.exponentialRampToValueAtTime(0.001, actx.currentTime + dur);
      osc.connect(gain);
      gain.connect(actx.destination);
      osc.start();
      osc.stop(actx.currentTime + dur);
    }, delay);
  }

  function sfxClick() { playNote(560, 'sine', 0.07); }
  function sfxOk() { playNote(587.33, 'triangle', 0.13, 0); playNote(880, 'triangle', 0.26, 110); }
  function sfxErr() { playNote(210, 'sawtooth', 0.15, 0); playNote(165, 'sawtooth', 0.22, 130); }
  function sfxWin() {
    playNote(523.25, 'triangle', 0.13, 0);
    playNote(659.25, 'triangle', 0.13, 120);
    playNote(783.99, 'triangle', 0.13, 240);
    playNote(1046.50, 'triangle', 0.38, 360);
  }

  function toggleSound() {
    soundOn = !soundOn;
    document.getElementById('btnSound').textContent = soundOn ? 'Âm thanh: ĐANG BẬT' : 'Âm thanh: ĐÃ TẮT';
    if (soundOn) sfxClick();
  }

  // ĐIỂM SỐ (TỔNG 100 ĐIỂM)
  let totalPts = 0;
  function addScore(val) {
    totalPts += val;
    document.getElementById('ptsVal').textContent = totalPts;
    if (totalPts === 100) setTimeout(sfxWin, 300);
  }

  // LOGIC TRẠM 1: SĂN TẬP HỢP Ư(18) (15 ĐIỂM)
  let foundU18 = 0;
  let doneU18 = false;
  function pickU18(el, isRight, msg) {
    if (el.classList.contains('correct') || el.classList.contains('wrong') || doneU18) return;
    const box = document.getElementById('msgU18');
    box.textContent = msg;
    if (isRight) {
      sfxOk();
      el.classList.add('correct');
      box.style.color = '#0369a1';
      foundU18++;
      if (foundU18 === 6) {
        doneU18 = true;
        addScore(15);
        box.textContent = 'HOÀN HẢO (+15 Điểm)! Bạn đã tìm đủ 6 ước của 18: Ư(18) = {1; 2; 3; 6; 9; 18}.';
      }
    } else {
      sfxErr();
      el.classList.add('wrong');
      box.style.color = '#9f1239';
    }
  }

  // LOGIC TRẠM 2: PHÒNG THÍ NGHIỆM ƯỚC & BỘI (20 ĐIỂM)
  const labDone = {};
  function checkLab(id, expected, okMsg) {
    if (labDone[id]) return;
    const val = parseInt(document.getElementById('inpLab' + id).value, 10);
    const fb = document.getElementById('msgLab' + id);
    if (val === expected) {
      sfxOk();
      fb.style.color = '#166534';
      fb.textContent = okMsg + ' (+10 Điểm)';
      labDone[id] = true;
      addScore(10);
    } else {
      sfxErr();
      fb.style.color = '#9f1239';
      fb.textContent = 'Chưa chính xác, hãy kiểm tra lại phép nhân nhé!';
    }
  }

  // LOGIC TRẠM 3: PHÂN LOẠI NHANH BIỂU THỨC (15 ĐIỂM — 3 CÂU x 5 ĐIỂM)
  const sortLocked = {};
  function sortCheck(id, btn, isOk, msg) {
    if (sortLocked[id]) return;
    const fb = document.getElementById('sfb-' + id);
    fb.style.display = 'block';
    fb.textContent = msg;
    if (isOk) {
      sfxOk();
      btn.classList.add('ok');
      fb.style.background = '#dcfce7';
      fb.style.color = '#166534';
      fb.style.border = '1px solid #16a34a';
      sortLocked[id] = true;
      addScore(5);
      document.querySelectorAll('#sbox-' + id + ' .s-btn').forEach(b => b.disabled = true);
    } else {
      sfxErr();
      btn.classList.add('err');
      fb.style.background = '#ffe4e6';
      fb.style.color = '#9f1239';
      fb.style.border = '1px solid #e11d48';
    }
  }

  // LOGIC VÒNG 1: NỐI CẶP (20 ĐIỂM — 4 CẶP x 5 ĐIỂM)
  let currA = null;
  let pairsCount = 0;
  function selA(el) {
    if (el.classList.contains('matched')) return;
    sfxClick();
    document.querySelectorAll('[data-a]').forEach(x => x.classList.remove('selected'));
    el.classList.add('selected');
    currA = el;
  }

  function selB(el) {
    if (el.classList.contains('matched') || !currA) return;
    const aId = currA.getAttribute('data-a');
    const bId = el.getAttribute('data-b');
    if (aId === bId) {
      sfxOk();
      currA.classList.remove('selected');
      currA.classList.add('matched');
      el.classList.add('matched');
      document.getElementById('bA-' + aId).textContent = 'Cặp #' + aId;
      document.getElementById('bB-' + bId).textContent = 'Cặp #' + aId;
      currA = null;
      pairsCount++;
      addScore(5);
      if (pairsCount === 4) {
        document.getElementById('matchMsg').textContent = 'Hoàn thành xuất sắc cả 4 cặp ghép nối (+20 Điểm)!';
        sfxWin();
      }
    } else {
      sfxErr();
      const tmp = currA;
      tmp.classList.add('wrong');
      el.classList.add('wrong');
      setTimeout(() => {
        tmp.classList.remove('wrong', 'selected');
        el.classList.remove('wrong');
      }, 450);
      currA = null;
    }
  }

  function resetMatching() {
    sfxClick();
    addScore(-(pairsCount * 5));
    pairsCount = 0;
    currA = null;
    document.getElementById('matchMsg').textContent = '';
    document.querySelectorAll('.m-card').forEach(x => x.classList.remove('matched', 'selected', 'wrong'));
  }

  // LOGIC VÒNG 2: TRẮC NGHIỆM (30 ĐIỂM — 3 CÂU x 10 ĐIỂM)
  const quizLocked = {};
  function ansQuiz(id, btn, isOk, msg) {
    if (quizLocked[id]) return;
    const exp = document.getElementById('qexp-' + id);
    exp.style.display = 'block';
    exp.textContent = msg;
    if (isOk) {
      sfxOk();
      btn.classList.add('ok');
      exp.style.background = '#dcfce7';
      exp.style.color = '#166534';
      exp.style.border = '1.5px solid #16a34a';
      quizLocked[id] = true;
      addScore(10);
      document.querySelectorAll('#qc-' + id + ' .q-btn').forEach(b => b.disabled = true);
    } else {
      sfxErr();
      btn.classList.add('err');
      exp.style.background = '#ffe4e6';
      exp.style.color = '#9f1239';
      exp.style.border = '1.5px solid #e11d48';
    }
  }
</script>
