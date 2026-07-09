<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>더와이즈컨설팅 | 교육설계부터 운영까지, HRD 파트너</title>
<link rel="preconnect" href="https://cdn.jsdelivr.net">
<link href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.9/dist/web/variable/pretendardvariable-dynamic-subset.min.css" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Noto+Serif+KR:wght@500;600;700&display=swap" rel="stylesheet">
<style>
:root{
  --ink:#14211B;
  --green:#175E43;
  --green-deep:#0E3D2C;
  --green-soft:#EAF2ED;
  --paper:#FFFFFF;
  --mist:#F6F7F4;
  --line:#E3E7E1;
  --gold:#C9A24B;
  --gray:#5C6660;
  --radius:18px;
  --serif:'Noto Serif KR', serif;
  --sans:'Pretendard Variable', Pretendard, -apple-system, sans-serif;
}
*{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth}
body{font-family:var(--sans);color:var(--ink);background:var(--paper);line-height:1.65;-webkit-font-smoothing:antialiased}
img{max-width:100%}
a{text-decoration:none;color:inherit}
ul{list-style:none}
.wrap{max-width:1180px;margin:0 auto;padding:0 24px}
section{padding:110px 0}
.eyebrow{display:inline-flex;align-items:center;gap:8px;font-size:13px;font-weight:700;letter-spacing:.14em;color:var(--green);text-transform:uppercase;margin-bottom:18px}
.eyebrow::before{content:"";width:26px;height:1.5px;background:var(--green)}
h2.title{font-family:var(--serif);font-size:clamp(28px,4vw,40px);font-weight:600;line-height:1.35;letter-spacing:-.01em}
p.lead{margin-top:16px;color:var(--gray);font-size:17px;max-width:640px}

/* ---------- Nav ---------- */
header{position:fixed;top:0;left:0;right:0;z-index:100;background:rgba(255,255,255,.86);backdrop-filter:blur(14px);border-bottom:1px solid transparent;transition:border-color .3s}
header.scrolled{border-bottom-color:var(--line)}
.nav{display:flex;align-items:center;justify-content:space-between;height:72px}
.logo{font-family:var(--serif);font-weight:700;font-size:20px;letter-spacing:-.01em}
.logo em{font-style:normal;color:var(--green)}
.nav ul{display:flex;gap:34px;font-size:15px;font-weight:500}
.nav ul a{color:var(--gray);transition:color .2s}
.nav ul a:hover{color:var(--ink)}
.btn{display:inline-flex;align-items:center;gap:8px;padding:12px 24px;border-radius:999px;font-size:15px;font-weight:600;transition:transform .2s,box-shadow .2s,background .2s;cursor:pointer;border:none}
.btn:focus-visible,a:focus-visible{outline:3px solid var(--gold);outline-offset:2px}
.btn-primary{background:var(--green);color:#fff}
.btn-primary:hover{background:var(--green-deep);transform:translateY(-2px);box-shadow:0 10px 24px rgba(23,94,67,.25)}
.btn-ghost{background:transparent;color:var(--ink);border:1.5px solid var(--line)}
.btn-ghost:hover{border-color:var(--ink)}
.nav .btn{padding:10px 20px;font-size:14px}
.menu-toggle{display:none;background:none;border:none;font-size:26px;cursor:pointer;color:var(--ink)}

/* ---------- Hero ---------- */
.hero{padding:190px 0 90px;background:
  radial-gradient(1100px 500px at 85% -10%, var(--green-soft), transparent 65%),
  var(--paper)}
.hero-grid{display:grid;grid-template-columns:1.15fr .85fr;gap:60px;align-items:center}
.hero h1{font-family:var(--serif);font-size:clamp(34px,5vw,54px);font-weight:600;line-height:1.32;letter-spacing:-.015em}
.hero h1 .hl{position:relative;white-space:nowrap}
.hero h1 .hl::after{content:"";position:absolute;left:0;bottom:6px;width:100%;height:34%;background:var(--green-soft);z-index:-1;border-radius:4px;transform:scaleX(0);transform-origin:left;animation:sweep 1s .5s ease forwards}
@keyframes sweep{to{transform:scaleX(1)}}
.hero p{margin:24px 0 36px;font-size:18px;color:var(--gray);max-width:520px}
.hero-cta{display:flex;gap:14px;flex-wrap:wrap}
/* signature: HRD value chain rail */
.chain{background:var(--ink);border-radius:var(--radius);padding:38px 34px;color:#fff;box-shadow:0 30px 60px rgba(20,33,27,.22)}
.chain h3{font-size:13px;font-weight:700;letter-spacing:.16em;color:var(--gold);margin-bottom:26px}
.chain ol{list-style:none;position:relative}
.chain ol::before{content:"";position:absolute;left:11px;top:14px;bottom:14px;width:2px;background:linear-gradient(var(--green),rgba(255,255,255,.15))}
.chain li{position:relative;padding:0 0 26px 40px}
.chain li:last-child{padding-bottom:0}
.chain li::before{content:"";position:absolute;left:4px;top:6px;width:16px;height:16px;border-radius:50%;background:var(--ink);border:2.5px solid var(--green);transition:background .3s}
.chain li:hover::before{background:var(--green)}
.chain strong{display:block;font-size:17px;font-weight:700}
.chain span{font-size:14px;color:rgba(255,255,255,.65)}

/* ---------- About ---------- */
.about{background:var(--mist)}
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:70px;margin-top:56px}
.values{display:grid;gap:16px}
.value{background:var(--paper);border:1px solid var(--line);border-radius:var(--radius);padding:26px 28px;display:flex;gap:20px;align-items:flex-start;transition:transform .25s,box-shadow .25s}
.value:hover{transform:translateY(-4px);box-shadow:0 16px 32px rgba(20,33,27,.08)}
.value .ic{flex:none;width:46px;height:46px;border-radius:12px;background:var(--green-soft);display:grid;place-items:center;font-size:20px}
.value strong{display:block;font-size:17px;margin-bottom:4px}
.value strong small{font-size:12px;font-weight:700;color:var(--gold);letter-spacing:.1em;margin-left:8px}
.value p{font-size:14.5px;color:var(--gray)}
.ceo{background:var(--paper);border:1px solid var(--line);border-radius:var(--radius);padding:40px}
.ceo blockquote{font-family:var(--serif);font-size:21px;line-height:1.7;font-weight:500}
.ceo blockquote::before{content:"“";display:block;font-size:54px;color:var(--gold);line-height:.6;margin-bottom:14px}
.ceo footer{margin-top:26px;font-size:14px;color:var(--gray)}
.ceo footer b{color:var(--ink);font-size:15px}

/* ---------- Services ---------- */
.svc-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:22px;margin-top:56px}
.svc{border:1px solid var(--line);border-radius:var(--radius);padding:36px 34px;position:relative;overflow:hidden;transition:border-color .25s,transform .25s}
.svc:hover{border-color:var(--green);transform:translateY(-4px)}
.svc .step{font-size:12px;font-weight:800;letter-spacing:.16em;color:var(--gold)}
.svc h3{font-size:21px;margin:12px 0 10px;font-weight:700}
.svc>p{font-size:15px;color:var(--gray);margin-bottom:18px}
.tags{display:flex;flex-wrap:wrap;gap:8px}
.tags li{font-size:12.5px;font-weight:600;color:var(--green);background:var(--green-soft);padding:6px 12px;border-radius:999px}

/* ---------- Programs ---------- */
.programs{background:var(--ink);color:#fff}
.programs .eyebrow{color:var(--gold)}
.programs .eyebrow::before{background:var(--gold)}
.programs p.lead{color:rgba(255,255,255,.6)}
.tabs{display:flex;gap:10px;flex-wrap:wrap;margin:44px 0 28px}
.tab{padding:10px 20px;border-radius:999px;border:1.5px solid rgba(255,255,255,.22);background:transparent;color:rgba(255,255,255,.75);font-size:14px;font-weight:600;cursor:pointer;transition:all .2s;font-family:var(--sans)}
.tab:hover{border-color:#fff;color:#fff}
.tab.on{background:#fff;color:var(--ink);border-color:#fff}
.prog-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
.prog{background:rgba(255,255,255,.05);border:1px solid rgba(255,255,255,.12);border-radius:var(--radius);padding:28px;transition:background .25s}
.prog:hover{background:rgba(255,255,255,.1)}
.prog .cat{font-size:11.5px;font-weight:800;letter-spacing:.12em;color:var(--gold)}
.prog h4{font-size:18px;margin:10px 0 8px;font-weight:700}
.prog p{font-size:14px;color:rgba(255,255,255,.6);margin-bottom:16px}
.prog .meta{display:flex;gap:14px;font-size:12.5px;color:rgba(255,255,255,.5)}
.prog .badge{display:inline-block;margin-top:14px;font-size:11.5px;font-weight:700;color:var(--ink);background:var(--gold);padding:4px 10px;border-radius:6px}

/* ---------- Cases ---------- */
.case-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px;margin-top:56px}
.case{border:1px solid var(--line);border-radius:var(--radius);overflow:hidden;transition:box-shadow .25s,transform .25s}
.case:hover{transform:translateY(-4px);box-shadow:0 20px 40px rgba(20,33,27,.1)}
.case .head{padding:24px 26px;background:var(--green-soft)}
.case .head .ind{font-size:12px;font-weight:800;letter-spacing:.12em;color:var(--green)}
.case .head h4{font-size:17.5px;font-weight:700;margin-top:6px}
.case .body{padding:24px 26px;font-size:14px;color:var(--gray)}
.case .body dt{font-weight:700;color:var(--ink);font-size:13px;margin-top:14px}
.case .body dt:first-child{margin-top:0}
.case .body dd{margin-top:3px}
.case .result{margin-top:16px;padding-top:16px;border-top:1px dashed var(--line);font-weight:700;color:var(--green);font-size:15px}
.quote-band{margin-top:64px;background:var(--mist);border-radius:var(--radius);padding:48px;text-align:center}
.quote-band blockquote{font-family:var(--serif);font-size:clamp(18px,2.4vw,23px);font-weight:500;max-width:760px;margin:0 auto;line-height:1.7}
.quote-band footer{margin-top:18px;font-size:14px;color:var(--gray)}

/* ---------- Insights ---------- */
.insight-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px;margin-top:56px}
.post{border-bottom:1px solid var(--line);padding-bottom:24px;transition:opacity .2s}
.post:hover h4{color:var(--green)}
.post .date{font-size:12.5px;color:var(--gray);letter-spacing:.04em}
.post h4{font-size:18px;font-weight:700;margin:10px 0;line-height:1.5;transition:color .2s}
.post p{font-size:14px;color:var(--gray)}
.post .more{display:inline-block;margin-top:14px;font-size:13.5px;font-weight:700;color:var(--green)}

/* ---------- Contact ---------- */
.contact{background:linear-gradient(160deg,var(--green-deep),var(--green));color:#fff}
.contact-grid{display:grid;grid-template-columns:1fr 1.1fr;gap:70px;align-items:start}
.contact h2{font-family:var(--serif);font-size:clamp(28px,4vw,40px);font-weight:600;line-height:1.4}
.contact .sub{margin:18px 0 34px;color:rgba(255,255,255,.75);font-size:16px}
.c-info{display:grid;gap:14px;font-size:15px}
.c-info div{display:flex;gap:12px;align-items:center}
.c-info .ic{width:38px;height:38px;border-radius:10px;background:rgba(255,255,255,.12);display:grid;place-items:center;font-size:16px;flex:none}
.form-card{background:#fff;border-radius:var(--radius);padding:18px;color:var(--ink);box-shadow:0 30px 60px rgba(0,0,0,.2);overflow:hidden}
.form-card iframe{display:block;width:100%;height:760px;border:none;border-radius:10px}
.form-fallback{padding:14px 10px 8px;text-align:center;font-size:13px;color:var(--gray)}
.form-fallback a{color:var(--green);font-weight:700;text-decoration:underline}
.contact .open-form{margin-top:28px}

/* ---------- Footer ---------- */
footer.site{background:var(--ink);color:rgba(255,255,255,.55);padding:56px 0;font-size:13.5px}
footer.site .top{display:flex;justify-content:space-between;gap:30px;flex-wrap:wrap;padding-bottom:30px;border-bottom:1px solid rgba(255,255,255,.12);margin-bottom:26px}
footer.site .logo{color:#fff}
footer.site nav{display:flex;gap:24px}
footer.site nav a:hover{color:#fff}
footer.site .legal{display:flex;justify-content:space-between;flex-wrap:wrap;gap:12px}

/* floating CTA */
.float-cta{position:fixed;right:26px;bottom:26px;z-index:90;box-shadow:0 14px 34px rgba(23,94,67,.4)}

/* reveal on scroll */
.reveal{opacity:0;transform:translateY(26px);transition:opacity .7s ease,transform .7s ease}
.reveal.in{opacity:1;transform:none}
@media(prefers-reduced-motion:reduce){
  .reveal{opacity:1;transform:none;transition:none}
  .hero h1 .hl::after{animation:none;transform:scaleX(1)}
  html{scroll-behavior:auto}
}

/* ---------- Responsive ---------- */
@media(max-width:960px){
  .hero-grid,.about-grid,.contact-grid{grid-template-columns:1fr}
  .svc-grid{grid-template-columns:1fr}
  .prog-grid,.case-grid,.insight-grid{grid-template-columns:1fr 1fr}
  .nav ul{display:none}
  .menu-toggle{display:block}
  .nav.open ul{display:flex;position:absolute;top:72px;left:0;right:0;background:#fff;flex-direction:column;padding:24px;gap:18px;border-bottom:1px solid var(--line)}
}
@media(max-width:600px){
  section{padding:76px 0}
  .hero{padding-top:140px}
  .prog-grid,.case-grid,.insight-grid{grid-template-columns:1fr}
  .ceo{padding:26px}
  .form-card iframe{height:680px}
}
</style>
</head>
<body>

<!-- ===== NAV ===== -->
<header id="header">
  <div class="wrap nav" id="nav">
    <a class="logo" href="#top">THE <em>WISE</em> CONSULTING</a>
    <ul>
      <li><a href="#about">회사소개</a></li>
      <li><a href="#services">사업영역</a></li>
      <li><a href="#programs">교육과정</a></li>
      <li><a href="#cases">고객사례</a></li>
      <li><a href="#insights">인사이트</a></li>
    </ul>
    <div style="display:flex;gap:12px;align-items:center">
      <a class="btn btn-primary" href="https://docs.google.com/forms/d/e/1FAIpQLSfky_2y_HdayvRIYDptsrdgaIuQ_l3Nn3VCoenrA29C_hPxNA/viewform?usp=header" target="_blank" rel="noopener">교육 문의하기</a>
      <button class="menu-toggle" aria-label="메뉴 열기" onclick="document.getElementById('nav').classList.toggle('open')">☰</button>
    </div>
  </div>
</header>

<!-- ===== HERO ===== -->
<section class="hero" id="top">
  <div class="wrap hero-grid">
    <div>
      <span class="eyebrow">HRD Total Solution Partner</span>
      <h1>사람의 성장이<br><span class="hl">기업의 성장</span>이 됩니다</h1>
      <p>더와이즈컨설팅은 교육과정 설계부터 운영, 성과 측정까지 HRD의 전 여정을 함께하는 기업교육 전문 파트너입니다.</p>
      <div class="hero-cta">
      </div>
    </div>
    <aside class="chain reveal" aria-label="HRD 밸류체인">
      <h3>HRD VALUE CHAIN</h3>
      <ol>
        <li><strong>진단 · 요구분석</strong><span>조직 · 직무 · 개인 단위 교육 니즈 도출</span></li>
        <li><strong>교육과정 설계</strong><span>역량모델 기반 맞춤형 커리큘럼 개발</span></li>
        <li><strong>교육 운영</strong><span>집합 · 라이브 · 블렌디드 원스톱 운영</span></li>
        <li><strong>성과 측정 · 보고</strong><span>4단계 평가와 데이터 기반 개선</span></li>
      </ol>
    </aside>
  </div>
</section>


<!-- ===== ABOUT ===== -->
<section class="about" id="about">
  <div class="wrap">
    <span class="eyebrow">About Us</span>
    <h2 class="title">지혜롭게 배우고,<br>단단하게 성장하는 조직을 만듭니다</h2>
    <p class="lead">더와이즈컨설팅은 '교육이 조직의 성과로 이어져야 한다'는 믿음으로, 일회성 교육이 아닌 성장의 구조를 설계합니다.</p>
    <div class="about-grid">
      <div class="ceo reveal">
        <blockquote>좋은 교육은 강의장에서 끝나지 않습니다. 현장의 행동이 바뀌고, 그 변화가 숫자로 증명될 때 비로소 교육은 완성됩니다. 더와이즈컨설팅은 그 마지막 순간까지 책임지는 파트너가 되겠습니다.</blockquote>
        <footer><b>대표 김윤정</b><br>The Wise Consulting CEO</footer>
      </div>
      <ul class="values">
        <li class="value reveal">
          <div class="ic" aria-hidden="true">🔍</div>
          <div><strong>Insight <small>통찰</small></strong><p>데이터와 현장 진단으로 조직의 진짜 교육 니즈를 발견합니다.</p></div>
        </li>
        <li class="value reveal">
          <div class="ic" aria-hidden="true">🌱</div>
          <div><strong>Growth <small>성장</small></strong><p>학습이 행동 변화로, 행동이 성과로 이어지는 성장 구조를 설계합니다.</p></div>
        </li>
        <li class="value reveal">
          <div class="ic" aria-hidden="true">🤝</div>
          <div><strong>Partnership <small>동행</small></strong><p>교육 담당자의 가장 든든한 실무 파트너로 처음부터 끝까지 함께합니다.</p></div>
        </li>
      </ul>
    </div>
  </div>
</section>

<!-- ===== SERVICES ===== -->
<section id="services">
  <div class="wrap">
    <span class="eyebrow">Our Services</span>
    <h2 class="title">HRD의 처음부터 끝까지,<br>하나의 파트너로 충분합니다</h2>
    <p class="lead">진단 – 설계 – 운영 – 평가로 이어지는 HRD 밸류체인 전 영역을 원스톱으로 제공합니다.</p>
    <div class="svc-grid">
      <article class="svc reveal">
        <span class="step">STEP 01 · DESIGN</span>
        <h3>교육과정 설계</h3>
        <p>요구분석부터 과정 개발, 콘텐츠 제작까지. ADDIE 모형과 역량모델링에 기반해 귀사만의 커리큘럼을 설계합니다.</p>
        <ul class="tags"><li>교육 요구분석</li><li>역량모델링</li><li>커리큘럼 개발</li><li>마이크로러닝 콘텐츠</li></ul>
      </article>
      <article class="svc reveal">
        <span class="step">STEP 02 · OPERATE</span>
        <h3>교육 운영</h3>
        <p>기획, 강사 섭외, 현장 운영, 결과 보고까지 원스톱. 집합교육·라이브 온라인·블렌디드 러닝 어떤 형태든 매끄럽게 운영합니다.</p>
        <ul class="tags"><li>집합교육</li><li>라이브 클래스</li><li>블렌디드 러닝</li><li>운영 대행</li></ul>
      </article>
      <article class="svc reveal">
        <span class="step">STEP 03 · LEAD</span>
        <h3>리더십 &amp; 조직개발</h3>
        <p>신임 리더부터 임원까지 리더십 파이프라인을 구축하고, 조직문화 진단과 워크숍으로 일하는 방식을 혁신합니다.</p>
        <ul class="tags"><li>계층별 리더십</li><li>조직문화 진단</li><li>팀빌딩 워크숍</li><li>코칭 프로그램</li></ul>
      </article>
      <article class="svc reveal">
        <span class="step">STEP 04 · MEASURE</span>
        <h3>성과 측정 &amp; HRD 컨설팅</h3>
        <p>커크패트릭 4단계 평가와 교육 ROI 분석으로 성과를 증명하고, 데이터에 기반해 HRD 체계 전반을 컨설팅합니다.</p>
        <ul class="tags"><li>4단계 평가</li><li>교육 ROI 리포트</li><li>HRD 체계 수립</li><li>연간 교육계획</li></ul>
      </article>
    </div>
  </div>
</section>

<!-- ===== PROGRAMS ===== -->
<section class="programs" id="programs">
  <div class="wrap">
    <span class="eyebrow">Programs</span>
    <h2 class="title">지금 조직에 필요한 교육,<br>여기 준비되어 있습니다</h2>
    <p class="lead">모든 과정은 귀사의 상황에 맞게 커스터마이징됩니다. 원하는 과정이 없다면, 함께 만들면 됩니다.</p>
    <div class="tabs" role="tablist" aria-label="교육과정 분류">
      <button class="tab on" data-f="all">전체</button>
      <button class="tab" data-f="lead">리더십</button>
      <button class="tab" data-f="job">직무역량</button>
      <button class="tab" data-f="cul">조직문화 · 소통</button>
      <button class="tab" data-f="dx">DX · AI</button>
      <button class="tab" data-f="new">신입 · 계층별</button>
    </div>
    <div class="prog-grid">
      <article class="prog reveal" data-c="lead">
        <span class="cat">LEADERSHIP</span>
        <h4>첫 리더의 90일</h4>
        <p>신임 팀장이 가장 먼저 겪는 실전 과제를 중심으로 한 리더십 온보딩 과정.</p>
        <div class="meta"><span>신임 팀장</span><span>16H</span></div>
        <span class="badge">커스터마이징 가능</span>
      </article>
      <article class="prog reveal" data-c="dx">
        <span class="cat">DX · AI</span>
        <h4>전 직원 AI 리터러시</h4>
        <p>생성형 AI를 업무에 바로 적용하는 실습 중심 프로그램. 직무별 활용 시나리오 제공.</p>
        <div class="meta"><span>전 직원</span><span>8H</span></div>
        <span class="badge">커스터마이징 가능</span>
      </article>
      <article class="prog reveal" data-c="cul">
        <span class="cat">CULTURE</span>
        <h4>세대공감 커뮤니케이션</h4>
        <p>세대 간 일하는 방식의 차이를 이해하고 협업 언어를 맞추는 워크숍형 과정.</p>
        <div class="meta"><span>전 구성원</span><span>7H</span></div>
        <span class="badge">커스터마이징 가능</span>
      </article>
      <article class="prog reveal" data-c="job">
        <span class="cat">JOB SKILL</span>
        <h4>문제해결 &amp; 기획력</h4>
        <p>로지컬씽킹부터 원페이지 보고서까지, 일 잘하는 사람의 사고 프로세스를 훈련합니다.</p>
        <div class="meta"><span>주니어~시니어</span><span>14H</span></div>
        <span class="badge">커스터마이징 가능</span>
      </article>
      <article class="prog reveal" data-c="new">
        <span class="cat">ONBOARDING</span>
        <h4>신입사원 온보딩 캠프</h4>
        <p>조직 적응, 비즈니스 매너, 협업 스킬을 담은 몰입형 온보딩 프로그램.</p>
        <div class="meta"><span>신입사원</span><span>2일</span></div>
        <span class="badge">커스터마이징 가능</span>
      </article>
      <article class="prog reveal" data-c="lead">
        <span class="cat">LEADERSHIP</span>
        <h4>임원 전략 리더십</h4>
        <p>비즈니스 관점의 의사결정과 조직 방향 설정을 다루는 임원 대상 소수정예 과정.</p>
        <div class="meta"><span>임원 · 본부장</span><span>12H</span></div>
        <span class="badge">커스터마이징 가능</span>
      </article>
    </div>
  </div>
</section>

<!-- ===== CASES ===== -->
<section id="cases">
  <div class="wrap">
    <span class="eyebrow">Success Stories</span>
    <h2 class="title">교육의 성과는<br>숫자로 증명됩니다</h2>
    <div class="case-grid">
      <article class="case reveal">
        <div class="head"><span class="ind">제조 · 대기업</span><h4>생산관리자 리더십 파이프라인 구축</h4></div>
        <dl class="body">
          <dt>Challenge</dt><dd>현장 관리자 승진 후 리더 역할 전환 실패율 증가</dd>
          <dt>Solution</dt><dd>역량진단 기반 3단계 리더십 여정 설계 · 12개월 운영</dd>
          <div class="result">리더십 진단 점수 27%p 향상</div>
        </dl>
      </article>
      <article class="case reveal">
        <div class="head"><span class="ind">금융</span><h4>전사 AI 리터러시 교육</h4></div>
        <dl class="body">
          <dt>Challenge</dt><dd>생성형 AI 도입 후 현업 활용률 저조</dd>
          <dt>Solution</dt><dd>직무별 활용 시나리오 개발 · 1,200명 블렌디드 운영</dd>
          <div class="result">주간 AI 활용률 3.4배 증가</div>
        </dl>
      </article>
      <article class="case reveal">
        <div class="head"><span class="ind">IT · 스타트업</span><h4>급성장 조직의 온보딩 체계 수립</h4></div>
        <dl class="body">
          <dt>Challenge</dt><dd>인원 2배 성장으로 조기 이탈 및 문화 희석 우려</dd>
          <dt>Solution</dt><dd>온보딩 여정맵 설계 · 버디 프로그램 · 90일 팔로업</dd>
          <div class="result">신규입사자 1년 잔존율 91% 달성</div>
        </dl>
      </article>
    </div>
    <div class="quote-band reveal">
      <blockquote>"교육을 맡긴 게 아니라, HRD 팀이 하나 더 생긴 느낌이었습니다. 요구분석부터 결과 보고까지 이렇게 꼼꼼한 파트너는 처음입니다."</blockquote>
      <footer>제조 대기업 인재개발팀 · 교육 담당 책임</footer>
    </div>
  </div>
</section>

<!-- ===== INSIGHTS ===== -->
<section id="insights" style="padding-top:0">
  <div class="wrap">
    <span class="eyebrow">Insights</span>
    <h2 class="title">HRD 트렌드, 한발 먼저 읽어드립니다</h2>
    <div class="insight-grid">
      <article class="post reveal">
        <span class="date">2026. 06 · HRD TREND</span>
        <h4>2026 하반기 기업교육 키워드 5가지</h4>
        <p>AI 협업 역량, 스킬 기반 조직, 마이크로러닝의 진화까지. 하반기 교육 계획에 담아야 할 트렌드를 정리했습니다.</p>
        <a class="more" href="#">읽어보기 →</a>
      </article>
      <article class="post reveal">
        <span class="date">2026. 05 · COLUMN</span>
        <h4>교육 만족도 95%인데 왜 성과는 그대로일까</h4>
        <p>반응 평가에 갇힌 교육 평가의 한계와, 행동 변화를 측정하는 실전 방법을 다룹니다.</p>
        <a class="more" href="#">읽어보기 →</a>
      </article>
      <article class="post reveal">
        <span class="date">2026. 04 · GUIDE</span>
        <h4>교육 담당자를 위한 연간 교육계획 수립 가이드</h4>
        <p>요구분석 설문 템플릿부터 예산 배분 기준까지, 실무에 바로 쓰는 체크리스트를 담았습니다.</p>
        <a class="more" href="#">읽어보기 →</a>
      </article>
    </div>
  </div>
</section>

<!-- ===== CONTACT ===== -->
<section class="contact" id="contact">
  <div class="wrap contact-grid">
    <div class="reveal">
      <h2>조직의 성장,<br>지금 이야기해 볼까요?</h2>
      <p class="sub">교육 니즈가 아직 명확하지 않아도 괜찮습니다. 무료 컨설팅을 통해 함께 방향을 찾아드립니다.</p>
      <div class="c-info">
        <div><span class="ic" aria-hidden="true">📞</span> 031-784-8315 (평일 09:00–18:00)</div>
        <div><span class="ic" aria-hidden="true">📞</span> 010-2310-5921 (상시)</div>
        <div><span class="ic" aria-hidden="true">📍</span> 경기도 화성시 동탄구 동탄기흥로 루체스타비즈 1017</div>
      </div>
      <a class="btn btn-ghost open-form" style="border-color:rgba(255,255,255,.4);color:#fff" href="https://docs.google.com/forms/d/e/1FAIpQLSfky_2y_HdayvRIYDptsrdgaIuQ_l3Nn3VCoenrA29C_hPxNA/viewform?usp=header" target="_blank" rel="noopener">문의 폼 새 창으로 열기 ↗</a>
    </div>
    <div class="form-card reveal">
      <iframe
        src="https://docs.google.com/forms/d/e/1FAIpQLSfky_2y_HdayvRIYDptsrdgaIuQ_l3Nn3VCoenrA29C_hPxNA/viewform?embedded=true"
        title="더와이즈컨설팅 교육 문의 폼"
        loading="lazy">
        불러오는 중…
      </iframe>
      <p class="form-fallback">폼이 보이지 않나요? <a href="https://docs.google.com/forms/d/e/1FAIpQLSfky_2y_HdayvRIYDptsrdgaIuQ_l3Nn3VCoenrA29C_hPxNA/viewform?usp=header" target="_blank" rel="noopener">여기를 눌러 문의 폼을 열어주세요</a>. 접수 후 3영업일 내 담당 컨설턴트가 연락드립니다.</p>
    </div>
  </div>
</section>

<!-- ===== FOOTER ===== -->
<footer class="site">
  <div class="wrap">
    <div class="top">
      <a class="logo" href="#top">THE <em style="color:var(--gold)">WISE</em> CONSULTING</a>
      <nav>
        <a href="#about">회사소개</a><a href="#services">사업영역</a><a href="#programs">교육과정</a><a href="#cases">고객사례</a><a href="https://docs.google.com/forms/d/e/1FAIpQLSfky_2y_HdayvRIYDptsrdgaIuQ_l3Nn3VCoenrA29C_hPxNA/viewform?usp=header" target="_blank" rel="noopener">문의</a>
      </nav>
    </div>
    <div class="legal">
      <span>(주)더와이즈컨설팅 · 대표 김윤정 · 사업자등록번호 736-27-01954 · 경기도 화성시 동탄구 동탄기흥로 루체스타비즈 1017</span>
      <span><a href="#">개인정보처리방침</a> · © 2021 The Wise Consulting. All rights reserved.</span>
    </div>
  </div>
</footer>

<a class="btn btn-primary float-cta" href="https://docs.google.com/forms/d/e/1FAIpQLSfky_2y_HdayvRIYDptsrdgaIuQ_l3Nn3VCoenrA29C_hPxNA/viewform?usp=header" target="_blank" rel="noopener">💬 교육 문의</a>

<script>
// nav shadow on scroll
const header=document.getElementById('header');
addEventListener('scroll',()=>header.classList.toggle('scrolled',scrollY>10),{passive:true});

// reveal on scroll
const io=new IntersectionObserver(es=>es.forEach(e=>{if(e.isIntersecting){e.target.classList.add('in');io.unobserve(e.target)}}),{threshold:.12});
document.querySelectorAll('.reveal').forEach(el=>io.observe(el));

// program filter tabs
document.querySelectorAll('.tab').forEach(tab=>tab.addEventListener('click',()=>{
  document.querySelectorAll('.tab').forEach(t=>t.classList.remove('on'));
  tab.classList.add('on');
  const f=tab.dataset.f;
  document.querySelectorAll('.prog').forEach(p=>{
    p.style.display=(f==='all'||p.dataset.c===f)?'':'none';
  });
}));
</script>
</body>
</html>
