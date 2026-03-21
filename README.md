<div align="center">

```
██╗   ██╗██╗███╗   ██╗ █████╗ ██╗   ██╗    ██████╗  █████╗ ████████╗██╗██╗
██║   ██║██║████╗  ██║██╔══██╗╚██╗ ██╔╝    ██╔══██╗██╔══██╗╚══██╔══╝██║██║
██║   ██║██║██╔██╗ ██║███████║ ╚████╔╝     ██████╔╝███████║   ██║   ██║██║
╚██╗ ██╔╝██║██║╚██╗██║██╔══██║  ╚██╔╝      ██╔═══╝ ██╔══██║   ██║   ██║██║
 ╚████╔╝ ██║██║ ╚████║██║  ██║   ██║       ██║     ██║  ██║   ██║   ██║███████╗
  ╚═══╝  ╚═╝╚═╝  ╚═══╝╚═╝  ╚═╝   ╚═╝       ╚═╝     ╚═╝  ╚═╝   ╚═╝   ╚═╝╚══════╝
```

[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=600&size=22&duration=3500&pause=800&color=6B57FF&center=true&vCenter=true&width=700&lines=Backend+Engineer+%7C+Java+%2F+Spring+Boot;Building+production-grade+systems+from+scratch;Auth+%7C+Security+%7C+Distributed+Infra;B.Tech+CS+%40+Bajaj+Institute+of+Technology)](https://github.com/Vinay2080)

<p align="center">
  <a href="https://github.com/Vinay2080"><img src="https://img.shields.io/badge/GitHub-Vinay2080-0D0D12?style=flat-square&logo=github&logoColor=6B57FF&labelColor=0D0D12&color=6B57FF"></a>
  <a href="https://verloren.dev"><img src="https://img.shields.io/badge/Portfolio-verloren.dev-0D0D12?style=flat-square&logo=vercel&logoColor=6B57FF&labelColor=0D0D12&color=6B57FF"></a>
  <a href="https://app.verloren.dev"><img src="https://img.shields.io/badge/Live_App-app.verloren.dev-0D0D12?style=flat-square&logo=spring&logoColor=6B57FF&labelColor=0D0D12&color=6B57FF"></a>
  <img src="https://visitor-badge.laobi.icu/badge?page_id=Vinay2080.Vinay2080" alt="visitors"/>
</p>

</div>

---

## `$ whoami`

```java
public class Vinay {

    private static final String NAME        = "Vinay Patil";
    private static final String ROLE        = "Backend Engineer (Aspiring)";
    private static final String COLLEGE     = "Bajaj Institute of Technology, Wardha";
    private static final String DEGREE      = "B.Tech Computer Science — May 2027";
    private static final String DOMAIN      = "verloren.dev";

    private static final String[] INTERESTS = {
        "Authentication & Security Systems",
        "Distributed Infrastructure",
        "API Design & Rate Limiting",
        "Observability & Load Testing"
    };

    private static final String CURRENTLY   = "Looking for Backend Engineering Internships / Entry-Level Roles";
    private static final String STACK       = "Java 21 · Spring Boot · PostgreSQL · Redis · AWS · Docker";
}
```

---

## 🛡️ Featured Project — Dragon of North

> A production-deployed authentication & security platform. Not a tutorial. Not a CRUD app. A real system.

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                         DRAGON OF NORTH — Architecture                      │
├──────────────┬──────────────────────────────┬──────────────────────────────┤
│   CLIENT     │        API LAYER             │        INFRA LAYER           │
│              │                              │                              │
│  React App   │  Spring Boot (Java 21)       │  PostgreSQL (RDS)            │
│  app.verloren│  JWT / RSA Signing           │  Redis (Rate Limiting)       │
│  .dev        │  OAuth2 Resource Server      │  AWS EC2 + SES + SNS         │
│              │  Device-Aware Sessions       │  Docker + GitHub Actions     │
│              │  OTP Verification            │  Flyway Migrations           │
│              │  Micrometer + Swagger        │  k6 Load Testing             │
└──────────────┴──────────────────────────────┴──────────────────────────────┘
```

**What it does:**
- 🔐 JWT access + refresh tokens signed with RSA-2048 — asymmetric, stateless, rotatable
- 📱 Device fingerprinting — sessions are tied to device context, not just user identity  
- 🚦 Redis-backed rate limiting — per-IP, per-user, configurable windows
- 📧 OTP email/SMS verification via AWS SES + SNS before account activation
- 🔄 Full CI/CD via GitHub Actions → EC2 with zero-downtime deploy
- 📊 Production observability with Micrometer metrics exposed to Prometheus
- 🧪 k6 load tests validating performance under concurrent auth pressure

<p align="center">
  <a href="https://github.com/Vinay2080/dragon-of-north">
    <img src="https://img.shields.io/badge/Source_Code-dragon--of--north-6B57FF?style=for-the-badge&logo=github&logoColor=white">
  </a>
  &nbsp;
  <a href="https://app.verloren.dev">
    <img src="https://img.shields.io/badge/Live_Demo-app.verloren.dev-0D0D12?style=for-the-badge&logo=spring&logoColor=6B57FF">
  </a>
  &nbsp;
  <a href="https://api.verloren.dev/swagger-ui/index.html">
    <img src="https://img.shields.io/badge/API_Docs-Swagger_UI-85EA2D?style=for-the-badge&logo=swagger&logoColor=black">
  </a>
</p>

---

## 🍽️ Restaurant Management System

A multi-module backend for full restaurant operations management.

| Module | Highlights |
|--------|-----------|
| **Auth & RBAC** | 4-tier role hierarchy — Owner → Manager → Staff → Customer |
| **Menu & Orders** | Full CRUD across 6 domain modules |
| **Payroll** | Automated salary computation, pay slip generation |
| **API Surface** | 40+ REST endpoints, fully documented |

<p align="center">
  <a href="https://github.com/Vinay2080/restaurant-management-system">
    <img src="https://img.shields.io/badge/Source_Code-restaurant--mgmt--system-6B57FF?style=for-the-badge&logo=github&logoColor=white">
  </a>
</p>

---

## 🔧 Tech Stack

| Layer | Tools |
|-------|-------|
| **Backend** | ![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white) |
| **Database** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white) |
| **Cloud / Infra** | ![AWS](https://img.shields.io/badge/AWS_EC2%2FSES%2FSNS-FF9900?style=flat-square&logo=amazonaws&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) |
| **Security** | ![JWT](https://img.shields.io/badge/JWT_/_RSA-000000?style=flat-square&logo=jsonwebtokens&logoColor=white) ![OAuth2](https://img.shields.io/badge/OAuth2-EB5424?style=flat-square&logo=auth0&logoColor=white) |
| **Observability** | ![Micrometer](https://img.shields.io/badge/Micrometer-1C4E80?style=flat-square) ![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black) ![k6](https://img.shields.io/badge/k6_Load_Testing-7D64FF?style=flat-square&logo=k6&logoColor=white) |
| **Tools** | ![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ_IDEA-000000?style=flat-square&logo=intellijidea&logoColor=white) ![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) |

---

## 📈 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Vinay2080&show_icons=true&theme=tokyonight&include_all_commits=true&hide_border=true&bg_color=0D0D12&title_color=6B57FF&icon_color=6B57FF&text_color=C9D1D9" height="165">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Vinay2080&theme=tokyonight&layout=compact&hide_border=true&bg_color=0D0D12&title_color=6B57FF&text_color=C9D1D9" height="165">
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Vinay2080&theme=tokyonight&hide_border=true&background=0D0D12&ring=6B57FF&fire=6B57FF&currStreakLabel=6B57FF">
</p>

---

## 📬 Reach Me

<p align="center">
  <a href="https://linkedin.com/in/vinay-patil-2080">
    <img src="https://img.shields.io/badge/LinkedIn-Vinay_Patil-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white">
  </a>
  &nbsp;
  <a href="mailto:vinay@verloren.dev">
    <img src="https://img.shields.io/badge/Email-vinay@verloren.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white">
  </a>
  &nbsp;
  <a href="https://verloren.dev">
    <img src="https://img.shields.io/badge/Portfolio-verloren.dev-6B57FF?style=for-the-badge&logo=vercel&logoColor=white">
  </a>
</p>

---

<div align="center">

```
// Still building. Still learning. Shipping to prod.
```

*Open to Backend Engineering Internships & Entry-Level Roles — Java / Spring Boot*

</div>
