<div align="center">

<img src="assets/favicon.svg" width="80" height="80" alt="SmartCare logo">

# SmartCare — Presentazione (GitHub Page)

### Sistema IoT real-time per il monitoraggio closed-loop di pazienti con scompenso cardiaco

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-live-2ee6b0?logo=github&logoColor=white)](#)
[![HTML5](https://img.shields.io/badge/HTML5-e34c26?logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](#)

</div>

---

## Indice

- [Panoramica del progetto](#panoramica-del-progetto)
- [Architettura del sistema](#architettura-del-sistema)
- [Repository collegati](#repository-collegati)
- [Questo repository: sito di presentazione](#questo-repository-sito-di-presentazione)
- [Sviluppo locale](#sviluppo-locale)
- [Pubblicazione su GitHub Pages](#pubblicazione-su-github-pages)
- [Contesto accademico](#contesto-accademico)

---

## Panoramica del progetto

**SmartCare** è un sistema IoT end-to-end per il monitoraggio in tempo reale di pazienti affetti da **insufficienza cardiaca congestizia**. Il sistema acquisisce segnali fisiologici (ECG, postura tramite IMU a 6 assi, temperatura corporea) da un dispositivo wearable, li classifica tramite modelli di Machine Learning per rilevare anomalie cliniche, e mette in comunicazione diretta **paziente** e **medico** attraverso un'architettura event-driven basata su MQTT, con persistenza su database e validazione clinica delle anomalie rilevate.

> 🩺 **Closed-loop**: ogni anomalia rilevata automaticamente viene validata da un medico (vero positivo / falso allarme); queste validazioni rientrano nel dataset di addestramento per ri-calibrare periodicamente il classificatore ECG, chiudendo il ciclo tra IA e giudizio clinico.

---

## Architettura del sistema

> Lo schema completo — dal dongle nRF52840 al broker MQTT, ai due rami di elaborazione (classificazione + persistenza) e presentazione (dashboard) — è illustrato interattivamente nella sezione **Architettura** della pagina pubblicata da questo repository (vedi [`index.html`](index.html)).

Questo repository **non contiene codice applicativo**: è la vetrina statica dell'intero sistema, pensata per essere consultata anche da chi non ha accesso ai repository privati del progetto (es. aziende, valutatori esterni).

---

## Repository collegati

| Repository | Contenuto
|---|---
| **[SmartCare — Backend](https://github.com/UniSalento-IDALab-IoTCourse-2025-2026/wot-project-2025-2026-backend-giuri)** | Backend: classificazione ML, API REST, persistenza, broker MQTT, notifiche
| **[smartcare-dashboard](https://github.com/UniSalento-IDALab-IoTCourse-2025-2026/wot-project-2025-2026-dashboard-giuri)** | Dashboard medico in React (Vite)
| **[IIT BioDataAcq](https://github.com/UniSalento-IDALab-IoTCourse-2025-2026/wot-project-2025-2026-patient-app-giuri)** | App Kivy di acquisizione + layer di integrazione MQTT
| **[wot-project-2025-2026-presentation-giuri](.)** *(questo repo)* | Sito di presentazione (GitHub Page)

---

## Questo repository: sito di presentazione

Sito statico **single-page** (`index.html`), HTML/CSS/JS in un unico file, senza framework né build step. Sezioni incluse:

| Sezione | Contenuto |
|---|---|
| **Hero** | Presentazione sintetica del progetto |
| **Il progetto** | Contesto clinico, obiettivi, principio closed-loop |
| **Architettura** | Diagramma SVG del sistema end-to-end |
| **Stack tecnologico** | Le tecnologie usate e perché |
| **Dimostrazione** | Video/screenshot del sistema in funzione |
| **Repository** | Link ai tre repository del progetto |

## 🔗 Demo online

**[Vedi il sito → unisalento-idalab-iotcourse-2025-2026.github.io/wot-project-2025-2026-presentation-giuri](https://unisalento-idalab-iotcourse-2025-2026.github.io/wot-project-2025-2026-presentation-giuri/)**

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-live-2ee6b0?style=flat-square&logo=github)](https://unisalento-idalab-iotcourse-2025-2026.github.io/wot-project-2025-2026-presentation-giuri/)

## Contesto accademico

Sito di presentazione realizzato per l'esame di Internet of Things presso l'Università del Salento, in collaborazione con:

- **IDA Lab** - Università del Salento
- **IIT — Istituto Italiano di Tecnologia**

Per la descrizione tecnica completa del sistema, fare riferimento al README del repository **[backend](https://github.com/UniSalento-IDALab-IoTCourse-2025-2026/wot-project-2025-2026-backend-giuri)** e alla relazione di progetto consegnata per l'esame.

---

<div align="center">

Realizzato da **Francesco Giuri** — Università del Salento

</div>
