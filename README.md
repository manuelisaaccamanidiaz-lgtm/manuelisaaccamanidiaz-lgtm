<h1 align="center">Manuel Isaac Camaño Díaz</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=1000&color=F59E0B&center=true&vCenter=true&width=640&lines=Junior+Backend+Developer;Java+%C2%B7+Spring+Boot+%C2%B7+PostgreSQL;Building+AI+agents+on+real+data;Bucaramanga%2C+Colombia" alt="Junior Backend Developer · Java · Spring Boot · PostgreSQL"/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/manuel-isaac-cama%C3%B1o-diaz-707006305/"><img src="https://img.shields.io/badge/LinkedIn-111827?style=flat-square" alt="LinkedIn"/></a>
  <a href="mailto:manuelisaaccamanidiaz@gmail.com"><img src="https://img.shields.io/badge/Email-111827?style=flat-square&logo=gmail&logoColor=F59E0B" alt="Email"/></a>
  <a href="https://manuelisaaccamanidiaz-lgtm.github.io/portafolio_profesional/"><img src="https://img.shields.io/badge/Portfolio-111827?style=flat-square&logo=githubpages&logoColor=F59E0B" alt="Portfolio"/></a>
</p>

---

**Junior Backend Developer** and **Software Development Technician** (Campuslands).
I build REST APIs with clean boundaries (hexagonal architecture, DDD), design normalized
relational databases, and develop **AI agents** that answer real questions with real data.

```java
public record Developer(String name, String role, String focus, List<String> stack, String nowBuilding) {

    public static Developer isaac() {
        return new Developer(
            "Manuel Isaac Camaño Díaz",
            "Junior Backend Developer",
            "Backend · Databases · AI agents",
            List.of("Java 21", "Spring Boot", "PostgreSQL", "Docker", "Python"),
            "Agents that help small businesses decide with data"
        );
    }
}
```

## Tech stack

| Area | Tools |
|---|---|
| **Backend** | ![Java](https://img.shields.io/badge/Java-111827?style=flat-square&logo=openjdk&logoColor=F59E0B) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-111827?style=flat-square&logo=springboot&logoColor=F59E0B) ![Maven](https://img.shields.io/badge/Maven-111827?style=flat-square&logo=apachemaven&logoColor=F59E0B) ![JWT](https://img.shields.io/badge/JWT-111827?style=flat-square&logo=jsonwebtokens&logoColor=F59E0B) |
| **Databases** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-111827?style=flat-square&logo=postgresql&logoColor=F59E0B) ![MySQL](https://img.shields.io/badge/MySQL-111827?style=flat-square&logo=mysql&logoColor=F59E0B) ![Flyway](https://img.shields.io/badge/Flyway-111827?style=flat-square&logo=flyway&logoColor=F59E0B) |
| **AI & Python** | ![Python](https://img.shields.io/badge/Python-111827?style=flat-square&logo=python&logoColor=F59E0B) ![LangChain](https://img.shields.io/badge/LangChain-111827?style=flat-square&logo=langchain&logoColor=F59E0B) ![Streamlit](https://img.shields.io/badge/Streamlit-111827?style=flat-square&logo=streamlit&logoColor=F59E0B) ![n8n](https://img.shields.io/badge/n8n-111827?style=flat-square&logo=n8n&logoColor=F59E0B) |
| **Frontend** | ![JavaScript](https://img.shields.io/badge/JavaScript-111827?style=flat-square&logo=javascript&logoColor=F59E0B) ![HTML5](https://img.shields.io/badge/HTML5-111827?style=flat-square&logo=html5&logoColor=F59E0B) ![CSS3](https://img.shields.io/badge/CSS3-111827?style=flat-square&logo=css&logoColor=F59E0B) ![React](https://img.shields.io/badge/React_%28learning%29-111827?style=flat-square&logo=react&logoColor=F59E0B) |
| **Tooling** | ![Docker](https://img.shields.io/badge/Docker-111827?style=flat-square&logo=docker&logoColor=F59E0B) ![Git](https://img.shields.io/badge/Git-111827?style=flat-square&logo=git&logoColor=F59E0B) ![Linux](https://img.shields.io/badge/Linux-111827?style=flat-square&logo=linux&logoColor=F59E0B) ![Postman](https://img.shields.io/badge/Postman-111827?style=flat-square&logo=postman&logoColor=F59E0B) |

## Featured projects

### [RentaHerramientas](https://github.com/manuelisaaccamanidiaz-lgtm/RentaHerramientas)
**Tool-rental platform connecting hardware stores with customers.** Providers publish inventory, customers book dates, pay (simulated) and download a PDF invoice.

- **Hexagonal architecture + DDD** split into Maven modules (`domain` · `application` · `infrastructure` · `bootstrap`) with bounded contexts
- **PostgreSQL normalized to 4NF**, versioned with **Flyway** migrations
- **JWT security** with three roles (admin, provider, customer)
- **Unit tests** for domain and use cases + **integration tests** against a real PostgreSQL container
- Runs with **Docker Compose** · API documented with Swagger and a Postman collection

`Java 21` `Spring Boot 4` `PostgreSQL` `Flyway` `JWT` `Docker` `JUnit`

### [Abona: AI agent for fertilizer prices](https://github.com/manuelisaaccamanidiaz-lgtm/agente_insumos)
**Helps small Colombian farmers decide when and where to buy fertilizer**, using official DANE (SIPSA) price data by municipality.

- LLM agent with **tool calling** that answers prices, buy-now-or-wait advice and order costs
- **Own evaluation suite:** 43 cases × 3 runs, **128 of 129 correct (99.2 %)**
- **Load test:** unattended run of **1,400 tasks over 12+ hours**, with a full log and report
- Cost tracked per query (≈ US$ 0.01) · [Demo video](https://youtu.be/_SfU-sRlvlQ)

`Python` `LLM tool calling` `ETL` `Streamlit` `pytest`

### [SICA: Access Control System](https://github.com/manuelisaaccamanidiaz-lgtm/proyecto_SICA)
**Replaces paper logbooks in a gated business complex** with automated check-in/out for workers and visitors.

- **Hexagonal architecture + Strategy pattern** for 4 different access flows, in plain Java (no frameworks)
- Role-based permissions (RBAC), real-time approval of unannounced visitors, **immutable audit log**
- Password hashing with jBCrypt and connection pooling with DBCP2

`Java 17` `MySQL` `JDBC` `Maven`

### [Multi-tenant SST & PESV database](https://github.com/manuelisaaccamanidiaz-lgtm/Sistema_de_gestion_SST_y_PESV)
**PostgreSQL database for occupational safety and road-safety management**, shared by many organizations.

- **Shared-schema multi-tenancy** with logical isolation by `tenant_id`
- Views and materialized views, stored procedures, functions, triggers and indexes
- Audit trail and edit locking for documents

`PostgreSQL` `PL/pgSQL` `Data modeling`

<details>
<summary><b>More projects</b></summary>
<br>

| Project | What it is | Stack |
|---|---|---|
| [Radar IA](https://github.com/manuelisaaccamanidiaz-lgtm/radar-ia) | Chatbot that records opinions about AI tools and classifies their sentiment | Python · LangChain · Gemini · Streamlit · Docker |
| [Neighborhood Tool Lending](https://github.com/manuelisaaccamanidiaz-lgtm/herramientad_del_vecindario) | CLI to manage shared tools, loans and returns, built with Git Flow | Python · JSON |
| [DeliveryBot](https://github.com/manuelisaaccamanidiaz-lgtm/DeliveryBot) | Telegram bot for internal cafeteria orders, with stock validation | n8n · Telegram · Google Sheets |
| [Pizzería Don Piccolo](https://github.com/manuelisaaccamanidiaz-lgtm/Pizzeria-don-Piccolo) | Orders, delivery and inventory database with triggers and views | MySQL |
| [Formula 1 Simulator](https://github.com/manuelisaaccamanidiaz-lgtm/proyecto_formula1) | Qualifying simulator with a real-time JavaFX race track | Java · JavaFX |
| [Portfolio](https://manuelisaaccamanidiaz-lgtm.github.io/portafolio_profesional/) | My personal portfolio website | HTML · CSS · JavaScript |

</details>

## Currently learning

**React + Vite** on the frontend, and **vector databases and embeddings** for AI agents.

---

<p align="center">
  <img src="https://raw.githubusercontent.com/manuelisaaccamanidiaz-lgtm/manuelisaaccamanidiaz-lgtm/output/github-contribution-grid-snake-dark.svg" alt="Contribution snake"/>
</p>
