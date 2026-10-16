<p align="center">
  <img src="assets/banner.svg" width="100%" alt="Sergio Pino Lagos · Software Architect · Senior Backend Engineer"/>
</p>

<p align="center">
  <a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3200&pause=900&color=22D3EE&center=true&vCenter=true&width=720&lines=Arquitectura+orientada+a+eventos+con+Kafka;DDD+%2B+Hexagonal+%2B+Transactional+Outbox;Zero-Trust%2C+OpenTelemetry+y+plataformas+cloud;Agentes+de+IA+con+Model+Context+Protocol;IA+aplicada+a+NPC+en+videojuegos" alt="Typing SVG"/></a>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/sergio-pino-lagos-07b465a2/"><img src="https://img.shields.io/badge/LinkedIn-Conectemos-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <img src="https://img.shields.io/badge/Abierto_a-Arquitectura_%26_Backend-2dd4bf?style=for-the-badge" alt="Abierto a roles de arquitectura y backend"/>
  <img src="https://img.shields.io/badge/Santiago-Chile-a78bfa?style=for-the-badge" alt="Santiago, Chile"/>
</p>

<img src="assets/divider.svg" width="100%" alt=""/>

## 👨‍💻 Sobre mí

Ingeniero en Informática con más de **9 años** diseñando plataformas de alto tráfico: iGaming y pagos 24/7, y logística omnicanal para retail regional (Chile, Perú y Colombia).

Trabajo con **microservicios orientados a eventos** sobre **DDD y Arquitectura Hexagonal**, con patrones como **Transactional Outbox, CQRS y Sagas**. Me ocupo de que la plataforma sea segura (**Zero-Trust, HashiCorp Vault**), observable de extremo a extremo (**OpenTelemetry**) y operable con ayuda de agentes de IA (**Model Context Protocol, LLMs**).

```yaml
sergio:
  rol: [Software Architect, Senior Backend Engineer, Tech Lead]
  dominio: [iGaming, pagos, retail omnicanal, logística portuaria]
  patrones: [EDA, DDD, Hexagonal, CQRS, Outbox, Sagas]
  ahora: [Bodega-CV, NewLife]
  idiomas: { español: nativo, inglés: profesional }
```

<img src="assets/divider.svg" width="100%" alt=""/>

## 🚀 Proyectos actuales

<p align="center">
  <img src="assets/card-bodega.svg" width="49%" alt="Bodega-CV: plataforma de logística portuaria con 5 microservicios, Kafka, Vault y copiloto AIOps"/>
  <img src="assets/card-newlife.svg" width="49%" alt="NewLife: agentes de IA para NPC y criaturas en videojuegos, con Godot y C#"/>
</p>

<details>
<summary><b>⚓ Ver la arquitectura de eventos de Bodega-CV</b></summary>
<br/>

```mermaid
flowchart LR
    subgraph SVC["Servicios de dominio"]
        CFS["cfs-warehouse<br/>Java 21"]
        VB["vessel-berth<br/>Go"]
        YD["yard-dispatch<br/>NestJS"]
        CT["customs-tariff<br/>Ruby"]
    end
    K[("Apache Kafka<br/>CloudEvents")]
    subgraph USE["Consumo"]
        BFF["pcs-bff + consola<br/>React MF"]
        CH[("ClickHouse<br/>8 alertas")]
        AI["Copiloto AIOps<br/>MCP + LLM"]
    end
    CFS -- outbox --> K
    VB -- outbox --> K
    YD -- outbox --> K
    CT -- outbox --> K
    K --> BFF
    K --> CH
    CH -- alertas --> TG["Telegram"]
    AI -. lectura .-> BFF
    AI -. trazas .-> OT["SigNoz<br/>OpenTelemetry"]

    classDef svc fill:#083344,stroke:#22d3ee,color:#e0f2fe
    classDef bus fill:#1e1b4b,stroke:#a78bfa,color:#ede9fe
    classDef use fill:#0f172a,stroke:#2dd4bf,color:#ccfbf1
    class CFS,VB,YD,CT svc
    class K bus
    class BFF,CH,AI,TG,OT use
```

</details>

<img src="assets/divider.svg" width="100%" alt=""/>

## 🧰 Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,cs,go,py,ts,cpp,ruby&theme=dark" alt="Lenguajes"/><br/>
  <img src="https://skillicons.dev/icons?i=spring,dotnet,nestjs,fastapi,react,godot&theme=dark" alt="Frameworks"/><br/>
  <img src="https://skillicons.dev/icons?i=kafka,postgres,redis,mongodb&theme=dark" alt="Datos y eventos"/><br/>
  <img src="https://skillicons.dev/icons?i=aws,azure,gcp,kubernetes,docker,terraform,githubactions,grafana,prometheus,linux&theme=dark" alt="Cloud y plataforma"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OpenShift-EE0000?style=flat-square&logo=redhatopenshift&logoColor=white" alt="OpenShift"/>
  <img src="https://img.shields.io/badge/Kong-003459?style=flat-square&logo=kong&logoColor=white" alt="Kong"/>
  <img src="https://img.shields.io/badge/Vault-FFEC6E?style=flat-square&logo=vault&logoColor=black" alt="HashiCorp Vault"/>
  <img src="https://img.shields.io/badge/Keycloak-4D4D4D?style=flat-square&logo=keycloak&logoColor=white" alt="Keycloak"/>
  <img src="https://img.shields.io/badge/ClickHouse-FFCC01?style=flat-square&logo=clickhouse&logoColor=black" alt="ClickHouse"/>
  <img src="https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat-square&logo=opentelemetry&logoColor=white" alt="OpenTelemetry"/>
  <img src="https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white" alt="Helm"/>
  <img src="https://img.shields.io/badge/Argo_CD-EF7B4D?style=flat-square&logo=argo&logoColor=white" alt="Argo CD"/>
  <img src="https://img.shields.io/badge/Apigee_%C2%B7_MuleSoft_%C2%B7_APIM-1e293b?style=flat-square" alt="Apigee, MuleSoft, Azure APIM"/>
  <img src="https://img.shields.io/badge/MCP_%C2%B7_Dify_%C2%B7_Ollama-7c3aed?style=flat-square" alt="MCP, Dify, Ollama"/>
</p>

<img src="assets/divider.svg" width="100%" alt=""/>

## 🧭 Trayectoria

<p align="center">
  <img src="assets/timeline.svg" width="100%" alt="Falabella: Líder Técnico 2019-2020 y Arquitecto Corporativo 2021. Stratech Corp.: Arquitecto de Software 2021-2025. Hoy: Bodega-CV y NewLife."/>
</p>

<img src="assets/divider.svg" width="100%" alt=""/>

<p align="center">
  <b>¿Conversamos sobre arquitectura, eventos o agentes de IA?</b><br/>
  <a href="https://www.linkedin.com/in/sergio-pino-lagos-07b465a2/">Escríbeme por LinkedIn</a>
</p>
