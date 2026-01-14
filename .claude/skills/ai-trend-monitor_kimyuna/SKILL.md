---
name: ai-trend-monitor
description: Monitor daily AI tools and services for design, development, and marketing practitioners. Use when user wants practical AI tools they can use immediately in their work. Focuses on actionable tools, excludes hardware/chips/autonomous vehicles/pure research. Designed for daily monitoring with hands-on, practitioner-focused formatting.
---

# AI Trend Monitor

## Overview

This skill provides daily monitoring of practical AI tools and services for design, development, and marketing professionals. It searches for immediately usable tools, excludes hardware/research/autonomous vehicles, and formats results for hands-on practitioners who want to know "what can I use today?"

**Language requirement: All output must be written in Korean.** Search queries can be in English for broader coverage, but all summaries, titles, and analysis must be in Korean.

## Target Audience

- **Designers**: Using AI for image generation, UI/UX, design automation
- **Developers**: Using AI coding assistants, APIs, frameworks
- **Marketers**: Using AI for content creation, SEO, analytics

## Workflow

### Step 1: Define Monitoring Scope

**Daily default parameters:**
- Time range: Last 24 hours (or specified range)
- Focus: Tools and services practitioners can use immediately
- Exclusions: Hardware, chips, autonomous vehicles, pure academic research

**Scope filters:**
- ✅ Include: Design tools, coding assistants, marketing tools, productivity apps, platform updates
- ❌ Exclude: Chips/hardware, autonomous vehicles, robotics (unless software tool release), pure research papers, funding news (unless affects tool availability)

### Step 2: Targeted Search Strategy

Execute 5-8 focused searches for practical tools:

**AI Tools & Services:**
- "new AI tool" OR "AI design tool"
- "AI coding assistant" OR "AI developer tool"
- "AI marketing tool" OR "AI content creation"

**Product Updates:**
- "ChatGPT update" OR "Claude update" OR "Gemini update"
- "Midjourney update" OR "Stable Diffusion"
- "GitHub Copilot" OR "Cursor IDE"

**Practical Applications:**
- "AI workflow" OR "AI productivity"
- "AI automation tutorial"
- "site:producthunt.com AI"

### Step 3: Filter for Practitioner Relevance

For each result, ask:
- **Can I use this today?** (Available now, not "coming soon")
- **Is this a tool/service?** (Not hardware, not pure research)
- **Will this help my daily work?** (Practical application for design/dev/marketing)

**Exclusion criteria:**
- NVIDIA/AMD chip announcements (unless about software tools)
- Self-driving car developments (unless about accessible software)
- Robotics hardware (unless about software/API release)
- Academic papers without released tools
- Funding/acquisition news (unless affects tool availability)

### Step 4: Categorize by Practitioner Role

Organize findings into:

1. **디자인 도구** (Design Tools)
   - Image/video generation tools
   - UI/UX design automation
   - Design workflow integrations

2. **개발 도구** (Development Tools)
   - Coding assistants and IDEs
   - APIs and frameworks
   - Developer productivity tools

3. **마케팅 도구** (Marketing Tools)
   - Content generation
   - SEO and analytics
   - Social media automation

4. **프로덕티비티** (Productivity)
   - Workflow automation
   - Collaboration tools
   - General productivity enhancements

5. **주요 플랫폼 업데이트** (Major Platform Updates)
   - ChatGPT, Claude, Gemini, Copilot updates
   - Major feature releases

6. **실전 팁 & 가이드** (Practical Tips & Guides)
   - Tutorials and how-tos
   - Workflow optimization
   - Best practices

7. **커뮤니티 발견** (Community Discoveries)
   - Interesting discussions
   - Tool recommendations from practitioners

### Step 5: Deep Analysis for Actionability

For each tool/service, extract:
- **What it does**: Core functionality in 2-3 sentences
- **Key features**: Bullet points of main capabilities
- **Practical use**: How a practitioner would actually use this
- **Difficulty level**: Easy / Medium / Hard
- **Access**: Free / Freemium / Paid, availability
- **Integration**: What existing tools it works with

Use `web_fetch` for:
- Reading full product announcements
- Checking pricing and availability
- Understanding real-world applications
- Gathering specific feature details

### Step 6: Format Practitioner Briefing

Structure for quick scanning and immediate action:

## Output Format

```markdown
# AI 트렌드 모니터 - [날짜]

## 📊 일일 요약
- 총 항목 수: [number]
- 오늘의 하이라이트: [가장 주목할 만한 도구/업데이트]
- 바로 시도해볼 것: [추천 도구 1-3개]

---

## 🎨 디자인 도구

### [도구명]
**출처:** [링크] | **플랫폼:** [웹사이트/제품헌트/etc] | **시간:** [발표 시각]

**무엇을 하는가:**
[2-3문장으로 핵심 기능 설명]

**주요 기능:**
- [기능 1]
- [기능 2]
- [가격/접근성]

**실무 활용:**
[디자이너가 실제로 어떻게 쓸 수 있는지 구체적 시나리오]

**사용 난이도:** [쉬움/보통/어려움]

**통합:** [Figma, Photoshop, 등 기존 도구와의 호환성]

**내 메모:**
- [실제로 써볼 가치가 있는지]
- [기존 도구 대비 장단점]
- [시도해볼 아이디어]

---

## 💻 개발 도구

[같은 형식 반복]

---

## 📢 마케팅 도구

[같은 형식 반복]

---

## ⚡ 프로덕티비티

[같은 형식 반복]

---

## 🔄 주요 플랫폼 업데이트

[같은 형식 반복]

---

## 💡 실전 팁 & 가이드

[같은 형식 반복]

---

## 🗣️ 커뮤니티 발견

[같은 형식 반복]

---

## 🚀 오늘 바로 시도해볼 것

**추천 순위:**
1. **[도구명]** - [이유] - [예상 소요시간]
2. **[도구명]** - [이유] - [예상 소요시간]
3. **[도구명]** - [이유] - [예상 소요시간]

**이번 주 실험 과제:**
- [ ] [구체적 실험 1]
- [ ] [구체적 실험 2]
- [ ] [구체적 실험 3]

---

## 📝 실무자 메모

- **오늘의 게임체인저:** [가장 임팩트 있을 것 같은 도구]
- **워크플로우 개선 아이디어:** [이 도구들로 어떻게 작업 방식을 개선할지]
- **배워야 할 것:** [이 도구를 잘 쓰기 위해 필요한 스킬]
- **다음 주 집중 영역:** [지속적으로 모니터링할 영역]
```

## Monitoring Guidelines

### Practicality First
- Focus on tools available for immediate use
- Prioritize "can I try this today?" over "interesting research"
- Value concrete applications over theoretical capabilities

### Actionability Check
- Every item should answer "how can I use this?"
- Include access information (free trial, pricing, waitlist)
- Note technical requirements (API key, platform, etc.)

### Real-World Context
- How does this fit into existing workflows?
- What tools does it replace or complement?
- What's the learning curve?

### ROI Mindset
- Time investment vs. productivity gain
- Cost vs. value for practitioners
- Adoption risk (is it stable? will it stick around?)

## Quality Standards

Before finalizing:
- [ ] All items are practitioner-actionable (not research/hardware)
- [ ] Each tool has clear "how to use" guidance
- [ ] Difficulty levels assigned appropriately
- [ ] Access/pricing information included
- [ ] Korean language used throughout (except for tool names)
- [ ] "Try today" section has specific, doable suggestions
- [ ] No autonomous vehicles, chips, or pure research papers
- [ ] Integration with existing tools noted where relevant

## Daily Routine Tips

**Best practices:**
- Run monitor daily at consistent time
- Spend 10-15 minutes reviewing
- Actually try 1-3 tools per week
- Keep notes on what worked/didn't work
- Share useful finds with team

**Follow-up workflow:**
1. Bookmark interesting tools
2. Sign up for free trials
3. Test in small project first
4. Document learnings
5. Share with colleagues if valuable

## Example Queries

**Good practitioner-focused queries:**
- "new AI design tool Figma plugin"
- "ChatGPT API update developer"
- "AI content writer tool free"
- "Midjourney alternative 2024"

**Avoid these queries:**
- "AI research paper" (too academic)
- "AI chip announcement" (hardware)
- "autonomous vehicle AI" (out of scope)
- "AI startup funding" (not actionable)
