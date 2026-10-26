<style>
  /* Ẩn tiêu đề mặc định của GitHub Pages & Thiết lập nền Tím Lavender Nhạt */
  .markdown-body > h1:first-child { display: none !important; }
  .container-lg, .markdown-body { max-width: 980px !important; margin: 0 auto !important; padding: 16px !important; font-family: 'Segoe UI', system-ui, -apple-system, sans-serif !important; color: #2e1065 !important; background-color: #f5f3ff !important; }
  body { background-color: #f5f3ff !important; }

  /* Thanh điều khiển cố định (Sticky Bar) */
  .vio-topbar { position: sticky; top: 10px; z-index: 999; background: #ffffff; border: 2px solid #8b5cf6; border-radius: 12px; padding: 10px 20px; margin-bottom: 24px; display: flex; justify-content: space-between; align-items: center; box-shadow: 0 8px 20px rgba(124, 58, 237, 0.14); flex-wrap: wrap; gap: 10px; }
  .vio-topbar-title { font-weight: 800; color: #4c1d95; font-size: 0.98rem; letter-spacing: 0.3px; }
  .vio-topbar-right { display: flex; align-items: center; gap: 12px; }
  .vio-score-badge { background: #ede9fe; color: #6d28d9; border: 1.5px solid #8b5cf6; padding: 5px 16px; border-radius: 99px; font-weight: 800; font-size: 0.95rem; }
  .vio-sound-btn { background: #7c3aed; color: #ffffff; border: none; padding: 7px 15px; border-radius: 8px; font-weight: 700; cursor: pointer; font-size: 0.88rem; transition: 0.2s; }
  .vio-sound-btn:hover { background: #6d28d9; }

  /* Khung Banner chính */
  .vio-hero { background: linear-gradient(135deg, #ede9fe 0%, #ddd6fe 100%); border: 2px solid #8b5cf6; border-radius: 16px; padding: 30px 24px; text-align: center; margin-bottom: 26px; box-shadow: 0 8px 22px rgba(124, 58, 237, 0.1); }
  .vio-hero-tag { display: inline-block; background: #7c3aed; color: #ffffff; font-weight: 800; font-size: 0.82rem; padding: 5px 16px; border-radius: 99px; text-transform: uppercase; letter-spacing: 0.7px; margin-bottom: 10px; }
  .vio-hero-title { color: #3b0764 !important; font-size: 1.95rem !important; font-weight: 800 !important; margin: 0 0 14px 0 !important; border: none !important; padding: 0 !important; }
  .vio-meta-row { display: flex; justify-content: center; flex-wrap: wrap; gap: 10px; }
  .vio-meta-item { background: #ffffff; border: 1px solid #c4b5fd; color: #5b21b6; padding: 5px 14px; border-radius: 8px; font-size: 0.9rem; font-weight: 600; }

  /* Hệ thống Khung bài giảng (Section Frames) */
  .vio-card { background: #ffffff; border: 2px solid #ddd6fe; border-radius: 16px; margin-bottom: 28px; overflow: hidden; box-shadow: 0 5px 15px rgba(124, 58, 237, 0.06); }
  .vio-card-head { background: linear-gradient(90deg, #ede9fe 0%, #ddd6fe 100%); border-bottom: 2px solid #c4b5fd; padding: 14px 22px; color: #3b0764; font-size: 1.18rem; font-weight: 800; display: flex; justify-content: space-between; align-items: center; }
  .vio-step-tag { background: #7c3aed; color: #fff; font-size: 0.78rem; padding: 3px 12px; border-radius: 12px; font-weight: 700; }
  .vio-card-body { padding: 24px; line-height: 1.7; font-size: 1rem; }

  /* Khung Lý thuyết cô đọng (Đặt trước Trạm khám phá) */
  .vio-theory-box { background: #f5f3ff; border: 1.5px solid #c4b5fd; border-left: 6px solid #7c3aed; border-radius: 12px; padding: 18px 20px; margin-bottom: 20px; }
  .vio-theory-head { font-weight: 800; color: #5b21b6; font-size: 1.05rem; margin-bottom: 12px; text-transform: uppercase; letter-spacing: 0.3px; border-bottom: 1.5px solid #ddd6fe; padding-bottom: 6px; }
  .vio-theory-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 14px; margin-top: 10px; }
  .vio-mini-card { background: #ffffff; border: 1px solid #ddd6fe; border-radius: 10px; padding: 14px 16px; }
  .vio-mini-title { font-weight: 800; color: #6d28d9; margin-bottom: 6px; font-size: 0.98rem; }
  .vio-tip-strip { background: #fef9c3; border: 1px solid #fde047; border-left: 5px solid #eab308; border-radius: 8px; padding: 12px 16px; margin-top: 14px; color: #713f12; font-size: 0.95rem; }

  /* Bảng quy trình 3 bước */
  .step-table { width: 100%; border-collapse: collapse; margin: 12px 0; border-radius: 10px; overflow: hidden; border: 1.5px solid #c4b5fd; }
  .step-table th { background: #7c3aed !important; color: #ffffff !important; padding: 11px 15px !important; text-align: left; font-weight: 800; border: 1px solid #6d28d9 !important; }
  .step-table td { padding: 11px 15px !important; border: 1px solid #ddd6fe !important; background: #ffffff !important; color: #2e1065 !important; vertical-align: top; }
  .step-table tr:nth-child(even) td { background: #faf5ff !important; }

  /* Khung Trạm khám phá tương tác */
  .vio-quest-box { background: #faf5ff; border: 2px dashed #8b5cf6; border-radius: 12px; padding: 18px 20px; margin-bottom: 10px; }
  .vio-quest-title { font-weight: 800; color: #6d28d9; margin-bottom: 10px; font-size: 1.03rem; text-transform: uppercase; }

  /* Nút chọn số (Number Chips) */
  .chip-grid { display: flex; flex-wrap: wrap; gap: 10px; margin: 12px 0; }
  .num-chip { background: #ffffff; border: 2px solid #c4b5fd; color: #3b0764; padding: 9px 16px; border-radius: 10px; font-weight: 800; font-size: 1rem; cursor: pointer; transition: 0.2s; user-select: none; text-align: center; min-width: 64px; }
  .num-chip:hover { background: #ede9fe; border-color: #7c3aed; transform: translateY(-2px); }
  .num-chip.correct { background: #7c3aed; border-color: #4c1d95; color: #ffffff; }
  .num-chip.wrong { background: #ffe4e6; border-color: #e11d48; color: #9f1239; text-decoration: line-through; opacity: 0.75; }

  /* Phòng thí nghiệm nhập số tương tác */
  .lab-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(270px, 1fr)); gap: 16px; margin: 14px 0; }
  .lab-box { background: #ffffff; border: 1.5px solid #ddd6fe; border-radius: 12px; padding: 16px; }
  .lab-row-inp { display: flex; align-items: center; gap: 8px; margin-top: 10px; flex-wrap: wrap; }
  .vio-input { width: 76px; padding: 6px 8px; border: 2px solid #8b5cf6; border-radius: 8px; font-weight: 800; text-align: center; font-size: 0.98rem; color: #3b0764; background: #f5f3ff; outline: none; }
  .vio-input:focus { border-color: #5b21b6; background: #ffffff; }
  .vio-btn { background: #7c3aed; color: #ffffff; border: none; padding: 8px 16px; border-radius: 8px; font-weight: 700; cursor: pointer; transition: 0.2s; }
  .vio-btn:hover { background: #5b21b6; }
  .lab-msg { font-size: 0.92rem; font-weight: 700; margin-top: 8px; min-height: 22px; }

  /* Phân số trực quan */
  .frac-wrap { display: inline-flex; flex-direction: column; align-items: center; vertical-align: middle; margin: 0 6px; font-weight: 800; }
  .frac-top { border-bottom: 2px solid #3b0764; padding: 0 6px; }
  .frac-bot { padding: 0 6px; }

  .v-tag { background: #ffffff; color: #6d28d9; border: 1px solid #a78bfa; padding: 1px 8px; border-radius: 6px; font-family: 'Consolas', monospace; font-weight: 800; font-size: 0.95em; display: inline-block; }

  /* Trò chơi Nối cặp (Matching Game) */
  .match-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; margin-top: 14px; }
  .match-head { background: #7c3aed; color: #ffffff; text-align: center; padding: 9px; border-radius: 8px; font-weight: 800; margin-bottom: 10px; }
  .m-card { background: #ffffff; border: 2px solid #c4b5fd; border-radius: 10px; padding: 13px 15px; margin-bottom: 10px; font-weight: 700; color: #3b0764; cursor: pointer; transition: 0.2s; display: flex; justify-content: space-between; align-items: center; user-select: none; }
  .m-card:hover:not(.matched) { background: #ede9fe; border-color: #7c3aed; transform: translateY(-2px); }
  .m-card.selected { background: #7c3aed; color: #ffffff; border-color: #3b0764; box-shadow: 0 0 0 4px rgba(124, 58, 237, 0.25); }
  .m-card.matched { background: #dcfce7; border-color: #16a34a; color: #166534; cursor: default; }
  .m-card.wrong { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .m-badge { font-size: 0.78rem; background: #16a34a; color: #fff; padding: 2px 8px; border-radius: 10px; display: none; }
  .m-card.matched .m-badge { display: inline-block; }

  /* Trắc nghiệm tốc độ */
  .q-card { background: #ffffff; border: 1.5px solid #c4b5fd; border-radius: 12px; padding: 16px; margin-bottom: 14px; }
  .q-title { font-weight: 800; color: #3b0764; margin-bottom: 10px; }
  .q-opts { display: grid; grid-template-columns: repeat(auto-fit, minmax(210px, 1fr)); gap: 10px; }
  .q-btn { background: #f5f3ff; border: 2px solid #ddd6fe; padding: 10px 14px; border-radius: 8px; font-weight: 700; color: #2e1065; cursor: pointer; text-align: left; transition: 0.2s; }
  .q-btn:hover:not(:disabled) { background: #ede9fe; border-color: #7c3aed; }
  .q-btn.ok { background: #dcfce7; border-color: #16a34a; color: #166534; }
  .q-btn.err { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .q-exp { display: none; margin-top: 10px; padding: 10px 14px; border-radius: 8px; font-weight: 600; font-size: 0.92rem; }

  /* Nút mở lời giải tự luận */
  details.vio-details { background: #ffffff; border: 2px solid #7c3aed; border-radius: 10px; margin-top: 14px; overflow: hidden; }
  details.vio-details summary { background: #ede9fe; color: #3b0764; padding: 12px 18px; font-weight: 800; cursor: pointer; list-style: none; user-select: none; transition: 0.2s; }
  details.vio-details summary:hover { background: #ddd6fe; }
  .vio-details-body { padding: 18px; border-top: 1.5px solid #ddd6fe; background: #ffffff; }

  @media (max-width: 680px) {
    .match-grid { grid-template-columns: 1fr; }
  }
</style>

<!-- THANH ĐIỀU KHIỂN CỐ ĐỊNH -->
<div class="vio-topbar">
  <div class="vio-topbar-title">TOÁN 6 — BÀI 11: ƯỚC CHUNG. ƯỚC CHUNG LỚN NHẤT</div>
  <div class="vio-topbar-right">
    <div class="vio-score-badge">ĐIỂM KHÁM PHÁ: <span id="ptsVal">0</span> / 100</div>
    <button class="vio-sound-btn" id="btnSound" onclick="toggleSound()">Âm thanh: ĐANG BẬT</button>
  </div>
</div>

<!-- BANNER MỞ ĐẦU -->
<div class="vio-hero">
  <div class="vio-hero-tag">CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN</div>
  <h1 class="vio-hero-title">BÀI 11: ƯỚC CHUNG. ƯỚC CHUNG LỚN NHẤT</h1>
  <div class="vio-meta-row">
    <div class="vio-meta-item">Toán 6 (Tập 1) — Kết nối tri thức với cuộc sống</div>
    <div class="vio-meta-item">Thời lượng: 60 phút (Lý thuyết chuyên sâu + Tương tác + Thực tiễn)</div>
  </div>
</div>

<!-- NỘI DUNG 1: ƯỚC CHUNG VÀ ƯỚC CHUNG LỚN NHẤT -->
<div class="vio-card">
  <div class="vio-card-head">
    <span>NỘI DUNG 1: ƯỚC CHUNG VÀ ƯỚC CHUNG LỚN NHẤT</span>
    <span class="vio-step-tag">Phần 1 / 4</span>
  </div>
  <div class="vio-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="vio-theory-box">
      <div class="vio-theory-head">1. LÝ THUYẾT CỐT LÕI CẦN NHỚ</div>
      <div class="vio-theory-grid">
        <div class="vio-mini-card">
          <div class="vio-mini-title">ƯỚC CHUNG (ƯC)</div>
          • <b>Định nghĩa:</b> Ước chung của hai hay nhiều số là <b>ước của tất cả</b> các số đó.<br>
          • <b>Kí hiệu:</b> Tập hợp các ước chung của <i>a</i> và <i>b</i> là <span class="v-tag">ƯC(a, b)</span>.<br>
          • <b>Điều kiện:</b> <span class="v-tag">x ∈ ƯC(a, b)</span> khi cả <span class="v-tag">a ⋮ x</span> và <span class="v-tag">b ⋮ x</span>.
        </div>
        <div class="vio-mini-card">
          <div class="vio-mini-title">ƯỚC CHUNG LỚN NHẤT (ƯCLN)</div>
          • <b>Định nghĩa:</b> Ước chung lớn nhất của hai hay nhiều số là <b>số lớn nhất</b> trong tập hợp các ước chung của các số đó.<br>
          • <b>Kí hiệu:</b> <span class="v-tag">ƯCLN(a, b)</span>.<br>
          • <b>Ví dụ:</b> Nếu <span class="v-tag">ƯC(12, 18) = {1; 2; 3; 6}</span> thì <span class="v-tag">ƯCLN(12, 18) = 6</span>.
        </div>
      </div>
      <div class="vio-tip-strip">
        <b>Mối liên hệ vàng giữa ƯC và ƯCLN:</b><br>
        • Tất cả các <b>ước chung</b> của hai hay nhiều số đều là <b>ước của ƯCLN</b> của các số đó!<br>
        ➔ Do đó, nếu biết <span class="v-tag">ƯCLN(a, b) = d</span> thì muốn tìm <span class="v-tag">ƯC(a, b)</span>, ta chỉ cần tìm <span class="v-tag">Ư(d)</span> mà không cần liệt kê từng tập hợp ước.
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ 1 -->
    <div class="vio-quest-box">
      <div class="vio-quest-title">TRẠM KHÁM PHÁ 1: SĂN TÌM PHẦN TỬ CHUNG CỦA HAI TẬP HỢP (+15 ĐIỂM)</div>
      <p>Cho hai tập hợp ước đã được liệt kê sẵn:<br>
      • <span class="v-tag">Ư(18) = {1; 2; 3; 6; 9; 18}</span><br>
      • <span class="v-tag">Ư(30) = {1; 2; 3; 5; 6; 10; 15; 30}</span></p>
      <p><b>Nhiệm vụ:</b> Hãy <b>bấm chọn tất cả 4 số thuộc tập hợp ƯC(18, 30)</b> (các số xuất hiện ở cả hai tập hợp trên):</p>
      <div class="chip-grid" id="ucGrid">
        <div class="num-chip" onclick="pickUC(this, true, 'Chính xác! Số 1 luôn là ước chung của mọi số tự nhiên.')">Số 1</div>
        <div class="num-chip" onclick="pickUC(this, true, 'Chính xác! Cả 18 và 30 đều là số chẵn nên chia hết cho 2.')">Số 2</div>
        <div class="num-chip" onclick="pickUC(this, true, 'Chính xác! 18 ⋮ 3 và 30 ⋮ 3 nên 3 ∈ ƯC(18, 30).')">Số 3</div>
        <div class="num-chip" onclick="pickUC(this, false, 'Sai rồi! 30 ⋮ 5 nhưng 18 không chia hết cho 5.')">Số 5</div>
        <div class="num-chip" onclick="pickUC(this, true, 'Xuất sắc! 6 vừa là ước chung, vừa là ƯCLN(18, 30)!')">Số 6</div>
        <div class="num-chip" onclick="pickUC(this, false, 'Sai rồi! 18 ⋮ 9 nhưng 30 không chia hết cho 9.')">Số 9</div>
        <div class="num-chip" onclick="pickUC(this, false, 'Sai rồi! 30 ⋮ 15 nhưng 18 không chia hết cho 15.')">Số 15</div>
      </div>
      <div id="msgUC" style="font-weight:700; color:#5b21b6; font-size:0.93rem; min-height:22px;"></div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 2: CÁCH TÌM ƯỚC CHUNG LỚN NHẤT BẰNG PHÂN TÍCH THỪA SỐ NGUYÊN TỐ -->
<div class="vio-card">
  <div class="vio-card-head">
    <span>NỘI DUNG 2: QUY TẮC 3 BƯỚC TÌM ƯỚC CHUNG LỚN NHẤT</span>
    <span class="vio-step-tag">Phần 2 / 4</span>
  </div>
  <div class="vio-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="vio-theory-box">
      <div class="vio-theory-head">2. QUY TRÌNH 3 BƯỚC TÌM ƯCLN (KHI SỐ LỚN)</div>
      <p>Khi các số lớn (như 84 và 120), việc liệt kê từng ước rất dễ sót nghiệm. Ta sử dụng phương pháp <b>phân tích ra thừa số nguyên tố</b> theo bảng quy tắc 3 bước sau:</p>
      <table class="step-table">
        <thead>
          <tr>
            <th width="18%">Bước</th>
            <th width="45%">Quy tắc thực hiện</th>
            <th width="37%">Ví dụ mẫu: Tìm ƯCLN(36, 48)</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><b>Bước 1</b></td>
            <td>Phân tích mỗi số ra <b>thừa số nguyên tố</b>.</td>
            <td>• <span class="v-tag">36 = 2² . 3²</span><br>• <span class="v-tag">48 = 2⁴ . 3</span></td>
          </tr>
          <tr>
            <td><b>Bước 2</b></td>
            <td>Chọn ra các thừa số nguyên tố <b>CHUNG</b> (có mặt ở tất cả các số).</td>
            <td>Thừa số nguyên tố chung là: <span class="v-tag">2</span> và <span class="v-tag">3</span>.</td>
          </tr>
          <tr>
            <td><b>Bước 3</b></td>
            <td>Lập tích các thừa số đã chọn, mỗi thừa số lấy với <b>số mũ NHỎ NHẤT</b> của nó. Tích đó là <b>ƯCLN</b>.</td>
            <td>• Số mũ nhỏ nhất của 2 là <span class="v-tag">2²</span>; của 3 là <span class="v-tag">3¹</span>.<br>➔ <span class="v-tag">ƯCLN(36, 48) = 2² . 3 = 12</span>.</td>
          </tr>
        </tbody>
      </table>
      <div class="vio-tip-strip">
        <b>2 Nhận xét giúp nhẩm ƯCLN trong 3 giây:</b><br>
        • Với mọi số tự nhiên <i>a</i> và <i>b</i>, ta luôn có: <span class="v-tag">ƯCLN(a, 1) = 1</span> và <span class="v-tag">ƯCLN(a, b, 1) = 1</span>.<br>
        • <b>Trường hợp chia hết:</b> Nếu <span class="v-tag">a ⋮ b</span> thì <span class="v-tag">ƯCLN(a, b) = b</span> (số nhỏ hơn chính là ƯCLN). <i>Ví dụ: Vì <span class="v-tag">45 ⋮ 15</span> nên <span class="v-tag">ƯCLN(45, 15) = 15</span> ngay lập tức!</i>
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ 2 -->
    <div class="vio-quest-box">
      <div class="vio-quest-title">TRẠM KHÁM PHÁ 2: PHÒNG THÍ NGHIỆM 3 BƯỚC TÌM ƯCLN (+20 ĐIỂM)</div>
      <p><b>Bài toán thực hành:</b> Tìm <span class="v-tag">ƯCLN(60, 90)</span> và suy ra tập hợp <span class="v-tag">ƯC(60, 90)</span>.</p>
      <p>Ta đã phân tích sẵn Bước 1: <span class="v-tag">60 = 2² . 3 . 5</span> và <span class="v-tag">90 = 2 . 3² . 5</span>.</p>

      <div class="lab-grid">
        <div class="lab-box">
          <b>Nhiệm vụ A: Tính ƯCLN(60, 90)</b><br>
          Các thừa số chung là 2, 3 và 5. Lấy mỗi thừa số với số mũ nhỏ nhất, ta được tích <span class="v-tag">2¹ . 3¹ . 5¹</span> bằng bao nhiêu?
          <div class="lab-row-inp">
            <span>ƯCLN(60, 90) = </span>
            <input type="number" id="inpLabA" class="vio-input" placeholder="?">
            <button class="vio-btn" onclick="checkLab('A', 30, 'Chính xác! 2 . 3 . 5 = 30. Vậy ƯCLN(60, 90) = 30!')">Kiểm tra</button>
          </div>
          <div class="lab-msg" id="msgLabA"></div>
        </div>

        <div class="lab-box">
          <b>Nhiệm vụ B: Nhẩm nhanh trường hợp đặc biệt</b><br>
          Không cần phân tích ra thừa số nguyên tố, hãy cho biết <span class="v-tag">ƯCLN(24, 72)</span> bằng bao nhiêu <i>(Gợi ý: 72 ⋮ 24)</i>?
          <div class="lab-row-inp">
            <span>ƯCLN(24, 72) = </span>
            <input type="number" id="inpLabB" class="vio-input" placeholder="?">
            <button class="vio-btn" onclick="checkLab('B', 24, 'Tuyệt vời! Vì 72 chia hết cho 24 nên số nhỏ hơn (24) chính là ƯCLN!')">Kiểm tra</button>
          </div>
          <div class="lab-msg" id="msgLabB"></div>
        </div>
      </div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 3: HAI SỐ NGUYÊN TỐ CÙNG NHAU & RÚT GỌN PHÂN SỐ -->
<div class="vio-card">
  <div class="vio-card-head">
    <span>NỘI DUNG 3: SỐ NGUYÊN TỐ CÙNG NHAU & RÚT GỌN VỀ PHÂN SỐ TỐI GIẢN</span>
    <span class="vio-step-tag">Phần 3 / 4</span>
  </div>
  <div class="vio-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="vio-theory-box">
      <div class="vio-theory-head">3. LÝ THUYẾT CỐT LÕI CẦN NHỚ</div>
      <div class="vio-theory-grid">
        <div class="vio-mini-card">
          <div class="vio-mini-title">HAI SỐ NGUYÊN TỐ CÙNG NHAU</div>
          • Hai số có <span class="v-tag">ƯCLN bằng 1</span> được gọi là <b>hai số nguyên tố cùng nhau</b>.<br>
          • <i>Ví dụ:</i> <span class="v-tag">8</span> và <span class="v-tag">15</span> đều là hợp số, nhưng không có thừa số nguyên tố chung nào nên <span class="v-tag">ƯCLN(8, 15) = 1</span> ➔ 8 và 15 nguyên tố cùng nhau.
        </div>
        <div class="vio-mini-card">
          <div class="vio-mini-title">PHÂN SỐ TỐI GIẢN</div>
          • Phân số <span class="v-tag">a / b</span> gọi là <b>phân số tối giản</b> nếu tử và mẫu là hai số nguyên tố cùng nhau, tức là <span class="v-tag">ƯCLN(a, b) = 1</span>.<br>
          • <b>Cách rút gọn 1 bước về tối giản:</b> Chia cả tử và mẫu của phân số <span class="v-tag">a / b</span> cho <span class="v-tag">ƯCLN(a, b)</span>.
        </div>
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ 3 -->
    <div class="vio-quest-box">
      <div class="vio-quest-title">TRẠM KHÁM PHÁ 3: XƯỞNG RÚT GỌN PHÂN SỐ TỐI GIẢN (+15 ĐIỂM)</div>
      <p><b>Thử thách:</b> Rút gọn phân số 
        <span class="frac-wrap"><span class="frac-top">28</span><span class="frac-bot">42</span></span>
        về <b>phân số tối giản</b> chỉ bằng 1 phép chia duy nhất cho <span class="v-tag">ƯCLN(28, 42) = 14</span>. Hãy điền tử số và mẫu số sau khi rút gọn:</p>
      <div class="lab-row-inp" style="margin-top:12px;">
        <span>Phân số tối giản: Tử số = </span>
        <input type="number" id="inpNum" class="vio-input" placeholder="Tử">
        <span> / Mẫu số = </span>
        <input type="number" id="inpDen" class="vio-input" placeholder="Mẫu">
        <button class="vio-btn" onclick="checkFraction()">Kiểm tra phân số</button>
      </div>
      <div class="lab-msg" id="msgFrac"></div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 4: ĐẤU TRƯỜNG TRÒ CHƠI & BÀI TOÁN THỰC TIỄN -->
<div class="vio-card">
  <div class="vio-card-head">
    <span>NỘI DUNG 4: ĐẤU TRƯỜNG NỐI CẶP, TRẮC NGHIỆM & TOÁN THỰC TẾ</span>
    <span class="vio-step-tag">Phần 4 / 4</span>
  </div>
  <div class="vio-card-body">

    <!-- VÒNG 1: TRÒ CHƠI NỐI CẶP (20 ĐIỂM) -->
    <div class="vio-quest-box" style="margin-bottom:20px;">
      <div class="vio-quest-title">VÒNG 1: GHÉP NỐI TỐC ĐỘ (20 ĐIỂM — 5 Điểm / Cặp)</div>
      <p><b>Cách chơi:</b> Nhấn chọn một yêu cầu ở <b>CỘT A</b>, sau đó nhấn chọn kết quả tương ứng ở <b>CỘT B</b>.</p>

      <div class="match-grid">
        <div>
          <div class="match-head">CỘT A: BÀI TOÁN</div>
          <div class="m-card" data-a="1" onclick="selA(this)">
            <span>1. ƯCLN(16, 24)</span>
            <span class="m-badge" id="bA-1"></span>
          </div>
          <div class="m-card" data-a="2" onclick="selA(this)">
            <span>2. ƯCLN(15, 28)</span>
            <span class="m-badge" id="bA-2"></span>
          </div>
          <div class="m-card" data-a="3" onclick="selA(this)">
            <span>3. ƯCLN(18, 54, 90)</span>
            <span class="m-badge" id="bA-3"></span>
          </div>
          <div class="m-card" data-a="4" onclick="selA(this)">
            <span>4. Tập hợp ƯC(16, 24)</span>
            <span class="m-badge" id="bA-4"></span>
          </div>
        </div>

        <div>
          <div class="match-head">CỘT B: ĐÁP ÁN</div>
          <div class="m-card" data-b="3" onclick="selB(this)">
            <span>a) Bằng 18 (vì 54 ⋮ 18 và 90 ⋮ 18)</span>
            <span class="m-badge" id="bB-3"></span>
          </div>
          <div class="m-card" data-b="1" onclick="selB(this)">
            <span>b) Bằng 8 (vì 16 = 2⁴; 24 = 2³.3)</span>
            <span class="m-badge" id="bB-1"></span>
          </div>
          <div class="m-card" data-b="4" onclick="selB(this)">
            <span>c) {1; 2; 4; 8} (là các ước của 8)</span>
            <span class="m-badge" id="bB-4"></span>
          </div>
          <div class="m-card" data-b="2" onclick="selB(this)">
            <span>d) Bằng 1 (hai số nguyên tố cùng nhau)</span>
            <span class="m-badge" id="bB-2"></span>
          </div>
        </div>
      </div>

      <div id="matchMsg" style="margin-top:8px; font-weight:800; color:#5b21b6;"></div>
      <button class="vio-btn" style="margin-top:8px;" onclick="resetMatching()">Chơi lại Vòng 1</button>
    </div>

    <!-- VÒNG 2: TRẮC NGHIỆM VẬN DỤNG (30 ĐIỂM) -->
    <div class="vio-quest-box" style="margin-bottom:20px;">
      <div class="vio-quest-title">VÒNG 2: BẮT BẪY TƯ DUY & TOÁN THỰC TIỄN (30 ĐIỂM — 10 Điểm / Câu)</div>

      <div class="q-card" id="qc-1">
        <div class="q-title">Câu 1: Cho hai số a = 2³ . 3² . 5 và b = 2² . 3 . 7. Ước chung lớn nhất của a và b là:</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Sai rồi! Bạn đã lấy cả thừa số không chung (5 và 7) và lấy số mũ lớn nhất mất rồi.')">A. 2³ . 3² . 5 . 7</button>
          <button class="q-btn" onclick="ansQuiz(1, this, true, 'CHÍNH XÁC (+10 Điểm)! Chỉ chọn thừa số nguyên tố CHUNG là 2 và 3, với số mũ NHỎ NHẤT là 2² và 3¹. Kết quả: 2² . 3 = 12.')">B. 2² . 3 = 12</button>
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Chưa chính xác! Số mũ nhỏ nhất của 3 là 3¹ chứ không phải 3².')">C. 2² . 3² = 36</button>
        </div>
        <div class="q-exp" id="qexp-1"></div>
      </div>

      <div class="q-card" id="qc-2">
        <div class="q-title">Câu 2: Trong các cặp số sau, cặp số nào là HAI SỐ NGUYÊN TỐ CÙNG NHAU?</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Sai rồi! 14 và 21 cùng chia hết cho 7 nên ƯCLN(14, 21) = 7 ≠ 1.')">A. 14 và 21</button>
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Sai rồi! 12 và 30 đều là số chẵn (cùng chia hết cho 6).')">B. 12 và 30</button>
          <button class="q-btn" onclick="ansQuiz(2, this, true, 'XUẤT SẮC (+10 Điểm)! 9 = 3² và 16 = 2⁴ không có thừa số nguyên tố chung nào nên ƯCLN(9, 16) = 1.')">C. 9 và 16</button>
        </div>
        <div class="q-exp" id="qexp-2"></div>
      </div>

      <div class="q-card" id="qc-3" style="margin-bottom:0;">
        <div class="q-title">Câu 3 (Bài toán chia phần thưởng): Một đội tình nguyện có 24 nam và 32 nữ. Người phụ trách muốn chia đội thành các nhóm nhỏ sao cho số nam và số nữ được chia đều vào các nhóm. Hỏi có thể chia được NHIỀU NHẤT thành bao nhiêu nhóm?</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(3, this, false, 'Chưa phải nhiều nhất! Chia 4 nhóm thì chia đều được, nhưng đề hỏi số nhóm NHIỀU NHẤT.')">A. 4 nhóm</button>
          <button class="q-btn" onclick="ansQuiz(3, this, true, 'ĐỈNH CAO (+10 Điểm)! Số nhóm nhiều nhất chính là ƯCLN(24, 32) = 8 nhóm (khi đó mỗi nhóm có 3 nam và 4 nữ).')">B. 8 nhóm</button>
          <button class="q-btn" onclick="ansQuiz(3, this, false, 'Sai rồi! 32 không chia hết cho 6 nên không thể chia đều thành 6 nhóm.')">C. 6 nhóm</button>
        </div>
        <div class="q-exp" id="qexp-3"></div>
      </div>
    </div>

    <!-- VÒNG 3: BÀI TẬP TỰ LUẬN TRỌNG TÂM -->
    <div class="vio-quest-box" style="margin-bottom:0;">
      <div class="vio-quest-title">VÒNG 3: BÀI TOÁN TỰ LUẬN THỰC TẾ (LÀM VÀO VỞ & ĐỐI CHIẾU ĐÁP ÁN)</div>
      <ul>
        <li><b>Bài toán 1 (Tìm ƯC thông qua ƯCLN):</b> Tìm tập hợp <span class="v-tag">ƯC(56, 140)</span> bằng cách tìm <span class="v-tag">ƯCLN(56, 140)</span>.</li>
        <li><b>Bài toán 2 (Toán thực tế chuẩn SGK):</b> Để chuẩn bị cho năm học mới, mẹ mua cho An <b>18 chiếc bút bi</b> và <b>30 quyển vở</b>. An muốn chia đều cả bút và vở vào các túi quà để tặng các bạn vùng cao sao cho số túi quà lớn hơn 2. Hỏi An có những cách chia nào? Cách chia nào được nhiều túi quà nhất?</li>
      </ul>

      <details class="vio-details" onclick="sfxClick()">
        <summary>[ NHẤN ĐỂ MỞ KHÓA LỜI GIẢI TRÌNH BÀY MẪU VÒNG 3 ]</summary>
        <div class="vio-details-body">
          <p><b>Hướng dẫn giải Bài toán 1:</b></p>
          <ul>
            <li>Phân tích ra thừa số nguyên tố: <span class="v-tag">56 = 2³ . 7</span> và <span class="v-tag">140 = 2² . 5 . 7</span>.</li>
            <li>Thừa số nguyên tố chung là 2 và 7, lấy với số mũ nhỏ nhất: <span class="v-tag">ƯCLN(56, 140) = 2² . 7 = 28</span>.</li>
            <li>Suy ra <span class="v-tag">ƯC(56, 140) = Ư(28) = {1; 2; 4; 7; 14; 28}</span>.</li>
          </ul>
          <hr style="margin:12px 0; border:0; border-top:1px solid #ddd6fe;">
          <p><b>Hướng dẫn giải Bài toán 2:</b></p>
          <ul>
            <li>Gọi số túi quà An có thể chia là <i>x</i> (túi) với điều kiện <span class="v-tag">x ∈ ℕ</span> và <span class="v-tag">x &gt; 2</span>.</li>
            <li>Vì 18 bút bi và 30 quyển vở được chia đều vào <i>x</i> túi nên <span class="v-tag">18 ⋮ x</span> và <span class="v-tag">30 ⋮ x</span>, suy ra <span class="v-tag">x ∈ ƯC(18, 30)</span>.</li>
            <li>Ta có: <span class="v-tag">18 = 2 . 3²</span> và <span class="v-tag">30 = 2 . 3 . 5</span> ➔ <span class="v-tag">ƯCLN(18, 30) = 2 . 3 = 6</span>.</li>
            <li>Do đó <span class="v-tag">x ∈ ƯC(18, 30) = Ư(6) = {1; 2; 3; 6}</span>.</li>
            <li>Vì <span class="v-tag">x &gt; 2</span> nên <span class="v-tag">x ∈ {3; 6}</span> (Có 2 cách chia: chia thành <b>3 túi</b> hoặc chia thành <b>6 túi</b>).</li>
            <li><b>Kết luận:</b> Cách chia được nhiều túi quà nhất là <b>6 túi</b> (khi đó mỗi túi có <span class="v-tag">18 : 6 = 3</span> bút bi và <span class="v-tag">30 : 6 = 5</span> quyển vở).</li>
          </ul>
        </div>
      </details>
    </div>

  </div>
</div>

<!-- BẢNG TỔNG KẾT CỐT LÕI BÀI 11 -->
<div class="vio-card" style="margin-bottom:0;">
  <div class="vio-card-head">
    <span>BẢNG TÓM TẮT CỐT LÕI BÀI 11: ƯỚC CHUNG & ƯỚC CHUNG LỚN NHẤT</span>
    <span class="vio-step-tag">Ôn tập nhanh</span>
  </div>
  <div class="vio-card-body">
    <table class="step-table">
      <thead>
        <tr>
          <th width="26%">Nội dung</th>
          <th width="42%">Công thức / Quy tắc trọng tâm</th>
          <th width="32%">Mẹo áp dụng nhanh</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><b>Ước chung (ƯC)</b></td>
          <td><span class="v-tag">x ∈ ƯC(a, b)</span> ⇔ <span class="v-tag">a ⋮ x</span> và <span class="v-tag">b ⋮ x</span></td>
          <td>Tìm <span class="v-tag">ƯC(a, b)</span> bằng cách tìm các <b>ước của ƯCLN(a, b)</b>.</td>
        </tr>
        <tr>
          <td><b>Tìm ƯCLN bằng phân tích TSNT</b></td>
          <td>1. Phân tích ra TSNT.<br>2. Chọn thừa số nguyên tố <b>CHUNG</b>.<br>3. Lập tích với số mũ <b>NHỎ NHẤT</b>.</td>
          <td>Nếu <span class="v-tag">a ⋮ b</span> thì <span class="v-tag">ƯCLN(a, b) = b</span>.<br>Khẩu quyết: <b>"ƯCLN = Chung + Mũ nhỏ nhất"</b>.</td>
        </tr>
        <tr>
          <td><b>Số nguyên tố cùng nhau & Phân số tối giản</b></td>
          <td>• Nguyên tố cùng nhau ⇔ <span class="v-tag">ƯCLN(a, b) = 1</span>.<br>• Rút gọn tối giản: Chia cả tử và mẫu cho <span class="v-tag">ƯCLN(tử, mẫu)</span>.</td>
          <td>Hai số tự nhiên liên tiếp (như 8 và 9) luôn nguyên tố cùng nhau.</td>
        </tr>
        <tr>
          <td><b>Nhận diện bài toán thực tế dùng ƯCLN</b></td>
          <td>Đề bài yêu cầu <b>"chia đều"</b> các vật vào các nhóm/túi và hỏi <b>"số nhóm nhiều nhất (lớn nhất)"</b>.</td>
          <td>Số nhóm nhiều nhất chính là <span class="v-tag">ƯCLN</span> của các số đã cho.</td>
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

  // LOGIC TRẠM 1: SĂN TẬP HỢP ƯC(18, 30) (15 ĐIỂM)
  let foundUC = 0;
  let doneUC = false;
  function pickUC(el, isRight, msg) {
    if (el.classList.contains('correct') || el.classList.contains('wrong') || doneUC) return;
    const box = document.getElementById('msgUC');
    box.textContent = msg;
    if (isRight) {
      sfxOk();
      el.classList.add('correct');
      box.style.color = '#5b21b6';
      foundUC++;
      if (foundUC === 4) {
        doneUC = true;
        addScore(15);
        box.textContent = 'HOÀN HẢO (+15 Điểm)! ƯC(18, 30) = {1; 2; 3; 6} và ƯCLN(18, 30) = 6.';
      }
    } else {
      sfxErr();
      el.classList.add('wrong');
      box.style.color = '#9f1239';
    }
  }

  // LOGIC TRẠM 2: PHÒNG THÍ NGHIỆM ƯCLN (20 ĐIỂM)
  const labDone = {};
  function checkLab(key, expected, okMsg) {
    if (labDone[key]) return;
    const val = parseInt(document.getElementById('inpLab' + key).value, 10);
    const fb = document.getElementById('msgLab' + key);
    if (val === expected) {
      sfxOk();
      fb.style.color = '#166534';
      fb.textContent = okMsg + ' (+10 Điểm)';
      labDone[key] = true;
      addScore(10);
    } else {
      sfxErr();
      fb.style.color = '#9f1239';
      fb.textContent = 'Chưa chính xác, hãy kiểm tra lại phép nhân các thừa số nguyên tố chung nhé!';
    }
  }

  // LOGIC TRẠM 3: RÚT GỌN PHÂN SỐ (15 ĐIỂM)
  let fracDone = false;
  function checkFraction() {
    if (fracDone) return;
    const num = parseInt(document.getElementById('inpNum').value, 10);
    const den = parseInt(document.getElementById('inpDen').value, 10);
    const fb = document.getElementById('msgFrac');
    if (num === 2 && den === 3) {
      sfxOk();
      fb.style.color = '#166534';
      fb.textContent = 'XUẤT SẮC (+15 Điểm)! Chia cả tử và mẫu của 28/42 cho ƯCLN(28, 42) = 14 ta được phân số tối giản 2/3!';
      fracDone = true;
      addScore(15);
    } else {
      sfxErr();
      fb.style.color = '#9f1239';
      fb.textContent = 'Chưa đúng! Hãy lấy 28 : 14 (Tử số) và 42 : 14 (Mẫu số) nhé!';
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
