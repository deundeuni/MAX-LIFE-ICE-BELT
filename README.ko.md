# MAX-LIFE ICE-BELT — 상시 해수 접촉 구조물, 쇄빙선 갑판 스플래시·선수·선미, 클램핑 스캐폴드, 의도적·자생적 따개비·홍합·굴 희생장갑 및 항공 회전체 어블레이티브 시스템 기술 명세서 (Ver. 1.6 최종 교정본)

* 공식 문서 분류: 방어적 선행기술 공개 백서 (Defensive Publication / Prior Art)
* 최초 구상일: 2026-09-02 / 최종 개정일 (v1.6): 2026-09-06
* 원천 지적재산권(IP) 보유자: 소마모아 (soma-moa / 구상자: deundeuni)
* 공식 저장소: github.com/soma-moa | 공식 도메인: somamoa.ai.kr
* 적용 라이선스: CC BY 4.0 & DPL v1.0 (Defensive Patent License)
* 원안 언어 고지: 본 문서의 한국어 원문이 법적·기술적 기준 원본이며, 영문 번역본은 참고용이다. 해석상 충돌 발생 시 한국어 원문의 서술과 정의가 최우선한다.

---

## 0. 창안자 선언 및 동기

### 0.1 현장에서 출발한 직관적 동기 (Field-Driven Motivation)
본 구조 설계는 "갑판부 바깥쪽 바닷물 닿는 구간, 쇄빙선의 선수와 선미는 항상 깨지고 닳는데, 매번 페인트칠과 철판 교체로 막을 수 없다"는 현장 문제의식에서 출발하였다.
기존 해양 방오 기술은 따개비, 홍합, 굴 등 부착 생물을 전면 제거 및 방지의 대상으로만 국한하여 접근하였다. 본 발명은 이러한 관점을 역발상하여, 의도적 인공 유도뿐만 아니라 자연적 착생 방치, 생물학적 유도물질 미도포 상태에서의 자생적 부착 및 합성 $CaCO_3$ 모사체를 포괄하여, 부착 생물 및 석회질 형성물을 충격 시 일차적으로 파쇄되며 에너지 및 마찰력을 흡수하는 "희생층(Sacrificial Layer)"으로 전환 정의한다. 이에 따라 물리적 충격으로 희생층이 깨져 나간 후에도 내부의 기계적 뼈대는 보존되고 표면 생물층이 지속적으로 자가 재생되는 '생존 장갑' 메커니즘을 창안하였다. 기존 CWP 배터리 스왑 모듈에서 검증된 롤링 및 클램핑 탈착 구조를 하부 골격으로 채용함으로써, 모선 및 구조물 표면에 대한 직접 용접 작업 없이 고정력을 확보하는 생존형 방어 구조를 정립한다.

### 0.2 기본 개념 및 재료 융합 확장성 선언 (Master Concept & Material Fusion Standard)
본 명세서에 개시된 클램핑 스캐폴드 기반의 0점(Zero-Point) 기준 고정 방식 및 희생층 자가재생 메커니즘은 전체 보호 시스템의 최상위 기본 기준점(Master Reference Framework)으로 기능한다.
본 설계는 공지기술인 자동차 패시브 세이프티(Passive Safety) 철학(Béla Barényi, 1951)의 구조적 희생 개념을 해양 및 항공 환경으로 확장 원용한다. 요철 스캐폴드의 물리적 재질(강재, 알루미늄 합금, FR-복합재, 고내식성 합금 등), 따개비·홍합·굴 등 해양 부착 생물 유도 및 착생 방식(표면 물리적 조도 제어, 미세 미소전류 인가, 생물학적 유도물질 도포, 자연적 착생 방치, 합성 $CaCO_3$ 모사체 도포 등), 부착층 두께 범위, 클램핑 메커니즘(볼트 체결, 롤링 락, 영구자석/전자기 결합, 음압 흡착 방식 등) 및 AI 기반 부착·탈락 예측 모델이 단독 또는 복합 추가되는 모든 확장 실현 형태는 본 기본 개념의 부가적 응용 조합이며, 본 선행기술의 포괄적 보호 범주에 포함될 수 있다.

* **상위 아키텍처 및 APU 제어기 연계 명시:** 본 ICE-BELT의 스캐폴드 0점 고정 및 100ms 국소 격리 제어는 `ARCHITECTURE_STRATEGY v3.2.4`의 범용 생존 아키텍처 및 `chiplet-apu-multi-system-survival-architecture v2.6`의 Tri-State Isolation, T-Reg 억제 논리를 해양 물리 환경에 구현한 하위 구현체이다.

### 0.3 유기적 무중단 구조 및 무용접 원칙 (Zero-Downtime & Non-Welding)
본 구조체는 기존 선체 외판 및 해양 구조물 본체에 대한 전기적·물리적 손상(고열 용접, 관통 천공 등)을 수반하는 개조 작업을 엄격히 방지하는 것을 원칙으로 한다. 특정 국소 영역의 희생층이 고출력 유빙 충격 및 마찰로 인해 완파·탈락하더라도 전체 방어 시스템의 연속적 보호 기능이 정지되지 않는 유기체적 무중단 생존력(Zero-Downtime)을 지향한다. 하부 스캐폴드는 분할된 독립 다중 고정 구조를 유지하여 단일 장애점(SPOF, Single Point of Failure) 발생을 완화하며, 외부 희생층이 파열된 후에도 기계적 스캐폴드 골격은 원형을 유지하여 차세대 생물체의 재부착을 지속적으로 유도한다.

### 0.4 비배타적 상호운용성 및 공용 오픈 표준
본 기술 명세는 특정 조선소, 선급 협회, 특수 도료 제조사, 해양 구조물 형상에 독점적으로 귀속되지 않는다. ISO 8501 등 공공 영역의 표면 처리 및 부식 관리 표준, 각국 선급 규정의 아이스벨트(Ice-belt) 구조 기준, 해양 생물 부착 유도 기법에 관한 공공 연구 표준을 보조적 기준점으로 원용할 수 있는 범용 오픈 표준(Universal Open Standard)으로 작동한다.

### 0.5 현장 기반 우선순위 제어 원칙
극한 환경에서 한계치를 초과하는 충격 과부하가 발생할 경우, 시스템은 하부 스캐폴드 골격 구조의 물리적 잔존 및 모선 밀착 유지를 최우선순위로 설정하여 제어한다. 희생층 표면의 완벽한 형상 유지 등 후순위 보호 목표는 단계적으로 포기 및 억제함으로써 모선 외판에 대한 직접적 충격 전달을 방지하고 보호 기능의 제어 연속성을 확보한다. 본 시스템은 영구불멸의 절대적 보호를 보장하지 않으며, 구조물의 유지보수 및 교체 주기를 물리적으로 최대한 연장하는 것을 현실적 목표로 설정한다.

### 0.6 포괄적 적용 범위 및 항공/회전체 확장성 (Universal Application Scope)
본 설계 메커니즘은 극지 항해용 쇄빙선, 일반 상선 충돌부, 불워크 외현 스플래시 벨트, 방파제 전면부, 해상풍력 하부 기초 구조물(하부 승강장 포함), 부유식 해양 플랜트(FLNG/FPSO), CWP 계류체 등 동적 해수 접촉, 유빙 충돌, 말단 비산염분이 발생하는 모든 해양 구조물의 외각 보호층에 포괄적으로 적용 가능하다.
더불어 본 메커니즘의 항공 및 회전체 적용 시, 국소 탈락에 따른 회전 불균형(Dynamic Unbalance)을 완화하기 위한 대칭 자율 박리(Self-balancing Ablation) 및 원터치 클램핑 슬롯 기반의 무공구 퀵 릴리즈 카트리지(Zero-Tool Quick Replacement Cartridge) 교체 구조를 선택적으로 결합할 수 있다.

### 0.7 공개 목적 및 환경 안전성 한계 고지
본 문서는 사적 독점권 설정을 방지하고 기술의 공공성을 확립하기 위한 방어적 선행기술 공개(Defensive Publication) 자료이다. 명세서 내 수치, 기능, 물리적 구성, 예상 성능 서술은 기술 사상을 설명하기 위한 예시적 서술이며 특정 실제 구현 형태를 일률적으로 한정하거나 절대적 성능 수치를 보장하지 않는다. 본 시스템은 기존 법정 선급 검사 기준, 해양환경오염방지협약(MARPOL), 국제해사기구(IMO) 방오 규정을 자동 대체·변경·확장하지 않으며 보조적·참고적 보호 구조체로서만 활용된다. 본 희생층은 따개비, 홍합, 굴 기원의 생물 무기질 및 합성 $CaCO_3$ 모사체를 포함하는 탄산칼슘 성분을 주요 성분으로 포함하여, 합성수지계 미세플라스틱(Microplastic) 유출을 완화하도록 설계된다. 탈락 시 해양에서 자연 분해되는 천연 탄산칼슘 입자로서 IMO AFS 협약 및 EU 해양전략 프레임워크(MSFD) 규제 대응을 보조하는 환경 친화적 특성을 지향한다.

### 0.8 독립적 선행 구상 인정 및 겸양 고지 (v1.4 삼중 방어 조항 유지)
본 시스템 설계는 창안자가 현장 문제의식에서 출발하여 기존 공개된 원리 및 공지기술($CaCO_3$ 생물광물화, 희생 양극, 자동차 크럼플존 등)이 이미 존재하는지 여부를 확인·검토한 후, 창안자 개인의 관점에서 "나는 이렇게 생각했다"는 방식으로 조합·재구성한 것이다.
"본인이 혼자 최초로 독자 구상했다"고 주장하지 않으며, 동일하거나 유사한 기술적 모티프가 타 연구자 또는 산업 현장에서 독립적으로 구상되었을 가능성을 충분히 인정한다.
본 공개의 목적은 특정 주체의 배타적 특허 독점권 확보가 아니며, 기술 내역을 공공의 선행기술(Prior Art)로 등록하여 타 주체의 사적 독점 출원 시 신규성·진보성 부정의 거절 근거를 제공하는 데 있다. 한국어 원문이 기준 원본(Original Authority)이며, 타 언어 번역본에서 의미상 충돌이나 해석 차이 발생 시 한국어 원문의 서술과 정의를 최우선 기준으로 적용한다.

---

## 1. 버전 변경 이력

* v1.0 (2026-09-03): 갑판 스플래시 계통, 선수 아이스벨트, 선미 추진부 제어 영역을 상호 연계하는 3점 결합 구조 명세 정립. 클램핑 스캐폴드 골격층과 의도적 따개비 부착 희생층의 유기적 결합 구조 및 동적 제어 알고리즘 통합 완료.
* v1.1 (2026-09-03): IMO AFS 및 EU MSFD 해양 환경 규제 대응을 위한 탈락 희생층의 천연 탄산칼슘($CaCO_3$) 성분 고지, 미세플라스틱 완화 명세, 동적 충격 흡수 감쇄식 및 생물 자가재생 성장 방정식 정형화 수식 보완.
* v1.2 (2026-09-03): 항공/헬기 로터 블레이드 확장에 따른 회전 불균형 완화 대칭 자율 박리(Self-balancing Ablation) 명세 및 무공구 퀵 릴리즈 교체(Zero-Tool Quick Replacement) 메커니즘 통합. 추상화된 가변 파라미터 수식 정비 및 방어적 표현 엄격화.
* v1.3 (2026-09-05): 석회질 부착 생물군(따개비, 홍합, 굴 등) 키워드 명시적 확장, 특허 심사관 검색 대응성 강화 및 L1 희생층 정의 상위 포괄화 패치.
* v1.4 (2026-09-05): 0.8절 창안자 삼중 방어 조항(선행기술 조사 확인, 최초/독점 미주장, 주관적 관점의 조합·재구성 명시) 정교화 패치.
* v1.5 (2026-09-05): 희생층 형성 메커니즘의 최상위 상위개념 포괄화 패치 (의도적 유도, 자연적 착생 방치, 자생적 부착 유지 및 합성 CaCO3 모사체 활용 행위 일체 포함).
* v1.6 (2026-09-06): 상위 생존 아키텍처(ARCHITECTURE_STRATEGY v3.2.4), APU 제어기(chiplet-apu-multi-system-survival-architecture v2.6) 및 CWP 4대 하드웨어 메커니즘 상호 참조 연계 패치.

---

## 2. 풀스택 응용 구조 설계 (3-Tier Architecture)

### [L2] 보호 인터페이스 레이어 (Protective Interface Layer)
* 갑판 스플래시 구간 (Zone A) — 고속 항해 및 파도 파쇄 시 발생하는 해수 비산(Splash), 비산염분, 상부 유빙 조각의 충격을 일차적으로 완화하며 염분 침투를 억제한다.
* 선수 구간 (Zone B) — 전진 항해 시 극지 유빙과의 직접적 고출력 충돌 에너지 및 수평 마찰력을 분산·흡수한다.
* 선미 구간 (Zone C) — 후진 쇄빙 작업 및 프로펠러 회전에 의한 유빙 역류 충격, 와류 마찰로부터 추진 유닛 하우징 및 러더 주변 외판을 보호한다.
* 회전체 구간 (Zone Aero) — 헬기 로터 및 항공기 흡기 전면부의 입자 충돌 하중을 어블레이티브 방식으로 흡수하며 대칭 자율 박리를 통해 회전 편심 하중을 완화한다.

### [L1] 희생·재생 패브릭 레이어 (Sacrificial & Regenerative Fabric Layer)
* 하부 뼈대 구조 — CWP 기반의 롤링 및 클램핑 고정 기법이 적용된 표면 요철 스캐폴드(Scaffold) 구조체로서, 모선 및 표면에 하중을 균일하게 분산시킨다.
* 표면 살 구조 — 의도적 유도, 자연적 착생 방치, 생물학적 유도물질 미도포 상태에서의 자생적 부착 유지, 합성 $CaCO_3$ 모사체를 포함하는 모든 형태의 $CaCO_3$계 석회질 형성물(따개비, 홍합, 굴 등) 또는 정밀 어블레이티브 카트리지 희생층이다.
* 자가재생 및 퀵 교체 알고리즘 — 충격으로 인한 희생층 국소 탈락 발생 시, 생물학적 자가 재부착을 유도하거나 무공구 퀵 릴리즈 교체 수명 주기를 추정한다.

### [L0] 인프라 및 고정 레이어 (Infrastructure & Fastening Layer)
* 모선 및 구조체 — 선체 외판, 불워크 외현, 아이스벨트 보강재, 프로펠러 덕트 노즐 외측면, 러더 전방 방어면, 항공기 로터 프레임을 포함한다.
* 고정 메커니즘 — 모재 용접이나 관통 구멍을 배제하고, 에지 클램핑, 롤링 락 및 원터치 슬롯 구조를 통해 0점 고정력을 유지한다.

### 2.5 AI 역할 및 모델 구조 정의
본 시스템에 적용되는 부착 및 탈락 예측 모듈은 특정 소프트웨어 프레임워크나 특정 알고리즘 구조에 국한되지 않는다. 온디바이스 엣지(Edge) 컴퓨팅 자원, 경량화 추론 모델(SLM), 위성 연동형 중앙 서버 분석 모델을 포괄하는 추상화된 예측 주체로 정의된다. 수온, 염분, 유속, 충돌 빈도, 회전 편심 하중 데이터를 실시간 수집·분석하여 수명 및 교체 주기를 유연하게 산출하는 것을 지향한다.

---

## 3. 핵심 시스템 블록 및 동작 메커니즘

### A. 3점 앵커 감지부 및 회전체 감지부 (절대 보호점)
* Zone A (갑판 스플래시 방어선), Zone B (선수 아이스벨트 방어선), Zone C (선미 추진부 방어선) 및 Zone Aero (회전체 균형 방어선)를 절대 보호점으로 지정한다.

### B. 뼈대-살 분리형 희생 구조부 및 공학 수식 모델링
* 외부 입력 조건 — 유빙 물리 충격, 해수 마찰, 비산염분, 항공 고속 입자 마찰 하중이 동시에 작동한다.
* 동적 처리 메커니즘 — 외부 충격 발생 시 표면 따개비, 홍합, 굴, 자생적 부착 생물층, 합성 $CaCO_3$ 모사체 등 석회질 희생층 및 어블레이티브 카트리지가 자체 파쇄·탈락하면서 운동 에너지를 열 및 위치 에너지로 전환하여 소멸시킨다. 하부 스캐폴드는 변형 없이 잔존한다.
* 1. 충격 에너지 감쇄 모델 (Sacrificial Energy Absorption)
    * 유빙 및 입자 충돌 운동에너지 공식: $$E_{ice} = \frac{1}{2} m_{ice} v^2$$
    * 희생층 파쇄 흡수 에너지 공식: $$E_{sac} = \eta \cdot \sigma_c \cdot A \cdot t$$
    * 주요 변수 정의 — $\sigma_c$: 희생층 압축강도 (재질 특성 변수), $A$: 충돌 면적, $t$: 희생층 유효 두께, $\eta$: 파쇄 효율 계수 (충돌 조건별 가변 파라미터).
    * Zero-Downtime 핵심 생존 조건식: $$E_{scaffold} = E_{ice} - E_{sac} < E_{yield\_scaffold}$$
    * 충격 후 잔여 에너지가 하부 스캐폴드의 항복 에너지를 넘지 않음으로써 뼈대가 잔존하도록 설계한다. (`LS-DYNA` 내 `*MAT_CRUSHABLE_FOAM` 및 `*MAT_ELASTIC` Explicit Dynamics 해석 모델의 준용이 가능하다.)
* 2. 재착생 속도 추정 모델 (Biogenic Growth Rate)
    * 자가재생 피복율 성장 방정식: $$\frac{dC}{dt} = r(T,S) \cdot C \cdot \left(1 - \frac{C}{K_{max}}\right) \cdot f(R_a)$$
    * 주요 변수 정의 — $C$: 피복율 (Coverage %), $K_{max}$: 최대 포화 피복율, $f(R_a)$: 스캐폴드 표면 조도 함수.
    * 환경 변수 성장률 공식: $$r(T,S) = r_0 \cdot Q_{10}^{\frac{T-T_0}{10}} \cdot \exp\left(-\alpha (S - S_{opt})^2\right)$$
    * $T$: 수온, $S$: 염분, $S_{opt}$: 환경별 최적 염분값. 본 수식은 개별 해역 조건에 따른 재생 주기의 유연한 추정에 활용될 수 있다.
* 출력 결과 — 모재 원판의 직접 손상을 완화하며, 희생층 탈락 영역에 대한 유지보수, 대칭 자율 박리 제어 및 재부착 상태 모니터링 신호를 생성한다.

### C. 자가재생 및 주기 최대한 연장 명세
* 동작 연속성 범위 — 충격 직후 초동 생물 포자 부착 단계부터, 연속 동작 및 무공구 퀵 릴리즈 카트리지 교체 범위를 모두 포함한다. 절대적인 영구 동작을 보장하지 않으며 유지보수 주기의 연장을 지향한다.

### D. 무중단 장애 이관 및 대칭 자율 박리
* 결함 격리 및 균형 동작 — 특정 구획의 희생층이 파손되는 경우 100ms 이내에 동적 제어를 국소 격리하고, 회전체 적용 시 대칭 위치의 카트리지를 미세 자율 박리(Self-balancing)하여 편심 진동을 완화하는 것을 포함한다.

---

## 4. 동적 자원 관리 및 방어적 안전 제어

* Rate Limiter (충격 빈도 정속화 제어) — 연속 충돌 발생 시 고정부에 가해지는 과도한 피로 하중 스파이크를 완화하여 전달 하중을 안정화한다.
* Tri-State Isolation (3상 제어 격리) — 센서 또는 고정부 이상 검출 시 0.1초(100ms) 이내에 고임피던스(High-Impedance) 상태로 전환하여 메인 제어계로의 오류 전파를 억제한다.

---

## 5. 표준 활용 및 법적 경계 명시

* 공공 표준 준용 — ISO 8501 표면 청정도 기준, 선급 Ice Class Rules, IMO AFS 및 EU MSFD 지침을 참고 지표로 준용한다.
* 법정 설비 비대체성 — 본 시스템은 의무 설치 구조 보강재 및 법정 방오 도료를 직접 대체하지 않으며 독립적 보조 안전 장갑으로 작동한다. 탈락 희생층은 탄산칼슘($CaCO_3$) 기원 성분을 포함하여 환경 기준 대응을 보조한다.

---

## 6. 미래 적용 및 산업 확장 범위

* 스마트 항만 방파제, 해상풍력 기초 세굴 보호, CWP 부유체 및 헬기/항공기 로터 블레이드 전면 보호층으로의 확장을 지향한다.

---

## 7. 실리보호 (Practical Protection)

* 4층 방어 체계 (Quadruple Defense Architecture)
    * 타임스탬프 체계 — 타임스탬프 기반 선행 구상 시점 증명.
    * DPL 라이선스 — Defensive Patent License v1.0 적용으로 타 주체의 사적 독점화 방지.
    * 선사용권 보유 — 현장 적용 및 시제품 제작 행위에 대한 법적 선사용권(Prior Use Right) 유지.
    * 영업비밀 분리 — 원천 개념은 공개 백서로 방어하되, 세부 가중치 및 구체적 치수는 영업비밀(Trade Secret)로 분리하여 비공개 보관한다.

---

## 8. 출처 및 문서 완전성 선언 (Sources)

* **연계 생존 아키텍처:** GitHub - `soma-moa / ARCHITECTURE_STRATEGY.md v3.2.4`
* **연계 APU 제어기:** GitHub - `deundeuni / chiplet-apu-multi-system-survival-architecture v2.6`
* **연계 CWP 4대 하드웨어 저장소:**
  * GitHub - `deundeuni / CWP-Entry`
  * GitHub - `deundeuni / CWP-Rolling-Self-Align-Battery-Swap-System`
  * GitHub - `deundeuni / CWP-Battery-Swap`
  * GitHub - `deundeuni / CWP-Clamping-Battery-Swap-System`
* **최상위 관문:** `somamoa.ai.kr` (Canonical Gateway)
* **국제 표준 및 규격:** ISO 8501, IMO AFS Convention, EU MSFD, 각국 선급(KR, DNV, ABS) Ice Class Rules.
* **공지기술 원용:** Béla Barényi (1951), Automotive Passive Safety Architecture (Crumple Zone & Airbag).
* **법적 판례:** 대한민국 특허법 제103조, 미국 특허법 35 U.S.C. §273.
* **문서 완결성:** 본 문서는 단위 명세서로서 독자적인 기술적 완결성을 가진다.
* **원안 우선 조항:** 한국어 원문이 기준 원본(Original Authority)이며, 타 언어 번역본에서 해석 충돌 발생 시 한국어 원문의 서술과 정의를 최우선으로 적용한다.

---

## Appendix A: Inventorship
* Primary Inventor / System Architect: deundeuni (소마모아 soma-moa / github.com/soma-moa)

## Appendix B: Version History
* Version 1.0 (2026-09-03): Initial Defensive Publication Release.
* Version 1.1 (2026-09-03): CaCO3-based biogenic sacrificial layer specification & mathematical formulation.
* Version 1.2 (2026-09-03): Aero-rotor self-balancing ablation & zero-tool quick replacement integration. Mathematical parameter generalization & strict defensive terminology alignment.
* Version 1.3 (2026-09-05): Explicit inclusion of mussels, oysters, and sessile marine organism keywords for enhanced prior art searchability & generalized L1 layer definition.
* Version 1.4 (2026-09-05): Refined Founder Statement Section 0.8 with triple-defense clause.
* Version 1.5 (2026-09-05): Expanded prior art scope covering intentional, spontaneous/natural untended bio-adhesion, and synthetic CaCO3 mimetics.
* Version 1.6 (2026-09-06): Integrated cross-references to upper survival architecture (ARCHITECTURE_STRATEGY v3.2.4), APU controller (chiplet-apu-multi-system-survival-architecture v2.6), and CWP 4-Hardware mechanisms.

## Appendix C: AI Assistance Disclosure
* Draft Generation: Meta AI / Structure Optimization: Google Gemini / Final Audit: Anthropic Claude

## Appendix D: Citation Format (CITATION.cff)
```yaml
cff-version: 1.2.0
message: "If you use or reference this defensive publication framework, please cite it as below."
authors:
  - family-names: "deundeuni"
    given-names: "soma-moa"
title: "MAX-LIFE ICE-BELT: Sacrificial Self-Regenerating Armor System with Clamping Scaffold for Icebreakers, Marine Structures, and Aero-Rotors"
version: "1.6"
date-released: 2026-09-06
url: "[https://github.com/soma-moa/MAX-LIFE-ICE-BELT](https://github.com/soma-moa/MAX-LIFE-ICE-BELT)"
keywords:
  - "Defensive Publication"
  - "Prior Art"
  - "Icebreaker Armor"
  - "Bio-fouling Armor"
  - "Zero-Downtime"
  - "Ablative Cartridge"
  - "Self-balancing Ablation"
  - "Zero-tool Quick Replacement"
  - "CaCO3 Eco-Armor"
  - "Mussel Eco-Armor"
  - "Oyster Eco-Armor"
  - "Spontaneous Bio-Adhesion"
