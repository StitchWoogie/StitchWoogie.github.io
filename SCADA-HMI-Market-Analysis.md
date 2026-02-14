# SCADA/HMI 시장 분석 보고서

> 10년차 SCADA/HMI 개발자 관점에서 작성한 시장 분석
> 작성일: 2026-02-14

---

## 목차

1. [시장 개요](#1-시장-개요)
2. [가장 수익성 높은 비즈니스 모델 Top 5](#2-가장-수익성-높은-비즈니스-모델-top-5)
3. [최종사용자(End-User)가 필요로 하는 핵심 기능](#3-최종사용자end-user가-필요로-하는-핵심-기능)
4. [개발자(Developer)가 필요로 하는 핵심 기능](#4-개발자developer가-필요로-하는-핵심-기능)
5. [구매를 결정짓는 서비스 유형](#5-구매를-결정짓는-서비스-유형)
6. [주요 플랫폼 비교: Ignition vs Wonderware vs WinCC](#6-주요-플랫폼-비교-ignition-vs-wonderware-vs-wincc)
7. [한국 시장 특수성 및 기회](#7-한국-시장-특수성-및-기회)
8. [현직 개발자로서의 전략적 제언](#8-현직-개발자로서의-전략적-제언)
9. [FAQ — 자주 묻는 질문](#9-faq--자주-묻는-질문)

---

## 1. 시장 개요

### 글로벌 SCADA 시장 규모

| 구분 | 2025년 | 전망 | CAGR |
|------|--------|------|------|
| Fortune Business Insights | $44.59B | $78.25B (2032) | 8.4% |
| MarketsandMarkets | $12.89B | $20.05B (2030) | 9.2% |
| Precedence Research | $11.76B | $31.45B (2034) | 11.53% |
| Business Research Insights | $13.95B | $31.19B (2035) | 6.3% |

> 리서치 기관마다 SCADA 범위 정의가 달라 수치 차이가 있으나, **모든 기관이 연 6~12% 성장**을 예측한다는 점이 핵심이다.

### 세그먼트별 매출 비중 (2024 기준)

```
Hardware  ████████████████████████  43.5%  ← 현재 매출 최대
Software  ███████████████          31.6%  ← 성장률 최고 (클라우드 전환)
Services  ████████████             24.9%  ← 가장 빠른 성장 예측
```

### 산업별 매출 비중 (2024 기준)

```
전력/에너지      ██████████████████████  39.3%
수처리/폐수      █████████████          24.1%
Oil & Gas       ████████████           22.9%
제조업           ██████████             18.6%
```

### HMI 세그먼트

HMI는 SCADA 컴포넌트 중 **가장 빠르게 성장하는 세그먼트**다. 실시간 모니터링과 직관적인 시각화에 대한 수요가 제조, 에너지, 유틸리티 전 분야에서 급증하고 있다.

---

## 2. 가장 수익성 높은 비즈니스 모델 Top 5

### 모델 1: 클라우드/하이브리드 SaaS SCADA 플랫폼

**수익성 등급: ★★★★★ (최고)**

| 항목 | 내용 |
|------|------|
| 매출 구조 | 월/연간 구독 (OpEx) |
| 성장률 | 연 12.8% (클라우드 배포 기준) |
| 핵심 가치 | 초기 투자 최소화, 예측 가능한 비용, 자동 업데이트, 탄력적 확장 |
| 시장 침투 | 신규 구축의 40%가 하이브리드 클라우드 또는 순수 SaaS 선택 |

**왜 수익성이 높은가:**
- **반복 매출(Recurring Revenue)**: 한 번 판매하면 해지할 때까지 매월/매년 매출 발생
- **높은 Lock-in**: 데이터가 축적될수록 이탈 비용 증가
- **유지보수 비용의 구독화**: 과거 별도 계약이던 유지보수가 구독에 포함
- **확장성**: 사용량 증가 시 자동으로 매출 증가

**실전 사례:** AWS + Rockwell Automation 파트너십 — 클라우드 게이트웨이 + 분석 파이프라인 통합으로 OpEx 선호 기업 공략

---

### 모델 2: 통합 플랫폼 (HMI + SCADA + MES + Historian)

**수익성 등급: ★★★★★ (최고)**

| 항목 | 내용 |
|------|------|
| 매출 구조 | 플랫폼 라이선스 + 모듈별 추가 과금 |
| 대표 사례 | Inductive Automation Ignition, AVEVA System Platform |
| 핵심 가치 | 단일 플랫폼에서 HMI/SCADA/MES/Historian 통합 운영 |

**왜 수익성이 높은가:**
- **모듈 확장 매출**: 기본 SCADA에서 MES, Historian, Alarm, Report 모듈 추가 구매 유도
- **TCO 절감 마케팅**: "별도 시스템 3개 대신 하나로" → 의사결정 단순화
- **생태계 종속**: 한 번 플랫폼을 선택하면 모듈 추가는 같은 벤더에서
- **Ignition 모델의 파괴력**: $7,500/서버 시작, 무제한 태그/클라이언트/개발자

---

### 모델 3: 사이버보안 관리 서비스 (Managed Cybersecurity)

**수익성 등급: ★★★★☆**

| 항목 | 내용 |
|------|------|
| 매출 구조 | 월간 구독 패키지 (소프트웨어 업데이트 + 취약점 스캔 + 컴플라이언스 보고) |
| 성장 동력 | IEC 62443, NERC CIP 등 규제 의무화 |
| 대표 사례 | Schneider Electric SCADAPack 470i/474i — RBAC + Active Directory 통합 |

**왜 수익성이 높은가:**
- **규제 강제**: 고객이 "선택"이 아닌 "의무"로 구매
- **전문 인력 부족**: 중견 유틸리티는 자체 OT 보안팀이 없어 외주 의존
- **높은 갱신률**: 보안 서비스를 중단하는 것 자체가 리스크

---

### 모델 4: 시스템 통합(SI) + 컨설팅

**수익성 등급: ★★★★☆**

| 항목 | 내용 |
|------|------|
| 매출 구조 | 프로젝트 기반 (설계 → 개발 → 시운전 → 유지보수) |
| 서비스 매출 비중 | 전체 시장의 24.9% (2024), 가장 빠른 성장률 |
| 평균 프로젝트 규모 | 중소: $50K~$500K / 대형: $1M~$10M+ |

**수익 구조 상세:**
```
┌──────────────────────────────────────────┐
│  프로젝트 단계별 매출 비중               │
├──────────────────────────────────────────┤
│  컨설팅/설계       15~20%               │
│  하드웨어 조달     20~30%               │
│  소프트웨어 개발   25~35%  ← 마진 최고  │
│  시운전/교육       10~15%               │
│  유지보수 계약     10~15%  ← 반복 매출  │
└──────────────────────────────────────────┘
```

---

### 모델 5: OEM 임베디드 HMI 라이선스

**수익성 등급: ★★★☆☆ (안정적)**

| 항목 | 내용 |
|------|------|
| 매출 구조 | OEM 장비 1대당 라이선스 과금 (런타임 라이선스) |
| 대표 사례 | AVEVA Edge (구 InduSoft), COPA-DATA zenon |
| 핵심 가치 | 장비 제조사가 자사 기계에 HMI를 내장하여 출하 |

**왜 안정적인가:**
- **볼륨 기반**: 장비 판매량에 비례하여 라이선스 매출 자동 증가
- **저접점 매출**: 한 번 통합하면 추가 영업 없이 반복 발생
- **장비 수명 = 매출 수명**: 산업 장비 교체 주기 10~20년

---

## 3. 최종사용자(End-User)가 필요로 하는 핵심 기능

10년간 현장에서 고객의 요구를 직접 듣고 구현해 온 경험에 기반한 기능 우선순위:

### Tier 1: 반드시 있어야 하는 기능 (Deal-Breaker)

| 기능 | 상세 | 현장 경험 코멘트 |
|------|------|------------------|
| **실시간 모니터링 & 제어** | 1,000~100,000+ 태그 실시간 수집/표시/제어 | 태그 처리 10,000+/sec 이상 안 되면 대형 현장 입찰 탈락 |
| **알람 관리** | 필터링, 셸빙, 이력관리, SMS/이메일 알림, 연락처 로스터 | 알람 폭주(alarm flooding) 방지 기능이 없으면 운전원이 무시함 |
| **트렌드/히스토리안** | 장기 데이터 저장, 압축, 빠른 조회(<5ms) | TimescaleDB 기반 Hypertable로 97% 저장소 절감 가능 |
| **안정성 (24/7/365)** | 무정지 운전, 이중화, 자동 복구 | "서버 죽으면 공장이 멈춘다" — 이건 협상 불가 |
| **PLC/RTU 연결성** | OPC UA, Modbus, EtherNet/IP, DNP3 등 산업 프로토콜 지원 | MELSEC, AB, Siemens 드라이버 없으면 한국 시장 진입 불가 |

### Tier 2: 경쟁 우위를 만드는 기능 (Differentiator)

| 기능 | 상세 | 비즈니스 임팩트 |
|------|------|----------------|
| **웹/모바일 접근** | HTML5 기반, 브라우저만으로 어디서든 모니터링 | 관리자/경영진 접근성 ↑, 코로나 이후 필수 기능화 |
| **다국어 지원** | 런타임 언어 전환 (ko/en/zh/ja/vi) | 글로벌 수출 장비에 필수, 재시작 없는 전환 중요 |
| **레포트 & 대시보드** | 일/월/년 자동 보고서, KPI 대시보드 | 경영진이 "데이터 보여달라"고 할 때 바로 대응 |
| **예측 정비(Predictive Maintenance)** | AI/ML 기반 설비 고장 예측 | 비계획 정지 30~50% 감소, ROI 명확 |
| **사이버보안** | RBAC, 감사 로그, 암호화, AD 연동 | IEC 62443 인증 요구 증가 추세 |

### Tier 3: 미래 투자 (Future-Proof)

| 기능 | 상세 |
|------|------|
| **UNS (Unified Namespace)** | MQTT/Sparkplug B 기반 데이터 통합 아키텍처 |
| **디지털 트윈** | 물리적 설비의 가상 복제로 시뮬레이션 |
| **에지 컴퓨팅** | 현장 데이터 전처리, 클라우드 의존도 감소 |
| **AI/ML 네이티브** | 온프레미스 ML 모델 실행 (클라우드 없이) |

---

## 4. 개발자(Developer)가 필요로 하는 핵심 기능

### 개발 생산성 직결 기능

| 기능 | 중요도 | 상세 |
|------|--------|------|
| **현대적 스크립팅 언어** | ★★★★★ | Python, JavaScript, C# — VBA/독자 언어는 개발자 이탈 원인 |
| **무제한 개발 라이선스** | ★★★★★ | Ignition 방식: 라이선스 1개로 무제한 개발자 동시 작업 |
| **크로스플랫폼** | ★★★★★ | Windows, Linux, macOS, Web, 임베디드 모두 지원 |
| **통합 IDE** | ★★★★☆ | 별도 설치 없이 플랫폼 내장 IDE로 즉시 개발 가능 |
| **템플릿/재사용 시스템** | ★★★★☆ | 화면 40% 더 빠르게 개발 가능, 객체 지향적 화면 설계 |
| **협업 개발** | ★★★★☆ | 동시 접속 개발, 버전 관리, 변경 이력 추적 |
| **API/SDK 개방성** | ★★★★☆ | REST/GraphQL API, 서드파티 통합 용이성 |
| **빠른 프로토타이핑** | ★★★☆☆ | 드래그앤드롭, SVG 임포트, 위젯 라이브러리 |
| **시뮬레이션 모드** | ★★★☆☆ | PLC 없이 태그 시뮬레이션으로 개발 가능 |

### 개발자가 싫어하는 것 (Anti-Pattern)

```
[경고] 이것들은 개발자를 떠나게 만든다:

✗ 태그 수에 따른 과금 — 확장할수록 비용 폭발
✗ 클라이언트 수 제한 — "라이선스가 부족합니다" 에러
✗ 별도 구매 필요한 개발 환경 — 현장 가서 수정 못하는 상황
✗ Windows 전용 — 리눅스 서버/임베디드 대응 불가
✗ 독자 스크립팅 언어 — 학습 곡선 ↑, 생태계 없음
✗ 폐쇄적 통신 드라이버 — 새 PLC 추가마다 벤더 의존
```

---

## 5. 구매를 결정짓는 서비스 유형

### 서비스 유형별 구매 영향도

```
구매 영향도 (High → Low)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. 기술 지원 & SLA        ████████████████████  98%
   "장애 시 4시간 내 응답 보장이 없으면 계약 안 함"

2. 시스템 통합(SI) 서비스  ███████████████████   92%
   "우리가 직접 못 하니까 다 해주는 곳을 원함"

3. 교육/트레이닝           █████████████████     85%
   "운전원이 못 쓰면 소용없다"

4. 마이그레이션 서비스     ████████████████      80%
   "기존 시스템에서 데이터/화면 옮겨줘야 함"

5. 사이버보안 서비스       ███████████████       75%
   "컴플라이언스 감사 대비 필수"

6. 원격 모니터링/관리      ██████████████        70%
   "관리자 없어도 돌아가게"

7. 클라우드 호스팅         ████████████          60%
   "서버 관리 안 하고 싶다"

8. 컨설팅/아키텍처 설계    ███████████           55%
   "처음부터 제대로 설계하고 싶다"
```

### 서비스 유형 상세 분석

#### 5.1 기술 지원 & SLA (구매 영향도: 98%)

고객이 가장 먼저 확인하는 항목. 특히 24/7 운전 현장에서는 SLA가 계약 성사의 핵심.

- **24시간 전화 지원** + 원격 접속 트러블슈팅
- **긴급 현장 출동** 보장 (SLA에 응답 시간 명시)
- **연간 유지보수 계약 (AMC)** — 매출의 15~20%를 반복 매출로 확보

#### 5.2 턴키 시스템 통합 (구매 영향도: 92%)

중소기업 고객의 대부분은 자체 SCADA 엔지니어가 없다. "설계부터 시운전까지 다 해주는" 턴키가 핵심.

- 시스템 설계 → HW/SW 조달 → PLC 프로그래밍 → HMI 개발 → 통신 구축 → 시운전 → 교육
- **프로젝트 평균 마진: 25~40%** (소프트웨어 개발 부분이 마진 최고)

#### 5.3 교육/트레이닝 (구매 영향도: 85%)

- 운전원 교육 (시스템 사용법)
- 엔지니어 교육 (개발/수정 방법)
- **인증 프로그램**: 벤더 인증 SI 파트너 양성 → 생태계 확장

#### 5.4 마이그레이션 서비스 (구매 영향도: 80%)

SCADA의 교체 주기는 10~20년. 기존 시스템에서의 이전이 최대 진입 장벽.

- 기존 태그/알람/트렌드 데이터 이관
- HMI 화면 자동/반자동 변환 도구
- **호환 레이어**: 기존 데이터를 신규 시스템에서 조회 가능하게 (다운타임 없이)

#### 5.5 사이버보안 서비스 (구매 영향도: 75%)

- 취약점 스캔 + 패치 관리
- IEC 62443 / NERC CIP 컴플라이언스 감사 대응
- 역할 기반 접근 제어 (RBAC) 설정
- **월간 구독 패키지**: 소프트웨어 업데이트 + 취약점 스캔 + 컴플라이언스 보고

---

## 6. 주요 플랫폼 비교: Ignition vs Wonderware vs WinCC

### 가격 및 라이선스 비교

| 항목 | Ignition | Wonderware (AVEVA) | WinCC (Siemens) |
|------|----------|-------------------|-----------------|
| **시작 가격** | ~$7,500/서버 | ~$25,000+ | ~$15,000+ |
| **태그 라이선스** | 무제한 | 태그/I/O 수 기반 과금 | 구성별 과금 |
| **클라이언트 라이선스** | 무제한 | 클라이언트 수 기반 과금 | 클라이언트 수 기반 과금 |
| **개발 환경** | 무료 포함 | 별도 라이선스 필요 | TIA Portal 포함 |
| **스크립팅** | Python/Java | 독자 언어/VBA | JavaScript/.NET |
| **크로스플랫폼** | Win/Linux/Mac/Web | Windows 주로 | Windows 주로 |
| **웹 클라이언트** | 네이티브 지원 | 제한적 | WinCC Unified에서 지원 |
| **최적 생태계** | 벤더 무관 | AVEVA/다양한 PLC | Siemens PLC |

### 개발자 경험 평가

```
Ignition     ████████████████████  9.0/10  "Python이 VBA보다 광년 앞서 있다"
Wonderware   ██████████████        7.0/10  "빠르게 배우지만 라이선스가 짜증"
WinCC        ██████████            5.0/10  "매우 어렵고 사용자 비친화적"
```

### 10년차 개발자의 판단

**Ignition이 현재 시장에서 가장 파괴적인 모델**이다:
- 무제한 라이선스 = 규모가 커질수록 경쟁사 대비 TCO 압도적 우위
- 크로스플랫폼 + 웹 네이티브 = 미래 대응력
- Python 기반 = 개발자 풀이 넓음

**그러나 Wonderware/WinCC가 죽지 않는 이유:**
- 기존 설치 기반 (installed base)이 압도적 — 교체 비용이 높음
- 대기업은 "검증된 벤더"를 선호 — Schneider, Siemens의 브랜드 파워
- Siemens PLC + WinCC의 TIA Portal 통합은 Siemens 생태계에서 대체 불가

---

## 7. 한국 시장 특수성 및 기회

### 한국 SCADA 시장 규모

- 2024년: **$4.17억** (약 5,500억 원)
- 2033년 전망: **$5.91억** (약 7,800억 원)
- CAGR: **3.95%**

### 한국 시장의 특수성

| 특성 | 시사점 |
|------|--------|
| **MELSEC(미쓰비시) PLC 점유율 높음** | MELSEC 3E 드라이버 필수 |
| **수처리/반도체/자동차 중심** | 이 3개 산업 특화 기능이 경쟁력 |
| **SI 의존도 높음** | SI 파트너 네트워크가 곧 시장 지배력 |
| **가격 민감도** | Ignition식 무제한 라이선스가 어필 가능 |
| **보수적 벤더 선택** | 레퍼런스 사이트 수가 의사결정의 핵심 |
| **스마트팩토리 정부 지원** | 중소기업 스마트팩토리 보조금 활용 가능 |

### 한국 시장 진입/확장 전략

1. **수처리/반도체 특화 템플릿** 사전 구축 → 시운전 기간 단축 → SI 원가 절감
2. **MELSEC + Modbus 네이티브 드라이버** 완벽 지원 → 한국 PLC 시장 커버
3. **Korean + 다국어 런타임 전환** → 해외 수출 장비 대응
4. **스마트팩토리 보조금 패키지** → 중소기업 진입 장벽 낮춤
5. **클라우드 하이브리드** → 본사에서 지방 공장 원격 모니터링

---

## 8. 현직 개발자로서의 전략적 제언

### 지금 당장 수익을 만들 수 있는 3가지

#### 1. "SCADA-as-a-Service" 구독 모델

```
기존 모델:        라이선스 $50K + 연 유지보수 $8K = 첫해 $58K, 이후 $8K/년
SaaS 모델:        월 $2K × 12개월 = $24K/년 → 3년 차부터 기존 모델 초과 수익
                  + 해지율 낮음 (데이터 종속) + 자동 업그레이드 포함
```

핵심: **초기 진입 장벽을 낮추고 장기 Lock-in으로 LTV(Lifetime Value) 극대화**

#### 2. 사이버보안 번들 패키지

규제 의무화가 진행 중인 지금이 골든 타임:

- SCADA 라이선스 + 사이버보안 월간 구독 번들
- IEC 62443 컴플라이언스 보고서 자동 생성
- 취약점 스캔 + 패치 관리 포함
- **이건 "팔아야 하는" 게 아니라 "고객이 사야만 하는" 서비스**

#### 3. 마이그레이션 가속 도구

SCADA 교체 주기(10~20년)가 도래하는 시스템이 급증하고 있다:

- 기존 화면 자동 변환 도구 (Wonderware → 신규 플랫폼)
- 태그/알람 매핑 자동화
- 히스토리 데이터 무중단 이관
- **"전환 비용 절감"은 가장 강력한 영업 무기**

### 기술 로드맵 제안

```
2026 H1:  웹 기반 HMI (HTML5/WASM) + 클라우드 하이브리드
2026 H2:  UNS(Unified Namespace) + MQTT/Sparkplug B 통합
2027 H1:  AI/ML 예측 정비 모듈 (온프레미스, 클라우드 불필요)
2027 H2:  디지털 트윈 연동 + 에지 컴퓨팅 최적화
2028:     완전한 클라우드 네이티브 SCADA + 멀티테넌시
```

### 최종 요약: 돈이 되는 SCADA/HMI 만들기

```
┌─────────────────────────────────────────────────────────┐
│                                                         │
│  수익성 = 반복매출(구독) × 규모(무제한 라이선스)        │
│          × Lock-in(데이터 종속) × 규제 의무(보안)       │
│                                                         │
│  고객이 사는 이유:                                       │
│  1. "이거 없으면 공장이 멈춘다" (안정성)                │
│  2. "법적으로 해야 한다" (사이버보안 규제)              │
│  3. "기존 것보다 운영비가 싸다" (TCO 절감)              │
│  4. "우리가 직접 할 수 없다" (SI 서비스 의존)           │
│  5. "사장님이 대시보드 보고 싶다" (웹/모바일 접근)      │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

---

## 9. FAQ — 자주 묻는 질문

### Q1. 24시간 기술 지원이 되는 SCADA/HMI 벤더가 있는가?

**있다. 단, 대부분 프리미엄/상위 지원 계약에서만 제공된다.**

#### 벤더별 24/7 기술 지원 비교

| 벤더 | 24/7 포함 여부 | 지원 티어 | P1(긴급) 응답 시간 | 가격 공개 |
|------|---------------|----------|-------------------|----------|
| **AVEVA (Wonderware)** | Premium/Elite 포함 | Standard / Premium / Elite | 30분~2시간 | 비공개 |
| **Rockwell (FactoryTalk)** | TechConnect 24x7 포함 | Self-Assist / Product / System / Application | 즉시 콜백 | 약 £15,000/년 |
| **VTScada** | 애드온으로 제공 | Standard / 24/7 Emergency / Premium | 보장 (협의) | **공개** — 라이선스의 20%/년 |
| **Schneider Electric** | Premium 포함 | Standard / Premium | 비공개 | 비공개 |
| **Ignition** | **별도 과금** ($450/시간) | BasicCare / TotalCare / PriorityCare | 비공개 | 라이선스의 16~24%/년 |
| **Siemens (WinCC)** | 계약별 협의 | Basic / Priority / Managed / Custom | 비공개 | 비공개 |
| **GE Vernova (iFIX)** | 미확인 | Premier / Enterprise | 비공개 | 비공개 |
| **COPA-DATA (zenon)** | 커스텀 SLA 필요 | Standard / Long-Term / Custom | 비공개 | 비공개 |

#### 10년차 개발자의 현장 코멘트

```
[핵심 포인트]

✓ "진짜 24/7"이 필요하면 → AVEVA Premium/Elite 또는 Rockwell TechConnect
  - AVEVA는 SLA 응답 시간이 가장 명확하게 문서화되어 있음 (P1: 30분 Elite)
  - Rockwell은 24x7x365가 기본 옵션으로 제공됨

✓ 합리적 가격에 24/7 원하면 → VTScada
  - 가격이 완전 공개 (라이선스의 20%/년, 최소 $1,500)
  - 전담 담당자가 고객 시스템을 숙지하는 방식 → "벤더가 아니라 우리 팀 같다"는 평가

✓ Ignition은 커뮤니티/인티그레이터 생태계가 강점
  - 공식 24/7은 $450/시간으로 비쌈
  - 대안: Ignition 전문 SI 업체가 24/7 매니지드 서비스 제공 (더 경제적)

✗ 한국 시장에서 "24시간 지원"을 찾는다면:
  - 글로벌 벤더의 한국 지사/파트너를 통한 로컬 지원 체계 확인 필수
  - CIMON(시몬): 한국 본사 기반, 삼성/LG/현대 등 대기업 레퍼런스 보유
  - 실질적으로는 SI 업체의 유지보수 계약이 24시간 대응의 핵심
```

#### 한국 시장 현실

한국에서 "24시간 지원"은 대부분 **SI 업체의 유지보수 계약**을 통해 이루어진다. 글로벌 벤더의 한국 지사는 영업시간 지원이 기본이고, 야간/주말 긴급 대응은 SI 파트너가 담당하는 구조다.

| 경로 | 특징 |
|------|------|
| 글로벌 벤더 한국 지사 | 평일 영업시간 기술 지원 + 긴급 시 본사 에스컬레이션 |
| 국내 SI 업체 (유지보수 계약) | **실질적 24시간 대응**의 핵심, 현장 출동 포함 |
| 국내 벤더 (CIMON 등) | 한국어 직접 지원, 로컬 대응 빠름 |

---

### Q2. "턴키 SI 서비스"란 무엇인가?

**턴키(Turnkey)**란 "열쇠만 돌리면 바로 사용할 수 있는" 상태까지 **모든 것을 일괄 제공**하는 서비스를 말한다.

#### 턴키 SI의 전체 범위

```
┌─────────────────────────────────────────────────────────────────┐
│                    턴키 SI 서비스 전체 흐름                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  1. 컨설팅/설계    고객 요구사항 분석 → 시스템 아키텍처 설계     │
│       ↓            P&ID, 통신 구성도, 태그 리스트 작성           │
│                                                                 │
│  2. HW 조달        PLC, RTU, 네트워크 장비, 서버, 패널 등       │
│       ↓            벤더 선정, 구매, 입고 검수                    │
│                                                                 │
│  3. SW 개발        PLC 프로그래밍 + HMI/SCADA 화면 개발         │
│       ↓            알람 설정, 트렌드 구성, 리포트 개발           │
│                                                                 │
│  4. 통신 구축      PLC ↔ SCADA 통신 설정 (OPC UA, Modbus 등)   │
│       ↓            네트워크 구성, 방화벽, VPN 설정               │
│                                                                 │
│  5. FAT            공장 출하 전 사내 테스트 (Factory Acceptance) │
│       ↓            고객 입회 하에 기능/성능 검증                 │
│                                                                 │
│  6. 현장 설치      장비 설치, 배선, 접지, 전원 공급              │
│       ↓                                                         │
│  7. SAT/시운전     현장 실제 환경에서 최종 테스트                │
│       ↓            (Site Acceptance Test)                        │
│                                                                 │
│  8. 운전원 교육    시스템 사용법, 비상 대응 절차 교육            │
│       ↓                                                         │
│  9. 인수인계       문서 납품, 검수 완료                          │
│       ↓                                                         │
│  10. 유지보수      연간 유지보수 계약 (AMC)                      │
│                    장애 대응, 소프트웨어 업데이트, 24시간 콜 대응 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

#### 턴키 vs 부분 SI 비교

| 구분 | 턴키 SI | 부분 SI |
|------|---------|---------|
| **범위** | 설계~시운전~유지보수 전체 | 특정 단계만 (예: HMI 개발만) |
| **책임** | SI 업체가 전체 책임 (단일 창구) | 고객이 여러 업체 조율 |
| **비용** | 높지만 예측 가능 | 낮지만 추가 비용 발생 가능 |
| **리스크** | SI 업체가 흡수 | 고객이 분산 관리 |
| **적합 대상** | 자체 SCADA 엔지니어 없는 중소기업 | 자체 엔지니어링 역량 보유 기업 |

#### 왜 턴키가 구매 영향도 92%인가?

```
고객의 속마음:

"우리는 제조/발전/수처리를 하는 회사지, IT 회사가 아니다."
"PLC 프로그래밍? HMI 개발? 통신 설정? 우리가 어떻게 하나?"
"문제 생기면 한 곳에만 전화하고 싶다."
"도입부터 운영까지 다 맡길 수 있는 곳을 찾는다."
```

**핵심:** 한국 시장에서 SI 의존도가 특히 높은 이유는 **중소기업 비율이 높고, 자체 OT 엔지니어를 고용하기 어렵기 때문**이다. SI 파트너 네트워크의 규모와 품질이 곧 SCADA 플랫폼의 시장 지배력을 결정한다.

#### 턴키 SI의 수익 구조

```
프로젝트 매출 분해 (중형 프로젝트 $300K 기준):

컨설팅/설계       $45K~$60K    (15~20%)   마진 60~70%  ← 고부가가치
하드웨어 조달     $60K~$90K    (20~30%)   마진 10~20%  ← 볼륨 딜 마진
소프트웨어 개발   $75K~$105K   (25~35%)   마진 50~70%  ← 마진 최고
시운전/교육       $30K~$45K    (10~15%)   마진 30~40%
유지보수 계약     $30K~$45K/년 (10~15%)   마진 40~50%  ← 반복 매출

총 프로젝트 마진: 평균 25~40%
+ 유지보수 반복 매출이 연간 프로젝트 매출의 10~15% 추가
```

---

### Q3. 클라우드 SCADA를 선택하는 이유는?

#### 클라우드를 선택하는 8가지 이유

| # | 이유 | 데이터/근거 |
|---|------|------------|
| 1 | **비용 절감 (CapEx → OpEx)** | 클라우드 전환 시 TCO 25~35% 절감. Ignition Cloud + AWS는 전통 플랫폼 대비 **60~70% 비용 절감** (10,000태그 기준 $15K~$25K vs $80K~$150K) |
| 2 | **탄력적 확장** | 태그 수, 사이트 수, 스토리지를 HW 구매 없이 즉시 확장. 인수합병 시 새 사이트 추가도 용이 |
| 3 | **원격 접근 / 멀티사이트** | 인터넷만 있으면 어디서든 모니터링. 코로나 이후 필수 기능화. 지방 공장 37개 사이트를 중앙에서 관리한 사례 (ARB Midstream + AWS) |
| 4 | **자동 업데이트** | 보안 패치, 기능 업데이트가 자동 적용. 레거시 시스템의 미패치 취약점 문제 해소 |
| 5 | **재해 복구 / 이중화** | 지리적으로 분산된 자동 백업, 멀티리전 복제. 온프레미스에서 같은 수준의 이중화를 구현하면 비용이 2~3배 |
| 6 | **AI/ML 통합** | AWS SageMaker, Azure AI 등 클라우드 네이티브 AI 서비스와 즉시 연동. 예측정비, 공정 최적화에 활용 |
| 7 | **IT 인력 절감** | 서버 관리, HW 교체, 네트워크 유지보수를 클라우드 제공자가 담당. 소규모 중앙팀으로 다수 사이트 관리 가능 |
| 8 | **배포 속도** | ARB Midstream: 37개 사이트 SCADA를 **6개월**에 구축. Weatherford CygNet: **수 시간**에 설치 완료 |

#### 그러나 클라우드만으로는 안 되는 이유 (리스크)

| # | 우려 사항 | 현실 |
|---|----------|------|
| 1 | **실시간 제어 지연** | 필드버스/컨트롤러는 250μs~1ms 응답 필요. 퍼블릭 클라우드는 이 지연을 보장 불가. **직접 제어는 반드시 엣지/온프레미스에서** |
| 2 | **인터넷 의존성** | 연결 끊기면 가시성 상실. 미션 크리티컬 현장은 **로컬 백업 노드 필수** |
| 3 | **데이터 주권/규제** | NERC CIP에는 클라우드 가상화/멀티테넌시 규정 미비. GDPR 등 각국 규제 충돌 가능 |
| 4 | **보안 위협** | 공격 표면 확대. Colonial Pipeline 랜섬웨어, 플로리다 수처리 시설 해킹 등 실제 사고 발생 |
| 5 | **벤더 종속** | AWS IoT SiteWise, Azure Digital Twins 등 독점 서비스에 깊이 통합하면 전환 비용 급증 |

#### 결론: 하이브리드가 정답

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   업계 컨센서스: "순수 클라우드 SCADA"는 실시간 제어에       │
│   적합하지 않다. 그러나 "하이브리드 아키텍처"는 양쪽의       │
│   장점을 모두 취한다.                                        │
│                                                             │
│   ┌──────────────┐        ┌──────────────────┐             │
│   │  엣지/로컬    │  ←──→  │  클라우드          │             │
│   │              │        │                  │             │
│   │ • 실시간 제어 │        │ • 모니터링/분석   │             │
│   │ • PLC 통신   │        │ • AI/ML          │             │
│   │ • 알람 처리   │        │ • 멀티사이트 뷰   │             │
│   │ • 로컬 HMI   │        │ • 재해 복구       │             │
│   │ • 오프라인 운전│        │ • 대시보드/리포트  │             │
│   └──────────────┘        └──────────────────┘             │
│                                                             │
│   핵심: 결정적(Deterministic) 제어는 엣지에서,              │
│         가시성과 분석은 클라우드에서.                         │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

#### 주요 클라우드 SCADA 제품

| 제품 | 제공사 | 배포 방식 | 과금 모델 | 최적 용도 |
|------|--------|----------|----------|----------|
| **AWS IoT SiteWise** | Amazon | 클라우드 매니지드 | 사용량 기반 | 멀티사이트 모니터링, ML |
| **Ignition Cloud Edition** | Inductive Automation | AWS/Azure/GCP | 시간 기반, 무제한 태그 | 멀티클라우드 유연성 |
| **AVEVA Connect** | AVEVA (Schneider) | 클라우드/온프레미스 | $25,000+ | 기존 Wonderware 사용자 |
| **Azure IoT / Digital Twins** | Microsoft | 클라우드 네이티브 | 사용량 기반 | MS 생태계, 디지털 트윈 |
| **CygNet SCADA** | Weatherford | Google Cloud | 커스텀 | Oil & Gas 특화, 최속 배포 |
| **VTScada** | Trihedral | 온프레미스/클라우드 | 영구 라이선스 | 수처리, 무제한 이중화 |

---

## 참고 자료 (Sources)

- [Fortune Business Insights - SCADA Market](https://www.fortunebusinessinsights.com/scada-market-102433)
- [MarketsandMarkets - SCADA Market](https://www.marketsandmarkets.com/Market-Reports/scada-market-19487518.html)
- [Precedence Research - SCADA Market](https://www.precedenceresearch.com/scada-market)
- [Business Research Insights - SCADA Market](https://www.businessresearchinsights.com/market-reports/scada-market-119383)
- [Grand View Research - SCADA Systems](https://www.grandviewresearch.com/industry-analysis/supervisory-control-data-acquisition-systems-scada-market)
- [Top 8 SCADA Platforms Compared for 2025](https://tatsoft.com/top-8-scada-platforms-compared/)
- [Top 12 HMI/SCADA Selection Criteria for 2025](https://www.industrialautomationco.com/blogs/news/top-12-hmi-scada-selection-criteria-for-2025)
- [How to Choose an HMI/SCADA Vendor in 2025](https://industrialautomationco.com/blogs/news/how-to-choose-an-hmi-scada-vendor-in-2025-pricing-support-and-key-considerations)
- [SCADA Software Comparison: Wonderware vs Ignition vs WinCC](https://eureka.patsnap.com/article/scada-software-comparison-wonderware-vs-ignition-vs-wincc)
- [Ignition SCADA Pricing](https://inductiveautomation.com/pricing/ignition)
- [AVEVA Edge - HMI and IoT Edge](https://www.aveva.com/en/products/edge/)
- [Essential Features for Rapid HMI/SCADA Development](https://www.aveva.com/en/perspectives/blog/essential-features-for-rapid-hmi-scada-development/)
- [Best SCADA Software 2025](https://plcprogramming.io/blog/best-scada-software-2025)
- [SCADA Software Price In 2025](https://savvycomsoftware.com/blog/scada-software-price/)
- [VTScada - Total Cost of SCADA Ownership](https://www.vtscada.com/what-determines-total-cost-of-scada-system-ownership/)
- [IMARC Group - South Korea SCADA Market](https://www.imarcgroup.com/south-korea-scada-market)
- [여기에뉴스 - 국내 SCADA 시스템 시장동향](https://yeogienews.com/today/265267)
- [Emerson HMI/SCADA Software Adds Features](https://www.automation.com/en-us/products/august-2025/emerson-hmi-scada-software-adds-features)
- [Inductive Automation - Support Policy](https://inductiveautomation.com/support/policy/)
- [Ignition Product Support Plans](https://page.inductiveautomation.com/product-support-plans)
- [AVEVA Customer FIRST Program](https://www.aveva.com/content/dam/aveva/documents/legal/policies/UserGuide_AVEVA_CustomerFIRSTProgram.pdf)
- [Rockwell Automation - TechConnect Support](https://support.rockwellautomation.com/)
- [VTScada - Premium 24/7 Support](https://www.vtscada.com/premium-24-7/)
- [VTScada - SupportPlus Service Pricing](https://www.vtscada.com/vtscada-supportplus-service-pricing/)
- [COPA-DATA - Product Life Cycle & Support](https://www.copadata.com/en/support-services/product-life-cycle-and-support/)
- [CIMON - Korean SCADA Vendor](https://www.cimon.com/)
- [AWS - Cloud-Based SCADA for Industrial Operations](https://aws.amazon.com/blogs/industries/improve-your-industrial-operations-with-cloud-scada/)
- [DataStackHub - Cloud TCO Statistics](https://www.datastackhub.com/insights/cloud-tco-total-cost-of-ownership-statistics/)
- [PAK Energy - Advantages of Cloud-Based SCADA](https://pakenergy.com/blog/the-advantages-of-cloud-based-scada)
- [Weatherford - IoT/SCADA Platform on Google Cloud](https://www.weatherford.com/products-and-services/production-and-intervention/production-4-0/iot-scada-platform/)
- [NERC - BES Operations in Cloud White Paper](https://www.nerc.com/comm/RSTC_Reliability_Guidelines/SITES_WhitePaper_BES_Ops_in_Cloud.pdf)
