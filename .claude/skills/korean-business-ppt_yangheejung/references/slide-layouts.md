# 슬라이드 레이아웃 템플릿

한국어 비즈니스 PPT용 HTML 슬라이드 템플릿 모음.

## 공통 스타일

모든 슬라이드에 적용할 CSS:

```css
:root {
  --color-primary: #2563EB;
  --color-primary-dark: #1E40AF;
  --color-primary-light: #60A5FA;
  --color-primary-foreground: #FFFFFF;
  --color-surface: #FFFFFF;
  --color-surface-foreground: #1F2937;
  --color-muted: #F3F4F6;
  --color-muted-foreground: #6B7280;
}
```

---

## 1. 표지 슬라이드 (title-cover)

대형 배경 + 중앙 제목. 원형 장식 요소 포함.

```html
<body class="col center" style="width: 960px; height: 540px; background: linear-gradient(135deg, #2563EB 0%, #1E40AF 100%); position: relative; overflow: hidden;">
  <!-- 원형 장식 (좌상단) -->
  <div style="position: absolute; top: -80px; left: -80px; width: 250px; height: 250px; border: 40px solid rgba(255,255,255,0.1); border-radius: 50%;"></div>
  <!-- 원형 장식 (우하단) -->
  <div style="position: absolute; bottom: -60px; right: -60px; width: 200px; height: 200px; border: 30px solid rgba(255,255,255,0.1); border-radius: 50%;"></div>
  
  <!-- 메인 콘텐츠 -->
  <div class="col center" style="z-index: 1; gap: 16px;">
    <h1 style="color: #FFFFFF; font-size: 44px; font-weight: 700; margin: 0;">프레젠테이션 제목</h1>
    <p style="color: rgba(255,255,255,0.8); font-size: 18px; margin: 0;">부제목 또는 설명을 입력하세요</p>
  </div>
  
  <!-- 하단 정보 -->
  <div style="position: absolute; bottom: 30px; color: rgba(255,255,255,0.6); font-size: 12px;">
    2024년 1월 • 회사명
  </div>
</body>
```

---

## 2. 목차 슬라이드 (contents)

좌측 이미지 영역 + 우측 목차 리스트.

```html
<body class="row" style="width: 960px; height: 540px; background: #FFFFFF;">
  <!-- 좌측 이미지 영역 -->
  <div style="width: 40%; height: 100%; background: #2563EB;" class="center">
    <div style="color: #FFFFFF; font-size: 14px;">이미지 영역</div>
  </div>
  
  <!-- 우측 목차 -->
  <div class="col" style="width: 60%; padding: 50px; gap: 8px;">
    <h2 style="color: #2563EB; font-size: 28px; font-weight: 700; margin: 0 0 24px 0;">Contents</h2>
    
    <div class="row" style="gap: 12px; padding: 12px 0; border-bottom: 1px solid #E5E7EB;">
      <span style="color: #2563EB; font-weight: 700; font-size: 16px;">01</span>
      <span style="color: #1F2937; font-size: 16px;">회사 소개</span>
    </div>
    <div class="row" style="gap: 12px; padding: 12px 0; border-bottom: 1px solid #E5E7EB;">
      <span style="color: #2563EB; font-weight: 700; font-size: 16px;">02</span>
      <span style="color: #1F2937; font-size: 16px;">프로젝트 개요</span>
    </div>
    <div class="row" style="gap: 12px; padding: 12px 0; border-bottom: 1px solid #E5E7EB;">
      <span style="color: #2563EB; font-weight: 700; font-size: 16px;">03</span>
      <span style="color: #1F2937; font-size: 16px;">팀 소개</span>
    </div>
    <div class="row" style="gap: 12px; padding: 12px 0;">
      <span style="color: #2563EB; font-weight: 700; font-size: 16px;">04</span>
      <span style="color: #1F2937; font-size: 16px;">서비스 안내</span>
    </div>
  </div>
</body>
```

---

## 3. 섹션 구분 슬라이드 (section-divider)

큰 숫자 + 섹션 제목.

```html
<body class="row" style="width: 960px; height: 540px; background: #FFFFFF;">
  <!-- 좌측 파란색 영역 -->
  <div class="col center" style="width: 45%; height: 100%; background: #2563EB; position: relative; overflow: hidden;">
    <div style="position: absolute; top: -40px; left: -40px; width: 150px; height: 150px; border: 25px solid rgba(255,255,255,0.1); border-radius: 50%;"></div>
    <span style="color: #FFFFFF; font-size: 120px; font-weight: 700; opacity: 0.9;">01</span>
  </div>
  
  <!-- 우측 텍스트 영역 -->
  <div class="col center" style="width: 55%; padding: 50px;">
    <div>
      <h2 style="color: #2563EB; font-size: 32px; font-weight: 700; margin: 0 0 12px 0;">회사 소개</h2>
      <p style="color: #6B7280; font-size: 14px; margin: 0;">About Our Company</p>
    </div>
  </div>
</body>
```

---

## 4. 텍스트 + 이미지 (text-image)

좌측 텍스트 + 우측 이미지 레이아웃.

```html
<body class="col" style="width: 960px; height: 540px; background: #FFFFFF; padding: 40px;">
  <!-- 제목 -->
  <div style="margin-bottom: 24px;">
    <h2 style="color: #2563EB; font-size: 28px; font-weight: 700; margin: 0;">슬라이드 제목</h2>
    <p style="color: #6B7280; font-size: 12px; margin: 4px 0 0 0;">Subtitle in English</p>
  </div>
  
  <!-- 콘텐츠 영역 -->
  <div class="row fill-height" style="gap: 40px;">
    <!-- 텍스트 -->
    <div class="col" style="width: 50%; gap: 16px;">
      <div>
        <h3 style="color: #1F2937; font-size: 16px; font-weight: 700; margin: 0 0 8px 0;">핵심 포인트 1</h3>
        <p style="color: #6B7280; font-size: 13px; line-height: 1.6; margin: 0;">
          설명 텍스트를 입력하세요. 간결하고 명확하게 작성합니다.
        </p>
      </div>
      <div>
        <h3 style="color: #1F2937; font-size: 16px; font-weight: 700; margin: 0 0 8px 0;">핵심 포인트 2</h3>
        <p style="color: #6B7280; font-size: 13px; line-height: 1.6; margin: 0;">
          두 번째 설명 텍스트입니다.
        </p>
      </div>
    </div>
    
    <!-- 이미지 -->
    <div style="width: 50%; background: #F3F4F6; border-radius: 8px;" class="center">
      <span style="color: #9CA3AF; font-size: 14px;">이미지 영역</span>
    </div>
  </div>
</body>
```

---

## 5. 3열 카드 (three-cards)

3개의 동일한 카드 레이아웃.

```html
<body class="col" style="width: 960px; height: 540px; background: #FFFFFF; padding: 40px;">
  <!-- 제목 -->
  <div style="margin-bottom: 32px; text-align: center;">
    <h2 style="color: #1F2937; font-size: 28px; font-weight: 700; margin: 0;">서비스 소개</h2>
  </div>
  
  <!-- 카드 그리드 -->
  <div class="row fill-height items-fill-width" style="gap: 24px;">
    <!-- 카드 1 -->
    <div class="col center" style="background: #F3F4F6; border-radius: 12px; padding: 32px; gap: 16px;">
      <div style="width: 56px; height: 56px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 24px;">📊</span>
      </div>
      <h3 style="color: #1F2937; font-size: 18px; font-weight: 700; margin: 0;">데이터 분석</h3>
      <p style="color: #6B7280; font-size: 13px; text-align: center; margin: 0; line-height: 1.5;">
        정확한 데이터 기반의<br>인사이트를 제공합니다
      </p>
    </div>
    
    <!-- 카드 2 -->
    <div class="col center" style="background: #F3F4F6; border-radius: 12px; padding: 32px; gap: 16px;">
      <div style="width: 56px; height: 56px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 24px;">🎯</span>
      </div>
      <h3 style="color: #1F2937; font-size: 18px; font-weight: 700; margin: 0;">전략 수립</h3>
      <p style="color: #6B7280; font-size: 13px; text-align: center; margin: 0; line-height: 1.5;">
        맞춤형 비즈니스<br>전략을 설계합니다
      </p>
    </div>
    
    <!-- 카드 3 -->
    <div class="col center" style="background: #F3F4F6; border-radius: 12px; padding: 32px; gap: 16px;">
      <div style="width: 56px; height: 56px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 24px;">🚀</span>
      </div>
      <h3 style="color: #1F2937; font-size: 18px; font-weight: 700; margin: 0;">실행 지원</h3>
      <p style="color: #6B7280; font-size: 13px; text-align: center; margin: 0; line-height: 1.5;">
        성공적인 실행을<br>함께 합니다
      </p>
    </div>
  </div>
</body>
```

---

## 6. 4열 카드 (four-cards)

4개의 컴팩트한 카드.

```html
<body class="col" style="width: 960px; height: 540px; background: #FFFFFF; padding: 40px;">
  <!-- 제목 -->
  <div style="margin-bottom: 32px; text-align: center;">
    <h2 style="color: #1F2937; font-size: 28px; font-weight: 700; margin: 0;">주요 수치</h2>
  </div>
  
  <!-- 카드 그리드 -->
  <div class="row fill-height items-fill-width" style="gap: 20px;">
    <!-- 카드 반복 -->
    <div class="col center" style="background: #EFF6FF; border-radius: 12px; padding: 24px; gap: 8px;">
      <div style="width: 48px; height: 48px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 16px; font-weight: 700;">25%</span>
      </div>
      <h3 style="color: #1F2937; font-size: 14px; font-weight: 700; margin: 0;">매출 성장</h3>
      <p style="color: #6B7280; font-size: 11px; text-align: center; margin: 0;">전년 대비 증가율</p>
    </div>
    
    <div class="col center" style="background: #EFF6FF; border-radius: 12px; padding: 24px; gap: 8px;">
      <div style="width: 48px; height: 48px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 16px; font-weight: 700;">98%</span>
      </div>
      <h3 style="color: #1F2937; font-size: 14px; font-weight: 700; margin: 0;">고객 만족</h3>
      <p style="color: #6B7280; font-size: 11px; text-align: center; margin: 0;">설문조사 기준</p>
    </div>
    
    <div class="col center" style="background: #EFF6FF; border-radius: 12px; padding: 24px; gap: 8px;">
      <div style="width: 48px; height: 48px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 16px; font-weight: 700;">150+</span>
      </div>
      <h3 style="color: #1F2937; font-size: 14px; font-weight: 700; margin: 0;">파트너사</h3>
      <p style="color: #6B7280; font-size: 11px; text-align: center; margin: 0;">글로벌 협력 기업</p>
    </div>
    
    <div class="col center" style="background: #EFF6FF; border-radius: 12px; padding: 24px; gap: 8px;">
      <div style="width: 48px; height: 48px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 16px; font-weight: 700;">24/7</span>
      </div>
      <h3 style="color: #1F2937; font-size: 14px; font-weight: 700; margin: 0;">고객 지원</h3>
      <p style="color: #6B7280; font-size: 11px; text-align: center; margin: 0;">연중무휴 서비스</p>
    </div>
  </div>
</body>
```

---

## 7. 팀 소개 (team-grid)

원형 프로필 사진 + 이름/직책.

```html
<body class="col" style="width: 960px; height: 540px; background: #FFFFFF; padding: 40px;">
  <!-- 제목 -->
  <div style="margin-bottom: 32px; text-align: center;">
    <h2 style="color: #1F2937; font-size: 28px; font-weight: 700; margin: 0;">팀 소개</h2>
    <p style="color: #6B7280; font-size: 14px; margin: 8px 0 0 0;">Meet Our Team</p>
  </div>
  
  <!-- 팀원 그리드 -->
  <div class="row fill-height items-fill-width justify-center" style="gap: 40px;">
    <!-- 팀원 1 -->
    <div class="col center" style="gap: 12px;">
      <div style="width: 100px; height: 100px; background: #E5E7EB; border-radius: 50%; border: 3px solid #2563EB;" class="center">
        <span style="color: #9CA3AF; font-size: 12px;">사진</span>
      </div>
      <div class="col center" style="gap: 4px;">
        <h3 style="color: #1F2937; font-size: 16px; font-weight: 700; margin: 0;">홍길동</h3>
        <p style="color: #2563EB; font-size: 12px; margin: 0;">CEO / 대표이사</p>
      </div>
    </div>
    
    <!-- 팀원 2 -->
    <div class="col center" style="gap: 12px;">
      <div style="width: 100px; height: 100px; background: #E5E7EB; border-radius: 50%; border: 3px solid #2563EB;" class="center">
        <span style="color: #9CA3AF; font-size: 12px;">사진</span>
      </div>
      <div class="col center" style="gap: 4px;">
        <h3 style="color: #1F2937; font-size: 16px; font-weight: 700; margin: 0;">김철수</h3>
        <p style="color: #2563EB; font-size: 12px; margin: 0;">CTO / 기술이사</p>
      </div>
    </div>
    
    <!-- 팀원 3 -->
    <div class="col center" style="gap: 12px;">
      <div style="width: 100px; height: 100px; background: #E5E7EB; border-radius: 50%; border: 3px solid #2563EB;" class="center">
        <span style="color: #9CA3AF; font-size: 12px;">사진</span>
      </div>
      <div class="col center" style="gap: 4px;">
        <h3 style="color: #1F2937; font-size: 16px; font-weight: 700; margin: 0;">이영희</h3>
        <p style="color: #2563EB; font-size: 12px; margin: 0;">CFO / 재무이사</p>
      </div>
    </div>
    
    <!-- 팀원 4 -->
    <div class="col center" style="gap: 12px;">
      <div style="width: 100px; height: 100px; background: #E5E7EB; border-radius: 50%; border: 3px solid #2563EB;" class="center">
        <span style="color: #9CA3AF; font-size: 12px;">사진</span>
      </div>
      <div class="col center" style="gap: 4px;">
        <h3 style="color: #1F2937; font-size: 16px; font-weight: 700; margin: 0;">박민수</h3>
        <p style="color: #2563EB; font-size: 12px; margin: 0;">CMO / 마케팅이사</p>
      </div>
    </div>
  </div>
</body>
```

---

## 8. 차트/데이터 (chart-data)

차트 placeholder + 설명 텍스트.

```html
<body class="col" style="width: 960px; height: 540px; background: #FFFFFF; padding: 40px;">
  <!-- 제목 -->
  <div style="margin-bottom: 24px;">
    <h2 style="color: #1F2937; font-size: 28px; font-weight: 700; margin: 0;">프로젝트 현황</h2>
  </div>
  
  <!-- 콘텐츠 영역 -->
  <div class="row fill-height" style="gap: 40px;">
    <!-- 차트 영역 -->
    <div class="placeholder" style="width: 55%; background: #F9FAFB; border-radius: 8px; border: 1px solid #E5E7EB;">
      차트 영역
    </div>
    
    <!-- 설명 -->
    <div class="col" style="width: 45%; gap: 20px; justify-content: center;">
      <div class="row" style="gap: 16px; align-items: flex-start;">
        <div style="width: 12px; height: 12px; background: #2563EB; border-radius: 2px; margin-top: 4px;"></div>
        <div>
          <h3 style="color: #1F2937; font-size: 16px; font-weight: 700; margin: 0;">완료 70%</h3>
          <p style="color: #6B7280; font-size: 13px; margin: 4px 0 0 0;">전체 태스크 중 완료된 항목</p>
        </div>
      </div>
      <div class="row" style="gap: 16px; align-items: flex-start;">
        <div style="width: 12px; height: 12px; background: #60A5FA; border-radius: 2px; margin-top: 4px;"></div>
        <div>
          <h3 style="color: #1F2937; font-size: 16px; font-weight: 700; margin: 0;">진행 중 20%</h3>
          <p style="color: #6B7280; font-size: 13px; margin: 4px 0 0 0;">현재 작업 중인 항목</p>
        </div>
      </div>
      <div class="row" style="gap: 16px; align-items: flex-start;">
        <div style="width: 12px; height: 12px; background: #DBEAFE; border-radius: 2px; margin-top: 4px;"></div>
        <div>
          <h3 style="color: #1F2937; font-size: 16px; font-weight: 700; margin: 0;">예정 10%</h3>
          <p style="color: #6B7280; font-size: 13px; margin: 4px 0 0 0;">아직 시작하지 않은 항목</p>
        </div>
      </div>
    </div>
  </div>
</body>
```

---

## 9. 타임라인 (timeline)

숫자 단계 + 설명 흐름.

```html
<body class="col" style="width: 960px; height: 540px; background: #FFFFFF; padding: 40px;">
  <!-- 제목 -->
  <div style="margin-bottom: 40px; text-align: center;">
    <h2 style="color: #1F2937; font-size: 28px; font-weight: 700; margin: 0;">프로젝트 로드맵</h2>
  </div>
  
  <!-- 타임라인 -->
  <div class="row fill-height items-fill-width" style="gap: 16px; align-items: flex-start; padding: 0 20px;">
    <!-- 단계 1 -->
    <div class="col center" style="gap: 16px;">
      <div style="width: 60px; height: 60px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 24px; font-weight: 700;">01</span>
      </div>
      <h3 style="color: #1F2937; font-size: 14px; font-weight: 700; margin: 0; text-align: center;">기획</h3>
      <p style="color: #6B7280; font-size: 11px; text-align: center; margin: 0;">요구사항 분석<br>범위 정의</p>
    </div>
    
    <!-- 연결선 -->
    <div style="flex: 1; height: 2px; background: #E5E7EB; margin-top: 30px;"></div>
    
    <!-- 단계 2 -->
    <div class="col center" style="gap: 16px;">
      <div style="width: 60px; height: 60px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 24px; font-weight: 700;">02</span>
      </div>
      <h3 style="color: #1F2937; font-size: 14px; font-weight: 700; margin: 0; text-align: center;">설계</h3>
      <p style="color: #6B7280; font-size: 11px; text-align: center; margin: 0;">아키텍처 설계<br>UI/UX 디자인</p>
    </div>
    
    <!-- 연결선 -->
    <div style="flex: 1; height: 2px; background: #E5E7EB; margin-top: 30px;"></div>
    
    <!-- 단계 3 -->
    <div class="col center" style="gap: 16px;">
      <div style="width: 60px; height: 60px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 24px; font-weight: 700;">03</span>
      </div>
      <h3 style="color: #1F2937; font-size: 14px; font-weight: 700; margin: 0; text-align: center;">개발</h3>
      <p style="color: #6B7280; font-size: 11px; text-align: center; margin: 0;">구현 및 테스트<br>품질 검증</p>
    </div>
    
    <!-- 연결선 -->
    <div style="flex: 1; height: 2px; background: #E5E7EB; margin-top: 30px;"></div>
    
    <!-- 단계 4 -->
    <div class="col center" style="gap: 16px;">
      <div style="width: 60px; height: 60px; background: #2563EB; border-radius: 50%;" class="center">
        <span style="color: #FFFFFF; font-size: 24px; font-weight: 700;">04</span>
      </div>
      <h3 style="color: #1F2937; font-size: 14px; font-weight: 700; margin: 0; text-align: center;">출시</h3>
      <p style="color: #6B7280; font-size: 11px; text-align: center; margin: 0;">배포 및 런칭<br>모니터링</p>
    </div>
  </div>
</body>
```

---

## 10. 감사 슬라이드 (thank-you)

심플한 마무리.

```html
<body class="col center" style="width: 960px; height: 540px; background: linear-gradient(135deg, #2563EB 0%, #1E40AF 100%); position: relative; overflow: hidden;">
  <!-- 원형 장식 -->
  <div style="position: absolute; bottom: -100px; right: -100px; width: 300px; height: 300px; border: 50px solid rgba(255,255,255,0.1); border-radius: 50%;"></div>
  
  <!-- 메인 텍스트 -->
  <div class="col center" style="gap: 24px; z-index: 1;">
    <h1 style="color: #FFFFFF; font-size: 52px; font-weight: 700; margin: 0;">감사합니다</h1>
    <p style="color: rgba(255,255,255,0.8); font-size: 16px; margin: 0;">Thank you for your attention</p>
  </div>
  
  <!-- 연락처 -->
  <div style="position: absolute; bottom: 40px; color: rgba(255,255,255,0.6); font-size: 13px; text-align: center;">
    contact@company.com • www.company.com
  </div>
</body>
```

---

## 차트 추가 방법

HTML에서 `class="placeholder"`로 영역 지정 후, JavaScript에서 차트 삽입:

```javascript
const { slide, placeholders } = await html2pptx("chart-slide.html", pptx);

slide.addChart(pptx.charts.PIE, [
  {
    name: "진행 현황",
    labels: ["완료", "진행 중", "예정"],
    values: [70, 20, 10]
  }
], {
  ...placeholders[0],
  showPercent: true,
  chartColors: ["2563EB", "60A5FA", "DBEAFE"]
});
```
