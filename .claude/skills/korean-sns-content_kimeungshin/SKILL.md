---
name: korean-sns-content
description: |
  외국인 학습자를 위한 한국어 교육 SNS 콘텐츠 생성. 하나의 한국어 표현을 입력받아 여러 SNS 플랫폼(Instagram, TikTok, Twitter, YouTube Shorts, Facebook, Pinterest)에 최적화된 텍스트 콘텐츠와 AI 이미지 생성 프롬프트를 자동 생성한다.

  사용 시점: (1) "한국어 SNS 콘텐츠 만들어줘" (2) "Korean SNS content" (3) "한국어 표현 [표현] 콘텐츠로 만들어줘" (4) "외국인용 한국어 교육 콘텐츠" (5) "[표현]을 SNS에 올릴 콘텐츠로 변환"
---

# Korean SNS Content Generator

## 워크플로우

### 1. 정보 수집

사용자에게 확인:

**필수:**
- 한국어 표현 (예: "밥 먹었어요?")
- 영어 의미 (예: "Have you eaten?")
- 플랫폼: instagram_feed, instagram_story, tiktok, twitter, youtube_shorts, facebook, pinterest

**선택 (기본값):**
- 난이도: beginner / intermediate / advanced [기본: beginner]
- 콘텐츠 유형: daily_expression / kpop_kdrama / slang / grammar / culture / quiz [기본: daily_expression]
- 이미지 스타일: cute_korean / modern_seoul / neon_hangul / traditional / minimalist / kpop_vibrant [기본: cute_korean]

### 2. 로마자 발음 생성

국립국어원 표준 로마자 표기법 사용. 음절 구분 하이픈(-), 대괄호 표시: `[bap meo-geo-sseo-yo?]`

### 3. 플랫폼별 콘텐츠 생성

플랫폼 사이즈, 이미지 스타일, 해시태그 가이드는 [references/examples.md](references/examples.md) 참조.

#### 이미지 프롬프트 구조
```
[스타일 설명], Korean language educational content,
[표현 관련 시각적 장면],
text space for overlay "[한국어 표현]",
[색감/분위기], --ar {width}:{height}
```

#### 캡션 템플릿

**Instagram Feed (긴 형식):**
```
🇰🇷 [시리즈명] #[번호]
━━━━━━━━━━━━━━━━━━━
📝 "[한국어 표현]"
🔊 [로마자 발음]
🇬🇧 "[영어 의미]"
━━━━━━━━━━━━━━━━━━━
💡 What does it mean?
[설명]
🎭 Cultural Note:
[문화적 맥락]
📊 Level: [난이도]
━━━━━━━━━━━━━━━━━━━
💾 Save this post!
🔔 Follow for daily Korean!
━━━━━━━━━━━━━━━━━━━
[해시태그 20-30개]
```

**Twitter (280자 제한):**
```
🇰🇷 [한국어 표현]
🔊 [로마자]
= "[영어 의미]"
💡 [짧은 설명]
[해시태그 3-5개]
```

**TikTok (훅 중심):**
```
[훅 문장] 🤯🇰🇷
[한국어 표현] = [영어 의미]
[CTA]
[해시태그 5-7개]
```

### 4. 출력 형식

```json
{
  "expression": {
    "korean": "한국어 표현",
    "romanization": "[로마자 발음]",
    "english": "영어 의미",
    "level": "난이도",
    "category": "카테고리"
  },
  "cultural_note": "문화적 설명",
  "platforms": {
    "platform_name": {
      "image": {
        "size": "너비x높이",
        "prompt": "AI 이미지 생성 프롬프트",
        "text_overlay": {"main": "메인 텍스트", "sub": "서브 텍스트"}
      },
      "caption": "플랫폼용 캡션",
      "hashtags": ["해시태그 목록"]
    }
  }
}
```

## 주의사항

- **로마자 표기**: 국립국어원 표준, 외국인이 읽기 쉽게 음절 구분
- **문화적 정확성**: 일반화 피하고 정확하게
- **이미지 프롬프트**: 텍스트 오버레이 공간 확보 (실제 한글은 오버레이로 추가)
- **해시태그**: 플랫폼별 최적 개수 준수

## 확장 기능

- 시리즈 번호: 연속 콘텐츠 시 자동 넘버링
- A/B 버전: 같은 표현에 2가지 스타일 제안
- 퀴즈 변환: 같은 표현을 퀴즈 형식으로 변환
