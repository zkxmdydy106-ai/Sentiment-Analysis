<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>감성 분석 + 알바 선택 활동</title>
  <style>
    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: #f5f7fb;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 1100px;
      margin: 0 auto;
      padding: 20px;
    }
    h1 {
      text-align: center;
      margin-bottom: 10px;
    }
    .subtitle {
      text-align: center;
      color: #666;
      margin-bottom: 20px;
    }
    .grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 16px;
    }
    .card {
      background: #fff;
      border-radius: 14px;
      padding: 16px 18px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.04);
    }
    .card h2 {
      font-size: 18px;
      margin-top: 0;
      margin-bottom: 10px;
    }
    label {
      display: block;
      font-size: 13px;
      margin: 6px 0 3px;
      color: #555;
    }
    input[type="text"],
    input[type="number"],
    textarea {
      width: 100%;
      box-sizing: border-box;
      padding: 8px 10px;
      border-radius: 8px;
      border: 1px solid #d0d5dd;
      font-size: 13px;
      resize: vertical;
    }
    textarea {
      min-height: 80px;
    }
    button {
      margin-top: 8px;
      padding: 7px 14px;
      border: none;
      border-radius: 999px;
      background: #4A90E2;
      color: #fff;
      font-size: 13px;
      cursor: pointer;
    }
    button:hover {
      opacity: 0.9;
    }
    .result-box {
      margin-top: 8px;
      padding: 8px 10px;
      background: #f4f8ff;
      border-radius: 10px;
      font-size: 13px;
    }
    .tag {
      display: inline-block;
      padding: 2px 8px;
      border-radius: 12px;
      font-size: 11px;
      margin: 2px;
    }
    .tag-pos { background:#e6f6e8; color:#1b7f3b; }
    .tag-neg { background:#ffe7ea; color:#b7283c; }
    .tag-neu { background:#eef0f5; color:#555; }
    .tag-student { background:#fff1d1; color:#8a5d00; }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 8px;
      font-size: 13px;
    }
    table th, table td {
      border: 1px solid #e0e4ef;
      padding: 6px 8px;
      text-align: left;
    }
    table th {
      background: #f8fafc;
    }
    .highlight {
      background: #fff9e6;
    }
    .small {
      font-size: 11px;
      color: #888;
    }
    .flex-row {
      display: flex;
      gap: 8px;
      flex-wrap: wrap;
    }
    .pill {
      padding: 3px 8px;
      border-radius: 999px;
      background:#f0f2f8;
      font-size:11px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>원하는 물건, 감성 분석 & 알바 계획</h1>
    <div class="subtitle">리뷰 감성 분석으로 물건을 고르고, 알바 계획으로 언제 살 수 있을지 계산해 보자.</div>

    <!-- =========================== -->
    <!-- 0. 학생 감성 단어 추가 기능 -->
    <!-- =========================== -->
    <div class="card">
      <h2>0. 내가 만드는 감성 단어 사전</h2>

      <label>➕ 긍정 단어 추가</label>
      <div class="flex-row">
        <input type="text" id="addPositiveWord" placeholder="예: 예쁘다, 튼튼함">
        <button id="addPosBtn">추가</button>
      </div>

      <label style="margin-top:10px;">➕ 부정 단어 추가</label>
      <div class="flex-row">
        <input type="text" id="addNegativeWord" placeholder="예: 별로다, 약하다">
        <button id="addNegBtn">추가</button>
      </div>

      <div class="result-box" id="wordLists" style="margin-top:12px;">
        <!-- 단어 목록 표시 영역 -->
      </div>
    </div>

    <!-- 1. 원하는 물건 설정 -->
    <div class="card">
      <h2>1. 원하는 물건 설정</h2>
      <div class="flex-row">
        <div style="flex:2;">
          <label>원하는 물건 이름</label>
          <input type="text" id="itemName" placeholder="예: 무선 이어폰, 운동화, 키보드">
        </div>
        <div style="flex:1;">
          <label>가격(원)</label>
          <input type="number" id="itemPrice" placeholder="예: 129000">
        </div>
      </div>
      <div class="small" style="margin-top:6px;">
        ※ 수업 전에 학생이 진짜로 사고 싶은 물건을 하나 정한 뒤 가격을 검색해서 적게 해 보세요.
      </div>
    </div>

    <div class="grid" style="margin-top:16px;">

      <!-- 2. 단어 / 짧은 문장 감성 분석 -->
      <div class="card">
        <h2>2. 감성 단어 실험</h2>
        <label>단어 또는 짧은 문장 입력</label>
        <input type="text" id="wordInput" placeholder="예: 가성비 좋고 디자인이 예쁘다">
        <button id="analyzeWordBtn">감성 분석</button>
        <div id="wordResult" class="result-box">
          감성 점수와 해석이 여기에 표시됩니다.
        </div>
        <div class="small">
          예시 단어: <span class="pill">좋다</span> <span class="pill">가성비 좋다</span>
          <span class="pill">생각보다 별로다</span> <span class="pill">튼튼하고 예쁘다</span>
        </div>
      </div>

      <!-- 3. 실제 리뷰 감성 분석 -->
      <div class="card">
        <h2>3. 실제 리뷰 감성 분석</h2>
        <label>실제 리뷰 여러 개 입력 (한 줄에 하나씩)</label>
        <textarea id="reviewsInput" placeholder="예)&#10;너무 예쁘고 가벼워요. 배송도 빨라요.&#10;생각보다 별로고 소음이 심하네요.&#10;가성비 좋고 튼튼해서 만족합니다."></textarea>
        <button id="analyzeReviewsBtn">리뷰 감성 분석</button>
        <div id="reviewsResult" class="result-box">
          리뷰별 감성 점수 표가 여기에 표시됩니다.
        </div>
      </div>
    </div>

    <!-- 4. 알바 선택 & 목표 달성 계산 -->
    <div class="card" style="margin-top:16px;">
      <h2>4. 알바 선택 & 목표 달성 시뮬레이션</h2>
      <div class="small">
        아래 표에 알바 정보를 입력한 후, <b>계산하기</b> 버튼을 누르면<br>
        각 알바로 한 달 일했을 때의 월 소득과, 원하는 물건을 사기까지 걸리는 개월 수가 계산됩니다.
      </div>

      <table>
        <thead>
          <tr>
            <th>알바 이름</th>
            <th>시급(원)</th>
            <th>하루 근무 시간(시간)</th>
            <th>한 달 근무 일수(일)</th>
          </tr>
        </thead>
        <tbody id="jobsBody">
          <tr>
            <td><input type="text" value="카페 알바"></td>
            <td><input type="number" value="10000"></td>
            <td><input type="number" step="0.5" value="3"></td>
            <td><input type="number" value="20"></td>
          </tr>
          <tr>
            <td><input type="text" value="편의점 야간"></td>
            <td><input type="number" value="13000"></td>
            <td><input type="number" step="0.5" value="4"></td>
            <td><input type="number" value="16"></td>
          </tr>
        </tbody>
      </table>

      <button id="calcJobsBtn">알바 수입 & 목표 달성 개월 계산하기</button>

      <div id="jobsResult" class="result-box">
        알바별 월 소득과 목표 달성까지 걸리는 개월 수가 여기에 표시됩니다.
      </div>
    </div>
  </div>

  <script>
    // ------------------------------------------------------------------
    // 기본 감성 사전 + 학생 추가 단어 목록
    // ------------------------------------------------------------------
    const basePositiveWords = ["좋다","만족","추천","훌륭","완벽","가성비","튼튼","예쁘","이쁘","최고","편하","빠르","감동","괜찮","좋아요"];
    const baseNegativeWords = ["별로","최악","실망","부족","불편","망함","후회","느리","끊기","깨지","부서지","나쁘","비추","문제"];

    let studentPositive = [];
    let studentNegative = [];

    function updateWordListUI() {
      const box = document.getElementById("wordLists");
      box.innerHTML = `
        <b>긍정 단어:</b><br>
        ${basePositiveWords.map(w=>`<span class='tag tag-pos'>${w}</span>`).join("")}
        ${studentPositive.map(w=>`<span class='tag tag-student'>${w}</span>`).join("")}
        <br><br>
        <b>부정 단어:</b><br>
        ${baseNegativeWords.map(w=>`<span class='tag tag-neg'>${w}</span>`).join("")}
        ${studentNegative.map(w=>`<span class='tag tag-student'>${w}</span>`).join("")}
      `;
    }
    updateWordListUI();


    // ------------------------------------------------------------------
    // 학생 단어 추가 기능
    // ------------------------------------------------------------------
    document.getElementById("addPosBtn").onclick = () => {
      const w = document.getElementById("addPositiveWord").value.trim();
      if (w !== "") studentPositive.push(w);
      document.getElementById("addPositiveWord").value = "";
      updateWordListUI();
    };
    document.getElementById("addNegBtn").onclick = () => {
      const w = document.getElementById("addNegativeWord").value.trim();
      if (w !== "") studentNegative.push(w);
      document.getElementById("addNegativeWord").value = "";
      updateWordListUI();
    };


    // ------------------------------------------------------------------
    // 감성 분석 함수
    // ------------------------------------------------------------------
    function sentimentScore(text) {
      if (!text) return 0;
      let pos = 0, neg = 0;

      [...basePositiveWords, ...studentPositive].forEach(w => { if (text.includes(w)) pos++; });
      [...baseNegativeWords, ...studentNegative].forEach(w => { if (text.includes(w)) neg++; });

      if (pos + neg === 0) return 0;
      return (pos - neg) / (pos + neg);
    }

    function sentimentLabel(score) {
      if (score > 0.4) return "매우 긍정";
      else if (score > 0.1) return "긍정";
      else if (score > -0.1) return "중립";
      else if (score > -0.4) return "부정";
      else return "매우 부정";
    }

    function labelTag(score) {
      const label = sentimentLabel(score);
      let cls = "tag-neu";
      if (score > 0.1) cls = "tag-pos";
      if (score < -0.1) cls = "tag-neg";
      return `<span class="tag ${cls}">${label}</span>`;
    }


    // ------------------------------------------------------------------
    // 2. 단어/문장 감성 분석 기능
    // ------------------------------------------------------------------
    document.getElementById("analyzeWordBtn").onclick = () => {
      const text = document.getElementById("wordInput").value.trim();
      const box = document.getElementById("wordResult");

      if (!text) {
        box.textContent = "분석할 문장을 입력해 주세요.";
        return;
      }

      const score = sentimentScore(text);
      box.innerHTML = `
        <b>입력 문장:</b> ${text}<br>
        <b>감성 점수:</b> ${score.toFixed(2)} ${labelTag(score)}
      `;
    };


    // ------------------------------------------------------------------
    // 3. 리뷰 감성 분석 기능
    // ------------------------------------------------------------------
    document.getElementById("analyzeReviewsBtn").onclick = () => {
      const raw = document.getElementById("reviewsInput").value.trim();
      const box = document.getElementById("reviewsResult");

      if (!raw) {
        box.textContent = "리뷰를 입력해 주세요.";
        return;
      }

      const lines = raw.split("\n").filter(x => x.trim().length > 0);
      let html = `
        <table>
          <thead>
            <tr><th>#</th><th>리뷰 내용</th><th>감성 점수</th></tr>
          </thead><tbody>
      `;

      lines.forEach((r,i)=>{
        const s = sentimentScore(r);
        html += `
          <tr>
            <td>${i+1}</td>
            <td>${r}</td>
            <td>${s.toFixed(2)} ${labelTag(s)}</td>
          </tr>`;
      });

      html += `</tbody></table>`;
      box.innerHTML = html;
    };


    // ------------------------------------------------------------------
    // 4. 알바 계산 기능
    // ------------------------------------------------------------------
    document.getElementById("calcJobsBtn").onclick = () => {
      const itemName = document.getElementById("itemName").value.trim() || "물건";
      const itemPrice = parseFloat(document.getElementById("itemPrice").value);
      const box = document.getElementById("jobsResult");

      const rows = Array.from(document.querySelectorAll("#jobsBody tr"));
      let data = [];

      rows.forEach(r=>{
        const c = r.querySelectorAll("td input");
        const name = c[0].value;
        const wage = parseFloat(c[1].value);
        const hours = parseFloat(c[2].value);
        const days = parseFloat(c[3].value);

        const monthly = wage * hours * days;
        const monthsNeed = itemPrice / monthly;

        data.push({name, monthly, monthsNeed});
      });

      let html = `
        <b>${itemName} (${itemPrice.toLocaleString()}원)</b><br>
        <table>
        <tr><th>알바</th><th>월 소득</th><th>필요 개월</th></tr>
      `;

      data.sort((a,b)=>a.monthsNeed-b.monthsNeed);
      data.forEach((d,i)=>{
        html += `
          <tr ${i===0?"class='highlight'":""}>
            <td>${d.name}</td>
            <td>${d.monthly.toLocaleString()}원</td>
            <td>${d.monthsNeed.toFixed(2)}개월</td>
          </tr>`;
      });

      html += `</table>`;
      box.innerHTML = html;
    };
  </script>
</body>
</html>
