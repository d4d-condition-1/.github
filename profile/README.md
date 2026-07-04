<div align="center">

# 🎖️ D4D

### 숙련이 정점에 닿기 전에 전역합니다.
### D4D는 그 시간을 앞당깁니다.

**단기복무 전투원을 위한 전술 숙달 가속 시뮬레이터**
*Conscript Readiness Accelerator*

![Track](https://img.shields.io/badge/Track-Force%20Readiness%2C%20Training%20%26%20Simulation-0ea5e9)
![Node](https://img.shields.io/badge/Node.js-23.4+-339933?logo=node.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-ESM-3178C6?logo=typescript&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-node%3Asqlite-003B57?logo=sqlite&logoColor=white)
![Runtime deps](https://img.shields.io/badge/runtime%20deps-0-brightgreen)

> ### 숙련도는 훈련의 횟수 × 질에서 나옵니다.
> 그런데 실제 훈련은 마음대로 늘릴 수 없고, 집체교육은 개인을 보지 못하며, 교재는 전장을 따라가지 못합니다.
> **D4D는 이 세 가지 벽을 하나의 시스템으로 넘습니다.**

<sub>트랙 · Force Readiness, Training & Simulation (전투준비·교육·시뮬레이션) · EGCED TECH</sub>

</div>

---

## ⏱️ 30초 요약

| | |
| --- | --- |
| **무엇을** | 진단 → 가상 반복 훈련 → 약점 집중 → 전력 가시화까지, 개인 맞춤 적응형 훈련 시뮬레이터 |
| **누구를 위해** | 복무 기간이 짧은 초급 전투원, 그리고 그들을 짧은 시간 안에 길러내야 하는 교관·부대 |
| **어떻게** | 시공간 제약 없는 Pre-train 시뮬레이션 + 약점 진단·적응형 출제 + 부대 전력 대시보드 |
| **뭐가 다른가** | 교육 콘텐츠까지 시스템이 만듭니다 — 최신 전장 소스에서, 출처 검증과 교관 검수를 거쳐 |

---

## ❗ 문제 · 제한된 복무 기간, 숙련을 가로막는 세 가지 벽

숙련된 전투원은 **훈련의 횟수와 질**로 만들어집니다. 그런데 의무·단기 복무 구조에서는 이 두 가지가 모두 구조적으로 막혀 있습니다.

| | 벽 | 현실 |
| :---: | --- | --- |
| 1️⃣ | **훈련량의 물리적 한계** | 숙련은 반복에서 나오지만, 실제 훈련은 탄약·훈련장·안전·비용에 묶여 무작정 늘릴 수 없습니다. |
| 2️⃣ | **일방향 집체교육** | 개인마다 편차가 커도 모두 같은 교육을 받습니다. 맞춤화도, 개인별 분석도 안 되니 부대는 **전력을 측정하지 못합니다**. |
| 3️⃣ | **전장을 못 따라가는 교재** | 전술·장비·위협은 계속 최신화되는데 공식 교본의 갱신은 느립니다. 낡은 교재로는 다음 전장에 대비할 수 없습니다. |

---

## ✅ 해결 · 세 가지 벽에 1:1로 답합니다

### 1️⃣ 실전 훈련을 늘릴 수 없다면 → 시공간 제약 없는 Pre-train

훈련장은 늘릴 수 없어도, **훈련장에 들어가기 전의 숙련도**는 끌어올릴 수 있습니다. D4D는 전술기동·장비운용·전투부상자처치 같은 절차를 AI 생성 상황 이미지와 함께 단계별로 반복 훈련시킵니다. 생활관에서든 대기 시간에든 — 실제 훈련의 밀도를 높이는 사전 숙달입니다.

<div align="center">
<img src="https://raw.githubusercontent.com/d4d-condition-1/.github/main/profile/assets/sim-procedure.png" alt="절차 시뮬레이션 · 전투부상자처치 단계별 훈련" width="860"/>
<br/><sub>▲ 절차 시뮬레이션 · 전투부상자처치(지혈대 적용)를 단계별 상황 이미지와 판단 기준으로 반복 훈련</sub>
</div>

7대 전투역량 · `전술기동` `화력운용` `지형판독` `통신절차` `전장응급처치` `화생방` `장비운용`

### 2️⃣ 집체교육이 못 보는 개인 → 병사는 약점을 알고, 간부는 전력을 봅니다

먼저 진단으로 7대 역량 중 최약점을 찾고, 각자 실력에 맞는 난이도로 그 약점만 집중 반복시킵니다. 같은 시간을 훈련해도 숙련이 올라오는 속도가 달라집니다.

<img src="https://raw.githubusercontent.com/d4d-condition-1/.github/main/profile/assets/diagram2.svg" alt="적응형 훈련 루프" width="820"/>

<div align="center">
<img src="https://raw.githubusercontent.com/d4d-condition-1/.github/main/profile/assets/report-radar.png" alt="개인 역량 리포트 · 7대 역량 레이더와 약점 우선순위" width="330"/>
<img src="https://raw.githubusercontent.com/d4d-condition-1/.github/main/profile/assets/report-vs-unit.png" alt="나 vs 부대 평균 역량 분석" width="330"/>
<br/><sub>▲ 개인 리포트 · 7대 역량 레이더 · 약점 우선순위 · 나 vs 부대 평균 · 부대 내 순위</sub>
</div>

이 데이터가 쌓이면 교관 콘솔에서 **부대 전체와 개인의 전력이 한 화면에** 보입니다. 감으로 짐작하던 단기복무 장병의 전투 준비태세가 숫자로 잡히기 시작합니다.

<div align="center">
<img src="https://raw.githubusercontent.com/d4d-condition-1/.github/main/profile/assets/admin-dashboard.png" alt="부대 현황 대시보드" width="880"/>
<br/><sub>▲ 부대 현황 · 전체 인원 · 평균 숙련도 · 등급 분포(S~D) · 카테고리별 부대 평균 · 최근 활동</sub>
</div>

- **부대 조망** · 평균 숙련도, 등급 분포(S~D), 카테고리별 부대 평균, 오늘 훈련 인원까지 한눈에.
- **개인 조망** · 부대 평균과의 격차, 부대 내 순위, 가장 벌어진 약점(우선 보강 대상)을 바로 확인.
- **그래서** · 약한 역량과 뒤처진 인원에게 맞춤 교재·과제를 배정하고, 전력 공백을 실시간으로 메웁니다.

### 3️⃣ 교본이 전장을 못 따라간다면 → 최신 전장 소스가 검증을 거쳐 교재가 됩니다

뉴스·텔레그램·유튜브에 흩어진 최신 전장 교훈을 자동 수집해 교재와 문항 초안으로 바꿉니다. 단, **바로 출제하지 않습니다.** 모든 초안에는 원문 링크가 붙어 신뢰성을 눈으로 확인할 수 있고, 유사 소스가 반복 누적되는지 검토해 실효성을 거르며, 교관이 승인해야만 배포됩니다.

<img src="https://raw.githubusercontent.com/d4d-condition-1/.github/main/profile/assets/diagram1.svg" alt="지침 생성 흐름 · 수집→검증→검수→배포" width="820"/>

<div align="center"><sub><b>✅ 현재 구현</b> · <b>◔ 설계·진행 중</b></sub></div>

부대의 목적에 맞는 문제도 AI로 생성해 교관이 직접 검수·출제합니다. **우리 부대에 필요한 교육을, 우리가 만듭니다.**

<div align="center">
<img src="https://raw.githubusercontent.com/d4d-condition-1/.github/main/profile/assets/console-authoring.png" alt="교관 출제 콘솔 · 문항 검수와 직접 출제" width="880"/>
<br/><sub>▲ 교관 출제 콘솔 · 역량·난이도·배점·출처(교범 인용)를 지정해 문항을 검수하고 출제</sub>
</div>

> 저희가 만드는 건 "AI가 대충 써준 교본"이 아닙니다. **출처로 검증하고 사람이 승인하는** 교육 콘텐츠입니다.

---

## 🧭 트랙 적합성 · 요구 역량 5개에 구현으로 답합니다

| 트랙 요구 역량 | D4D 구현 | 상태 |
| --- | --- | :---: |
| 개인별 숙련도 진단·적응형 커리큘럼 | 7대 역량 진단 → 최약점을 개인 난이도(1~5)로 집중 출제 | ✅ |
| 장비·절차 반복 시뮬레이션 | 상황형·선택형 문항 + AI 상황 이미지로 절차를 단계별 반복 | ✅ |
| 약점 자동 식별·집중 훈련 추천 | 지식·체력·미완료 과제를 종합한 "지금 할 일" 추천 | ✅ |
| 숙련 도달 시간 단축 지표 | 역량 점수·등급(S~D) 변화와 훈련 세션 이력으로 성장 추적 | ✅ |
| 부대 단위 숙련도 현황 가시화 | 교관 콘솔 — 부대 조망·개인 조망·맞춤 과제 배정 | ✅ |

> **그리고 하나 더** — 훈련 콘텐츠 자체가 최신 전장에서 옵니다. 출처 추적 수집·검수 파이프라인은 구현 완료(✅), 교차검증 자동 승격은 진행 중(◔)입니다.

---

## 🛠️ 기술 · 가볍고, 닫혀도 돌아갑니다

### 설계 철학 · 런타임 의존성 0

국방 환경을 전제로 런타임 의존성을 아예 **0**으로 뒀습니다. 외부 패키지 없이 Node 내장 모듈만 쓰기 때문에 공급망 공격이 파고들 틈이 없고, 폐쇄망에서도 빌드·배포가 간단합니다. RSS·텔레그램·웹 수집기와 WebSocket 서버까지 직접 구현해, 무엇이 어떻게 도는지 전부 저희가 통제합니다.

<img src="https://raw.githubusercontent.com/d4d-condition-1/.github/main/profile/assets/diagram3.svg" alt="아키텍처" width="820"/>

### 스택

| 영역 | 채택 | 비고 |
| --- | --- | --- |
| 런타임 | **Node.js 23.4+** | `node:http` · `node:sqlite` · `node:crypto` · `node:net` |
| 언어 | **TypeScript (ESM)** | `tsc` 빌드, `--watch` 개발 |
| 데이터베이스 | **SQLite** (`node:sqlite`) | WAL 저널, FK 제약, 무설치 |
| 정보 수집 | **커스텀 수집기** (`src/scrapers/`) | RSS·텔레그램·유튜브·웹·API, 키워드·기간 필터, 중복 제거 |
| AI 생성 | **Anthropic · OpenAI · Gemini** | 문항 초안(스키마 강제·PDF) + 상황 이미지(gpt-image-1·Imagen 3) |
| 실시간 | **커스텀 WebSocket** | RFC 6455 직접 구현 (`lib/ws.ts`), 알림·채팅 |
| 라우팅 | **커스텀 미니 라우터** | `:param` 지원 (`router.ts`) |
| 인증 | 세션 토큰 → **sha256 해시 저장** | httpOnly 쿠키 + `Bearer` 병행 |
| 비밀번호·시크릿 | **scrypt** 해시 · **AES-256-GCM** | AI 키는 암호문으로만 저장, 위·변조 탐지 (`APP_SECRET_KEY`) |
| 문서·배포 | **OpenAPI/Swagger** · **Docker + GitHub Webhook** | `/api/docs`, HMAC 검증 자동배포 |

> 장병 웹앱과 교관 콘솔은 별도 프론트엔드(포트 `9555`)로 제공되며, 이 서버의 REST API와 WebSocket을 그대로 씁니다. 이 저장소는 백엔드(`d4d_server`) 범위입니다.

### 구현 현황

| 기능 | 상태 |
| --- | :---: |
| 다중 출처 자동 수집(RSS·텔레그램·유튜브·웹·API) · 키워드·기간 필터 · 중복 제거 | ✅ |
| 아티클 아카이브 · 원문 링크·이미지·발행일 보존 | ✅ |
| 아티클 → 교재(교안) 변환 · 원문 연결(출처 추적) | ✅ |
| 교재 → AI 문항 초안 · 근거 기반·환각 차단·멀티프로바이더·PDF | ✅ |
| 상황 이미지 자동 생성(OpenAI·Gemini) | ✅ |
| 전문가 검수 후 저장·과제 배정 · 적응형 훈련·리포트·부대 대시보드 | ✅ |
| 사건·장소·피해·패턴 자동 구조화 · 교차검증 후보 승격 | ◔ 진행 중 |

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

## 📡 API 요약

Swagger 문서는 `http://localhost:9666/api/docs` 에서 확인할 수 있습니다. Authorize에 로그인 `token`을 넣으면 브라우저에서 바로 테스트됩니다.

| Method | Path | Auth | 설명 |
| --- | --- | --- | --- |
| GET/POST | `/api/admin/feeds/channels` | 교관 | 수집 채널(뉴스·텔레그램…) 목록/등록 |
| POST | `/api/admin/feeds/channels/:id/fetch` | 교관 | 채널 수집 실행 → 아티클 아카이브(중복 제거) |
| GET | `/api/admin/feeds/articles` | 교관 | 수집된 아티클(원문 링크 포함) |
| POST | `/api/admin/feeds/articles/:id/to-material` | 교관 | 아티클 → 교재(교안) 변환 |
| POST | `/api/admin/materials/:id/generate-questions` | 교관 | 교재 → AI 문항 초안 생성 |
| GET/POST | `/api/admin/questions` · `/api/admin/assignments` | 교관 | 문항 검수·저장 / 과제 배정 |
| POST | `/api/training/sessions` · `/:id/answers` | 장병 | 적응형 세션 시작 / 답안 제출(서버 채점) |
| GET | `/api/report` · `/api/me/scores` | 장병 | 학습 리포트 / 역량 점수 |
| GET | `/api/admin/dashboard` | 교관 | 부대 현황 대시보드 |

점수 규칙 · 정답 `+points`, 오답 `−⌈points/2⌉`, 0~100 클램프 · 등급 S(90+) / A(75+) / B(60+) / C(40+) / D

---

## ▶️ 실행

```bash
cp .env.example .env   # 값 채우기
npm run dev            # 개발 (--watch)
npm start              # 운영
```

처음 켜면 SQLite(`data/d4d.db`)에 스키마와 기본 데이터가 자동으로 들어가고, 관리자 계정이 생성됩니다. `ADMIN_PASSWORD`를 비워두면 랜덤 비밀번호가 로그에 한 번 출력됩니다.

---

## 🚀 배포

GitHub push → 웹훅 서버(`:9446`)가 HMAC 검증 후 `deploy/deploy.sh` 실행 → docker build → 컨테이너 교체(포트 `9666`). SQLite 데이터는 네임드 볼륨 `d4d-server-data`에 보존됩니다.

```bash
bash deploy/webhook-up.sh          # 웹훅 컨테이너 기동
bash deploy/deploy.sh              # 수동 배포
docker logs -f d4d-server          # API 로그
```

포트 정리 · front 앱 `9555` / front 웹훅 `9444` / **server API `9666` / server 웹훅 `9446`**

<details>
<summary><b>트러블슈팅</b></summary>

`Error: unable to open database file` (ERR_SQLITE_ERROR, errcode 14) — DB 디렉터리에 컨테이너 사용자(node, uid 1000)가 쓸 수 없을 때 납니다. 기본 구성(네임드 볼륨 `d4d-server-data`)에서는 발생하지 않습니다. 직접 바인드 마운트로 바꿨다면 호스트에서 `sudo chown -R 1000:1000 <호스트경로>` 로 소유권을 맞춰 주세요. 배포 스크립트는 웹훅 컨테이너 안에서 도니까, 바인드 마운트가 필요하면 반드시 호스트 기준 절대경로를 쓰세요.

</details>

---

<div align="center">
<sub><b>D4D</b> · 제한된 복무 기간 안에, 검증된 최신 콘텐츠로 숙련을 가속합니다 · EGCED TECH · Force Readiness, Training & Simulation</sub>
</div>
