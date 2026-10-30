<div align="center">

# Vinay Patil
### Backend Software Engineer · Scalable Systems, Security & Developer Tooling

[![Live Application](https://img.shields.io/badge/Live_App-app.verloren.dev-6B57FF?style=flat-square&logo=googlechrome&logoColor=white)](https://app.verloren.dev)
[![API Documentation](https://img.shields.io/badge/API_Docs-Swagger_UI-85EA2D?style=flat-square&logo=swagger&logoColor=black)](https://api.verloren.dev/swagger-ui/index.html)
[![Java 21](https://img.shields.io/badge/Java-21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](https://openjdk.org/)
[![Spring Boot 3](https://img.shields.io/badge/Spring_Boot-3.x-6DB33F?style=flat-square&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Status](https://img.shields.io/badge/Status-Open_to_Opportunities-brightgreen?style=flat-square)](#-connect)

</div>

---

### 💡 Engineering Philosophy

I design and build **production-oriented backend systems and developer tooling** engineered around real failure modes: refresh-token replay, session hijacking, distributed brute-force pressure, and compiler/AST tooling constraints.

* 🔐 **Security & IAM:** Moving beyond standard CRUD — implementing stateless JWT authorization paired with authoritative server-side session liveness, asymmetric RSA cryptography, and AES-GCM encrypted MFA secrets.
* 🛠️ **Developer Tooling & Compilers:** Authoring IDE language support, lexers, BNF grammars, and AST inspectors for domain-specific languages on the JetBrains IntelliJ Platform.
* 📈 **Reliability & Telemetry:** Validated via automated k6 concurrent load scenarios, containerized CI/CD pipelines, and Prometheus observability.

---

### 🚀 Highlighted Systems & Tooling

#### 1. [Dragon of North](https://github.com/Vinay2080/dragon-of-north) — Production IAM & Authentication Platform
*A production-deployed Identity & Access Management system combining stateless JWT efficiency with authoritative server-side session control.*

```
[ Client Request ] 
        │
        ▼
[ RateLimitFilter ] ──────────► Redis Token Bucket (Per-IP / Per-User sliding window)
        │
        ▼
[ Spring Security Filter ] ───► CORS, CSRF synchronization, exception handling
        │
        ▼
[ JwtFilter ] ────────────────► RSA-2048 asymmetric signature verification
        │
        ▼
[ SidLivenessFilter ] ────────► Session state verification (ALL_AUTH / MFA_ONLY / SENSITIVE_ONLY)
        │
        ▼
[ Controller & Services ] ────► PostgreSQL (Auth state) + Redis (MFA challenges, OTP state)
                                └─► AWS SES / SNS (Verification dispatch)
```

* **Asymmetric Token Security:** RSA-2048 signed access tokens with refresh token rotation and automated replay attack invalidation.
* **Authoritative Session Liveness:** Granular `SidLivenessFilter` balancing database lookup overhead against token revocation guarantees.
* **MFA & Step-Up Security:** TOTP setup with AES-GCM encrypted secret persistence, one-time recovery codes, and `@RequireRecentMfa` interceptors for sensitive account operations.
* **Abuse Resistance:** Redis-backed distributed rate limiting via Bucket4j across authentication and OTP endpoints.
* **Infrastructure & Testing:** Docker multi-stage containers, Flyway migrations, AWS EC2 hosting, Prometheus telemetry, and k6 concurrency validation.
* **Links:** [Source Code](https://github.com/Vinay2080/dragon-of-north) · [Live App](https://app.verloren.dev) · [Swagger UI](https://api.verloren.dev/swagger-ui/index.html)

---

#### 2. [Midnight Compact Plugin](https://github.com/Vinay2080/midnight-compact-plugin) — JetBrains IntelliJ Platform Tooling
*Industrial-grade IDE language support for Compact, the smart contract domain-specific language for the Midnight zero-knowledge blockchain.*

* **Lexical Analysis & Parsing:** Custom lexer compiled via JFlex and grammar parser generated with GrammarKit BNF.
* **Program Structure Interface (PSI):** Real-time mapping of language tokens to JetBrains AST/PSI elements for structured syntax trees.
* **Developer Experience:** Syntax highlighting, code folding, bracket matching, identifier navigation, and custom static code inspections.
* **Toolchain & Quality:** Automated builds using Gradle IntelliJ Plugin (`build.gradle.kts`), verified against JetBrains Checkstyle and Qodana static analysis in GitHub Actions.
* **Links:** [Source Code](https://github.com/Vinay2080/midnight-compact-plugin)

---

### 📦 Additional Engineering Projects

| Project | Focus | Architecture & Stack |
| :--- | :--- | :--- |
| **[project-restaurant](https://github.com/Vinay2080/project-restaurant)** | Enterprise Backend & RBAC | • Spring Boot with asymmetric RSA-signed JWTs<br>• 4-tier method-level authorization (`@PreAuthorize`)<br>• PostgreSQL schema for payroll, staff, and table reservation flows |
| **[robe-of-feathers](https://github.com/Vinay2080/robe-of-feathers)** | Cloud Infrastructure as Code | • Declarative provisioning of serverless backend workloads<br>• Automated cloud resource lifecycle with Terraform |
| **[fox-sister](https://github.com/Vinay2080/fox-sister)** | Decoupled 3-Tier Architecture | • Decoupled multi-cloud setup: Netlify (React SPA) + Render (Node.js API) + MongoDB Atlas (TLS DB)<br>• Monorepo management with health monitoring and architecture status displays |

---

### 🛠️ Technical Stack & Tooling

| Layer | Technologies |
| :--- | :--- |
| **Languages** | ![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white) |
| **Frameworks & Core** | ![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white) ![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=flat-square&logo=spring&logoColor=white) ![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white) |
| **Databases & Cache** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white) |
| **Cloud & DevOps** | ![AWS EC2](https://img.shields.io/badge/AWS_EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white) ![AWS SES](https://img.shields.io/badge/AWS_SES-FF9900?style=flat-square&logo=amazonsimpleemailservice&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) |
| **Testing & Tooling** | ![k6](https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white) ![JUnit 5](https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white) ![Mockito](https://img.shields.io/badge/Mockito-C53435?style=flat-square) ![IntelliJ Platform SDK](https://img.shields.io/badge/IntelliJ_SDK-000000?style=flat-square&logo=intellijidea&logoColor=white) |

---

### 📊 GitHub Activity & Telemetry

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Vinay2080&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D0D12&title_color=6B57FF&icon_color=6B57FF&text_color=C9D1D9" height="155" alt="GitHub Stats" />
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Vinay2080&theme=tokyonight&layout=compact&hide_border=true&bg_color=0D0D12&title_color=6B57FF&text_color=C9D1D9" height="155" alt="Top Languages" />
</p>

---

### 📫 Connect

<p align="left">
  <a href="mailto:shaking.121@gmail.com">
    <img src="https://img.shields.io/badge/Email-shaking.121%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://linkedin.com/in/vinay-patil" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Vinay_Patil-0A66C2?style=flat-square&logo=linkedin&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://github.com/Vinay2080">
    <img src="https://img.shields.io/badge/GitHub-Vinay2080-181717?style=flat-square&logo=github&logoColor=white" />
  </a>
</p>

<div align="center">
<sub>B.Tech Computer Science · Bajaj Institute of Technology, Wardha (Class of 2027)</sub>
</div>
