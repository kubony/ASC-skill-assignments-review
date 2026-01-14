# ASC-skill-assignments-review

ASC 5기 Agent Track 3조 과제를 모아서 테스트하는 레포지토리입니다.

## 📋 목차

- [프로젝트 개요](#프로젝트-개요)
- [공유 스킬](#공유-스킬)
- [참여자별 과제](#참여자별-과제)
  - [손한승](#손한승)
  - [김은신](#김은신)
  - [김유나](#김유나)
  - [안경희](#안경희)
- [설치 및 사용](#설치-및-사용)

## 프로젝트 개요

이 레포지토리는 ASC (Anthropic Study Club) 5기 Agent Track 3조의 Claude Code 스킬 및 에이전트 과제를 모아 관리하고 테스트하기 위한 공간입니다.

**구성:**
- **공유 스킬**: 유용한 스킬을 공유하기 위한 목적
- **참여자별 과제**: 각 참여자의 과제를 사용 가능한 형식으로 정리

---

## 공유 스킬

### ppt-generator
한국어에 최적화된 미니멀 프레젠테이션 생성 스킬

**주요 기능:**
- python-pptx 기반 PPTX 파일 직접 생성
- 3가지 컬러 팔레트 (Sage / Mono / Navy)
- 7가지 레이아웃 패턴 (Cover, Section, Stats Grid, Two Column, Three Column, Image+Text, Closing)
- Pretendard + Noto Serif KR 폰트 사용

**기술 스택:**
- Python, python-pptx, Pillow

**사용법:**
```bash
/ppt-generator
```

**위치:** `.claude/skills/ppt-generator/`

---

### slash-command-creator
Claude Code 슬래시 커맨드 생성 가이드 스킬

**주요 기능:**
- 슬래시 커맨드 작성 가이드 제공
- Frontmatter 옵션 설명
- 예시 및 베스트 프랙티스 제공

**위치:** `.claude/skills/slash-command-creator/`

---

### subagent-creator
Claude Code 서브 에이전트 생성 가이드 스킬

**주요 기능:**
- 커스텀 에이전트 생성 가이드
- 시스템 프롬프트 및 도구 설정 방법 제공
- 사용 가능한 도구 목록 및 예시

**위치:** `.claude/skills/subagent-creator/`

---

## 참여자별 과제

### 손한승

#### youtube-script-kr
한국 유튜브 사고 해설형 인문 커뮤니케이션 콘텐츠 제작 자동화 스킬

**과제 내용:**
내향적 성향의 시청자를 위한 사고 해설형 유튜브 콘텐츠 대본을 자동으로 생성하는 스킬입니다. 주제 발굴부터 대본 작성, 비롤 아이디어, DOCX 패키징까지 전체 워크플로우를 자동화합니다.

**주요 기능:**
- 날카로운 주제 자동 발굴 (4가지 방법론: 모순 찾기, 반복되는 고통 지점, 작은 불편함, 설명되지 않는 관찰)
- 6단계 소제목 구조 대본 작성 (개인 경험 → 통념 → 오해 차단 → 구조 해체 → 판단 기준 → 불편한 진실)
- 웹 리서치 및 권위 학자 인용
- 비롤 아이디어 및 스토리텔링 설명 생성
- DOCX 패키지 자동 생성

**타겟:**
- 20대 후반 ~ 40대 초반 내향적 성향 직장인/프리랜서
- 사고 해설형 콘텐츠 제작자

**사용법:**
```bash
/youtube-script-kr
```

**위치:** `.claude/skills/youtube-script-kr_sonhanseung/`

---

### 김은신

#### korean-sns-content
외국인 학습자를 위한 한국어 교육 SNS 콘텐츠 생성 스킬

**과제 내용:**
하나의 한국어 표현을 입력받아 여러 SNS 플랫폼에 최적화된 교육 콘텐츠와 AI 이미지 생성 프롬프트를 자동 생성하는 스킬입니다.

**주요 기능:**
- 하나의 한국어 표현 → 여러 SNS 플랫폼 콘텐츠 자동 변환
- 국립국어원 표준 로마자 표기법 적용
- 플랫폼별 최적화 (Instagram, TikTok, Twitter, YouTube Shorts, Facebook, Pinterest)
- AI 이미지 생성 프롬프트 자동 생성
- 문화적 맥락 설명 포함

**타겟:**
- 한국어 학습 콘텐츠 제작자
- 외국인 대상 한국어 교육자

**사용법:**
```bash
/korean-sns-content
```

**위치:** `.claude/skills/korean-sns-content_kimeungshin/`

---

### 김유나

#### ai-trend-monitor (Skill)
디자인/개발/마케팅 실무자를 위한 AI 도구 일일 모니터링 스킬

**과제 내용:**
실무자가 바로 사용할 수 있는 AI 도구와 서비스를 매일 모니터링하고, 실전 활용 가이드와 함께 정리하는 스킬입니다. 하드웨어, 연구, 자율주행 등은 제외하고 순수하게 실무에 활용 가능한 도구에 집중합니다.

**주요 기능:**
- 실용적 AI 도구/서비스 일일 검색 및 분류
- 디자인/개발/마케팅 도구별 카테고리 정리
- 실무 활용 시나리오 및 난이도 분석
- "오늘 바로 시도해볼 것" 추천 리스트 생성
- 실무자 관점의 ROI 평가

**타겟:**
- 디자이너, 개발자, 마케터
- AI 도구를 업무에 활용하려는 실무자

**사용법:**
```bash
/ai-trend-monitor
```

**위치:** `.claude/skills/ai-trend-monitor_kimyuna/`

---

#### ai-trend-pptx (Agent)
AI 트렌드 모니터링 후 PPTX 프레젠테이션 생성 에이전트

**과제 내용:**
ai-trend-monitor 스킬의 실행 결과를 받아 전문적인 PPTX 프레젠테이션으로 자동 변환하는 에이전트입니다.

**주요 기능:**
- ai-trend-monitor 스킬 실행 → 결과 분석
- 카테고리별 슬라이드 자동 구성
- 실행 가능한 액션 아이템 제시
- 모던한 디자인 팔레트 적용

**워크플로우:**
1. AI 트렌드 모니터링 실행
2. 결과를 마크다운 파일로 저장
3. PPTX 프레젠테이션 생성 (pptx 스킬 활용)

**위치:** `.claude/agents/ai-trend-pptx.md`

---

### 안경희

#### slide-structure-designer (Agent)
강의/세일즈/컨설팅 목적의 PPT 슬라이드 구조 설계 에이전트

**과제 내용:**
발표 주제와 목적에 맞춰 전문적인 슬라이드 구조를 자동으로 설계하는 에이전트입니다. AskUserQuestion 도구를 활용하여 필요한 정보를 수집하고, 메시지 중심의 발표 흐름을 설계합니다.

**주요 기능:**
- 발표 목적에 맞는 슬라이드 구조 자동 설계
- 문제 인식 (30%) → 구조 제안 (40%) → 전환 유도 (30%) 흐름
- AskUserQuestion 도구를 활용한 정보 수집
- 메시지 중심 제목 작성 (설명이 아닌 단정형 문장)

**입력 정보:**
- 주제, 대상, 목표, 슬라이드 수

**사용 모델:**
- Claude Opus

**위치:** `.claude/agents/slide-structure-designer.md`

---

## 설치 및 사용

### 전제 조건

- [Claude Code CLI](https://github.com/anthropics/claude-code) 설치 필요
- Python 3.8+ (ppt-generator 스킬 사용 시)

### 스킬 사용 방법

각 스킬은 Claude Code에서 다음과 같이 호출할 수 있습니다:

```bash
# 공유 스킬
/ppt-generator

# 참여자별 과제 스킬
/youtube-script-kr          # 손한승
/korean-sns-content         # 김은신
/ai-trend-monitor           # 김유나
```

### 에이전트 사용 방법

에이전트는 Task 도구를 통해 호출할 수 있습니다:

```python
# 김유나 - AI 트렌드 PPTX 생성
Task(
    subagent_type="ai-trend-pptx",
    prompt="오늘의 AI 트렌드를 모니터링하고 PPTX로 만들어주세요."
)

# 안경희 - 슬라이드 구조 설계
Task(
    subagent_type="slide-structure-designer",
    prompt="강의용 PPT 12장 구조를 설계해주세요."
)
```

---

**ASC 5기 Agent Track 3조**

---

## 라이선스

이 프로젝트는 ASC 5기 학습 목적으로 제작되었습니다.
