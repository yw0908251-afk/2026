<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>소도시패스 — 일본 소도시 교통패스 스마트 비교</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400;1,500&family=Noto+Serif+KR:wght@300;400;500;600;700&family=DM+Mono:ital,wght@0,300;0,400;0,500;1,300&display=swap" rel="stylesheet">
<style>
:root {
  --ink:     #18160F;
  --ink-90:  rgba(24,22,15,.9);
  --ink-60:  rgba(24,22,15,.6);
  --ink-30:  rgba(24,22,15,.3);
  --ink-10:  rgba(24,22,15,.07);
  --paper:   #F9F6F0;
  --paper-d: #F3EFE6;
  --red:     #BC2822;
  --red-10:  rgba(188,40,34,.1);
  --gold:    #A38A53;
  --shadow:  0 12px 32px rgba(24,22,15,.06), 0 2px 8px rgba(24,22,15,.04);
  --f-serif: 'Cormorant Garamond', 'Noto Serif KR', serif;
  --f-mono:  'DM Mono', monospace;
  --ease:    cubic-bezier(0.25, 1, 0.5, 1);
}

* { box-sizing: border-box; margin: 0; padding: 0; }
body {
  background-color: var(--paper);
  color: var(--ink);
  font-family: var(--f-serif);
  font-size: 15px;
  line-height: 1.6;
  overflow-x: hidden;
  -webkit-font-smoothing: antialiased;
}

/* Background Texture */
body::before {
  content: "";
  position: fixed; top: 0; left: 0; width: 100vw; height: 100vh;
  opacity: 0.02; pointer-events: none; z-index: 9999;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.65' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)'/%3E%3C/svg%3E");
}

header {
  border-bottom: 1px solid var(--ink-10);
  padding: 24px 40px;
  display: flex; justify-content: space-between; align-items: center;
  position: sticky; top: 0; background: rgba(249,246,240,.9);
  backdrop-filter: blur(12px); -webkit-backdrop-filter: blur(12px); z-index: 100;
}
.logo { font-size: 20px; font-weight: 600; letter-spacing: -0.02em; cursor: pointer; }
.logo span { font-family: var(--f-serif); font-style: italic; color: var(--red); font-weight: 500; margin-left: 4px;}

/* 개선 포인트 3: 헤더 환율 영역 및 드롭다운 레이어 */
.hdr-rate-container { position: relative; }
.hdr-rate {
  font-family: var(--f-mono); font-size: 12px; color: var(--ink-60);
  background: var(--paper-d); padding: 6px 12px; border-radius: 20px;
  cursor: pointer; transition: all 0.2s var(--ease); display: flex; align-items: center; gap: 4px;
}
.hdr-rate:hover { background: var(--ink-10); color: var(--ink); }
.rate-dropdown {
  position: absolute; top: calc(100% + 8px); right: 0;
  background: var(--paper); border: 1px solid var(--ink-30); border-radius: 8px;
  padding: 16px; box-shadow: var(--shadow); display: none; width: 220px; z-index: 110;
}
.rate-dropdown.active { display: block; animation: fadeIn 0.2s var(--ease); }
.rate-dropdown label { display: block; font-size: 12px; margin-bottom: 6px; color: var(--ink-60); }
.rate-dropdown input {
  width: 100%; padding: 6px 10px; font-family: var(--f-mono); font-size: 13px;
  border: 1px solid var(--ink-10); background: var(--paper-d); color: var(--ink); border-radius: 4px;
}

main { max-width: 1280px; margin: 40px auto; padding: 0 40px; }
.intro { margin-bottom: 40px; max-width: 600px; }
.intro h1 { font-size: 36px; font-weight: 400; line-height: 1.3; margin-bottom: 12px; letter-spacing: -0.03em; }
.intro p { color: var(--ink-60); font-size: 16px; }

/* 개선 포인트 4 & 6: 반응형 그리드 및 터치 환경 대응 */
.city-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 32px; margin-bottom: 60px;
}
.city-card {
  background: var(--paper-d); border-radius: 12px; overflow: hidden;
  position: relative; cursor: pointer; transition: transform 0.4s var(--ease), box-shadow 0.4s var(--ease);
  aspect-ratio: 4/5; display: flex; flex-direction: column; justify-content: flex-end; padding: 28px;
}
.city-card:hover { transform: translateY(-4px); box-shadow: var(--shadow); }
.cc-bg {
  position: absolute; top: 0; left: 0; width: 100%; height: 100%;
  background-size: cover; background-position: center; filter: grayscale(20%);
  transition: transform 0.6s var(--ease); z-index: 1;
}
.city-card:hover .cc-bg { transform: scale(1.03); }
.city-card::after {
  content: ""; position: absolute; top: 0; left: 0; width: 100%; height: 100%;
  background: linear-gradient(to top, rgba(24,22,15,0.85) 0%, rgba(24,22,15,0.3) 50%, rgba(24,22,15,0) 100%); z-index: 2;
}
.cc-info { position: relative; z-index: 3; color: var(--paper); }
.cc-en { font-family: var(--f-serif); font-style: italic; font-size: 16px; opacity: 0.8; margin-bottom: 2px; }
.cc-name { font-size: 26px; font-weight: 500; line-height: 1.2; margin-bottom: 8px; }

/* 모바일 및 터치 환경을 고려하여 투명도 기반으로 상시 인지 가능하도록 변경 */
.cc-tags { display: flex; gap: 6px; flex-wrap: wrap; opacity: 0.85; transition: opacity 0.3s ease; }
.cc-tag { font-size: 11px; background: rgba(255,255,255,0.15); padding: 2px 8px; border-radius: 4px; backdrop-filter: blur(4px); }
.cc-arrow {
  position: absolute; right: 28px; bottom: 28px; width: 36px; height: 36px;
  border: 1px solid rgba(255,255,255,0.3); border-radius: 50%;
  display: flex; align-items: center; justify-content: center; color: var(--paper);
  z-index: 3; opacity: 0.7; transition: all 0.3s var(--ease);
}
.city-card:hover .cc-arrow { opacity: 1; background: var(--paper); color: var(--ink); border-color: var(--paper); }

/* 개선 포인트 5: 우측 슬라이딩 모달 가로폭 최적화 (맥락 유지) */
.modal-overlay {
  position: fixed; top: 0; left: 0; width: 100vw; height: 100vh;
  background: rgba(24,22,15,0.3); backdrop-filter: blur(4px);
  z-index: 900; display: none; opacity: 0; transition: opacity 0.4s var(--ease);
}
.modal-overlay.active { display: block; opacity: 1; }
.modal {
  position: fixed; top: 0; right: -100%; width: min(560px, 88vw); height: 100vh;
  background: var(--paper); box-shadow: -8px 0 40px rgba(24,22,15,0.08);
  z-index: 1000; transition: right 0.4s var(--ease); display: flex; flex-direction: column;
}
.modal.active { right: 0; }

/* 개선 포인트 5: 밝은 이미지 대비 오버레이 농도 강화 및 텍스트 섀도우 안전망 */
.modal-hero { height: 200px; position: relative; background-size: cover; background-position: center; display: flex; align-items: flex-end; padding: 32px 40px; }
.modal-hero::after {
  content: ""; position: absolute; top: 0; left: 0; width: 100%; height: 100%;
  background: linear-gradient(to top, rgba(24,22,15,0.9) 0%, rgba(24,22,15,0.4) 60%, rgba(24,22,15,0.2) 100%);
}
.mhero-content { position: relative; z-index: 2; color: var(--paper); }
.mhero-en { font-family: var(--f-serif); font-style: italic; opacity: 0.8; }
.mhero-kr { font-size: 32px; font-weight: 600; text-shadow: 0 2px 4px rgba(0,0,0,0.4); }
.m-close {
  position: absolute; top: 24px; right: 24px; width: 36px; height: 36px; border-radius: 50%;
  background: rgba(255,255,255,0.2); backdrop-filter: blur(4px); border: none; color: var(--paper);
  font-size: 18px; cursor: pointer; z-index: 10; display: flex; align-items: center; justify-content: center;
}

.modal-tabs { display: flex; border-bottom: 1px solid var(--ink-10); background: var(--paper-d); }
.m-tab {
  flex: 1; text-align: center; padding: 14px 0; font-size: 14px; color: var(--ink-60);
  cursor: pointer; border-bottom: 2px solid transparent; transition: all 0.2s ease;
}
.m-tab.active { color: var(--red); border-bottom-color: var(--red); font-weight: 500; background: var(--paper); }
.modal-body { flex: 1; overflow-y: auto; padding: 32px 40px; }
.tab-content { display: none; }
.tab-content.active { display: block; }

/* 개선 포인트 1 & 6: 스팟 카드 터치 타겟(44px) 분리 및 일차 즉시 배정 넛지UI */
.spot-card {
  background: var(--paper-d); padding: 16px 20px; border-radius: 8px; margin-bottom: 16px;
  display: flex; justify-content: space-between; align-items: center; position: relative;
}
.sp-info { flex: 1; padding-right: 12px; }
.sp-name { font-size: 16px; font-weight: 500; }
.sp-fare { font-family: var(--f-mono); font-size: 12px; color: var(--ink-60); }
.sp-actions { display: flex; align-items: center; gap: 8px; }

/* 터치 영역 44x44px 확보 */
.sp-add, .sp-nudge-trigger {
  width: 44px; height: 44px; border: 1px solid var(--ink-30); border-radius: 50%;
  background: transparent; color: var(--ink); font-size: 16px; cursor: pointer;
  display: flex; align-items: center; justify-content: center; transition: all 0.2s ease;
}
.sp-add:hover, .sp-nudge-trigger:hover { background: var(--ink); color: var(--paper); }
.sp-add.added { background: var(--red); color: var(--paper); border-color: var(--red); }

/* 넛지 레이어 인터랙션 */
.nudge-layer {
  position: absolute; right: 70px; top: 50%; transform: translateY(-50%);
  background: var(--paper); border: 1px solid var(--ink-30); border-radius: 6px;
  padding: 6px; box-shadow: var(--shadow); display: none; gap: 4px; z-index: 10;
}
.nudge-layer.active { display: flex; animation: fadeIn 0.15s var(--ease); }
.nudge-btn {
  padding: 4px 10px; font-size: 12px; border: 1px solid var(--ink-10);
  background: var(--paper-d); border-radius: 4px; cursor: pointer;
}
.nudge-btn:hover { background: var(--red); color: var(--paper); }

/* 개선 포인트 7: AI Route 타임라인 시각화 및 패스 Verdict 인포그래픽 디자인 */
.route-timeline { position: relative; margin-top: 20px; padding-left: 24px; }
.route-timeline::before {
  content: ""; position: absolute; top: 8px; left: 7px; width: 2px; height: calc(100% - 24px); background: var(--ink-10);
}
.route-node { position: relative; margin-bottom: 24px; }
.route-node::before {
  content: ""; position: absolute; top: 6px; left: -21px; width: 8px; height: 8px; border-radius: 50%; background: var(--gold);
}
.route-node-name { font-size: 15px; font-weight: 500; }
.route-link {
  position: relative; margin: -12px 0 12px -24px; padding-left: 24px;
  font-family: var(--f-mono); font-size: 11px; color: var(--gold); display: flex; align-items: center; gap: 6px;
}
.route-link-icon { font-size: 12px; }

.verdict-box {
  background: var(--paper-d); border-radius: 8px; padding: 20px; margin-top: 24px;
  border-left: 4px solid var(--ink-30); transition: all 0.3s ease;
}
.verdict-box.good { border-left-color: var(--red); background: var(--red-10); }
.verdict-title { font-size: 13px; text-transform: uppercase; letter-spacing: 0.1em; color: var(--ink-60); margin-bottom: 4px; }
.verdict-status { font-size: 20px; font-weight: 600; margin-bottom: 6px; }
.verdict-calc { font-size: 14px; line-height: 1.4; }

.day-spot-card {
  display: flex; justify-content: space-between; align-items: center;
  background: var(--paper); padding: 12px 16px; border-radius: 6px; margin-bottom: 8px;
  border: 1px solid var(--ink-10);
}
.day-spot-left { display: flex; align-items: center; gap: 10px; }
.day-spot-n { font-family: var(--f-mono); font-size: 11px; background: var(--ink-10); width: 20px; height: 20px; border-radius: 50%; display: flex; align-items: center; justify-content: center; }
.day-spot-name { font-size: 14px; }
.day-spot-fare { font-family: var(--f-mono); font-size: 12px; color: var(--ink-60); }

.pass-selector { margin-bottom: 24px; }
.pass-selector label { display: block; font-size: 12px; margin-bottom: 6px; color: var(--ink-60); }
.pass-select {
  width: 100%; padding: 10px; border: 1px solid var(--ink-10); background: var(--paper);
  color: var(--ink); font-family: var(--f-serif); font-size: 15px; border-radius: 6px;
}

.day-tabs { display: flex; gap: 6px; margin-bottom: 16px; overflow-x: auto; padding-bottom: 4px; }
.day-tab {
  padding: 6px 12px; font-size: 12px; border: 1px solid var(--ink-10); border-radius: 4px; cursor: pointer; white-space: nowrap;
}
.day-tab.active { background: var(--ink); color: var(--paper); border-color: var(--ink); }

.empty { text-align: center; padding: 48px 0; color: var(--ink-30); }
.empty-ico { font-size: 32px; display: block; margin-bottom: 8px; }
.empty-txt { font-size: 13px; }

@keyframes fadeIn { from { opacity: 0; transform: translate(0, 4px); } to { opacity: 1; transform: translate(0, 0); } }
@keyframes slideIn { from { right: -100%; } to { right: 0; } }

/* 모바일 전용 반응형 브레이크포인트 미디어쿼리 최적화 */
@media (max-width: 640px) {
  header { padding: 16px 20px; }
  main { margin: 24px auto; padding: 0 20px; }
  .intro h1 { font-size: 28px; }
  .modal-hero { padding: 24px; height: 16px; }
  .modal-hero { height: 16px; display: flex; align-items: center; }
  .mhero-kr { font-size: 24px; }
  .modal-body { padding: 20px; }
}
</style>
</head>
<body>

<header>
  <div class="logo" onclick="location.reload()">소도시패스<span>Sodosipass</span></div>
  <div class="hdr-rate-container">
    <div class="hdr-rate" id="hdrRateDisplay" onclick="toggleRateDropdown()">
      <span>¥ 100 = </span><span id="hdrRateVal">900</span><span>원 ▾</span>
    </div>
    <div class="rate-dropdown" id="rateDropdown">
      <label for="rateInput">원엔 환율 설정 (100엔당)</label>
      <input type="number" id="rateInput" value="900" oninput="updateExchangeRate(this.value)">
    </div>
  </header>

<main>
  <div class="intro">
    <h1>일본 소도시 교통패스<br>스마트하게 비교하세요</h1>
    <p>가고 싶은 곳들을 담으면 최적의 교통패스와 실제 개별 발권 비용을 정밀하게 대조해 드립니다.</p>
  </div>
  <div class="city-grid" id="cityGrid"></div>
</main>

<div class="modal-overlay" id="modalOverlay" onclick="closeModal()"></div>
<div class="modal" id="modal">
  <button class="m-close" onclick="closeModal()">×</button>
  <div class="modal-hero" id="modalHero">
    <div class="mhero-content">
      <div class="mhero-en" id="mheroEn">Takayama Hokuriku</div>
      <div class="mhero-kr" id="mheroKr">기후·다카야마</div>
    </div>
  </div>
  <div class="modal-tabs">
    <div class="m-tab active" onclick="switchTab('spots')" id="tabBtn-spots">스팟 담기</div>
    <div class="m-tab" onclick="switchTab('schedule')" id="tabBtn-schedule">일차별 일정</div>
    <div class="m-tab" onclick="switchTab('ai')" id="tabBtn-ai">AI 추천 경로</div>
  </div>
  <div class="modal-body">
    <div class="tab-content active" id="tab-spots"></div>
    <div class="tab-content" id="tab-schedule">
      <div class="pass-selector">
        <label>비교할 교통패스 선택</label>
        <select class="pass-select" id="passSelect" onchange="renderSchedule()"></select>
      </div>
      <div class="day-tabs" id="dayTabs"></div>
      <div id="dayScheduleBody"></div>
      <div id="verdictContainer"></div>
    </div>
    <div class="tab-content" id="tab-ai">
      <div id="aiRouteBody"></div>
    </div>
  </div>
</div>

<script>
// 샘플 데이터 구조 정의 (개선 포인트 2: 이동 비용 경로 데이터 가이드 포함)
const mockData = {
  "gifu": {
    name: "기후·다카야마", en: "Gifu · Takayama",
    bg: "https://images.unsplash.com/photo-1605018169211-096d2e9ccf0c?auto=format&fit=crop&w=800&q=80",
    tags: ["시라카와고", "온천마을", "전통거리"],
    passes: [
      { name: "다카야마·호쿠리쿠 지역 투어리스트 패스", jpy: 14260 },
      { name: "JR 미나미큐슈 레일패스 (대조군)", jpy: 9000 }
    ],
    // 개선 포인트 2: 인접 스팟 간 이동 비용(transitFare) 및 수단/시간 메타데이터 구조화
    spots: [
      { id: "g1", name: "JR 다카야마역 (기점)", fare: 0, nextTransit: { type: "버스", duration: "50분", fare: 2600 } },
      { id: "g2", name: "시라카와고 합장촌", fare: 0, nextTransit: { type: "도보", duration: "10분", fare: 0 } },
      { id: "g3", name: "다카야마 옛 거리 (산마치스지)", fare: 0, nextTransit: { type: "기차", duration: "15분", fare: 410 } },
      { id: "g4", name: "게로 온천마을", fare: 1200, nextTransit: { type: "버스", duration: "30분", fare: 700 } },
      { id: "g5", name: "신호타카 로프웨이", fare: 3300, nextTransit: null }
    ]
  },
  "shizuoka": {
    name: "시즈오카", en: "Shizuoka",
    bg: "https://images.unsplash.com/photo-1524413840807-0c3cb6fa808d?auto=format&fit=crop&w=800&q=80",
    tags: ["후지산 조망", "녹차밭", "미니 패스"],
    passes: [
      { name: "후지산·시즈오카 지역 미니 패스", jpy: 5080 }
    ],
    spots: [
      { id: "s1", name: "시즈오카역", fare: 0, nextTransit: { type: "기차", duration: "20분", fare: 590 } },
      { id: "s2", name: "미호노 마츠바라", fare: 0, nextTransit: { type: "버스", duration: "45분", fare: 900 } },
      { id: "s3", name: "니혼다이라 로프웨이", fare: 1250, nextTransit: { type: "기차", duration: "35분", fare: 1140 } },
      { id: "s4", name: "슈젠지 온천", fare: 0, nextTransit: null }
    ]
  }
};

let currentCityKey = null;
let exchangeRate = 900; 
let bucket = []; // 구조: { spotId, day }
let activeDay = 1;

// 초기화
function init() {
  renderCityGrid();
}

function renderCityGrid() {
  const grid = document.getElementById('cityGrid');
  grid.innerHTML = Object.keys(mockData).map(key => {
    const c = mockData[key];
    return `
      <div class="city-card" onclick="openModal('${key}')">
        <div class="cc-bg" style="background-image:url('${c.bg}')"></div>
        <div class="cc-arrow">→</div>
        <div class="cc-info">
          <div class="cc-en">${c.en}</div>
          <div class="cc-name">${c.name}</div>
          <div class="cc-tags">
            ${c.tags.map(t => `<span class="cc-tag"># ${t}</span>`).join('')}
          </div>
        </div>
      </div>
    `;
  }).join('');
}

// 개선 포인트 3: 환율 컨트롤러 UI 변경 토글 및 수동 수정 로직 연동
function toggleRateDropdown() {
  document.getElementById('rateDropdown').classList.toggle('active');
}

function updateExchangeRate(val) {
  if (!val || val <= 0) return;
  exchangeRate = parseFloat(val);
  document.getElementById('hdrRateVal').innerText = exchangeRate;
  if(currentCityKey) renderSchedule();
}

// 문서의 다른 곳 클릭 시 환율 드롭다운 닫기 인터랙션 방어
document.addEventListener('click', function(e) {
  const container = document.querySelector('.hdr-rate-container');
  if (!container.contains(e.target)) {
    document.getElementById('rateDropdown').classList.remove('active');
  }
});

// 모달 기믹
function openModal(key) {
  currentCityKey = key;
  const c = mockData[key];
  bucket = []; 
  activeDay = 1;

  document.getElementById('mheroEn').innerText = c.en;
  document.getElementById('mheroKr').innerText = c.name;
  document.getElementById('modalHero').style.backgroundImage = `url('${c.bg}')`;
  
  // 패스 셀렉터 동적 바인딩
  const pSelect = document.getElementById('passSelect');
  pSelect.innerHTML = c.passes.map((p, i) => `<option value="${i}">${p.name} (${p.jpy}엔)</option>`).join('');

  switchTab('spots');
  document.getElementById('modalOverlay').classList.add('active');
  document.getElementById('modal').classList.add('active');
}

function closeModal() {
  document.getElementById('modalOverlay').classList.remove('active');
  document.getElementById('modal').classList.remove('active');
  currentCityKey = null;
}

function switchTab(tab) {
  document.querySelectorAll('.m-tab').forEach(t => t.classList.remove('active'));
  document.querySelectorAll('.tab-content').forEach(c => c.classList.remove('active'));
  
  document.getElementById(`tabBtn-${tab}`).classList.add('active');
  document.getElementById(`tab-${tab}`).classList.add('active');

  if(tab === 'spots') renderSpots();
  if(tab === 'schedule') renderSchedule();
  if(tab === 'ai') renderAiRoute();
}

// 개선 포인트 1 & 6: 넛지 레이어 팝오버 및 컴포넌트 렌더링
function renderSpots() {
  const container = document.getElementById('tab-spots');
  const city = mockData[currentCityKey];
  
  if(!city.spots.length) {
    container.innerHTML = '<div class="empty">등록된 명소 정보가 없습니다.</div>';
    return;
  }

  container.innerHTML = city.spots.map(s => {
    const isAdded = bucket.some(b => b.spotId === s.id);
    const addedBucketItem = bucket.find(b => b.spotId === s.id);
    const dayLabel = addedBucketItem ? `${addedBucketItem.day}일차` : '';

    return `
      <div class="spot-card" id="spot-${s.id}">
        <div class="sp-info">
          <div class="sp-name">${s.name} ${dayLabel ? `<span style="font-size:11px; color:var(--red); font-weight:bold; margin-left:4px;">[${dayLabel}]</span>` : ''}</div>
          <div class="sp-fare">기본 입장료/고정비: ${s.fare}엔</div>
        </div>
        <div class="sp-actions">
          <button class="sp-nudge-trigger" onclick="toggleNudge('${s.id}', event)">📅</button>
          <button class="sp-add ${isAdded ? 'added' : ''}" onclick="toggleSpotSimple('${s.id}')">
            ${isAdded ? '✓' : '+'}
          </button>
          
          <div class="nudge-layer" id="nudge-${s.id}">
            <button class="nudge-btn" onclick="assignSpotDay('${s.id}', 1, event)">1일</button>
            <button class="nudge-btn" onclick="assignSpotDay('${s.id}', 2, event)">2일</button>
            <button class="nudge-btn" onclick="assignSpotDay('${s.id}', 3, event)">3일</button>
          </div>
        </div>
      </div>
    `;
  }).join('');
}

function toggleNudge(id, event) {
  event.stopPropagation();
  const layer = document.getElementById(`nudge-${id}`);
  const isActive = layer.classList.contains('active');
  
  // 다른 오픈된 넛지 레이어 닫기
  document.querySelectorAll('.nudge-layer').forEach(l => l.classList.remove('active'));
  
  if(!isActive) layer.classList.add('active');
}

// 넛지 영역 외부 클릭 시 차단
document.addEventListener('click', () => {
  document.querySelectorAll('.nudge-layer').forEach(l => l.classList.remove('active'));
});

function assignSpotDay(id, day, event) {
  if(event) event.stopPropagation();
  // 기존 할당 제거 후 재할당
  bucket = bucket.filter(b => b.spotId !== id);
  bucket.push({ spotId: id, day: day });
  document.getElementById(`nudge-${id}`).classList.remove('active');
  renderSpots();
}

function toggleSpotSimple(id) {
  const index = bucket.findIndex(b => b.spotId === id);
  if(index > -1) {
    bucket.splice(index, 1);
  } else {
    // 기본적으로 현재 선택된 활성 일차(activeDay)에 배정
    bucket.push({ spotId: id, day: activeDay });
  }
  renderSpots();
}

// 개선 포인트 2 & 7: 정밀 차액 수치 수식화 계산 및 Verdict 리포팅 기능 보완
function renderSchedule() {
  const tabsContainer = document.getElementById('dayTabs');
  const body = document.getElementById('dayScheduleBody');
  const verdictContainer = document.getElementById('verdictContainer');
  const city = mockData[currentCityKey];

  // 3일치 일정 탭 생성
  tabsContainer.innerHTML = [1, 2, 3].map(d => `
    <div class="day-tab ${activeDay === d ? 'active' : ''}" onclick="setScheduleDay(${d})">${d}일차</div>
  `).join('');

  const spotsForDay = city.spots.filter(s => bucket.some(b => b.spotId === s.id && b.day === activeDay));

  if(!bucket.length) {
    body.innerHTML = `<div class="empty"><span class="empty-ico">📅</span><p class=\"empty-txt\">스팟 담기 탭에서 가고 싶은 곳을 추가하면<br>일차별로 일정을 확인할 수 있어요</p></div>`;
    verdictContainer.innerHTML = '';
    return;
  }

  // 총비용 산출 계산식 고도화 (개선 포인트 2: 고정 요금 + 구간 이동 비용 합산)
  let totalFixedFare = 0;
  let totalTransitFare = 0;

  // 전체 선택된 스팟들의 고정비 및 인접 이동 요금 정밀 추적 계산
  bucket.forEach(bItem => {
    const sMeta = city.spots.find(s => s.id === bItem.spotId);
    if(sMeta) {
      totalFixedFare += sMeta.fare;
      if(sMeta.nextTransit) {
        totalTransitFare += sMeta.nextTransit.fare;
      }
    }
  });

  const totalCalculatedFare = totalFixedFare + totalTransitFare;
  
  const selPassIdx = document.getElementById('passSelect').value || 0;
  const selPass = city.passes[selPassIdx];
  const passJPY = selPass ? selPass.jpy : 0;
  
  // 패스 이득 판정 조건식
  const isGoodChoice = passJPY > 0 && totalCalculatedFare > passJPY;
  const diffFare = Math.abs(totalCalculatedFare - passJPY);
  
  // 환율 환산 적용
  const krwTotalFare = Math.floor((totalCalculatedFare * exchangeRate) / 100);
  const krwPassPrice = Math.floor((passJPY * exchangeRate) / 100);
  const krwDiff = Math.floor((diffFare * exchangeRate) / 100);

  // 현재 탭 일차의 할당 스팟 렌더링
  if(!spotsForDay.length) {
    body.innerHTML = `<div class="empty" style="padding:28px 0"><span class="empty-ico">—</span><p class="empty-txt">${activeDay}일차에 배정된 명소가 없습니다.</p></div>`;
  } else {
    body.innerHTML = `
      <div style="margin-bottom:8px; font-family:var(--f-mono); font-size:10px; color:var(--ink-30); text-transform:uppercase;">${activeDay}일차 배정 스팟 (${spotsForDay.length}곳)</div>
      ${spotsForDay.map((s, i) => `
        <div class="day-spot-card">
          <div class="day-spot-left">
            <div class="day-spot-n">${i+1}</div>
            <div class="day-spot-name">${s.name}</div>
          </div>
          <div class="day-spot-fare">${s.fare}엔</div>
        </div>
      `).join('')}
    `;
  }

  // 개선 포인트 7: 판정 컴포넌트 시각적 쾌감 리포트 디자인 고도화
  verdictContainer.innerHTML = `
    <div class="verdict-box ${isGoodChoice ? 'good' : ''}">
      <div class="verdict-title">PASS VERDICT REPORT</div>
      <div class="verdict-status" style="color: ${isGoodChoice ? 'var(--red)' : 'var(--ink)'}">
        ${isGoodChoice ? '✓ 패스 구매 적극 추천' : '✕ 개별 발권 권장'}
      </div>
      <div class="verdict-calc">
        총 예상 비용 (교통비+입장료): <strong>${totalCalculatedFare}엔</strong> (약 ${krwTotalFare.toLocaleString()}원)<br>
        선택 패스 권면가: <strong>${passJPY}엔</strong> (약 ${krwPassPrice.toLocaleString()}원)<br>
        <span style="display:block; margin-top:8px; font-size:15px; color:${isGoodChoice ? 'var(--red)' : 'var(--ink)'}">
          ${isGoodChoice ? `👉 개별 발권보다 <span style="font-weight:bold;">[${diffFare}엔] (약 ${krwDiff.toLocaleString()}원)</span> 만큼 더 이득이에요!` : `👉 패스 구매 시 <span style="font-weight:bold;">[${diffFare}엔] (약 ${krwDiff.toLocaleString()}원)</span> 만큼 손해이니 사지 마세요.`}
        </span>
      </div>
    </div>
  `;
}

function setScheduleDay(d) {
  activeDay = d;
  renderSchedule();
}

// 개선 포인트 7: AI Route 타임라인 형태의 시각화 컴포넌트 구현
function renderAiRoute() {
  const container = document.getElementById('aiRouteBody');
  const city = mockData[currentCityKey];

  // 버킷에 담긴 스팟들을 도시 시퀀스 데이터 순서대로 정렬
  const selectedSpots = city.spots.filter(s => bucket.some(b => b.spotId === s.id));

  if(!selectedSpots.length) {
    container.innerHTML = '<div class="empty">스팟을 담으시면 AI 최적화 동선 타임라인이 시각화됩니다.</div>';
    return;
  }

  container.innerHTML = `
    <div style="margin-bottom:16px; font-family:var(--f-mono); font-size:10px; color:var(--ink-30);">AI GENERATED OPTIMAL ROUTE</div>
    <div class="route-timeline">
      ${selectedSpots.map((s, idx) => {
        let nodeHtml = `<div class="route-node"><div class="route-node-name">${s.name}</div></div>`;
        
        // 마지막 노드가 아니고 다음 이동 트랜짓 메타데이터가 존재할 경우 타임라인 선 연결
        if(idx < selectedSpots.length - 1 && s.nextTransit) {
          nodeHtml += `
            <div class="route-link">
              <span class="route-link-icon">🚌</span>
              <span>${s.nextTransit.type} 이용 (${s.nextTransit.duration}) · <strong>+${s.nextTransit.fare}엔</strong></span>
            </div>
          `;
        }
        return nodeHtml;
      }).join('')}
    </div>
  `;
}

window.onload = init;
</script>
</body>
</html>
