<h1 align="center">Sergio Pino Lagos</h1>

<p align="center">
  <b>Software Architect · Senior Backend Engineer · Distributed Systems & Cloud</b><br/>
  Santiago, Chile · Español nativo · English (professional)
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/sergio-pino-lagos-07b465a2/"><img src="https://img.shields.io/badge/LinkedIn-sergio--pino--lagos-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <img src="https://img.shields.io/badge/Open%20to-Architecture%20%26%20Backend%20roles-2ea44f?style=flat" alt="Open to work"/>
</p>

---

### Sobre mí

Ingeniero en Informática con más de **9 años** diseñando plataformas de alto tráfico: iGaming y pagos 24/7, y logística omnicanal para retail regional (Chile, Perú y Colombia).

Trabajo con **microservicios orientados a eventos** sobre **DDD y Arquitectura Hexagonal**, con patrones transaccionales como **Transactional Outbox, CQRS y Sagas**. Me ocupo de que la plataforma sea segura (**Zero-Trust, HashiCorp Vault**), observable de extremo a extremo (**OpenTelemetry**) y operable con ayuda de agentes de IA (**Model Context Protocol, LLMs**).

- 🏗️ Hoy construyo una **plataforma de referencia de logística portuaria** con 5 servicios políglotas y un copiloto AIOps.
- 🎮 En paralelo, investigo **IA aplicada a videojuegos**: agentes que controlan NPC y criaturas en un mundo persistente.
- 💬 Me interesa hablar de arquitectura de eventos, observabilidad, plataformas internas y agentes LLM en producción.

---

### Proyectos actuales

#### ⚓ Bodega-CV: plataforma de logística portuaria (CFS)
Implementación de referencia de grado enterprise para un terminal portuario y su bodega extraportuaria (*Container Freight Station*): arribo de naves, patio de contenedores, aforo aduanero y tarificación.

- **5 microservicios políglotas** (Java 21 + Spring Boot 3.3, Go, NestJS ×2, Ruby 3.3) bajo DDD y Arquitectura Hexagonal.
- **Malla de eventos en Apache Kafka (KRaft) con CloudEvents**, cada servicio con su **Transactional Outbox** y productor idempotente, sin 2PC.
- **BFF en NestJS + consola React 18 con Module Federation** (22 suites, 255 tests).
- **Seguridad Zero-Trust:** secretos en HashiCorp Vault, contenedores non-root, Kong Gateway DB-less (GitOps) con OpenAPI 3.1.
- **Observabilidad de negocio:** OpenTelemetry + SigNoz con atributos de dominio, y analítica en ClickHouse con 8 alertas de negocio notificadas por Telegram.
- **Copiloto AIOps:** servidores MCP en Python + Dify/LLM para diagnosticar el clúster y consultar la operación en lenguaje natural.

`Java 21` `Spring Boot` `Go` `NestJS` `Ruby` `React` `Kafka` `PostgreSQL` `ClickHouse` `Vault` `Kong` `OpenTelemetry` `OpenShift` `MCP`

#### 🎮 NewLife: IA para NPC y criaturas en videojuegos
Investigación sobre agentes de IA que dan comportamiento propio a personajes no jugadores en un mundo de rol persistente.

- **Motor de decisión desacoplado:** el juego solo consulta a la IA a través de un contrato; la lógica de comportamiento vive en un servicio aparte.
- **Banco de pruebas visual en Godot (C# / .NET 8)** con Arquitectura Hexagonal, para observar y medir el comportamiento de los agentes en tiempo real.
- Hoja de ruta: cliente de pruebas primero; después, NPC y criaturas controlados por el servicio de IA.

`C#` `.NET 8` `Godot` `IA aplicada` `Arquitectura Hexagonal`

---

### Stack

- **Lenguajes:** Java · C# · Go · Python · TypeScript · C/C++
- **Backend:** Spring Boot · .NET · NestJS · FastAPI · gRPC/Protobuf · OpenAPI 3.1
- **Eventos y datos:** Apache Kafka · Azure Service Bus · GCP Pub/Sub · PostgreSQL · Redis · ClickHouse · MongoDB · BigQuery
- **Cloud y plataforma:** AWS · Azure · GCP · Kubernetes · OpenShift · Docker · Terraform · Helm · ArgoCD
- **API Gateways:** Kong · Apigee · MuleSoft · Azure APIM
- **Seguridad:** HashiCorp Vault · Keycloak · Auth0 · OAuth2/OIDC
- **Observabilidad:** OpenTelemetry · SigNoz · Grafana Stack · ELK · Datadog
- **IA:** Model Context Protocol (MCP) · Dify · Ollama · agentes LLM

---

### Experiencia

| Empresa | Rol | Período |
|:--|:--|:--|
| **Stratech Corp.** | Arquitecto de Software / Senior Developer (iGaming y pagos) | 2021 – 2025 |
| **Falabella Sistemas Corporativos** | Arquitecto Corporativo (mensajería empresarial multicloud) | 2021 |
| **Falabella Sistemas Corporativos** | Líder Técnico (Click & Collect: Chile, Perú y Colombia) | 2019 – 2020 |

---

<p align="center"><i>¿Conversamos? Escríbeme por <a href="https://www.linkedin.com/in/sergio-pino-lagos-07b465a2/">LinkedIn</a>.</i></p>
