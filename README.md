## 👋 Hi, I'm **Sanguk Park**  
Industrial Software Engineer | SCADA/HMI Expert | .NET Architect

I specialize in **modernizing large-scale legacy systems** and building  
**high-performance industrial automation platforms (SCADA/HMI)**.

Over the past years, I’ve worked on transforming a massive WinForms/.NET 3.5/ASMX-based system  
into a modern architecture using **.NET 4.8, .NET 8, .NET 9, Web API, Avalonia UI, MAUI, WASM, and PostgreSQL**.

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
- C# (7.3 ~ 11), .NET Framework 3.5 ~ 4.8, .NET 6/7/8/9
- SQL (PostgreSQL, MariaDB, MySQL), C/C++(MFC), Python(For tool making)
- JavaScript, HTML, CSS

### **Back-end**
- ASP.NET Web API  
- WCF, ASMX(SOAP), TCP Socket  
- Entity Framework, Npgsql  
- Serilog, JWT, OAuth  

### **Front-end / Desktop**
- WinForms  
- Avalonia UI  
- MAUI (Android, iOS)
- OpenSilver (WASM)  
- Blazor Hybrid  

### **Database**
- PostgreSQL / TimescaleDB  
- Hypertables, Compression, Retention  
- Trend/Log Engine Architecture Design

### **DevOps / Infra**
- IIS, Kestrel  
- Ubuntu/Debian Linux  
- Systemd, Shell Script  
- Azure DevOps  
- NSIS Installer  

### **Embedded & Industrial**
- RK3568 Linux Boards  
- Windows CE  
- PLC(MELSEC, Modbus), Serial/TCP Communication 

---

## 🚀 **Major Project: SCADA/HMI Platform Modernization**

**Large-scale Automation Platform Upgrade (Autobase)**  
📅 2023 ~ Present  
⚙ C#, .NET 4.8 + .NET 8, Web API, WCF, PostgreSQL/TimescaleDB, Avalonia UI

### 🔧 Highlights
- 🧩 **ASMX → WCF → Web API Building a phased migration structure**
  - Remove SOAP-based ArrayOfString → Design API based purely on JSON
  - BasicHttpBinding deadlock fix
  - Introduction of dynamic EndpointAddress pattern
  - 
- ⚡ **Real-time tag processing performance improvement**
  - Async/await-based parallel optimization  
  - Solving ThreadPool starvation  
  - Improved processing speed for 1,000–100,000 tags 

- 🗄 **Trend/Log Big Data Engine Redesign**
  - Complete migration from file-based to PostgreSQL/TimescaleDB
  - Establishment of Hypertable, Chunk, Compression, and Retention policies
  - Completed a structure capable of operating for 10 years

- 🖥 **Cross-platform HMI UI Construction**
  - WinForms → Avalonia UI Architecture Design 
  - Development of a web HMI prototype based on OpenSilver (WASM)
  - Building a runtime multilingual (ko/en/zh/ja/vi) switching system

- 🔐 **License/Session/Heartbeat Architecture Design**
 - KeyLock-based authentication
 - GUID heartbeat + simultaneous login restriction
 - 10-minute trial mode implementation

- 🐞 **Solve complex deadlock/timeout issues**
 - Resolved the issue where `await db.OpenAsync()` would stop by overriding WCF timeout
 - Fixed System.Memory version conflicts
 - Checked IIS concurrency issues and stabilized

---

## 🧠 Advanced Troubleshooting & Architecture-Level Problem Solving

### ⚙️ 1. Legacy Service Layer Modernization Without Downtime
Refactored a monolithic ASMX/WCF service stack into a hybrid Web API architecture  
while maintaining full backward compatibility with thousands of deployed clients.

- Reverse-engineered SOAP contract behaviors to create drop-in REST replacements.
- Designed a multi-endpoint routing layer allowing ASMX, WCF, and Web API to coexist.
- Implemented dynamic endpoint injection to migrate clients without redeployment.
- Eliminated all `ArrayOfString`/XML serializer legacy types and normalized transport models.

### 🔄 2. Resolving SynchronizationContext Deadlocks in IIS + WCF Async Pipelines
Identified and eliminated a rare deadlock caused by ASP.NET’s SynchronizationContext  
when WCF proxies were invoked with `async/await` under certain thread starvation conditions.

- Mapped the exact interaction between BasicHttpBinding, IIS request threads,  
  and WCF's channel factory lifecycle.
- Rewrote the binding initialization pipeline to avoid channel recreation on every call.
- Introduced a custom WCF client factory with connection pooling & Timeout override.
- Result: **100% elimination of deadlocks and 40% lower response latency.**

### 🧵 3. High-Throughput Multi-Thread Engine Refactor (10k+ Tags/sec)
Optimized a real-time SCADA tag-processing engine responsible for ingesting  
over 10,000+ analog/digital samples per second.

- Converted synchronous blocking loops to an async streaming pipeline.
- Batched disk I/O and DB writes using lock-free queues.
- Removed GC pressure hot spots (large object heap & string allocations).
- Profiling via dotMemory, built custom allocation map.
- Result: **3× throughput, 70% fewer context switches, stable under 24h burn tests.**

### 🗄 4. Trend/Log Engine Modernization: File → TimescaleDB
Redesigned a 20-year-old file-based trend/log subsystem to a fully  
time-series optimized backend powered by PostgreSQL + TimescaleDB.

- Modeled hypertables for minute/hour/day/month rollups.
- Built compression/retention pipelines reducing storage by 97%.
- Eliminated month-file fragmentation & CRC-based recovery logic.
- Wrote a compatibility layer to read legacy data without downtime.
- Result: **multi-year retention with <5ms average query latency.**

### 🌐 5. Cross-Platform Rendering Engine Migration (WinForms → Avalonia/WASM)
Ported a massive WinForms HMI visualization layer to a modern UI stack.

- Implemented a cross-platform graphics abstraction (Skia/Avalonia).
- Unified drawing primitives, event model, and real-time rendering loop.
- Reduced GDI+/Win32 dependency footprint by >90%.
- Enabled WASM-based Web HMI using OpenSilver without rewriting core logic.

### 🧩 6. Reverse Engineering Proprietary Industrial Protocols
Analyzed and re-implemented proprietary PLC communication behaviors  
(MELSEC ENET 3E, Modbus variations, custom OEM protocols).

- Built a binary frame parser with extensible opcodes.
- Reproduced undocumented timing constraints and reconnection sequences.
- Added error-correcting logic to handle PLC-side quirks.
- Result: drop-in interoperability even with legacy hardware.

### 🔐 7. Enterprise Licensing & Session Consistency Under Load
Re-architected a multi-tier license enforcement system that spans:

- Hardware dongles, machine identifiers, concurrent-session limits,
- Heartbeat with GUID session tracking,
- Grace periods & fallback trial logic,
- Secure AES/SHA hashing pipeline to prevent tampering.

Designed to operate reliably across Windows, Linux, embedded devices.

### 💾 8. Memory Pressure Mitigation in Long-Running Real-Time Systems
Diagnosed and mitigated memory fragmentation issues in a 24/7 SCADA runtime.

- Replaced large contiguous buffers with pooled segmented structures.
- Eliminated 1.9GB LOH allocations (ReSharper DPA warnings).
- Tuned interval timers, throttled high-frequency tasks.
- Introduced memory watermark alerts + graceful load shedding.

### 📡 9. Embedded Linux Deployment Optimization (RK3568)
Migrated system components to RK3568 boards:

- Tuned kernel parameters for low-latency GPIO/ADC/DIO access.
- Implemented custom C# interop for hardware drivers via P/Invoke.
- Designed systemd units for stable auto-start + watchdog recovery.

### 📦 10. Multi-Language Runtime Switching (ko/en/zh/ja/vi)
Created a robust runtime language-switching framework:

- Eliminated WinForms static resource binding errors.
- Centralized CultureInfo initialization via middleware.
- Fully dynamic UI refresh without application restarts.
---

## 📚 **Interests**
- Cross-platform UI Architecture  
- Real-time Data Processing  
- Embedded + Cloud Industrial Systems  
- .NET Runtime, WASM  
- Modernizing legacy codebases  

---

## 📫 Contact
**Email:** *sanguke3@gmail.com*  
**GitHub:** https://github.com/StitchWoogie 
**LinkedIn:** *_*

---

_If you're working on complex legacy modernization, SCADA/HMI platforms,  
or high-performance .NET systems, feel free to reach out!_
