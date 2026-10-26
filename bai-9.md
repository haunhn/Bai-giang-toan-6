<style>
  /* Ẩn tiêu đề mặc định của GitHub Pages & Thiết lập nền Vàng nhạt */
  .markdown-body > h1:first-child { display: none !important; }
  .container-lg, .markdown-body { max-width: 960px !important; margin: 0 auto !important; padding: 16px !important; font-family: 'Segoe UI', system-ui, -apple-system, sans-serif !important; color: #422006 !important; background-color: #fefce8 !important; }
  body { background-color: #fefce8 !important; }

  /* Thanh điều khiển cố định (Sticky Bar) */
  .amb-topbar { position: sticky; top: 10px; z-index: 999; background: #ffffff; border: 2px solid #f59e0b; border-radius: 12px; padding: 10px 20px; margin-bottom: 24px; display: flex; justify-content: space-between; align-items: center; box-shadow: 0 8px 20px rgba(217, 119, 6, 0.12); flex-wrap: wrap; gap: 10px; }
  .amb-topbar-title { font-weight: 800; color: #92400e; font-size: 0.98rem; letter-spacing: 0.3px; }
  .amb-topbar-right { display: flex; align-items: center; gap: 12px; }
  .amb-score-badge { background: #fef3c7; color: #b45309; border: 1.5px solid #f59e0b; padding: 5px 16px; border-radius: 99px; font-weight: 800; font-size: 0.95rem; }
  .amb-sound-btn { background: #d97706; color: #ffffff; border: none; padding: 7px 15px; border-radius: 8px; font-weight: 700; cursor: pointer; font-size: 0.88rem; transition: 0.2s; }
  .amb-sound-btn:hover { background: #b45309; }

  /* Khung Banner chính */
  .amb-hero { background: linear-gradient(135deg, #fef3c7 0%, #fde68a 100%); border: 2px solid #f59e0b; border-radius: 16px; padding: 28px 24px; text-align: center; margin-bottom: 26px; box-shadow: 0 8px 22px rgba(217, 119, 6, 0.1); }
  .amb-hero-tag { display: inline-block; background: #d97706; color: #ffffff; font-weight: 800; font-size: 0.82rem; padding: 5px 16px; border-radius: 99px; text-transform: uppercase; letter-spacing: 0.7px; margin-bottom: 10px; }
  .amb-hero-title { color: #78350f !important; font-size: 1.95rem !important; font-weight: 800 !important; margin: 0 0 14px 0 !important; border: none !important; padding: 0 !important; }
  .amb-meta-row { display: flex; justify-content: center; flex-wrap: wrap; gap: 10px; }
  .amb-meta-item { background: #ffffff; border: 1px solid #fcd34d; color: #92400e; padding: 5px 14px; border-radius: 8px; font-size: 0.9rem; font-weight: 600; }

  /* Hệ thống Khung bài giảng (Section Frames) */
  .amb-card { background: #ffffff; border: 2px solid #fde68a; border-radius: 16px; margin-bottom: 26px; overflow: hidden; box-shadow: 0 5px 15px rgba(217, 119, 6, 0.06); }
  .amb-card-head { background: linear-gradient(90deg, #fef3c7 0%, #fde68a 100%); border-bottom: 2px solid #fcd34d; padding: 14px 22px; color: #78350f; font-size: 1.18rem; font-weight: 800; display: flex; justify-content: space-between; align-items: center; }
  .amb-step-tag { background: #d97706; color: #fff; font-size: 0.78rem; padding: 3px 10px; border-radius: 12px; font-weight: 700; }
  .amb-card-body { padding: 22px; line-height: 1.65; font-size: 1rem; }

  /* Khung bài tập dẫn dắt (Interactive Discovery Box) */
  .amb-quest-box { background: #fffbeb; border: 1.5px dashed #f59e0b; border-radius: 12px; padding: 18px; margin-bottom: 16px; }
  .amb-quest-title { font-weight: 800; color: #b45309; margin-bottom: 10px; font-size: 1.02rem; text-transform: uppercase; }

  /* Các nút chọn số tương tác (Number Chips) */
  .chip-grid { display: flex; flex-wrap: wrap; gap: 10px; margin: 12px 0; }
  .num-chip { background: #ffffff; border: 2px solid #fcd34d; color: #78350f; padding: 10px 18px; border-radius: 10px; font-weight: 800; font-size: 1.05rem; cursor: pointer; transition: 0.2s; user-select: none; }
  .num-chip:hover { background: #fef3c7; border-color: #d97706; transform: translateY(-2px); }
  .num-chip.correct { background: #dcfce7; border-color: #16a34a; color: #166534; }
  .num-chip.wrong { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }

  /* Ô nhập liệu khám phá (Interactive Input) */
  .lab-row { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 14px; margin: 14px 0; }
  .lab-card { background: #ffffff; border: 1.5px solid #fde68a; border-radius: 10px; padding: 14px; }
  .lab-input-group { display: flex; align-items: center; gap: 8px; margin-top: 8px; }
  .lab-input { width: 80px; padding: 7px 10px; border: 2px solid #fcd34d; border-radius: 8px; font-weight: 800; text-align: center; font-size: 1rem; color: #78350f; outline: none; }
  .lab-input:focus { border-color: #d97706; background: #fffbeb; }
  .lab-btn { background: #d97706; color: #ffffff; border: none; padding: 8px 14px; border-radius: 8px; font-weight: 700; cursor: pointer; transition: 0.2s; }
  .lab-btn:hover { background: #b45309; }
  .lab-feedback { font-size: 0.9rem; font-weight: 700; margin-top: 8px; min-height: 22px; }

  /* Hộp chốt kiến thức (Rút gọn, mở khóa sau khi khám phá) */
  .amb-rule-box { background: #fef3c7; border-left: 6px solid #d97706; border-radius: 10px; padding: 16px 20px; margin-top: 14px; color: #78350f; }
  .amb-rule-title { font-weight: 800; color: #92400e; margin-bottom: 6px; text-transform: uppercase; font-size: 0.95rem; }
  .k-tag { background: #ffffff; color: #b45309; border: 1px solid #f59e0b; padding: 1px 8px; border-radius: 6px; font-family: 'Consolas', monospace; font-weight: 800; font-size: 0.95em; display: inline-block; }

  /* Bảng tổng kết gọn đẹp */
  .amb-table { width: 100%; border-collapse: collapse; margin-top: 10px; border-radius: 10px; overflow: hidden; border: 1.5px solid #fcd34d; }
  .amb-table th { background: #d97706 !important; color: #ffffff !important; padding: 11px 15px !important; text-align: left; font-weight: 800; border: 1px solid #b45309 !important; }
  .amb-table td { padding: 11px 15px !important; border: 1px solid #fde68a !important; background: #ffffff !important; color: #422006 !important; }
  .amb-table tr:nth-child(even) td { background: #fffbeb !important; }

  /* Trò chơi Nối cặp (Matching Game) */
  .match-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; margin-top: 14px; }
  .match-head { background: #d97706; color: #ffffff; text-align: center; padding: 9px; border-radius: 8px; font-weight: 800; margin-bottom: 10px; }
  .m-card { background: #fffbeb; border: 2px solid #fcd34d; border-radius: 10px; padding: 13px 15px; margin-bottom: 10px; font-weight: 700; color: #78350f; cursor: pointer; transition: 0.2s; display: flex; justify-content: space-between; align-items: center; user-select: none; }
  .m-card:hover:not(.matched) { background: #fef3c7; border-color: #d97706; transform: translateY(-2px); }
  .m-card.selected { background: #d97706; color: #ffffff; border-color: #92400e; box-shadow: 0 0 0 4px rgba(217, 119, 6, 0.25); }
  .m-card.matched { background: #dcfce7; border-color: #16a34a; color: #166534; cursor: default; }
  .m-card.wrong { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .m-badge { font-size: 0.78rem; background: #16a34a; color: #fff; padding: 2px 8px; border-radius: 10px; display: none; }
  .m-card.matched .m-badge { display: inline-block; }

  /* Trắc nghiệm tốc độ */
  .q-card { background: #fffbeb; border: 1.5px solid #fcd34d; border-radius: 12px; padding: 16px; margin-bottom: 14px; }
  .q-title { font-weight: 800; color: #78350f; margin-bottom: 10px; }
  .q-opts { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 10px; }
  .q-btn { background: #ffffff; border: 2px solid #fde68a; padding: 10px 14px; border-radius: 8px; font-weight: 700; color: #422006; cursor: pointer; text-align: left; transition: 0.2s; }
  .q-btn:hover:not(:disabled) { background: #fef3c7; border-color: #d97706; }
  .q-btn.ok { background: #dcfce7; border-color: #16a34a; color: #166534; }
  .q-btn.err { background: #ffe4e6; border-color: #e11d48; color: #9f1239; }
  .q-exp { display: none; margin-top: 10px; padding: 10px 14px; border-radius: 8px; font-weight: 600; font-size: 0.92rem; }

  @media (max-width: 680px) {
    .match-grid { grid-template-columns: 1fr; }
  }
</style>

<!-- THANH ĐIỀU KHIỂN CỐ ĐỊNH -->
<div class="amb-topbar">
  <div class="amb-topbar-title">TOÁN 6 — BÀI 9: DẤU HIỆU CHIA HẾT</div>
  <div class="amb-topbar-right">
    <div class="amb-score-badge">ĐIỂM KHÁM PHÁ: <span id="ptsVal">0</span> / 100</div>
    <button class="amb-sound-btn" id="btnSound" onclick="toggleSound()">Âm thanh: ĐANG BẬT</button>
  </div>
</div>

<!-- BANNER MỞ ĐẦU -->
<div class="amb-hero">
  <div class="amb-hero-tag">CHƯƠNG II: TÍNH CHIA HẾT TRONG TẬP HỢP CÁC SỐ TỰ NHIÊN</div>
  <h1 class="amb-hero-title">BÀI 9: DẤU HIỆU CHIA HẾT</h1>
  <div class="amb-meta-row">
    <div class="amb-meta-item">Toán 6 (Tập 1) — Kết nối tri thức với cuộc sống</div>
    <div class="amb-meta-item">Phương pháp: Tương tác — Tự khám phá quy tắc</div>
  </div>
</div>

<!-- TRẠM KHÁM PHÁ 1: DẤU HIỆU CHIA HẾT CHO 2 VÀ 5 -->
<div class="amb-card">
  <div class="amb-card-head">
    <span>TRẠM KHÁM PHÁ 1: BÍ MẬT CỦA CHỮ SỐ TẬN CÙNG (CHIA HẾT CHO 2 VÀ 5)</span>
    <span class="amb-step-tag">Bước 1 / 3</span>
  </div>
  <div class="amb-card-body">

    <div class="amb-quest-box">
      <div class="amb-quest-title">THỬ THÁCH DẪN DẮT 1A: SĂN TÌM SỐ CHIA HẾT CHO 2 (+10 ĐIỂM)</div>
      <p><b>Nhiệm vụ:</b> Không đặt phép tính chia, hãy <b>bấm chọn 4 số chia hết cho 2</b> trong dãy số dưới đây và quan sát <b>chữ số tận cùng</b> của chúng:</p>
      <div class="chip-grid" id="group2">
        <div class="num-chip" onclick="checkChip2(this, true)">12<b>0</b></div>
        <div class="num-chip" onclick="checkChip2(this, false)">34<b>5</b></div>
        <div class="num-chip" onclick="checkChip2(this, true)">8<b>4</b></div>
        <div class="num-chip" onclick="checkChip2(this, false)">91<b>7</b></div>
        <div class="num-chip" onclick="checkChip2(this, true)">53<b>6</b></div>
        <div class="num-chip" onclick="checkChip2(this, true)">202<b>8</b></div>
      </div>
      <div id="msgChip2" style="font-weight:700; color:#b45309; font-size:0.92rem;"></div>
    </div>

    <div class="amb-quest-box">
      <div class="amb-quest-title">THỬ THÁCH DẪN DẮT 1B: SĂN TÌM SỐ CHIA HẾT CHO 5 (+10 ĐIỂM)</div>
      <p><b>Nhiệm vụ:</b> Hãy <b>bấm chọn 3 số chia hết cho 5</b> dưới đây. Số nào vừa chia hết cho 2, vừa chia hết cho 5?</p>
      <div class="chip-grid" id="group5">
        <div class="num-chip" onclick="checkChip5(this, true)">13<b>5</b></div>
        <div class="num-chip" onclick="checkChip5(this, false)">40<b>2</b></div>
        <div class="num-chip" onclick="checkChip5(this, true)">9<b>0</b></div>
        <div class="num-chip" onclick="checkChip5(this, false)">78<b>8</b></div>
        <div class="num-chip" onclick="checkChip5(this, true)">65<b>0</b></div>
      </div>
      <div id="msgChip5" style="font-weight:700; color:#b45309; font-size:0.92rem;"></div>
    </div>

    <div class="amb-rule-box">
      <div class="amb-rule-title">KẾT LUẬN RÚT RA TỪ THỬ THÁCH 1</div>
      <ul>
        <li><b>Dấu hiệu chia hết cho 2:</b> Các số có <b>chữ số tận cùng</b> là <span class="k-tag">0; 2; 4; 6; 8</span> (số chẵn) thì chia hết cho 2.</li>
        <li><b>Dấu hiệu chia hết cho 5:</b> Các số có <b>chữ số tận cùng</b> là <span class="k-tag">0</span> hoặc <span class="k-tag">5</span> thì chia hết cho 5.</li>
        <li><b>Hệ quả:</b> Số vừa chia hết cho 2, vừa chia hết cho 5 thì có <b>chữ số tận cùng bằng <span class="k-tag">0</span></b>.</li>
      </ul>
    </div>

  </div>
</div>

<!-- TRẠM KHÁM PHÁ 2: DẤU HIỆU CHIA HẾT CHO 9 VÀ 3 -->
<div class="amb-card">
  <div class="amb-card-head">
    <span>TRẠM KHÁM PHÁ 2: QUY LUẬT TỔNG CÁC CHỮ SỐ (CHIA HẾT CHO 9 VÀ 3)</span>
    <span class="amb-step-tag">Bước 2 / 3</span>
  </div>
  <div class="amb-card-body">

    <div class="amb-quest-box">
      <div class="amb-quest-title">THỬ THÁCH DẪN DẮT 2: PHÒNG THÍ NGHIỆM TỔNG CÁC CHỮ SỐ (+20 ĐIỂM)</div>
      <p><b>Tình huống:</b> Số <span class="k-tag">254</span> có chữ số tận cùng là 4 nhưng <b>không chia hết cho 3 và 9</b>. Ngược lại, số <span class="k-tag">378</span> lại <b>chia hết cho cả 3 và 9</b>! Vậy chữ số tận cùng không còn quyết định nữa. Hãy tính <b>tổng các chữ số</b> ở 2 thí nghiệm dưới đây để tìm ra bí mật:</p>

      <div class="lab-row">
        <!-- Thí nghiệm 1 -->
        <div class="lab-card">
          <b>Thí nghiệm A:</b> Xét số <span class="k-tag">378</span> <i>(Biết 378 ⋮ 9 và 378 ⋮ 3)</i>.<br>
          Hãy tính tổng các chữ số: <span class="k-tag">3 + 7 + 8 = ?</span>
          <div class="lab-input-group">
            <input type="number" id="inpLab1" class="lab-input" placeholder="?">
            <button class="lab-btn" onclick="verifyLab(1, 18, 'Chính xác! Tổng bằng 18 (chia hết cho cả 9 và 3) ➔ 378 chia hết cho 9 và 3!')">Kiểm tra</button>
          </div>
          <div class="lab-feedback" id="fbLab1"></div>
        </div>

        <!-- Thí nghiệm 2 -->
        <div class="lab-card">
          <b>Thí nghiệm B:</b> Tìm chữ số <span class="k-tag">x</span> để số <span class="k-tag">21x</span> chia hết cho 9.<br>
          Ta có: <span class="k-tag">2 + 1 + x = 3 + x</span>. Để <span class="k-tag">(3 + x) ⋮ 9</span> thì <span class="k-tag">x</span> bằng mấy?
          <div class="lab-input-group">
            <input type="number" id="inpLab2" class="lab-input" placeholder="x = ?">
            <button class="lab-btn" onclick="verifyLab(2, 6, 'Tuyệt vời! Với x = 6 thì tổng chữ số là 2 + 1 + 6 = 9 ⋮ 9 ➔ Số 216 ⋮ 9!')">Kiểm tra</button>
          </div>
          <div class="lab-feedback" id="fbLab2"></div>
        </div>
      </div>
    </div>

    <div class="amb-rule-box">
      <div class="amb-rule-title">KẾT LUẬN RÚT RA TỪ THỬ THÁCH 2</div>
      <ul>
        <li><b>Dấu hiệu chia hết cho 9:</b> Các số có <b>tổng các chữ số</b> chia hết cho 9 thì chia hết cho 9 (và chỉ những số đó mới chia hết cho 9).</li>
        <li><b>Dấu hiệu chia hết cho 3:</b> Các số có <b>tổng các chữ số</b> chia hết cho 3 thì chia hết cho 3 (và chỉ những số đó mới chia hết cho 3).</li>
        <li><b>Lưu ý quan trọng:</b> Mọi số chia hết cho 9 thì <b>luôn chia hết cho 3</b>, nhưng một số chia hết cho 3 thì <b>chưa chắc chia hết cho 9</b> <i>(Ví dụ: 15 ⋮ 3 nhưng 15 ∤ 9)</i>.</li>
      </ul>
    </div>

  </div>
</div>

<!-- ĐẤU TRƯỜNG TRÒ CHƠI TƯƠNG TÁC -->
<div class="amb-card">
  <div class="amb-card-head">
    <span>TRẠM KHÁM PHÁ 3: ĐẤU TRƯỜNG NỐI CẶP & PHẢN XẠ TOÁN HỌC</span>
    <span class="amb-step-tag">Bước 3 / 3</span>
  </div>
  <div class="amb-card-body">

    <!-- VÒNG 1: TRÒ CHƠI NỐI CẶP -->
    <div class="amb-quest-box">
      <div class="amb-quest-title">VÒNG 1: GHÉP NỐI TỐC ĐỘ (30 ĐIỂM — 10 Điểm / Cặp)</div>
      <p><b>Cách chơi:</b> Nhấn chọn một yêu cầu ở <b>CỘT A</b>, sau đó nhấn chọn số thỏa mãn tương ứng ở <b>CỘT B</b> để nối cặp.</p>

      <div class="match-grid">
        <div>
          <div class="match-head">CỘT A: ĐẶC ĐIỂM SỐ</div>
          <div class="m-card" data-a="1" onclick="selA(this)">
            <span>1. Chia hết cho cả 2, 3, 5 và 9</span>
            <span class="m-badge" id="bA-1"></span>
          </div>
          <div class="m-card" data-a="2" onclick="selA(this)">
            <span>2. Chia hết cho 3 nhưng KHÔNG chia hết cho 9</span>
            <span class="m-badge" id="bA-2"></span>
          </div>
          <div class="m-card" data-a="3" onclick="selA(this)">
            <span>3. Chia hết cho 5 nhưng KHÔNG chia hết cho 2</span>
            <span class="m-badge" id="bA-3"></span>
          </div>
        </div>

        <div>
          <div class="match-head">CỘT B: CON SỐ BÍ ẨN</div>
          <div class="m-card" data-b="2" onclick="selB(this)">
            <span>a) Số 2022 (Tổng chữ số = 6)</span>
            <span class="m-badge" id="bB-2"></span>
          </div>
          <div class="m-card" data-b="3" onclick="selB(this)">
            <span>b) Số 1945 (Tận cùng là 5)</span>
            <span class="m-badge" id="bB-3"></span>
          </div>
          <div class="m-card" data-b="1" onclick="selB(this)">
            <span>c) Số 450 (Tận cùng là 0, tổng chữ số = 9)</span>
            <span class="m-badge" id="bB-1"></span>
          </div>
        </div>
      </div>

      <div id="matchMsg" style="margin-top:8px; font-weight:800; color:#b45309;"></div>
      <button class="lab-btn" style="margin-top:8px;" onclick="resetMatching()">Chơi lại Vòng 1</button>
    </div>

    <!-- VÒNG 2: TRẮC NGHIỆM VẬN DỤNG -->
    <div class="amb-quest-box" style="margin-bottom:0;">
      <div class="amb-quest-title">VÒNG 2: THỬ THÁCH VẬN DỤNG THỰC TẾ (30 ĐIỂM — 15 Điểm / Câu)</div>

      <div class="q-card" id="qc-1">
        <div class="q-title">Câu 1: Một cửa hàng có 3 thùng sữa tươi với số hộp lần lượt là: 124 hộp, 180 hộp và 205 hộp. Người bán hàng muốn chia đều một thùng sữa vào 9 giỏ quà mà không bị lẻ hộp nào. Hỏi người đó phải chọn thùng nào?</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Chưa đúng! 124 có tổng các chữ số là 1 + 2 + 4 = 7 (không chia hết cho 9).')">A. Thùng 124 hộp</button>
          <button class="q-btn" onclick="ansQuiz(1, this, true, 'CHÍNH XÁC (+15 Điểm)! Số 180 có tổng các chữ số là 1 + 8 + 0 = 9 ⋮ 9 nên chia đều được vào 9 giỏ quà.')">B. Thùng 180 hộp</button>
          <button class="q-btn" onclick="ansQuiz(1, this, false, 'Chưa đúng! 205 có tổng các chữ số là 2 + 0 + 5 = 7 (không chia hết cho 9).')">C. Thùng 205 hộp</button>
        </div>
        <div class="q-exp" id="qexp-1"></div>
      </div>

      <div class="q-card" id="qc-2" style="margin-bottom:0;">
        <div class="q-title">Câu 2: Không thực hiện phép tính, hãy xét xem tổng S = 135 + 2020 + 45 có chia hết cho cả 3 và 5 hay không?</div>
        <div class="q-opts">
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Bị lừa rồi! Cả 3 số hạng đều chia hết cho 5, nhưng 2020 có tổng các chữ số là 4 ∤ 3 (trong khi 135 ⋮ 3 và 45 ⋮ 3) nên tổng S không chia hết cho 3.')">A. Chia hết cho cả 3 và 5</button>
          <button class="q-btn" onclick="ansQuiz(2, this, true, 'XUẤT SẮC (+15 Điểm)! Vì 135, 2020, 45 đều tận cùng là 0 hoặc 5 nên S ⋮ 5. Nhưng 135 ⋮ 3, 45 ⋮ 3 còn 2020 ∤ 3 (tổng chữ số = 4) nên S ∤ 3.')">B. Chia hết cho 5 nhưng không chia hết cho 3</button>
          <button class="q-btn" onclick="ansQuiz(2, this, false, 'Sai rồi! Các số hạng đều có tận cùng là 0 hoặc 5 nên tổng chắc chắn chia hết cho 5.')">C. Không chia hết cho cả 3 và 5</button>
        </div>
        <div class="q-exp" id="qexp-2"></div>
      </div>

    </div>

  </div>
</div>

<!-- BẢNG TỔNG KẾT SIÊU NGẮN GỌN -->
<div class="amb-card" style="margin-bottom:0;">
  <div class="amb-card-head">
    <span>BẢNG TÓM TẮT 4 DẤU HIỆU CHIA HẾT TRỌNG TÂM</span>
    <span class="amb-step-tag">Ghi nhớ 10 giây</span>
  </div>
  <div class="amb-card-body">
    <table class="amb-table">
      <thead>
        <tr>
          <th width="25%">Nhóm dấu hiệu</th>
          <th width="20%">Chia hết cho</th>
          <th width="55%">Quy tắc nhận biết nhanh</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td rowspan="2"><b>Nhìn chữ số tận cùng</b></td>
          <td><b>Cho 2</b></td>
          <td>Chữ số tận cùng là số chẵn: <span class="k-tag">0; 2; 4; 6; 8</span></td>
        </tr>
        <tr>
          <td><b>Cho 5</b></td>
          <td>Chữ số tận cùng là: <span class="k-tag">0</span> hoặc <span class="k-tag">5</span> <i>(Chia hết cho cả 2 và 5 ➔ Tận cùng là <span class="k-tag">0</span>)</i></td>
        </tr>
        <tr>
          <td rowspan="2"><b>Tính tổng các chữ số</b></td>
          <td><b>Cho 9</b></td>
          <td><b>Tổng các chữ số</b> chia hết cho <span class="k-tag">9</span></td>
        </tr>
        <tr>
          <td><b>Cho 3</b></td>
          <td><b>Tổng các chữ số</b> chia hết cho <span class="k-tag">3</span></td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<script>
  // BỘ PHÁT ÂM THANH TỰ ĐỘNG (WEB AUDIO API)
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

  // LOGIC TRẠM 1A: CHỌN SỐ CHIA HẾT CHO 2
  let count2 = 0;
  let done2 = false;
  function checkChip2(el, isRight) {
    if (el.classList.contains('correct') || el.classList.contains('wrong') || done2) return;
    if (isRight) {
      sfxOk();
      el.classList.add('correct');
      count2++;
      if (count2 === 4) {
        done2 = true;
        addScore(10);
        document.getElementById('msgChip2').textContent = 'Tuyệt vời (+10 Điểm)! Các số chia hết cho 2 đều có chữ số tận cùng là 0, 2, 4, 6, 8.';
      }
    } else {
      sfxErr();
      el.classList.add('wrong');
      setTimeout(() => el.classList.remove('wrong'), 500);
    }
  }

  // LOGIC TRẠM 1B: CHỌN SỐ CHIA HẾT CHO 5
  let count5 = 0;
  let done5 = false;
  function checkChip5(el, isRight) {
    if (el.classList.contains('correct') || el.classList.contains('wrong') || done5) return;
    if (isRight) {
      sfxOk();
      el.classList.add('correct');
      count5++;
      if (count5 === 3) {
        done5 = true;
        addScore(10);
        document.getElementById('msgChip5').textContent = 'Chính xác (+10 Điểm)! Các số chia hết cho 5 có tận cùng là 0 hoặc 5 (Riêng 90 và 650 tận cùng là 0 nên chia hết cho cả 2 và 5).';
      }
    } else {
      sfxErr();
      el.classList.add('wrong');
      setTimeout(() => el.classList.remove('wrong'), 500);
    }
  }

  // LOGIC TRẠM 2: PHÒNG THÍ NGHIỆM TỔNG CHỮ SỐ
  const labDone = {};
  function verifyLab(id, expected, okMsg) {
    if (labDone[id]) return;
    const val = parseInt(document.getElementById('inpLab' + id).value, 10);
    const fb = document.getElementById('fbLab' + id);
    if (val === expected) {
      sfxOk();
      fb.style.color = '#166534';
      fb.textContent = okMsg + ' (+10 Điểm)';
      labDone[id] = true;
      addScore(10);
    } else {
      sfxErr();
      fb.style.color = '#9f1239';
      fb.textContent = 'Chưa chính xác, hãy cộng lại các chữ số nhé!';
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
        document.getElementById('matchMsg').textContent = 'Hoàn thành xuất sắc cả 3 cặp ghép nối (+30 Điểm)!';
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
