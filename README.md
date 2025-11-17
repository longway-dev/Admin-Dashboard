<h1 align="center">Admin Dashboard (infrastructure)</h1>

<p align="center">
  <a href="https://nextjs.org/">
    <img src="https://skillicons.dev/icons?i=nextjs" />
  </a> 
  <a href="https://www.typescriptlang.org/">
    <img src="https://skillicons.dev/icons?i=ts" />
  </a>
  <a href="https://ui.shadcn.com/">
    <img src="https://skillicons.dev/icons?i=planetscale" />
  </a>
  <a href="https://tailwindcss.com/">
    <img src="https://skillicons.dev/icons?i=tailwind" />
  </a>
</p>

Operational infrastructure simulation platform focused on:
distributed systems monitoring, cascading infrastructure failures,
service dependency management, and real-time operational recovery workflows.

Built as a production-oriented infrastructure interface inspired by:
- observability platforms
- infrastructure operations tooling
- SaaS operational control systems
- distributed service monitoring environments

> This project is intentionally designed to emphasize:
> operational systems thinking, infrastructure visibility,
> maintainable architecture, and backend-oriented engineering execution.

---


## 📚 Table of Contents

- [Features](#%EF%B8%8F-features)
- [Architecture](#-architecture)
- [Infrastructure Model](#-infrastructure-model)
- [Getting Started](#-getting-started)
- [System Simulation](#-system-simulation)
- [Available Panels](#-available-panels)
- [Screenshots](#-screenshots)

---

## ⚙️ Features

 **Distributed Infrastructure Simulation**
  - Real-time service degradation cycles
  - Cascading dependency failures
  - Operational recovery orchestration
  - Infrastructure health monitoring

- **Operational Event Feed**
  - Incident escalation tracking
  - Recovery protocol logging
  - Cascade propagation visibility
  - Infrastructure alert streams

- **Service Topology Layer**
  - Distributed infrastructure nodes
  - Service dependency relationships
  - Health propagation simulation
  - Operational status indicators

- **Recovery & Isolation Systems**
  - Recovery protocol execution
  - Infrastructure isolation actions
  - Tradeoff-based operational decisions
  - Real-time system stabilization

- **UI Stack**
  - Next.js 14 (App Router)
  - TypeScript-ready architecture
  - TailwindCSS + Shadcn/UI
  - Dark operational interface
  - Infrastructure-oriented visual hierarchy


---

## 🏗 Architecture

- **Frontend-driven operational simulation**
  - Infrastructure state managed through React state orchestration
  - Simulated service topology and dependency propagation
  - Real-time degradation/recovery cycles

- **Infrastructure-oriented structure**
  - Distributed service simulation
  - Operational event feed
  - Dependency-aware system logic
  - Recovery workflow orchestration

- **Production-inspired design direction**
  - Observability platform aesthetics
  - Enterprise operational dashboard patterns
  - Low-noise infrastructure UI
  - Backend/system-oriented interaction model

---

## 📡 Infrastructure Model

The platform simulates:
- API gateways
- telemetry systems
- infrastructure monitoring services
- control mesh systems
- distributed edge clusters
- authentication relays
- cooling/recovery infrastructure

Each service:
- maintains independent health states
- participates in dependency chains
- reacts to cascading degradation
- contributes to global infrastructure stability

Operational failures can:
- propagate through dependency networks
- degrade related services
- trigger critical infrastructure alerts
- require intervention protocols

---

## 🚀 Getting Started

```bash
# install dependencies
npm install

# start development server
npm run dev

# open local environment
http://localhost:3000   # open http://localhost:3000
```

> Make sure the Python monitoring service is running and writing JSON into ../output/ (relative to this folder), otherwise panels will show empty/placeholder data.

---

## 🔧 Configuration

### Monitoring Config Bridge

- **Main config file:** `config.yaml` (lives in the Python project root)
- The dashboard accesses and updates it through `/api/settings`:
  - Load the current config
  - Apply changes from the settings UI
  - Validate and write back to file

Any new config sections added on the monitoring side will appear as raw fields until you wire them into the settings UI.

### Theming

- TailwindCSS + Shadcn/UI
- Dark theme is enabled by default

You can:
- Extend the Shadcn theme
- Add new Tailwind utilities
- Swap layouts while keeping the same data loaders

## 🗂 Available Pages

- `/` — **Overview**  
  General health snapshot: APIs, pages, server metrics, streams summary.

- `/docker` — **Docker**  
  Containers, nodes, events from `docker_stream.json`.

- `/databases` — **Databases**  
  DB instances, alerts, test query timings, backups from `database_stream.json`.

- `/queues` — **Queues**  
  Redis / RabbitMQ availability and metrics from `queue_stream.json`.

- `/supervisor` — **Supervisor**  
  Process monitoring (status, restarts, uptime) backed by supervisor output files.

- `/settings` — **Settings**  
  `config.yaml` editor: notifications, streams, thresholds, themes, and other monitoring options.

---

## 🖼 Screenshots

![Dashboard preview](https://github.com/longway-dev/Admin-Dashboard/blob/main/screenshots/1.png) 

![Docker preview](https://github.com/longway-dev/Admin-Dashboard/blob/main/screenshots/2.png)  

![Databases preview](https://github.com/longway-dev/Admin-Dashboard/blob/main/screenshots/3.png)  

![Queues preview](https://github.com/longway-dev/Admin-Dashboard/blob/main/screenshots/4.png)


---
