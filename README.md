<div align="center">

# Ameya Mhatre

Computer Science (Data Science) student building backend and distributed systems — payment networks, service-oriented LLM pipelines, and quantitative engines.

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://ameyamhatre.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ameya-mhatre-553003307/)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:ameyam.projects@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/AmeyaMprojects)

</div>

Previously a Software Engineering Intern at Mastek Ltd., where I built evaluation pipelines for a large-scale AI retrieval service and production LLM agent pipelines in LangGraph.

---

## Stack

**Languages**
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square)

**Backend & Infra**
![Microservices](https://img.shields.io/badge/Microservices-555555?style=flat-square)
![REST APIs](https://img.shields.io/badge/REST_APIs-555555?style=flat-square)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)

**Data Stores**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

**Cloud & DevOps**
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

---

## Selected Work

### CardSwitch
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

Six-service card payments network (gateway, authorization switch, issuer simulator, tokenization vault, ledger, settlement) with BIN-based routing, retries, circuit breaking, and automatic reversals on issuer failure. Idempotent charging over a double-entry PostgreSQL ledger: zero duplicate charges across 500 concurrent retries under chaos testing, and p99 under 550 ms at 100 req/s in k6 load tests. PANs are tokenized with AES-GCM at rest; Kafka-driven settlement batches reconcile against the ledger.

[![Code](https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/AmeyaMprojects/cardswitch)

### Multi-Market Quantitative Screening Engine
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST_APIs-555555?style=flat-square)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)

Modular backend service that decouples data ingestion, computation, and presentation, so each stage scales and configures independently. One core engine is exposed through both a REST API on AWS and a CLI. A rules-and-scoring engine evaluates multi-factor signals against an adaptive, volatility-anchored risk model instead of static thresholds.

[![Live Demo](https://img.shields.io/badge/Live_Demo-00A86B?style=flat-square&logo=amazonaws&logoColor=white)](https://s501e59h91.execute-api.ap-south-1.amazonaws.com)

### NBA Trade Machine
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

Full-stack trade validator and game over a 403-player dataset: a client-side rules engine plus an Express/MongoDB REST API. When the API is down, it falls back to full local play. Validation logic (salary-matching bands, apron restrictions) is written as pure functions shared verbatim between browser and server, giving the business rules a single source of truth.

[![Live Demo](https://img.shields.io/badge/Live_Demo-00A86B?style=flat-square&logo=vercel&logoColor=white)](https://nba-contract-analyzer.vercel.app/game.html)

### Production LLM Agent Pipelines
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)

Service-oriented LangChain/LangGraph pipelines built at Mastek, including a production three-stage flow (research → draft → edit). Each component is isolated and independently testable.

---

