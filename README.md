## 👋 Hi, I'm **Sanguk Park**  
Industrial Software Engineer | SCADA/HMI Expert | .NET Architect

I specialize in **modernizing large-scale legacy systems** and building  
**high-performance industrial automation platforms (SCADA/HMI)**.

Over the past years, I’ve worked on transforming a massive WinForms/.NET 3.5/ASMX-based system  
into a modern architecture using **.NET 4.8, .NET 8, Web API, Avalonia UI, MAUI, WASM, and PostgreSQL**.

I love deep-diving into complex systems, solving root problems,  
and designing architectures that last for years.

---

## 🧩 **What I Do**
- ⚡ Modernization of legacy systems (ASMX → WCF → Web API)
- ⚙ Building high-performance SCADA/HMI engines  
- 🗄 Trend/Log big-data optimization (TimescaleDB + PostgreSQL)
- 🖥 Cross-platform UI development (WinForms → Avalonia/Maui/OpenSilver)
- 🔐 License · Session · Heartbeat back-end architecture
- 🧵 Deadlock-free async/await + multi-thread processing  
- 🛠 Embedded device integration (RK3568, Linux, Windows CE)

---

## 🛠 **Tech Stack**

### **Languages**
- C# (7.3 ~ 11), .NET Framework 3.5 ~ 4.8, .NET 6/7/8
- SQL (PostgreSQL, MariaDB), C/C++(MFC), Python(툴 제작용)

### **Back-end**
- ASP.NET Web API  
- WCF, ASMX(SOAP), TCP Socket  
- Entity Framework, Npgsql  
- Serilog, JWT, OAuth  

### **Front-end / Desktop**
- WinForms  
- Avalonia UI  
- MAUI  
- OpenSilver (WASM)  
- Blazor Hybrid  

### **Database**
- PostgreSQL / TimescaleDB  
- Hypertables, Compression, Retention  
- Trend/Log 엔진 구조 설계  

### **DevOps / Infra**
- IIS, Kestrel  
- Ubuntu/Debian Linux  
- Systemd, Shell Script  
- Azure DevOps  
- NSIS Installer  

### **Embedded & Industrial**
- RK3568 Linux Boards  
- Windows CE  
- PLC(MELSEC, Modbus), Serial/TCP 통신  

---

## 🚀 **Major Project: SCADA/HMI Platform Modernization**

**Large-scale Automation Platform Upgrade (Autobase)**  
📅 2023 ~ Present  
⚙ C#, .NET 4.8 + .NET 8, Web API, WCF, PostgreSQL/TimescaleDB, Avalonia UI

### 🔧 Highlights
- 🧩 **ASMX → WCF → Web API 단계적 마이그레이션 구조 구축**
  - SOAP 기반 ArrayOfString 제거 → 순수 JSON 기반 API 설계
  - BasicHttpBinding deadlock 문제 해결
  - 동적 EndpointAddress 패턴 도입

- ⚡ **실시간 태그 처리 성능 개선**
  - async/await 기반 병렬 최적화  
  - ThreadPool starvation 해결  
  - 1,000~10,000 태그 처리 속도 향상  

- 🗄 **Trend/Log 빅데이터 엔진 재설계**
  - 파일 기반 → PostgreSQL/TimescaleDB로 완전 전환  
  - Hypertable, Chunk, Compression, Retention 정책 수립  
  - 10년 규모 운영 가능한 구조 완성  

- 🖥 **Cross-platform HMI UI 구축**
  - WinForms → Avalonia UI 구조 설계  
  - OpenSilver(WASM) 기반 웹 HMI 프로토타입 제작  
  - 런타임 다국어(ko/en/zh/ja/vi) 전환 시스템 구축  

- 🔐 **License/Session/Heartbeat 구조 설계**
  - KeyLock 기반 인증  
  - GUID Heartbeat + 동시 로그인 제한  
  - 10분 Trial 모드 구현  

- 🐞 **복잡한 Deadlock/Timeout 문제 해결**
  - WCF Timeout 재정의해 `await db.OpenAsync()` 멈춤 문제 해결  
  - System.Memory 버전 충돌 해결  
  - IIS 동시성 문제 점검 및 안정화  

---

## 🧪 **Problem Solving Examples**

### 🔥 WCF SendTimeout Deadlock Fix  
`await db.OpenAsync()`가 IIS에서 멈추던 문제를  
BasicHttpBinding 재할당 + Timeout 재설정으로 해결.

### 🧼 ASMX ArrayOfString 제거  
ASMX 자동 생성 타입을 제거하고  
string[] 기반 JSON API로 정규화.

### 🌐 다국어 시스템 초기화 문제 해결  
DefaultThreadCurrentUICulture를  
BeginRequest 및 Program.cs 초기화 로직으로 정리.

### 🔌 Npgsql 및 System.Memory 충돌 해결  
패키지 버전 불일치 추적 → Web.config assemblyBinding 재정의.

---

## 📚 **Interests**
- Cross-platform UI Architecture  
- Real-time Data Processing  
- Embedded + Cloud Industrial Systems  
- .NET Runtime, WASM  
- Modernizing legacy codebases  

---

## 📫 Contact
**Email:** *(원하면 이 부분 추가해줘)*  
**GitHub:** https://github.com/your-id  
**LinkedIn:** *(원하면 만들어줄게)*

---

_If you're working on complex legacy modernization, SCADA/HMI platforms,  
or high-performance .NET systems, feel free to reach out!_
