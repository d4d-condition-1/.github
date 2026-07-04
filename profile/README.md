<div align="center">

# 🎯 D4D

### 교본이 야전을 못 따라간다. D4D가 따라잡는다.

**최신 전장 교훈을 *출처 기반 교재*로 바로 만드는 국방 교육 시스템**
*Source-Grounded Doctrine & Training Generator*

![Node](https://img.shields.io/badge/Node.js-23.4+-339933?logo=node.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-ESM-3178C6?logo=typescript&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-node%3Asqlite-003B57?logo=sqlite&logoColor=white)
![Sources](https://img.shields.io/badge/수집-뉴스·텔레그램·유튜브·웹-e11d48)
![Runtime deps](https://img.shields.io/badge/runtime%20deps-0-brightgreen)

> ### 공식 교본 최신화는 느리다. 전장은 매주 바뀐다.
> D4D는 뉴스·텔레그램에 흩어진 **최신 전장 정보를 자동 수집**하고, **출처가 추적되는 교재·훈련 초안**으로 바꿔 교관에게 바로 건넨다.
> 핵심은 *"AI가 만든 교본"*이 아니라 ***"사람이 검증할 수 있는, 근거 있는 지침 생성"*** 이다.

**📸 [ 히어로: 지침 생성(수집→교안) 화면 — 캡처 예정 ]**
<!-- 준비되면 교체: <img src="docs/hero-generate.png" alt="D4D 지침 생성" width="860"/> -->

<sub>트랙 · **Force Readiness, Training & Simulation** (전투준비·교육·시뮬레이션) — EGCED TECH</sub>

</div>

---

## ⏱️ 30초 요약

| | |
| --- | --- |
| **무엇을** | 최신 전장 정보를 수집·검증해 **교재와 훈련 문항 초안**을 만드는 교육 시스템 |
| **누구를** | 교육 콘텐츠를 최신화해야 하는 **교관·부대** + 짧은 복무의 **초급 전투원** |
| **어떻게** | 뉴스·텔레그램 **자동 수집** → 출처 기반 교재 초안 → 문항·이미지 → **전문가 검수** → 적응형 교육 |
| **왜 다른가** | "AI 교본"이 아니라 **"출처 기반으로 검증 가능한 지침 생성"** — 모든 자료에 원문 링크 |

---

## ❗ 문제 — 교본이 전장의 속도를 못 따라간다

- 🐢 전술·장비·위협은 매주 바뀌는데, **공식 교본·지침의 최신화는 느리다**
- 🧩 최신 전장 교훈은 **뉴스·텔레그램에 흩어져** 교육 자료로 정리되지 못한다
- ✍️ 교관이 **일일이 자료를 찾아 교안을 만들** 시간이 없다
- ⏳ 복무 기간은 짧아지고 병력은 줄어 — **낡은 교재로는 정예를 못 만든다**

---

## ✅ 해결 — 출처 기반, 검증 가능한 지침 생성

D4D는 최신 전장 정보를 자동으로 모아 **출처가 추적되는 교재·훈련 초안**으로 바꿔 교관에게 바로 건넨다. AI는 리서치·정리를 대신할 뿐, **최종 판단은 사람이 한다.**

```mermaid
flowchart LR
  subgraph SRC["① 자동 수집 ✅"]
    N[뉴스 · RSS]
    TG[공식 텔레그램]
    YT[유튜브]
    WEB[웹]
  end
  SRC --> A["② 아티클 아카이브 ✅<br/>원문 링크·이미지 보존<br/>중복 제거"]
  A --> V{"③ 구조화·교차검증 ◔<br/>사건·장소·피해·패턴<br/>단일기사 차단"}
  V --> M["④ 교재(교안) 초안 ✅<br/>원문 연결·출처 추적"]
  M --> Q["⑤ 문항·상황이미지 초안 ✅<br/>근거 기반·환각 차단"]
  Q --> R["⑥ 전문가 검수 ✅<br/>승인해야 배포"]
  R --> EDU["⑦ 적응형 교육 배포 ✅"]
```

<div align="center"><sub><b>✅ 현재 구현</b> · <b>◔ 설계·진행 중</b></sub></div>

---

## 🔎 왜 신뢰할 수 있나 — "AI 교본"이 아니라 "검증 가능한 초안"

| | 원칙 | 상태 |
| :---: | --- | :---: |
| 📰 | **흩어진 최신 정보를 한곳에** — 뉴스·RSS·공식 텔레그램·유튜브·웹을 자동 수집 | ✅ |
| 🔗 | **모든 자료에 원문 링크** — 근거를 클릭 한 번으로 확인(출처 추적) | ✅ |
| 📝 | **결과는 '최종 교본'이 아니라 검토용 초안** — 사람이 승인해야 배포 | ✅ |
| ⚡ | **느린 교본 업데이트를 보완** — 최신 전장 교훈을 빠르게 반영 | ✅ |
| 🧑‍✈️ | **전문가를 대체하지 않는다** — 리서치·분류·근거 정리를 자동화해 검토 시간만 줄임 | ✅ |
| 🧠 | **사건·장소·피해 유형·반복 패턴 자동 구조화** | ◔ 진행 중 |
| 🛡️ | **단일 기사 기반 지침 차단** — 교차검증된 자료만 지침 후보로 승격 | ◔ 진행 중 |

> **핵심 가치는 "AI가 만든 교본"이 아니라 "출처 기반으로 검증 가능한 지침 생성 시스템"이다.**

---

## 🎓 교육 전달 — 만든 콘텐츠를 개인 맞춤으로 체득

생성한 교재·문항은 곧바로 **적응형 훈련**으로 이어진다. 진단으로 약점을 찾고, 개인 실력에 맞춘 난이도로 최약점을 집중 반복시켜 짧은 복무 기간 안에 **숙련 도달 시간을 압축**한다.

```mermaid
flowchart LR
  D[진단<br/>7역량] --> W{최약점 식별}
  W --> L["점수 → 난이도 1~5"]
  L --> Q[적응형 출제] --> S[서버 채점] --> U["점수 갱신"]
  U --> W
  U --> R[집중훈련 추천·리포트]
```

<div align="center">
<img src="docs/report-radar.png" alt="개인 역량 리포트 — 7대 역량 레이더와 약점 우선순위" width="330"/>
<br/><sub>▲ 개인 역량 리포트 — 7대 전투역량 레이더 · 약점 우선순위 · 추천 훈련</sub>
</div>

**7대 전투역량** · `전술기동` `화력운용` `지형판독` `통신절차` `전장응급처치` `화생방` `장비운용`

---

## 🖥️ 교관 콘솔 — 부대 전체와 개인을 동시에 조망

교관은 흩어진 데이터가 아니라 **부대 전체와 개인을 한 화면에서** 본다. 이 가시성이 두 가지를 가능하게 한다 — **개인화된 교육 배정**과 **부대 전력(전투준비태세)의 실시간 파악.**

<div align="center">
<img src="docs/admin-dashboard.png" alt="부대 현황 대시보드" width="880"/>
<br/><sub>▲ 부대 현황 — 전체 인원·평균 숙련도·등급 분포(S~D)·카테고리별 부대 평균·최근 활동·누적 AI 요청</sub>
</div>

- **부대 조망** — 전체 장병 수, 평균 숙련도, 등급 분포(S~D), 카테고리별 부대 평균, 오늘 훈련 인원, 최근 활동, 누적 AI 요청
- **개인 조망** — 나 vs 부대 평균, 부대 내 순위, 최대 격차 약점(우선 보강 대상)
- **→ 이렇게 쓰인다** — 약한 역량·저숙련 인원을 식별해 **맞춤 교재·과제를 배정**(개인화 교육)하고, **부대의 전력 공백을 실시간으로 파악**한다

<div align="center">
<img src="docs/report-vs-unit.png" alt="나 vs 부대 평균 역량 분석" width="330"/>
<br/><sub>▲ 개인 분석 — 나 vs 부대 평균 · 부대 내 순위 · 최대 격차 약점</sub>
</div>

---

## 🧭 트랙 적합성 — 요구 역량이 실제로 구현되어 있다

| 트랙 요구 역량 | D4D 구현 | 상태 |
| --- | --- | :---: |
| **최신 지침·교훈의 빠른 교육화** | 뉴스·텔레그램 자동 수집 → 출처 기반 교재·문항 초안 | ✅ |
| 개인별 숙련도 진단·적응형 커리큘럼 | 7대 역량 진단 → 최약점을 개인 난이도로 집중 출제 | ✅ |
| 장비·절차 반복 시뮬레이션 | 장비운용 포함 7역량, 상황형·선택형 + 상황 이미지 생성 | ✅ |
| 약점 자동 식별·집중 훈련 추천 | 지식·체력·미완료 과제를 종합한 "지금 할 일" 추천 | ✅ |
| 부대 단위 숙련도 현황 가시화 | 교관 콘솔 — 부대 조망 + 개인 조망 → 맞춤 교육 배정·전력 파악 | ✅ |
| 출처 기반 교차검증 지침 승격 | 수집·출처 추적은 구현, 교차검증 게이팅은 설계 | ◔ |

---
---

## 🛠️ 기술 스택 & 아키텍처

### 설계 철학 — "가볍고, 닫혀도 돌아가게"

국방 환경을 염두에 두고 **런타임 의존성 0**을 원칙으로 삼았다. 외부 패키지 없이 Node 내장 모듈만 쓰므로 공급망 공격 표면이 없고, 폐쇄망에서도 빌드·배포가 단순하다. RSS·텔레그램·웹 **수집기(scraper)와 WebSocket 서버까지 직접 구현**해 전체 동작을 투명하게 통제한다.

```mermaid
flowchart LR
  subgraph Ext["외부 출처"]
    NEWS[뉴스·RSS] & TGRAM[텔레그램] & YTB[유튜브] & WEBP[웹]
  end
  subgraph Server["D4D Server · Node 23.4+ · 런타임 의존성 0"]
    SCR[수집기<br/>rss·telegram·youtube·web·api] --> FEED[피드/아티클]
    FEED --> MAT[교재·문항 생성]
    R[미니 라우터] --> AUTH[세션 인증]
    R --> TR[적응형 출제 엔진]
    R --> REC[약점 추천]
    R --> ADM[부대 관리·대시보드]
    R --> WS[WebSocket 실시간]
  end
  DB[(SQLite · WAL)]
  LLM[["Anthropic · OpenAI · Gemini<br/>텍스트 + 이미지"]]
  Ext --> SCR
  MAT --> LLM
  MAT --> DB
  TR --> DB
  ADM --> DB
```

### 스택

| 영역 | 채택 | 비고 |
| --- | --- | --- |
| 런타임 | **Node.js 23.4+** | `node:http`·`node:sqlite`·`node:crypto`·`node:net` |
| 언어 | **TypeScript (ESM)** | `tsc` 빌드, `--watch` 개발 |
| 데이터베이스 | **SQLite** (`node:sqlite`) | WAL 저널, FK 제약, 무설치 |
| **정보 수집** | **커스텀 수집기** (`src/scrapers/`) | RSS·**텔레그램**·유튜브·웹·API, 키워드·기간 필터·중복 제거 |
| AI 생성 | **Anthropic · OpenAI · Gemini** | 문항 초안(스키마 강제·PDF) + 상황 이미지(gpt-image-1·Imagen 3) |
| 실시간 | **커스텀 WebSocket** | RFC 6455 직접 구현 (`lib/ws.ts`) — 알림·채팅 |
| 라우팅 | **커스텀 미니 라우터** | `:param` 지원 (`router.ts`) |
| 인증 | 세션 토큰 → **sha256 해시 저장** | httpOnly 쿠키 + `Bearer` 병행 |
| 비밀번호 · 시크릿 | **scrypt** 해시 · **AES-256-GCM** | AI 키는 암호문으로만 저장, 위·변조 탐지 (`APP_SECRET_KEY`) |
| 문서 · 배포 | **OpenAPI/Swagger** · **Docker + GitHub Webhook** | `/api/docs` · HMAC 검증 자동배포 |

> 장병 웹앱과 관리자(교관) 콘솔은 별도 프론트엔드로 제공되며, 본 서버의 REST API와 WebSocket을 그대로 사용한다(프론트 앱 포트 `9555`). 이 저장소는 백엔드(`d4d_server`) 범위다.

### 구현 현황 (What's built)

| 기능 | 상태 |
| --- | :---: |
| 다중 출처 자동 수집(RSS·텔레그램·유튜브·웹·API), 키워드·기간 필터, 중복 제거 | ✅ |
| 아티클 아카이브 — 원문 링크·이미지·발행일 보존 | ✅ |
| 아티클 → 교재(교안) 변환, 원문 연결(출처 추적) | ✅ |
| 교재 → AI 문항 초안(근거 기반·환각 차단·멀티프로바이더·PDF) | ✅ |
| 상황 이미지 자동 생성(OpenAI·Gemini) | ✅ |
| 전문가 검수 후 저장·과제 배정, 적응형 훈련·리포트·부대 대시보드 | ✅ |
| 사건·장소·피해·패턴 자동 구조화 / 교차검증 후보 승격 | ◔ 진행 중 |

### 데이터 모델 (핵심 테이블)

```
feed_channels · feed_articles       수집 채널(뉴스·텔레그램…) · 수집 아티클(원문 링크)
materials · questions               교재(교안) · 문항 (← 아티클/자료에서 생성)
categories · user_scores            7대 역량 · 개인 역량 점수
training_sessions · answers         훈련 세션 · 답안(서버 채점)
assignments · assignment_progress   커리큘럼(과제) 배정·수행
ai_providers                        AI 연동 (키 암호화)
units · users · sessions            부대 · 계정 · 세션
chat_threads · notifications        실시간 채팅 · 알림
```

### 디렉토리 구조

```
src/
├── scrapers/       # 정보 수집기: rss · telegram · youtube · web · api (+ utils)
├── routes/         # feeds(수집) · curriculum(교재·문항) · training · recommend
│                   # admin · report · chat · fitness · programs · notifications
├── services/       # 라우트별 비즈니스 로직 계층
├── lib/            # ai(문항) · aiImage(상황이미지) · ws · crypto · score · http …
├── db/             # SQLite 연결·스키마(migrate)·시드(seed)
├── middleware/     # 세션 인증 (requireAuth / requireAdmin)
├── index.ts        # HTTP 서버 + WS 업그레이드 + CORS
└── router.ts       # 초소형 라우터 (:param)
```

---

## 📡 API (요약)

**Swagger 문서: `http://localhost:9666/api/docs`** — Authorize 에 로그인 `token` 을 넣으면 바로 테스트할 수 있다.

| Method | Path | Auth | 설명 |
| --- | --- | --- | --- |
| GET/POST | `/api/admin/feeds/channels` | 교관 | 수집 채널(뉴스·텔레그램…) 목록/등록 |
| POST | `/api/admin/feeds/channels/:id/fetch` | 교관 | **채널 수집 실행** → 아티클 아카이브(중복 제거) |
| GET | `/api/admin/feeds/articles` | 교관 | 수집된 아티클(원문 링크 포함) |
| POST | `/api/admin/feeds/articles/:id/to-material` | 교관 | **아티클 → 교재(교안) 변환** |
| POST | `/api/admin/materials/:id/generate-questions` | 교관 | 교재 → **AI 문항 초안 생성** |
| GET/POST | `/api/admin/questions` · `/api/admin/assignments` | 교관 | 문항 검수·저장 / 과제 배정 |
| POST | `/api/training/sessions` · `/:id/answers` | 장병 | 적응형 세션 시작 / 답안 제출(서버 채점) |
| GET | `/api/report` · `/api/me/scores` | 장병 | 학습 리포트 / 역량 점수 |
| GET | `/api/admin/dashboard` | 교관 | 부대 현황 대시보드 |

점수 규칙: 정답 `+points`, 오답 `−⌈points/2⌉`, 0~100 클램프. 등급 S(90+)/A(75+)/B(60+)/C(40+)/D.

---

## ▶️ 실행

```bash
cp .env.example .env   # 값 채우기
npm run dev            # 개발 (--watch)
npm start              # 운영
```

최초 기동 시 SQLite(`data/d4d.db`)에 스키마와 기본 데이터가 자동 주입되고, 관리자 계정이 생성된다. `ADMIN_PASSWORD` 를 비워두면 랜덤 비밀번호가 로그에 1회 출력된다.

---

## 🚀 배포

GitHub push → 웹훅 서버(`:9446`)가 HMAC 검증 후 `deploy/deploy.sh` 실행 → docker build → 컨테이너 교체(포트 `9666`). SQLite 데이터는 네임드 볼륨 `d4d-server-data` 에 보존된다.

```bash
bash deploy/webhook-up.sh          # 웹훅 컨테이너 기동
bash deploy/deploy.sh              # 수동 배포
docker logs -f d4d-server          # API 로그
```

포트 정리: front 앱 `9555` / front 웹훅 `9444` / **server API `9666` / server 웹훅 `9446`**

<details>
<summary><b>트러블슈팅</b></summary>

**`Error: unable to open database file` (ERR_SQLITE_ERROR, errcode 14)** — DB 디렉터리에 컨테이너 사용자(node, uid 1000)가 쓸 수 없는 경우다. 기본 구성(네임드 볼륨 `d4d-server-data`)에서는 발생하지 않는다. 직접 바인드 마운트로 바꿨다면 호스트에서 `sudo chown -R 1000:1000 <호스트경로>` 로 소유권을 맞춰야 한다. 배포 스크립트는 웹훅 컨테이너 안에서 실행되므로, 바인드 마운트가 필요하면 반드시 **호스트 기준 절대경로**를 사용할 것.

</details>

---

<div align="center">
<sub><b>D4D</b> — 느린 교본을 대신해, 최신 전장 교훈을 출처 기반 교재로. · EGCED TECH · Force Readiness, Training & Simulation</sub>
</div>
