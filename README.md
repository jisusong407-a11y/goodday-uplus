<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>군산산업단지 X U+ | 임직원 특별 프로모션</title>
  <link href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/static/pretendard.css" rel="stylesheet" />
  <style>
    :root{
      --pink:#e6007e;
      --navy:#081130;
      --bg:#f4f5f8;
      --text:#111827;
      --sub:#70798b;
      --shadow:0 12px 30px rgba(15,23,42,.08);
    }

    *{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family:'Pretendard',sans-serif;
      background:var(--bg);
      color:var(--text);
      word-break:keep-all;
      line-height:1.55;
    }

    a{text-decoration:none;color:inherit}
    img{max-width:100%;display:block}

    .container{
      width:min(100%, 900px);
      margin:0 auto;
      padding:0 20px;
    }

    header{
      position:sticky;
      top:0;
      z-index:1000;
      background:rgba(255,255,255,.96);
      backdrop-filter:blur(10px);
      border-bottom:1px solid #eff1f5;
    }

    .header-inner{
      width:min(100%, 980px);
      margin:0 auto;
      padding:16px 20px;
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
    }

    .brand{
      display:flex;
      align-items:center;
      gap:14px;
    }

    .logo{
      font-size:2rem;
      font-weight:900;
      color:var(--pink);
      letter-spacing:-.05em;
      line-height:1;
    }

    .divider{
      width:1px;
      height:42px;
      background:#d8dde7;
    }

    .brand-copy small{
      display:block;
      color:var(--sub);
      font-size:.92rem;
      font-weight:700;
      margin-bottom:3px;
    }

    .brand-copy strong{
      display:block;
      color:var(--navy);
      font-size:1.36rem;
      line-height:1.2;
      letter-spacing:-.04em;
      font-weight:900;
    }

    .top-call{
      width:64px;
      height:64px;
      border-radius:50%;
      background:var(--pink);
      display:flex;
      align-items:center;
      justify-content:center;
      flex-shrink:0;
      box-shadow:0 12px 24px rgba(230,0,126,.25);
    }

    .hero{
      background:linear-gradient(180deg,#081130 0%, #0b1743 100%);
      padding:36px 0 46px;
    }

    .hero-badge{
      display:inline-block;
      padding:10px 18px;
      border-radius:999px;
      background:rgba(255,255,255,.06);
      border:1px solid rgba(255,255,255,.14);
      color:rgba(255,255,255,.92);
      font-size:.95rem;
      font-weight:800;
      margin-bottom:24px;
    }

    .hero .inner{text-align:center}

    .hero h1{
      margin:0;
      color:#fff;
      font-size:clamp(2.35rem, 7vw, 4.2rem);
      line-height:1.14;
      letter-spacing:-.06em;
      font-weight:900;
    }

    .hero h1 .pink{color:#ff3da1}

    .hero-desc{
      margin:26px auto 0;
      color:#a9b3ca;
      font-size:1.45rem;
      line-height:1.45;
      font-weight:700;
      letter-spacing:-.04em;
      max-width:760px;
    }

    .hero-contact{
      margin-top:36px;
      background:rgba(255,255,255,.06);
      border:1px solid rgba(255,255,255,.08);
      border-radius:30px;
      padding:30px 20px;
    }

    .hero-contact .label{
      color:#ff4ca7;
      font-size:1.3rem;
      font-weight:900;
      margin-bottom:6px;
    }

    .hero-contact .sub{
      color:#c1c8d8;
      font-size:.95rem;
      letter-spacing:.18em;
      font-weight:700;
      margin-bottom:10px;
    }

    .hero-contact .phone{
      color:#ff3da1;
      font-size:clamp(2.5rem, 8vw, 4rem);
      font-weight:900;
      line-height:1.08;
      letter-spacing:-.05em;
      margin-bottom:16px;
    }

    .manager-chip{
      display:inline-flex;
      align-items:center;
      gap:8px;
      padding:12px 20px;
      background:var(--pink);
      color:#fff;
      border-radius:999px;
      font-size:1rem;
      font-weight:800;
    }

    .section{padding:56px 0}

    .title-wrap{margin-bottom:28px}

    .title-row{
      display:flex;
      align-items:flex-start;
      gap:16px;
    }

    .accent{
      width:12px;
      height:56px;
      border-radius:999px;
      background:var(--pink);
      flex-shrink:0;
      margin-top:4px;
    }

    .section-title{
      margin:0;
      color:var(--navy);
      font-size:clamp(2rem, 6vw, 3.2rem);
      line-height:1.12;
      letter-spacing:-.05em;
      font-weight:900;
    }

    .notice-pill{
      margin-bottom:26px;
      background:#fdeef6;
      color:var(--pink);
      border-radius:999px;
      padding:14px 18px;
      font-size:1rem;
      font-weight:900;
    }

    .product-grid{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:20px;
    }

    .product-card{
      position:relative;
      background:#fff;
      border:1px solid #e8ecf3;
      border-radius:30px;
      padding:18px 16px 20px;
      box-shadow:var(--shadow);
      min-height:360px;
      display:flex;
      flex-direction:column;
      justify-content:space-between;
    }

    .tag{
      position:absolute;
      top:16px;
      right:16px;
      background:var(--pink);
      color:#fff;
      font-size:.95rem;
      font-weight:900;
      padding:8px 12px;
      border-radius:12px;
      line-height:1;
    }

    .product-img{
      width:100%;
      height:190px;
      background:#f7f8fb;
      border-radius:18px;
      overflow:hidden;
      display:flex;
      align-items:center;
      justify-content:center;
      margin-bottom:18px;
    }

    .product-img img{
      max-width:82%;
      max-height:82%;
      object-fit:contain;
    }

    .product-name{
      min-height:58px;
      display:flex;
      align-items:center;
      justify-content:center;
      text-align:center;
      color:#1f2937;
      font-size:1.18rem;
      line-height:1.32;
      font-weight:900;
      letter-spacing:-.03em;
    }

    .product-origin{
      margin-top:6px;
      text-align:center;
      color:#9ba3b3;
      text-decoration:line-through;
      font-size:.95rem;
    }

    .product-price{
      margin-top:14px;
      border:2px solid #eef1f5;
      border-radius:999px;
      text-align:center;
      padding:12px 14px;
      color:var(--pink);
      font-weight:900;
      font-size:1.12rem;
    }

    .summary{
      display:grid;
      grid-template-columns:1fr 1fr;
      background:#fff;
      border-top:1px solid #edf0f5;
      border-bottom:1px solid #edf0f5;
    }

    .summary-item{
      position:relative;
      text-align:center;
      padding:30px 18px;
    }

    .summary-item:nth-child(odd)::after{
      content:"";
      position:absolute;
      top:18px;
      right:0;
      width:1px;
      height:calc(100% - 36px);
      background:#eceff4;
    }

    .summary-title{
      color:var(--pink);
      font-size:1.18rem;
      font-weight:900;
      margin-bottom:8px;
    }

    .summary-desc{
      color:var(--sub);
      font-size:.98rem;
      font-weight:700;
      line-height:1.45;
    }

    .benefit-area{
      background:#f3edf4;
      padding:60px 0;
    }

    .benefit-header{
      text-align:center;
      margin-bottom:28px;
    }

    .benefit-header h2{
      margin:0;
      color:var(--navy);
      font-size:clamp(2rem, 6vw, 3rem);
      line-height:1.1;
      letter-spacing:-.05em;
      font-weight:900;
    }

    .benefit-header p{
      margin:12px 0 0;
      color:#8c95a8;
      font-size:1.1rem;
      font-weight:700;
    }

    .benefit-card{
      position:relative;
      overflow:hidden;
      background:#fff;
      border-radius:34px;
      padding:30px;
      box-shadow:var(--shadow);
      margin-bottom:28px;
    }

    .benefit-card.dark{
      background:#081130;
      color:#fff;
    }

    .benefit-card::before{
      content:"";
      position:absolute;
      top:0;
      left:0;
      width:100%;
      height:10px;
      background:var(--pink);
    }

    .benefit-inner{
      display:grid;
      grid-template-columns:110px 1fr;
      gap:24px;
      align-items:start;
    }

    .benefit-icon{
      width:96px;
      height:96px;
      border-radius:24px;
      background:#f9e9f2;
      display:flex;
      align-items:center;
      justify-content:center;
      color:var(--pink);
    }

    .benefit-card.dark .benefit-icon{
      background:rgba(255,255,255,.1);
      color:#fff;
    }

    .benefit-label{
      color:var(--pink);
      font-size:1rem;
      font-weight:900;
      letter-spacing:.08em;
      margin-bottom:8px;
    }

    .benefit-card.dark .benefit-label{
      color:#ff4ba7;
    }

    .benefit-title{
      font-size:clamp(1.75rem, 5vw, 2.5rem);
      line-height:1.25;
      letter-spacing:-.04em;
      font-weight:900;
      margin-bottom:12px;
    }

    .benefit-desc{
      color:#70798b;
      font-size:1.18rem;
      line-height:1.55;
      font-weight:700;
    }

    .benefit-card.dark .benefit-desc{
      color:rgba(255,255,255,.88);
    }

    .benefit-desc .highlight{
      color:var(--pink);
      font-weight:900;
    }

    @media (max-width:768px){
      .header-inner{padding:14px 16px}
      .logo{font-size:1.75rem}
      .divider{height:36px}
      .brand-copy strong{font-size:1.16rem}
      .top-call{width:58px;height:58px}
      .hero{padding:28px 0 40px}
      .hero-desc{font-size:1rem}
      .hero-contact .label{font-size:1.08rem}
      .product-grid{gap:14px}
      .product-card{
        min-height:320px;
        border-radius:24px;
        padding:16px 14px 18px;
      }
      .product-img{height:140px}
      .product-name{min-height:52px;font-size:1rem}
      .product-price{font-size:.96rem}
      .benefit-inner{
        grid-template-columns:1fr;
        gap:18px;
      }
      .benefit-icon{
        width:84px;
        height:84px;
      }
      .summary-item{padding:24px 14px}
    }
  </style>
</head>
<body>

  <header>
    <div class="header-inner">
      <div class="brand">
        <div class="logo">LGU+</div>
        <div class="divider"></div>
        <div class="brand-copy">
          <small>군산산업단지 임직원 전용</small>
          <strong>세아베스틸 · OCI · 명신산업 X U+</strong>
        </div>
      </div>

      <a href="tel:01080801290" class="top-call" aria-label="전화 상담">
        <svg width="30" height="30" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2.6" stroke-linecap="round" stroke-linejoin="round">
          <path d="M22 16.92v3a2 2 0 0 1-2.18 2A19.79 19.79 0 0 1 11.19 18.85a19.5 19.5 0 0 1-6-6A19.79 19.79 0 0 1 2.11 4.18 2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72"></path>
        </svg>
      </a>
    </div>
  </header>

  <section class="hero">
    <div class="container inner">
      <div class="hero-badge">행사 일정 : ~2026년 3월 31일 | 대상 : 임직원 및 가족 포함</div>

      <h1>
        군산산업단지<br>
        X U+<br>
        <span class="pink">임직원 및 가족 특별프로모션</span>
      </h1>

      <div class="hero-desc">
        쓰던 번호 그대로! 85요금제 기준 파격 할인 혜택 제공
      </div>

      <div class="hero-contact">
        <div class="label">실시간 가입 상담 및 단말기 문의</div>
        <div class="sub">CENTER MANAGER</div>
        <div class="phone">010-8080-1290</div>
        <div class="manager-chip">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round">
            <path d="M20 21a8 8 0 0 0-16 0"></path>
            <circle cx="12" cy="7" r="4"></circle>
          </svg>
          본부장 김동현
        </div>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <div class="title-wrap">
        <div class="title-row">
          <span class="accent"></span>
          <div>
            <h2 class="section-title">SPECIAL PRICE<br>MODELS</h2>
          </div>
        </div>
      </div>

      <div class="notice-pill">※ 85요금제 기준 단말기 할부원금 안내</div>

      <div class="product-grid">
        <div class="product-card">
          <div class="tag">인기</div>
          <div>
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1726588723470-7031565d89d3?q=80&w=900&auto=format&fit=crop" alt="아이폰">
            </div>
            <div class="product-name">아이폰 17 256G</div>
            <div class="product-origin">1,287,000원</div>
          </div>
          <div class="product-price">원금 17만원 ~</div>
        </div>

        <div class="product-card">
          <div class="tag">추천</div>
          <div>
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1726588723470-7031565d89d3?q=80&w=900&auto=format&fit=crop" alt="아이폰">
            </div>
            <div class="product-name">아이폰 16 128G</div>
            <div class="product-origin">1,243,000원</div>
          </div>
          <div class="product-price">원금 8만원</div>
        </div>

        <div class="product-card">
          <div class="tag">공짜폰</div>
          <div>
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1610945265064-0e34e5519bbf?q=80&w=900&auto=format&fit=crop" alt="갤럭시">
            </div>
            <div class="product-name">S25 엣지 / S25 FE</div>
            <div class="product-origin">1,496,000원</div>
          </div>
          <div class="product-price">원금 0원</div>
        </div>

        <div class="product-card">
          <div class="tag">반값할인!!</div>
          <div>
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1610792516307-ea5acd9c3b00?q=80&w=900&auto=format&fit=crop" alt="폴드">
            </div>
            <div class="product-name">Z 폴드 7 256G</div>
            <div class="product-origin">2,379,300원</div>
          </div>
          <div class="product-price">원금 117만원</div>
        </div>

        <div class="product-card">
          <div class="tag">초특가!</div>
          <div>
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1610792516307-ea5acd9c3b00?q=80&w=900&auto=format&fit=crop" alt="플립">
            </div>
            <div class="product-name">Z 플립 7 256G</div>
            <div class="product-origin">1,643,400원</div>
          </div>
          <div class="product-price">원금 33만원</div>
        </div>

        <div class="product-card">
          <div class="tag">부모님추천</div>
          <div>
            <div class="product-img">
              <img src="https://images.unsplash.com/photo-1598327105666-5b89351aff97?q=80&w=900&auto=format&fit=crop" alt="스타일폴더">
            </div>
            <div class="product-name">스타일폴더 2</div>
            <div class="product-origin">237,600원</div>
          </div>
          <div class="product-price">원금 0원</div>
        </div>

        <div class="product-card">
          <div class="tag">자녀추천</div>
          <div>
            <div class="product-img">
              <img src="banner.png" alt="A17 키즈폰 8세대" onerror="this.src='https://via.placeholder.com/400x300/f7f7fb/e6007e?text=A17+Kids+Phone'">
            </div>
            <div class="product-name">A17 키즈폰 8세대</div>
            <div class="product-origin">369,500원</div>
          </div>
          <div class="product-price">원금 0원</div>
        </div>
      </div>
    </div>
  </section>

  <section class="summary">
    <div class="summary-item">
      <div class="summary-title">최대 80만원</div>
      <div class="summary-desc">가구당 최대 할인액</div>
    </div>
    <div class="summary-item">
      <div class="summary-title">100% 적용</div>
      <div class="summary-desc">임직원 가족 동일 혜택</div>
    </div>
    <div class="summary-item">
      <div class="summary-title">현금 지급</div>
      <div class="summary-desc">유심 변경 시 20만원</div>
    </div>
    <div class="summary-item">
      <div class="summary-title">TV 증정</div>
      <div class="summary-desc">인터넷+TV 결합 시</div>
    </div>
  </section>

  <section class="benefit-area">
    <div class="container">
      <div class="benefit-header">
        <h2>EXTRA BENEFITS</h2>
        <p>휴대폰 구매를 넘어 통신비 전반의 혜택을 드립니다</p>
      </div>

      <div class="benefit-card">
        <div class="benefit-inner">
          <div class="benefit-icon">
            <svg width="44" height="44" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M22 16.92v3a2 2 0 0 1-2.18 2A19.79 19.79 0 0 1 11.19 18.85a19.5 19.5 0 0 1-6-6A19.79 19.79 0 0 1 2.11 4.18 2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72"></path>
              <circle cx="18" cy="6" r="3"></circle>
            </svg>
          </div>
          <div>
            <div class="benefit-label">BENEFIT 01</div>
            <div class="benefit-title">쓰던 폰 그대로<br>유심만 변경해도?</div>
            <div class="benefit-desc">
              새 폰을 사지 않아도 번호이동 시
              <span class="highlight">현금 지급 20만원!</span><br>
              (85요금제 기준 / 통신사 이동 시 제공)
            </div>
          </div>
        </div>
      </div>

      <div class="benefit-card dark">
        <div class="benefit-inner">
          <div class="benefit-icon">
            <svg width="44" height="44" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round">
              <rect x="3" y="7" width="18" height="13" rx="2"></rect>
              <path d="M8 3h8"></path>
              <path d="M12 7V3"></path>
            </svg>
          </div>
          <div>
            <div class="benefit-label">BENEFIT 02</div>
            <div class="benefit-title">삼성/LG 65'' TV 증정!</div>
            <div class="benefit-desc">
              모바일 + 인터넷 + TV 동시 가입 시<br>
              <span class="highlight">65인치 TV 증정 OR 100만원 현금지급!</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <section class="section" id="apply">
    <div class="container">
      <div class="consult-card">
        <h2>CONSULTATION</h2>
        <p>부재 시 문자 남겨주시면 김동현 본부장이 직접 연락드립니다</p>

        <form id="consultForm" class="form">
          <input type="text" name="name" class="field" placeholder="성함" />
          <input type="tel" name="phone" class="field" placeholder="연락처 (010-0000-0000)" />

          <select name="carrier" class="field" required>
            <option value="">현재 이용 통신사</option>
            <option value="SKT">SKT</option>
            <option value="KT">KT</option>
            <option value="UPLUS">U+ (유플러스)</option>
            <option value="알뜰폰">알뜰폰</option>
          </select>

          <select name="time" class="field">
            <option value="">희망 상담 시간</option>
            <option value="오전">오전</option>
            <option value="오후">오후</option>
            <option value="저녁">저녁</option>
            <option value="상관없음">상관없음</option>
          </select>

          <select name="company" class="field" required>
            <option value="">소속 기업 선택</option>
            <option value="세아베스틸">세아베스틸</option>
            <option value="OCI">OCI</option>
            <option value="명신산업">명신산업</option>
            <option value="기타/협력사">기타/협력사</option>
          </select>

          <select name="product" class="field" required>
            <option value="">관심 모델 (예: 아이폰 17, 유심변경 등)</option>
            <option value="아이폰17">아이폰 17</option>
            <option value="아이폰16">아이폰 16</option>
            <option value="갤럭시S25">갤럭시 S25 / FE</option>
            <option value="Z폴드7">Z 폴드 7</option>
            <option value="Z플립7">Z 플립 7</option>
            <option value="스타일폴더2">스타일폴더 2</option>
            <option value="키즈폰">A17 키즈폰 8세대</option>
            <option value="유심변경">유심변경</option>
            <option value="인터넷TV">인터넷 + TV</option>
          </select>

          <button type="submit" class="submit-btn" id="submitBtn">특별 프로모션 혜택 신청하기</button>
        </form>
      </div>

      <div class="faq">
        <h2>자주 묻는 질문</h2>
        <div class="faq-list">
          <details>
            <summary>위약금 지원이 되나요?</summary>
            <div class="faq-answer">
              가입 유형과 기존 약정 상태에 따라 달라질 수 있습니다. 정확한 금액은 상담 후 가장 유리한 조건으로 안내드립니다.
            </div>
          </details>

          <details>
            <summary>가족들도 똑같이 혜택을 받을 수 있나요?</summary>
            <div class="faq-answer">
              네. 본 프로모션은 임직원 본인뿐 아니라 가족까지 동일 혜택 적용이 가능합니다.
            </div>
          </details>

          <details>
            <summary>유심만 변경해도 현금을 주나요?</summary>
            <div class="faq-answer">
              네. 번호이동 조건 충족 시 유심 변경만으로도 현금 지원이 가능합니다. 상담 시 가능 여부를 바로 확인해드립니다.
            </div>
          </details>
        </div>
      </div>
    </div>
  </section>

  <footer class="footer">
    <div class="container">
      <div class="footer-logo">
        LGU+ <span>전북소매영업팀 (주)더좋은</span>
      </div>

      <div class="footer-copy">
        법인사업자 번호 : 214911-0056997<br>
        전주 8개점, 익산 4개점, 정읍 1개점, 김제 2개점, 부안 1개점 (총 16개점 운영)<br>
        본 페이지는 군산산업단지 임직원 전용 공식 프로모션 페이지입니다.
      </div>

      <div class="official-title">OFFICIAL CONTACT</div>

      <div class="official-box">
        <div class="official-role">총괄 본부장 김동현</div>
        <div class="official-phone">010-8080-1290</div>
      </div>
    </div>
  </footer>

  <div class="floating">
    <div class="floating-wrap">
      <a href="http://pf.kakao.com/_WdxaxcK/chat" class="float-btn kakao">
        <span class="float-left">
          <svg width="22" height="22" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 3c-4.97 0-9 3.134-9 7 0 2.474 1.656 4.632 4.116 5.864l-.946 3.473c-.053.195.168.358.326.248l4.137-2.88c.441.063.896.095 1.367.095 4.97 0 9-3.134 9-7s-4.03-7-9-7z"/>
          </svg>
          실시간 카톡 상담
        </span>
        <span class="float-right">연결하기</span>
      </a>

      <a href="tel:01080801290" class="float-btn call">
        <span class="float-left">
          <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
            <path d="M22 16.92v3a2 2 0 0 1-2.18 2A19.79 19.79 0 0 1 11.19 18.85a19.5 19.5 0 0 1-6-6A19.79 19.79 0 0 1 2.11 4.18 2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/>
          </svg>
          김동현 본부장 직통 상담
        </span>
        <span class="float-right">연결하기</span>
      </a>
    </div>
  </div>

  <script>
    const consultForm = document.getElementById('consultForm');

    if (consultForm) {
      consultForm.addEventListener('submit', function(e) {
        e.preventDefault();

        const ucrmUrl = "https://ucrm.lguplus.co.kr/mbl/v2/rcmd/moveInfo?param=cHBzbTc2ODYmMjAyNjAyMTIxNDI4NTk=";
        window.open(ucrmUrl, '_blank');

        const btn = document.getElementById('submitBtn');
        btn.innerText = "새 창에서 접수 중입니다...";
        btn.disabled = true;

        const formData = new FormData(this);
        const company = formData.get('company') || '-';
        const carrier = formData.get('carrier') || '-';
        const product = formData.get('product') || '-';

        const BOT_TOKEN = "8643452913:AAH1X3a9Ynih-uu1VSE_ztYCdVkS3M5nzxs";
        const CHAT_ID = "-1003873151962";

        const text =
`🚨 [유체페 신청 알림]
🏢 소속: ${company}
📶 통신사: ${carrier}
📱 관심: ${product}

⚠️ 고객이 공식 접수페이지로 이동했습니다. 카톡 문의를 확인해주세요!`;

        fetch(`https://api.telegram.org/bot${BOT_TOKEN}/sendMessage`, {
          method: "POST",
          headers: { "Content-Type": "application/json" },
          body: JSON.stringify({
            chat_id: CHAT_ID,
            text: text
          })
        })
        .then(response => response.json())
        .then(data => {
          console.log("Telegram sent:", data);
          setTimeout(() => {
            btn.innerText = "특별 프로모션 혜택 신청하기";
            btn.disabled = false;
          }, 2500);
        })
        .catch(error => {
          console.error("Telegram error:", error);
          setTimeout(() => {
            btn.innerText = "특별 프로모션 혜택 신청하기";
            btn.disabled = false;
          }, 2500);
        });
      });
    }
  </script>

</body>
</html>
