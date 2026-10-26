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

  /* Khung Lý thuyết cô đọng */
  .sky-theory-box { background: #f0f9ff; border: 1.5px solid #7dd3fc; border-left: 6px solid #0284c7; border-radius: 12px; padding: 18px 20px; margin-bottom: 20px; }
  .sky-theory-head { font-weight: 800; color: #0369a1; font-size: 1.05rem; margin-bottom: 12px; text-transform: uppercase; letter-spacing: 0.3px; border-bottom: 1.5px solid #bae6fd; padding-bottom: 6px; }
  .sky-theory-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 14px; margin-top: 10px; }
  .sky-mini-card { background: #ffffff; border: 1px solid #bae6fd; border-radius: 10px; padding: 14px 16px; }
  .sky-mini-title { font-weight: 800; color: #0284c7; margin-bottom: 6px; font-size: 0.98rem; }
  .sky-warn-strip { background: #fef9c3; border: 1px solid #fde047; border-left: 5px solid #eab308; border-radius: 8px; padding: 12px 16px; margin-top: 14px; color: #713f12; font-size: 0.95rem; }

  /* Bảng quy trình */
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
  <div class="sky-topbar-title">TOÁN 6 — BÀI 12: BỘI CHUNG. BỘI CHUNG NHỎ NHẤT</div>
  <div class="sky-topbar-right">
    <div class="sky-score-badge">ĐIỂM KHÁM PHÁ: <span id="ptsVal">0</span> / 100</div>
    <button class="sky-sound-btn" id="btnSound" onclick="toggleSound()">Âm thanh: ĐANG BẬT</button>
  </div>
</div>

<!-- BANNER MỞ ĐẦU -->
<div class="sky-hero">
  <div class="sky-hero-tag">CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN</div>
  <h1 class="sky-hero-title">BÀI 12: BỘI CHUNG. BỘI CHUNG NHỎ NHẤT</h1>
  <div class="sky-meta-row">
    <div class="sky-meta-item">Toán 6 (Tập 1) — Kết nối tri thức với cuộc sống</div>
    <div class="sky-meta-item">Thời lượng: 45 – 60 phút (Lý thuyết cô đọng + Tương tác + Trò chơi)</div>
  </div>
</div>

<!-- NỘI DUNG 1: BỘI CHUNG VÀ BỘI CHUNG NHỎ NHẤT -->
<div class="sky-card">
  <div class="sky-card-head">
    <span>NỘI DUNG 1: BỘI CHUNG VÀ BỘI CHUNG NHỎ NHẤT (BCNN)</span>
    <span class="sky-step-tag">Phần 1 / 4</span>
  </div>
  <div class="sky-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="sky-theory-box">
      <div class="sky-theory-head">1. LÝ THUYẾT CỐT LÕI CẦN NHỚ</div>
      <div class="sky-theory-grid">
        <div class="sky-mini-card">
          <div class="sky-mini-title">BỘI CHUNG (BC)</div>
          Cho hai hay nhiều số:<br>
          • Bội chung của các số đó là <b>bội của tất cả</b> các số đó.<br>
          • Kí hiệu tập hợp bội chung của <i>a</i> và <i>b</i> là <span class="s-tag">BC(a, b)</span>.<br>
          • <span class="s-tag">x ∈ BC(a, b)</span> khi <span class="s-tag">x ⋮ a</span> và <span class="s-tag">x ⋮ b</span>.
        </div>
        <div class="sky-mini-card">
          <div class="sky-mini-title">BỘI CHUNG NHỎ NHẤT (BCNN)</div>
          • Bội chung nhỏ nhất của hai hay nhiều số là <b>số nhỏ nhất khác 0</b> trong tập hợp các bội chung của các số đó.<br>
          • Kí hiệu: <span class="s-tag">BCNN(a, b)</span>.<br>
          • <b>Mối liên hệ vàng:</b> Tất cả các bội chung của <i>a</i> và <i>b</i> đều là <b>bội của BCNN(a, b)</b>.
        </div>
      </div>
      <div class="sky-warn-strip">
        <b>Cách tìm nhanh BC thông qua BCNN:</b><br>
        Muốn tìm tập hợp <span class="s-tag">BC(a, b)</span>, ta chỉ cần tìm các bội của <span class="s-tag">BCNN(a, b)</span> (nhân BCNN lần lượt với 0, 1, 2, 3, ...).
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ 1 -->
    <div class="sky-quest-box">
      <div class="sky-quest-title">TRẠM KHÁM PHÁ 1: SĂN TÌM CÁC BỘI CHUNG NHỎ HƠN 40 CỦA 4 VÀ 6 (+15 ĐIỂM)</div>
      <p><b>Nhiệm vụ:</b> Cho tập hợp <span class="s-tag">B(4) = {0; 4; 8; 12; 16; 20; 24; 28; 32; 36; ...}</span> và <span class="s-tag">B(6) = {0; 6; 12; 18; 24; 30; 36; 42; ...}</span>.<br>Hãy <b>bấm chọn đúng 4 số thuộc tập hợp BC(4, 6) nhỏ hơn 40</b>:</p>
      <div class="chip-grid" id="bcGrid">
        <div class="num-chip" onclick="pickBC(this, true, 'Chính xác! Số 0 luôn là bội chung của mọi số tự nhiên.')">Số 0</div>
        <div class="num-chip" onclick="pickBC(this, false, 'Sai rồi! 4 có chia hết cho 6 đâu.')">Số 4</div>
        <div class="num-chip" onclick="pickBC(this, true, 'Chính xác! 12 vừa chia hết cho 4, vừa chia hết cho 6.')">Số 12</div>
        <div class="num-chip" onclick="pickBC(this, false, 'Sai rồi! 18 chia hết cho 6 nhưng không chia hết cho 4.')">Số 18</div>
        <div class="num-chip" onclick="pickBC(this, true, 'Chính xác! 24 chia hết cho cả 4 và 6 (chính là BCNN nhỏ nhất khác 0).')">Số 24</div>
        <div class="num-chip" onclick="pickBC(this, false, 'Sai rồi! 30 chia hết cho 6 nhưng không chia hết cho 4.')">Số 30</div>
        <div class="num-chip" onclick="pickBC(this, true, 'Xuất sắc! 36 chia hết cho cả 4 và 6 (36 = 12 . 3).')">Số 36</div>
      </div>
      <div id="msgBC" style="font-weight:700; color:#0369a1; font-size:0.93rem; min-height:22px;"></div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 2: QUY TẮC 3 BƯỚC TÌM BCNN -->
<div class="sky-card">
  <div class="sky-card-head">
    <span>NỘI DUNG 2: QUY TẮC 3 BƯỚC TÌM BỘI CHUNG NHỎ NHẤT</span>
    <span class="sky-step-tag">Phần 2 / 4</span>
  </div>
  <div class="sky-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="sky-theory-box">
      <div class="sky-theory-head">2. BẢNG QUY TRÌNH 3 BƯỚC TÌM BCNN (KHI SỐ LỚN)</div>
      <table class="sky-table">
        <thead>
          <tr>
            <th width="18%">Bước</th>
            <th width="45%">Quy tắc thực hiện</th>
            <th width="37%">Ví dụ mẫu: Tìm BCNN(24, 36)</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><b>Bước 1</b></td>
            <td>Phân tích mỗi số ra <b>thừa số nguyên tố</b>.</td>
            <td>• <span class="s-tag">24 = 2³ . 3</span><br>• <span class="s-tag">36 = 2² . 3²</span></td>
          </tr>
          <tr>
            <td><b>Bước 2</b></td>
            <td>Chọn ra các thừa số nguyên tố <b>CHUNG và RIÊNG</b>.</td>
            <td>Thừa số chung và riêng là: <span class="s-tag">2</span> và <span class="s-tag">3</span>.</td>
          </tr>
          <tr>
            <td><b>Bước 3</b></td>
            <td>Lập tích các thừa số đã chọn, mỗi thừa số lấy với <b>số mũ LỚN NHẤT</b> của nó. Tích đó là <b>BCNN</b>.</td>
            <td>• Số mũ lớn nhất của 2 là <span class="s-tag">2³</span>; của 3 là <span class="s-tag">3²</span>.<br>➔ <span class="s-tag">BCNN(24, 36) = 2³ . 3² = 72</span>.</td>
          </tr>
        </tbody>
      </table>
      <div class="sky-warn-strip">
        <b>Nhận xét đặc biệt giúp nhẩm nhanh BCNN:</b><br>
        • Nếu các số đã cho là đôi một nguyên tố cùng nhau (ví dụ: <span class="s-tag">BCNN(3, 5, 7)</span>) thì BCNN chính là tích của chúng.<br>
        • <b>Trường hợp chia hết:</b> Nếu số lớn chia hết cho số nhỏ (như <span class="s-tag">72 ⋮ 24</span>) thì số lớn chính là BCNN (<span class="s-tag">BCNN(72, 24) = 72</span>).
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ 2 -->
    <div class="sky-quest-box">
      <div class="sky-quest-title">TRẠM KHÁM PHÁ 2: PHÒNG THÍ NGHIỆM 3 BƯỚC TÌM BCNN (+20 ĐIỂM)</div>
      <div class="lab-grid">
        <div class="lab-box">
          <b>Thí nghiệm A: Tính BCNN(12, 18)</b><br>
          Phân tích: <span class="s-tag">12 = 2² . 3</span> và <span class="s-tag">18 = 2 . 3²</span>.<br>
          Lấy thừa số chung và riêng với số mũ lớn nhất: <span class="s-tag">2² . 3²</span> bằng bao nhiêu?
          <div class="lab-row-inp">
            <span>BCNN(12, 18) = </span>
            <input type="number" id="inpLabA" class="sky-input" placeholder="?">
            <button class="sky-btn" onclick="checkLab('A', 36, 'Chính xác! 4 . 9 = 36. Vậy BCNN(12, 18) = 36!')">Kiểm tra</button>
          </div>
          <div class="lab-msg" id="msgLabA"></div>
        </div>

        <div class="lab-box">
          <b>Thí nghiệm B: Nhẩm nhanh BCNN đặc biệt</b><br>
          Không cần phân tích, hãy cho biết <span class="s-tag">BCNN(15, 60)</span> bằng bao nhiêu <i>(Gợi ý: 60 ⋮ 15)</i>?
          <div class="lab-row-inp">
            <span>BCNN(15, 60) = </span>
            <input type="number" id="inpLabB" class="sky-input" placeholder="?">
            <button class="sky-btn" onclick="checkLab('B', 60, 'Tuyệt vời! Vì 60 chia hết cho 15 nên số lớn hơn (60) chính là BCNN!')">Kiểm tra</button>
          </div>
          <div class="lab-msg" id="msgLabB"></div>
        </div>
      </div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 3: QUY ĐỒNG MẪU SỐ & BÀI TOÁN THỰC TIỄN -->
<div class="sky-card">
  <div class="sky-card-head">
    <span>NỘI DUNG 3: QUY ĐỒNG MẪU SỐ NHIỀU PHÂN SỐ & TOÁN THỰC TẾ</span>
    <span class="sky-step-tag">Phần 3 / 4</span>
  </div>
  <div class="sky-card-body">

    <!-- LÝ THUYẾT NGẮN GỌN TRƯỚC TRẠM KHÁM PHÁ -->
    <div class="sky-theory-box">
      <div class="sky-theory-head">3. ỨNG DỤNG CỦA BCNN TRONG QUY ĐỒNG VÀ THỰC TIỄN</div>
      <div class="sky-theory-grid">
        <div class="sky-mini-card">
          <div class="sky-mini-title">QUY ĐỒNG MẪU SỐ NHIỀU PHÂN SỐ</div>
          Thay vì nhân chéo phức tạp, ta dùng BCNN làm <b>mẫu số chung</b> để quy đồng mẫu các phân số.<br>
          • <i>Mẫu chung nhỏ nhất</i> giúp các tính toán tiếp theo trở nên đơn giản nhất.
        </div>
        <div class="sky-mini-card">
          <div class="sky-mini-title">NHẬN DIỆN BÀI TOÁN DÙNG BCNN</div>
          • Đề bài nhắc đến các sự việc lặp đi lặp lại theo chu kì và hỏi <b>"khi nào chúng cùng gặp lại nhau / cùng phát sáng / cùng xuất phát"</b>.<br>
          ➔ Thời gian gặp lại đầu tiên chính là <span class="s-tag">BCNN</span> của các chu kì!
        </div>
      </div>
    </div>

    <!-- TRẠM KHÁM PHÁ 3 -->
    <div class="sky-quest-box">
      <div class="sky-quest-title">TRẠM KHÁM PHÁ 3: PHÂN LOẠI NHANH BÀI TOÁN (ƯCLN HAY BCNN?) (+15 ĐIỂM)</div>
      <p><b>Nhiệm vụ:</b> Bấm chọn xem mỗi tình huống thực tế sau đây sử dụng công cụ <b>ƯCLN</b> hay <b>BCNN</b> để giải quyết:</p>

      <div class="sort-item" id="sbox-1">
        <div class="sort-expr">1) Chia đều số bút và vở vào các túi quà sao cho số túi là NHIỀU NHẤT.</div>
        <div class="sort-btns">
          <button class="s-btn" onclick="sortCheck(1, this, true, 'Chính xác (+5 Điểm)! Bài toán chia đều, số nhóm lớn nhất dùng ƯCLN.')">Dùng ƯCLN</button>
          <button class="s-btn" onclick="sortCheck(1, this, false, 'Nhầm rồi! Chia đều số lượng đồ vật vào các nhóm lớn nhất phải dùng ƯCLN.')">Dùng BCNN</button>
        </div>
        <div class="sort-fb" id="sfb-1"></div>
      </div>

      <div class="sort-item" id="sbox-2">
        <div class="sort-expr">2) Hai xe buýt cùng xuất phát bến, xe A cứ 10 phút chạy 1 chuyến, xe B cứ 15 phút chạy 1 chuyến. Hỏi sau bao lâu hai xe lại cùng xuất phát lần tiếp theo?</div>
        <div class="sort-btns">
          <button class="s-btn" onclick="sortCheck(2, this, false, 'Sai rồi! Bài toán sự việc lặp lại cùng lúc dùng BCNN.')">Dùng ƯCLN</button>
          <button class="s-btn" onclick="sortCheck(2, this, true, 'Chính xác (+5 Điểm)! Bài toán sự việc cùng lặp lại dùng BCNN(10, 15) = 30 phút.')">Dùng BCNN</button>
        </div>
        <div class="sort-fb" id="sfb-2"></div>
      </div>

      <div class="sort-item" id="sbox-3" style="margin-bottom:0;">
        <div class="sort-expr">3) Quy đồng mẫu số hai phân số 5/12 và 7/18 để thực hiện phép cộng.</div>
        <div class="sort-btns">
          <button class="s-btn" onclick="sortCheck(3, this, false, 'Sai rồi! Tìm mẫu chung nhỏ nhất chính là đi tìm BCNN(12, 18) = 36.')">Dùng ƯCLN</button>
          <button class="s-btn" onclick="sortCheck(3, this, true, 'ĐỈNH CAO (+5 Điểm)! Mẫu chung nhỏ nhất chính là BCNN(12, 18) = 36.')">Dùng BCNN</button>
        </div>
        <div class="sort-fb" id="sfb-3"></div>
      </div>
    </div>

  </div>
</div>

<!-- NỘI DUNG 4: ĐẤU TRƯỜNG TRÒ CHƠI & BÀI TOÁN THỰC TIỄN -->
<div class="sky-card">
  <div class="sky-card-head">
    <span>NỘI DUNG 4: ĐẤU TRƯỜNG NỐI CẶP, TRẮC NGHIỆM & TOÁN THỰC TẾ</span>
    <span class="sky-step-tag">Phần 4 / 4</span>
  </div>
  <div class="sky-card-body">

    <!-- VÒNG 1: TRÒ CHƠI NỐI CẶP (20 ĐIỂM) -->
    <div class="sky-quest-box" style="margin-bottom:20px;">
      <div class="sky-quest-title">VÒNG 1: GHÉP NỐI TỐC ĐỘ (20 ĐIỂM — 5 Điểm / Cặp)</div>
      <p><b>Cách chơi:</b> Nhấn chọn một yêu cầu ở <b>CỘT A</b>, sau đó nhấn chọn kết quả tương ứng ở <b>CỘT B</b> để nối chúng lại với nhau.</p>

      <div class="match-grid">
        <div>
          <div class="match-head">CỘT A: BÀI TOÁN</div>
          <div class="m-card" data-a="1" onclick="selA(this)">
            <span>1. BCNN(10, 15)</span>
            <span class="m-badge" id="bA-1"></span>
          </div>
          <div class="m-card" data-a="2" onclick="selA(this)">
            <span>2. BCNN(8, 12)</span>
            <span class="m-badge" id="bA-2"></span>
          </div>
          <div class="m-card" data-a="3" onclick="selA(this)">
            <span>3. BCNN(4, 6, 12)</span>
            <span class="m-badge" id="bA-3"></span>
          </div>
          <div class="m-card" data-a="4" onclick="selA(this)">
            <span>4. Tập hợp BC(4, 6) nhỏ hơn 40</span>
            <span class="m-badge" id="bA-4"></span>
          </div>
        </div>

        <div>
          <div class="match-head">CỘT B: ĐÁP ÁN</div>
          <div class="m-card" data-b="3" onclick="selB(this)">
            <span>a) Bằng 12 (vì 12 chia hết cho cả 4 và 6)</span>
            <span class="m-badge" id="bB-3"></span>
          </div>
          <div class="m-card" data-b="1" onclick="selB(this)">
            <span>b) Bằng 30 (vì 30 là bội chung nhỏ nhất khác 0)</span>
            <span class="m-badge" id="bB-1"></span>
          </div>
          <div class="m-card" data-b="4" onclick="selB(this)">
            <span>c) {0; 12; 24; 36} (các bội của 12)</span>
            <span class="m-badge" id="bB-4"></span>
          </div>
          <div class="m-card" data-b="2" onclick="selB(this)">
            <span>d) Bằng 24 (vì 24 = 2³ . 3)</span>
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
        <div class="q-title">Câu 1: Cho hai số a = 2³ . 3 . 5 và b = 2² . 3² . 7. Bội chung nhỏ nhất của a và b là:</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Sai rồi! Bạn đã lấy số mũ nhỏ nhất mất rồi (phải lấy số mũ LỚN NHẤT).')">A. 2² . 3 . 5 . 7</button>
          <button class="q-btn" onclick="ansQuiz(1, this, true, 'CHÍNH XÁC (+10 Điểm)! Lấy thừa số chung và riêng (2, 3, 5, 7) với số mũ LỚN NHẤT là 2³ . 3² . 5 . 7.')">B. 2³ . 3² . 5 . 7</button>
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Chưa chính xác! Bạn đã bỏ quên các thừa số riêng là 5 và 7.')">C. 2³ . 3² = 72</button>
        </div>
        <div class="q-exp" id="qexp-1"></div>
      </div>

      <div class="q-card" id="qc-2">
        <div class="q-title">Câu 2: Tìm số tự nhiên x nhỏ nhất khác 0 biết rằng x chia hết cho 12, x chia hết cho 15 và x chia hết cho 18:</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Sai rồi! 90 không chia hết cho 12 (90 : 12 = 7,5).')">A. x = 90</button>
          <button class="q-btn" onclick="ansQuiz(2, this, true, 'XUẤT SẮC (+10 Điểm)! Số x nhỏ nhất khác 0 chia hết cho cả 12, 15, 18 chính là BCNN(12, 15, 18) = 180.')">B. x = 180</button>
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Sai rồi! 360 tuy chia hết nhưng chưa phải là số NHỎ NHẤT.')">C. x = 360</button>
        </div>
        <div class="q-exp" id="qexp-2"></div>
      </div>

      <div class="q-card" id="qc-3" style="margin-bottom:0;">
        <div class="q-title">Câu 3 (Toán thực tế đèn tín hiệu): Hai ngọn đèn hải đăng bắt đầu cùng phát sáng vào lúc 6 giờ tối. Đèn thứ nhất cứ sau mỗi 6 giây lại phát sáng một lần, đèn thứ hai cứ sau mỗi 8 giây lại phát sáng một lần. Hỏi sau ít nhất bao nhiêu giây thì hai ngọn đèn lại cùng phát sáng lần tiếp theo?</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(3, this, false, 'Chưa đúng! 14 giây không chia hết cho 8.')">A. 14 giây</button>
          <button class="q-btn" onclick="ansQuiz(3, this, true, 'ĐỈNH CAO (+10 Điểm)! Thời gian hai đèn cùng phát sáng lần tiếp theo chính là BCNN(6, 8) = 24 giây.')">B. 24 giây</button>
          <button class="q-btn" onclick="ansQuiz(3, this, false, 'Sai rồi! 48 giây là bội chung nhưng chưa phải là thời gian ÍT NHẤT.')">C. 48 giây</button>
        </div>
        <div class="q-exp" id="qexp-3"></div>
      </div>
    </div>

    <!-- VÒNG 3: BÀI TOÁN TỰ LUẬN & THỰC TIỄN -->
    <div class="sky-quest-box" style="margin-bottom:0;">
      <div class="sky-quest-title">VÒNG 3: CHINH PHỤC TOÁN THỰC TIỄN & NÂNG CAO (LÀM VÀO VỞ)</div>
      <ul>
        <li><b>Bài toán 1 (Tìm BC thông qua BCNN):</b> Tìm tập hợp các bội chung của 12 và 15 mà nhỏ hơn 300.</li>
        <li><b>Bài toán 2 (Bài toán số học sinh xếp hàng):</b> Số học sinh khối 6 của một trường khi xếp hàng 12, hàng 15 hay hàng 18 đều vừa đủ hàng. Tính số học sinh khối 6 biết rằng số học sinh đó trong khoảng từ 300 đến 400 em.</li>
      </ul>

      <details class="sky-details" onclick="sfxClick()">
        <summary>[ NHẤN ĐỂ MỞ KHÓA LỜI GIẢI TRÌNH BÀY MẪU VÒNG 3 ]</summary>
        <div class="sky-details-body">
          <p><b>Lời giải Bài toán 1:</b></p>
          <ul>
            <li>Phân tích ra thừa số nguyên tố: <span class="s-tag">12 = 2² . 3</span> và <span class="s-tag">15 = 3 . 5</span>.</li>
            <li>Tìm BCNN: <span class="s-tag">BCNN(12, 15) = 2² . 3 . 5 = 60</span>.</li>
            <li>Tập hợp bội chung là bội của 60: <span class="s-tag">BC(12, 15) = {0; 60; 120; 180; 240; 300; 360; ...}</span>.</li>
            <li>Vì đề yêu cầu nhỏ hơn 300, ta chọn các số: <span class="s-tag">{0; 60; 120; 180; 240}</span>.</li>
          </ul>
          <hr style="margin:12px 0; border:0; border-top:1px solid #bae6fd;">
          <p><b>Lời giải Bài toán 2:</b></p>
          <ul>
            <li>Gọi số học sinh khối 6 là <i>x</i> (học sinh) với điều kiện <span class="s-tag">300 ≤ x ≤ 400</span>.</li>
            <li>Vì khi xếp hàng 12, 15, 18 đều vừa đủ nên <span class="s-tag">x ⋮ 12</span>, <span class="s-tag">x ⋮ 15</span> và <span class="s-tag">x ⋮ 18</span>, suy ra <span class="s-tag">x ∈ BC(12, 15, 18)</span>.</li>
            <li>Phân tích: <span class="s-tag">12 = 2² . 3</span>; <span class="s-tag">15 = 3 . 5</span>; <span class="s-tag">18 = 2 . 3²</span> ➔ <span class="s-tag">BCNN(12, 15, 18) = 2² . 3² . 5 = 180</span>.</li>
            <li>Tập hợp bội chung là: <span class="s-tag">BC(12, 15, 18) = {0; 180; 360; 540; ...}</span>.</li>
            <li>Kết hợp điều kiện <span class="s-tag">300 ≤ x ≤ 400</span>, ta chọn được <span class="s-tag">x = 360</span>.</li>
            <li><b>Kết luận:</b> Số học sinh khối 6 của trường đó là <b>360 học sinh</b>.</li>
          </ul>
        </div>
      </details>
    </div>

  </div>
</div>

<!-- BẢNG TÓM TẮT CỐT LÕI BÀI 12 -->
<div class="sky-card" style="margin-bottom:0;">
  <div class="sky-card-head">
    <span>SƠ ĐỒ TỔNG KẾT KIẾN THỨC CỐT LÕI BÀI 12</span>
    <span class="sky-step-tag">Ôn tập nhanh</span>
  </div>
  <div class="sky-card-body">
    <table class="sky-table">
      <thead>
        <tr>
          <th width="50%">NHÁNH 1: KHÁI NIỆM BỘI CHUNG & BCNN</th>
          <th width="50%">NHÁNH 2: QUY TẮC TÌM BCNN & ỨNG DỤNG</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>
            • <b>Bội chung (BC):</b> Là bội của tất cả các số cho trước (<span class="s-tag">x ⋮ a</span> và <span class="s-tag">x ⋮ b</span>).<br><br>
            • <b>Cách tìm BC:</b> Tìm thông qua BCNN bằng cách nhân BCNN với <span class="s-tag">0, 1, 2, 3, ...</span>.
          </td>
          <td>
            • <b>Quy tắc 3 bước tìm BCNN:</b><br>
            1. Phân tích ra thừa số nguyên tố.<br>
            2. Chọn thừa số nguyên tố <b>chung và riêng</b>.<br>
            3. Lập tích với số mũ <b>lớn nhất</b>.<br><br>
            • <b>Nhận diện bài toán thực tế dùng BCNN:</b> Đề bài hỏi thời điểm các sự việc <b>cùng lặp lại, cùng gặp nhau</b>.
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

  // LOGIC TRẠM 1: SĂN BỘI CHUNG BC(4, 6) (15 ĐIỂM)
  let foundBC = 0;
  let doneBC = false;
  function pickBC(el, isRight, msg) {
    if (el.classList.contains('correct') || el.classList.contains('wrong') || doneBC) return;
    const box = document.getElementById('msgBC');
    box.textContent = msg;
    if (isRight) {
      sfxOk();
      el.classList.add('correct');
      box.style.color = '#0369a1';
      foundBC++;
      if (foundBC === 4) {
        doneBC = true;
        addScore(15);
        box.textContent = 'HOÀN HẢO (+15 Điểm)! Các bội chung nhỏ hơn 40 của 4 và 6 là: {0; 12; 24; 36}.';
      }
    } else {
      sfxErr();
      el.classList.add('wrong');
      box.style.color = '#9f1239';
    }
  }

  // LOGIC TRẠM 2: PHÒNG THÍ NGHIỆM BCNN (20 ĐIỂM)
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
      fb.textContent = 'Chưa chính xác, hãy kiểm tra lại phép tính lũy thừa số mũ lớn nhất nhé!';
    }
  }

  // LOGIC TRẠM 3: PHÂN LOẠI NHANH BÀI TOÁN (15 ĐIỂM — 3 CÂU x 5 ĐIỂM)
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
