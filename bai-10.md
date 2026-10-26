<style>
  /* Ẩn tiêu đề mặc định của GitHub Pages & Thiết lập nền Xanh Ngọc Nhạt */
  .markdown-body > h1:first-child { display: none !important; }
  .container-lg, .markdown-body { max-width: 960px !important; margin: 0 auto !important; padding: 16px !important; font-family: 'Segoe UI', system-ui, -apple-system, sans-serif !important; color: #064e3b !important; background-color: #ecfdf5 !important; }
  body { background-color: #ecfdf5 !important; }

  /* Thanh điều khiển cố định (Sticky Bar) */
  .emr-topbar { position: sticky; top: 10px; z-index: 999; background: #ffffff; border: 2px solid #10b981; border-radius: 12px; padding: 10px 20px; margin-bottom: 24px; display: flex; justify-content: space-between; align-items: center; box-shadow: 0 8px 20px rgba(5, 150, 105, 0.12); flex-wrap: wrap; gap: 10px; }
  .emr-topbar-title { font-weight: 800; color: #065f46; font-size: 0.98rem; letter-spacing: 0.3px; }
  .emr-topbar-right { display: flex; align-items: center; gap: 12px; }
  .emr-score-badge { background: #d1fae5; color: #047857; border: 1.5px solid #10b981; padding: 5px 16px; border-radius: 99px; font-weight: 800; font-size: 0.95rem; }
  .emr-sound-btn { background: #059669; color: #ffffff; border: none; padding: 7px 15px; border-radius: 8px; font-weight: 700; cursor: pointer; font-size: 0.88rem; transition: 0.2s; }
  .emr-sound-btn:hover { background: #047857; }

  /* Khung Banner chính */
  .emr-hero { background: linear-gradient(135deg, #d1fae5 0%, #a7f3d0 100%); border: 2px solid #10b981; border-radius: 16px; padding: 28px 24px; text-align: center; margin-bottom: 26px; box-shadow: 0 8px 22px rgba(5, 150, 105, 0.1); }
  .emr-hero-tag { display: inline-block; background: #059669; color: #ffffff; font-weight: 800; font-size: 0.82rem; padding: 5px 16px; border-radius: 99px; text-transform: uppercase; letter-spacing: 0.7px; margin-bottom: 10px; }
  .emr-hero-title { color: #064e3b !important; font-size: 1.95rem !important; font-weight: 800 !important; margin: 0 0 14px 0 !important; border: none !important; padding: 0 !important; }
  .emr-meta-row { display: flex; justify-content: center; flex-wrap: wrap; gap: 10px; }
  .emr-meta-item { background: #ffffff; border: 1px solid #6ee7b7; color: #065f46; padding: 5px 14px; border-radius: 8px; font-size: 0.9rem; font-weight: 600; }

  /* Hệ thống Khung bài giảng (Section Frames) */
  .emr-card { background: #ffffff; border: 2px solid #a7f3d0; border-radius: 16px; margin-bottom: 26px; overflow: hidden; box-shadow: 0 5px 15px rgba(5, 150, 105, 0.06); }
  .emr-card-head { background: linear-gradient(90deg, #d1fae5 0%, #a7f3d0 100%); border-bottom: 2px solid #6ee7b7; padding: 14px 22px; color: #064e3b; font-size: 1.18rem; font-weight: 800; display: flex; justify-content: space-between; align-items: center; }
  .emr-step-tag { background: #059669; color: #fff; font-size: 0.78rem; padding: 3px 10px; border-radius: 12px; font-weight: 700; }
  .emr-card-body { padding: 22px; line-height: 1.65; font-size: 1rem; }

  /* Khung Lý thuyết ngắn gọn (Đặt trước Trạm khám phá) */
  .emr-theory-box { background: #ecfdf5; border: 1.5px solid #6ee7b7; border-left: 6px solid #059669; border-radius: 12px; padding: 18px 20px; margin-bottom: 20px; }
  .emr-theory-head { font-weight: 800; color: #065f46; font-size: 1.04rem; margin-bottom: 10px; text-transform: uppercase; letter-spacing: 0.3px; border-bottom: 1.5px solid #a7f3d0; padding-bottom: 6px; }
  .emr-theory-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 14px; margin-top: 10px; }
  .emr-mini-card { background: #ffffff; border: 1px solid #a7f3d0; border-radius: 10px; padding: 12px 15px; }
  .emr-mini-title { font-weight: 800; color: #047857; margin-bottom: 4px; font-size: 0.96rem; }
  .emr-warn-strip { background: #fef9c3; border: 1px solid #fde047; border-left: 5px solid #eab308; border-radius: 8px; padding: 10px 14px; margin-top: 12px; color: #713f12; font-size: 0.94rem; }

  /* Khung bài tập dẫn dắt (Interactive Discovery Box) */
  .emr-quest-box { background: #f8fafc; border: 2px dashed #10b981; border-radius: 12px; padding: 18px; margin-bottom: 8px; }
  .emr-quest-title { font-weight: 800; color: #047857; margin-bottom: 10px; font-size: 1.02rem; text-transform: uppercase; }

  /* Các nút chọn số tương tác (Number Chips) */
  .chip-grid { display: flex; flex-wrap: wrap; gap: 10px; margin: 12px 0; }
  .num-chip { background: #ffffff; border: 2px solid #6ee7b7; color: #064e3b; padding: 10px 16px; border-radius: 10px; font-weight: 800; font-size: 1.02rem; cursor: pointer; transition: 0.2s; user-select: none; text-align: center; min-width: 72px; }
  .num-chip:hover { background: #d1fae5; border-color: #059669; transform: translateY(-2px); }
  .num-chip.correct { background: #059669; border-color: #065f46; color: #ffffff; }
  .num-chip.wrong { background: #ffe4e6; border-color: #e11d48; color: #9f1239; text-decoration: line-through; opacity: 0.7; }

  /* Sơ đồ cây phân tích thừa số nguyên tố (Factor Tree Lab) */
  .tree-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 16px; margin: 14px 0; }
  .tree-card { background: #ffffff; border: 1.5px solid #a7f3d0; border-radius: 12px; padding: 16px; text-align: center; }
  .tree-node-root { display: inline-block; background: #059669; color: #ffffff; font-weight: 800; padding: 6px 18px; border-radius: 8px; margin-bottom: 8px; font-size: 1.1rem; }
  .tree-branches { font-family: monospace; font-weight: 800; color: #10b981; font-size: 1.1rem; line-height: 1; margin-bottom: 6px; }
  .tree-row { display: flex; justify-content: center; align-items: center; gap: 12px; margin-bottom: 8px; }
  .node-prime { background: #fef3c7; border: 2px solid #f59e0b; color: #92400e; font-weight: 800; padding: 5px 12px; border-radius: 99px; font-size: 0.95rem; }
  .node-comp { background: #e0f2fe; border: 2px solid #38bdf8; color: #0369a1; font-weight: 800; padding: 5px 12px; border-radius: 8px; font-size: 0.95rem; }
  .tree-input { width: 58px; padding: 5px 6px; border: 2px solid #10b981; border-radius: 8px; font-weight: 800; text-align: center; font-size: 0.95rem; color: #064e3b; background: #f0fdf4; outline: none; }
  .tree-btn { background: #059669; color: #ffffff; border: none; padding: 8px 16px; border-radius: 8px; font-weight: 700; cursor: pointer; margin-top: 8px; transition: 0.2s; }
  .tree-btn:hover { background: #047857; }
  .lab-feedback { font-size: 0.9rem; font-weight: 700; margin-top: 8px; min-height: 22px; }

  .p-tag { background: #ffffff; color: #047857; border: 1px solid #10b981; padding: 1px 8px; border-radius: 6px; font-family: 'Consolas', monospace; font-weight: 800; font-size: 0.95em; display: inline-block; }

  /* Bảng tổng kết gọn đẹp */
  .emr-table { width: 100%; border-collapse: collapse; margin-top: 10px; border-radius: 10px; overflow: hidden; border: 1.5px solid #6ee7b7; }
  .emr-table th { background: #059669 !important; color: #ffffff !important; padding: 11px 15px !important; text-align: left; font-weight: 800; border: 1px solid #047857 !important; }
  .emr-table td { padding: 11px 15px !important; border: 1px solid #a7f3d0 !important; background: #ffffff !important; color: #064e3b !important; }
  .emr-table tr:nth-child(even) td { background: #f0fdf4 !important; }

  /* Trò chơi Nối cặp (Matching Game) */
  .match-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; margin-top: 14px; }
  .match-head { background: #059669; color: #ffffff; text-align: center; padding: 9px; border-radius: 8px; font-weight: 800; margin-bottom: 10px; }
  .m-card { background: #f0fdf4; border: 2px solid #6ee7b7; border-radius: 10px; padding: 13px 15px; margin-bottom: 10px; font-weight: 700; color: #064e3b; cursor: pointer; transition: 0.2s; display: flex; justify-content: space-between; align-items: center; user-select: none; }
  .m-card:hover:not(.matched) { background: #d1fae5; border-color: #059669; transform: translateY(-2px); }
  .m-card.selected { background: #059669; color: #ffffff; border-color: #064e3b; box-shadow: 0 0 0 4px rgba(5, 150, 105, 0.25); }
  .m-card.matched { background: #dcfce7; border-color: #16a34a; color: #166534; cursor: default; }
  .m-card.wrong { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .m-badge { font-size: 0.78rem; background: #059669; color: #fff; padding: 2px 8px; border-radius: 10px; display: none; }
  .m-card.matched .m-badge { display: inline-block; }

  /* Trắc nghiệm tốc độ */
  .q-card { background: #ffffff; border: 1.5px solid #6ee7b7; border-radius: 12px; padding: 16px; margin-bottom: 14px; }
  .q-title { font-weight: 800; color: #064e3b; margin-bottom: 10px; }
  .q-opts { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 10px; }
  .q-btn { background: #f0fdf4; border: 2px solid #a7f3d0; padding: 10px 14px; border-radius: 8px; font-weight: 700; color: #064e3b; cursor: pointer; text-align: left; transition: 0.2s; }
  .q-btn:hover:not(:disabled) { background: #d1fae5; border-color: #059669; }
  .q-btn.ok { background: #dcfce7; border-color: #16a34a; color: #166534; }
  .q-btn.err { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .q-exp { display: none; margin-top: 10px; padding: 10px 14px; border-radius: 8px; font-weight: 600; font-size: 0.92rem; }

  @media (max-width: 680px) {
    .match-grid { grid-template-columns: 1fr; }
  }
</style>

<!-- THANH ĐIỀU KHIỂN CỐ ĐỊNH -->
<div class="emr-topbar">
  <div class="emr-topbar-title">TOÁN 6 — BÀI 10: SỐ NGUYÊN TỐ</div>
  <div class="emr-topbar-right">
    <div class="emr-score-badge">ĐIỂM KHÁM PHÁ: <span id="ptsVal">0</span> / 100</div>
    <button class="emr-sound-btn" id="btnSound" onclick="toggleSound()">Âm thanh: ĐANG BẬT</button>
  </div>
</div>

<!-- BANNER MỞ ĐẦU -->
<div class="emr-hero">
  <div class="emr-hero-tag">CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN</div>
  <h1 class="emr-hero-title">BÀI 10: SỐ NGUYÊN TỐ</h1>
  <div class="emr-meta-row">
    <div class="emr-meta-item">Toán 6 (Tập 1) — Kết nối tri thức với cuộc sống</div>
    <div class="emr-meta-item">Cấu trúc: Lý thuyết cô đọng ➔ Tương tác khám phá ➔ Trò chơi</div>
  </div>
</div>

<!-- NỘI DUNG 1: SỐ NGUYÊN TỐ VÀ HỢP SỐ -->
<div class="emr-card">
  <div class="emr-card-head">
    <span>NỘI DUNG 1: SỐ NGUYÊN TỐ VÀ HỢP SỐ</span>
    <span class="emr-step-tag">Phần 1 / 3</span>
  </div>
  <div class="emr-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="emr-theory-box">
      <div class="emr-theory-head">1. LÝ THUYẾT CỐT LÕI CẦN NHỚ</div>
      <div class="emr-theory-grid">
        <div class="emr-mini-card">
          <div class="emr-mini-title">SỐ NGUYÊN TỐ LÀ GÌ?</div>
          Là số tự nhiên <b>lớn hơn 1</b>, chỉ có <b>đúng 2 ước</b> là 1 và chính nó.<br>
          • <i>Ví dụ:</i> <span class="p-tag">2; 3; 5; 7; 11; 13; 17; 19; 23; 29...</span>
        </div>
        <div class="emr-mini-card">
          <div class="emr-mini-title">HỢP SỐ LÀ GÌ?</div>
          Là số tự nhiên <b>lớn hơn 1</b>, có <b>nhiều hơn 2 ước</b>.<br>
          • <i>Ví dụ:</i> Số <span class="p-tag">6</span> là hợp số vì có 4 ước là <span class="p-tag">{1; 2; 3; 6}</span>.
        </div>
      </div>
      <div class="emr-warn-strip">
        <b>Lưu ý đặc biệt:</b><br>
        • Số <span class="p-tag">0</span> và số <span class="p-tag">1</span> <b>không là số nguyên tố</b> và cũng <b>không là hợp số</b>.<br>
        • Số <span class="p-tag">2</span> là <b>số nguyên tố nhỏ nhất</b> và là <b>số nguyên tố chẵn duy nhất</b>.
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ TƯƠNG TÁC 1 -->
    <div class="emr-quest-box">
      <div class="emr-quest-title">TRẠM KHÁM PHÁ 1: THỬ THÁCH SÀNG LỌC SỐ NGUYÊN TỐ (+20 ĐIỂM)</div>
      <p><b>Nhiệm vụ:</b> Vận dụng ngay lý thuyết ở trên, hãy <b>bấm chọn đúng 5 SỐ NGUYÊN TỐ</b> trong danh sách dưới đây:</p>
      <div class="chip-grid" id="primeGrid">
        <div class="num-chip" onclick="pickPrime(this, false, 'Sai rồi! Số 1 chỉ có 1 ước nên KHÔNG phải số nguyên tố cũng KHÔNG phải hợp số.')">Số 1</div>
        <div class="num-chip" onclick="pickPrime(this, true, 'Chính xác! Ư(2) = {1; 2}. Số 2 là số nguyên tố chẵn duy nhất!')">Số 2</div>
        <div class="num-chip" onclick="pickPrime(this, true, 'Chính xác! Ư(3) = {1; 3} (chỉ có đúng 2 ước).')">Số 3</div>
        <div class="num-chip" onclick="pickPrime(this, false, 'Số 4 là HỢP SỐ vì ngoài 1 và 4 còn chia hết cho 2.')">Số 4</div>
        <div class="num-chip" onclick="pickPrime(this, true, 'Chính xác! Ư(5) = {1; 5} (chỉ có đúng 2 ước).')">Số 5</div>
        <div class="num-chip" onclick="pickPrime(this, false, 'Bẫy đấy! Số 9 là số lẻ nhưng là HỢP SỐ vì chia hết cho 3.')">Số 9</div>
        <div class="num-chip" onclick="pickPrime(this, true, 'Chính xác! Ư(11) = {1; 11} (chỉ có đúng 2 ước).')">Số 11</div>
        <div class="num-chip" onclick="pickPrime(this, false, 'Số 15 là HỢP SỐ vì chia hết cho cả 3 và 5.')">Số 15</div>
        <div class="num-chip" onclick="pickPrime(this, true, 'Xuất sắc! Ư(17) = {1; 17} (chỉ có đúng 2 ước).')">Số 17</div>
      </div>
      <div id="msgPrime" style="font-weight:700; color:#047857; font-size:0.93rem; min-height:22px;"></div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 2: PHÂN TÍCH MỘT SỐ RA THỪA SỐ NGUYÊN TỐ -->
<div class="emr-card">
  <div class="emr-card-head">
    <span>NỘI DUNG 2: PHÂN TÍCH MỘT SỐ RA THỪA SỐ NGUYÊN TỐ</span>
    <span class="emr-step-tag">Phần 2 / 3</span>
  </div>
  <div class="emr-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="emr-theory-box">
      <div class="emr-theory-head">2. LÝ THUYẾT CỐT LÕI CẦN NHỚ</div>
      <ul>
        <li><b>Khái niệm:</b> Phân tích một số tự nhiên lớn hơn 1 ra thừa số nguyên tố là viết số đó dưới dạng <b> một tích các thừa số nguyên tố</b>.</li>
        <li><b>2 Phương pháp thực hiện:</b>
          <ul>
            <li><b>Cách 1 (Sơ đồ cây):</b> Tách số ban đầu thành tích của 2 thừa số bất kì lớn hơn 1, tiếp tục tách các nhánh hợp số cho đến khi mọi nhánh tận cùng đều là <b>số nguyên tố</b>.</li>
            <li><b>Cách 2 (Sơ đồ cột dọc):</b> Chia số đó lần lượt cho các số nguyên tố từ nhỏ đến lớn (<span class="p-tag">2; 3; 5; 7; ...</span>) cho đến khi thương bằng <span class="p-tag">1</span>.</li>
          </ul>
        </li>
        <li><b>Quy ước trình bày:</b> Dùng <b>lũy thừa</b> để viết gọn các thừa số nguyên tố giống nhau và sắp xếp các thừa số từ nhỏ đến lớn <i>(Ví dụ: <span class="p-tag">24 = 2 . 2 . 2 . 3 = 2³ . 3</span>)</i>.</li>
      </ul>
    </div>

    <!-- TRẠM KHÁM PHÁ TƯƠNG TÁC 2 -->
    <div class="emr-quest-box">
      <div class="emr-quest-title">TRẠM KHÁM PHÁ 2: THỰC HÀNH SƠ ĐỒ CÂY NHÂN TỬ (+20 ĐIỂM)</div>
      <p><b>Nhiệm vụ:</b> Quan sát 2 sơ đồ cây dưới đây, điền <b>thừa số nguyên tố</b> còn thiếu vào ô trống <span class="p-tag">?</span> và bấm Kiểm tra:</p>

      <div class="tree-grid">
        <!-- Cây sơ đồ 1: Phân tích số 12 -->
        <div class="tree-card">
          <div style="font-weight:800; color:#065f46; margin-bottom:8px;">Sơ đồ A: Phân tích số 12</div>
          <div class="tree-node-root">12</div>
          <div class="tree-branches">/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; \</div>
          <div class="tree-row">
            <span class="node-prime" title="Số nguyên tố">2</span>
            <span>×</span>
            <span class="node-comp" title="Hợp số - tách tiếp">6</span>
          </div>
          <div class="tree-branches" style="padding-left:68px;">/ &nbsp;&nbsp; \</div>
          <div class="tree-row" style="padding-left:68px;">
            <span class="node-prime">2</span>
            <span>×</span>
            <input type="number" id="inpTree1" class="tree-input" placeholder="?">
          </div>
          <div style="font-size:0.9rem; margin-top:6px;">Viết gọn: <span class="p-tag">12 = 2² . ?</span></div>
          <button class="tree-btn" onclick="checkTree(1, 3, 'Chính xác! 6 = 2 . 3 ➔ Vậy 12 = 2 . 2 . 3 = 2² . 3')">Kiểm tra</button>
          <div class="lab-feedback" id="fbTree1"></div>
        </div>

        <!-- Cây sơ đồ 2: Phân tích số 36 -->
        <div class="tree-card">
          <div style="font-weight:800; color:#065f46; margin-bottom:8px;">Sơ đồ B: Phân tích số 36</div>
          <div class="tree-node-root">36</div>
          <div class="tree-branches">/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; \</div>
          <div class="tree-row">
            <span class="node-comp">4</span>
            <span>×</span>
            <span class="node-comp">9</span>
          </div>
          <div class="tree-branches">/ &nbsp; \ &nbsp;&nbsp;&nbsp;&nbsp; / &nbsp; \</div>
          <div class="tree-row">
            <span class="node-prime">2</span>
            <span class="node-prime">2</span>
            <span class="node-prime">3</span>
            <input type="number" id="inpTree2" class="tree-input" placeholder="?">
          </div>
          <div style="font-size:0.9rem; margin-top:6px;">Viết gọn: <span class="p-tag">36 = 2² . 3²</span></div>
          <button class="tree-btn" onclick="checkTree(2, 3, 'Tuyệt vời! 9 = 3 . 3 ➔ Vậy 36 = 2² . 3²')">Kiểm tra</button>
          <div class="lab-feedback" id="fbTree2"></div>
        </div>
      </div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 3: ĐẤU TRƯỜNG TRÒ CHƠI TƯƠNG TÁC -->
<div class="emr-card">
  <div class="emr-card-head">
    <span>NỘI DUNG 3: ĐẤU TRƯỜNG NỐI CẶP & VẬN DỤNG TOÁN HỌC</span>
    <span class="emr-step-tag">Phần 3 / 3</span>
  </div>
  <div class="emr-card-body">

    <!-- VÒNG 1: TRÒ CHƠI NỐI CẶP -->
    <div class="emr-quest-box" style="margin-bottom: 18px;">
      <div class="emr-quest-title">VÒNG 1: GHÉP NỐI PHÂN TÍCH THỪA SỐ NGUYÊN TỐ (30 ĐIỂM — 10 Điểm / Cặp)</div>
      <p><b>Cách chơi:</b> Nhấn chọn một hợp số ở <b>CỘT A</b>, sau đó nhấn chọn dạng phân tích ra thừa số nguyên tố đúng chuẩn ở <b>CỘT B</b>.</p>

      <div class="match-grid">
        <div>
          <div class="match-head">CỘT A: HỢP SỐ</div>
          <div class="m-card" data-a="1" onclick="selA(this)">
            <span>1. Số 24</span>
            <span class="m-badge" id="bA-1"></span>
          </div>
          <div class="m-card" data-a="2" onclick="selA(this)">
            <span>2. Số 45</span>
            <span class="m-badge" id="bA-2"></span>
          </div>
          <div class="m-card" data-a="3" onclick="selA(this)">
            <span>3. Số 70</span>
            <span class="m-badge" id="bA-3"></span>
          </div>
        </div>

        <div>
          <div class="match-head">CỘT B: TÍCH THỪA SỐ NGUYÊN TỐ</div>
          <div class="m-card" data-b="2" onclick="selB(this)">
            <span>a) 3² . 5 (vì 9 . 5 = 45)</span>
            <span class="m-badge" id="bB-2"></span>
          </div>
          <div class="m-card" data-b="3" onclick="selB(this)">
            <span>b) 2 . 5 . 7 (vì 10 . 7 = 70)</span>
            <span class="m-badge" id="bB-3"></span>
          </div>
          <div class="m-card" data-b="1" onclick="selB(this)">
            <span>c) 2³ . 3 (vì 8 . 3 = 24)</span>
            <span class="m-badge" id="bB-1"></span>
          </div>
        </div>
      </div>

      <div id="matchMsg" style="margin-top:8px; font-weight:800; color:#047857;"></div>
      <button class="tree-btn" style="margin-top:8px;" onclick="resetMatching()">Chơi lại Vòng 1</button>
    </div>

    <!-- VÒNG 2: TRẮC NGHIỆM VẬN DỤNG -->
    <div class="emr-quest-box" style="margin-bottom:0;">
      <div class="emr-quest-title">VÒNG 2: BẮT BẪY TƯ DUY & TOÁN THỰC TẾ (30 ĐIỂM — 15 Điểm / Câu)</div>

      <div class="q-card" id="qc-1">
        <div class="q-title">Câu 1: Bạn Nam phân tích số 60 ra thừa số nguyên tố và viết kết quả là: 60 = 2² . 15. Theo em, kết quả của bạn Nam đã đúng chuẩn chưa?</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Bị lừa rồi! Tuy 4 . 15 = 60, nhưng số 15 là HỢP SỐ (15 = 3 . 5), chưa phải là thừa số nguyên tố!')">A. Đúng hoàn toàn vì 2² . 15 = 60</button>
          <button class="q-btn" onclick="ansQuiz(1, this, true, 'CHÍNH XÁC (+15 Điểm)! Số 15 vẫn là hợp số. Phải tách tiếp 15 = 3 . 5 để được kết quả chuẩn là: 60 = 2² . 3 . 5.')">B. Chưa đúng vì 15 là hợp số (Đúng phải là 2² . 3 . 5)</button>
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Sai rồi! Số 2 là số nguyên tố chẵn duy nhất nên 2² hoàn toàn hợp lệ.')">C. Sai vì không được dùng số chẵn 2</button>
        </div>
        <div class="q-exp" id="qexp-1"></div>
      </div>

      <div class="q-card" id="qc-2" style="margin-bottom:0;">
        <div class="q-title">Câu 2 (Toán thực tế): Cô giáo có 19 quyển vở thưởng và muốn chia đều vào các phần quà (mỗi phần quà có nhiều hơn 1 quyển vở và số phần quà phải nhiều hơn 1). Hỏi cô giáo có thực hiện được không?</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(2, this, true, 'XUẤT SẮC (+15 Điểm)! Vì 19 là SỐ NGUYÊN TỐ nên chỉ có 2 ước là 1 và 19 (chỉ xếp được 1 túi 19 quyển hoặc 19 túi mỗi túi 1 quyển). Do đó không thể chia thành các phần quà nhiều hơn 1 quyển!')">A. Không thể chia được vì 19 là số nguyên tố</button>
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Thử kiểm tra lại nhé! 19 không hề chia hết cho 3.')">B. Chia được thành 3 phần quà</button>
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Thử kiểm tra lại nhé! 19 là số lẻ nên không chia hết cho 2.')">C. Chia được thành 2 phần quà</button>
        </div>
        <div class="q-exp" id="qexp-2"></div>
      </div>

    </div>

  </div>
</div>

<!-- BẢNG TỔNG KẾT SIÊU NGẮN GỌN -->
<div class="emr-card" style="margin-bottom:0;">
  <div class="emr-card-head">
    <span>BẢNG TÓM TẮT CỐT LÕI BÀI 10: SỐ NGUYÊN TỐ</span>
    <span class="emr-step-tag">Ôn tập nhanh</span>
  </div>
  <div class="emr-card-body">
    <table class="emr-table">
      <thead>
        <tr>
          <th width="28%">Khái niệm</th>
          <th width="37%">Bản chất cốt lõi</th>
          <th width="35%">Ví dụ / Lưu ý trọng tâm</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><b>Số nguyên tố</b></td>
          <td>Số tự nhiên <span class="p-tag">&gt; 1</span>, chỉ có <b>đúng 2 ước</b> (1 và chính nó).</td>
          <td><span class="p-tag">2; 3; 5; 7; 11; 13; 17; 19; ...</span><br><i>(Số 2 là số nguyên tố chẵn duy nhất)</i>.</td>
        </tr>
        <tr>
          <td><b>Hợp số</b></td>
          <td>Số tự nhiên <span class="p-tag">&gt; 1</span>, có <b>nhiều hơn 2 ước</b>.</td>
          <td><span class="p-tag">4; 6; 8; 9; 10; 12; 15; ...</span></td>
        </tr>
        <tr>
          <td><b>Số đặc biệt (0 và 1)</b></td>
          <td><b>Không</b> là số nguyên tố, <b>không</b> là hợp số.</td>
          <td>Luôn loại trừ số <span class="p-tag">0</span> và <span class="p-tag">1</span> khi tìm số nguyên tố.</td>
        </tr>
        <tr>
          <td><b>Phân tích ra thừa số nguyên tố</b></td>
          <td>Viết số đó dưới dạng <b>tích các thừa số nguyên tố</b> (thu gọn bằng lũy thừa).</td>
          <td><span class="p-tag">24 = 2³ . 3</span><br><span class="p-tag">60 = 2² . 3 . 5</span></td>
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

  // ĐIỂM SỐ
  let totalPts = 0;
  function addScore(val) {
    totalPts += val;
    document.getElementById('ptsVal').textContent = totalPts;
    if (totalPts === 100) setTimeout(sfxWin, 300);
  }

  // LOGIC TRẠM 1: SĂN SỐ NGUYÊN TỐ
  let foundPrimes = 0;
  let donePrimes = false;
  function pickPrime(el, isPrime, msg) {
    if (el.classList.contains('correct') || el.classList.contains('wrong') || donePrimes) return;
    const msgBox = document.getElementById('msgPrime');
    msgBox.textContent = msg;
    if (isPrime) {
      sfxOk();
      el.classList.add('correct');
      msgBox.style.color = '#047857';
      foundPrimes++;
      if (foundPrimes === 5) {
        donePrimes = true;
        addScore(20);
        msgBox.textContent = 'HOÀN HẢO (+20 Điểm)! Bạn đã lọc chính xác cả 5 số nguyên tố: 2, 3, 5, 11, 17.';
      }
    } else {
      sfxErr();
      el.classList.add('wrong');
      msgBox.style.color = '#9f1239';
    }
  }

  // LOGIC TRẠM 2: CÂY NHÂN TỬ
  const treeDone = {};
  function checkTree(id, ans, okText) {
    if (treeDone[id]) return;
    const val = parseInt(document.getElementById('inpTree' + id).value, 10);
    const fb = document.getElementById('fbTree' + id);
    if (val === ans) {
      sfxOk();
      fb.style.color = '#047857';
      fb.textContent = okText + ' (+10 Điểm)';
      treeDone[id] = true;
      addScore(10);
    } else {
      sfxErr();
      fb.style.color = '#9f1239';
      fb.textContent = 'Chưa đúng! Hãy điền một số nguyên tố sao cho tích đúng bằng nhánh phía trên nhé!';
    }
  }

  // LOGIC VÒNG 1: NỐI CẶP
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
      addScore(10);
      if (pairsCount === 3) {
        document.getElementById('matchMsg').textContent = 'Hoàn thành xuất sắc cả 3 cặp phân tích thừa số nguyên tố (+30 Điểm)!';
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
    addScore(-(pairsCount * 10));
    pairsCount = 0;
    currA = null;
    document.getElementById('matchMsg').textContent = '';
    document.querySelectorAll('.m-card').forEach(x => x.classList.remove('matched', 'selected', 'wrong'));
  }

  // LOGIC VÒNG 2: TRẮC NGHIỆM
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
      addScore(15);
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
