# 🛡️ Blue Team Labs | Laboratorios Blue Team

**Deyvi Francisco Lora Poche** · Cybersecurity Engineering Student | Estudiante de Ingeniería en Ciberseguridad
🎯 Focus / Enfoque: Blue Team · SOC · Log & Alert Analysis

🌐 [English](#-english) | [Español](#-español)

---

## 🇬🇧 English

### About this repository
This repository documents my hands-on practice in defensive security (Blue Team). I'm working through the beginner track of **Academia SPG**, where each lab simulates a task a junior SOC analyst performs: reading logs, investigating suspicious web traffic and triaging alerts.

> 🔒 **Note:** I intentionally do not publish flags or step-by-step solutions, out of respect for the platform and other learners. This repo documents *skills and concepts*, not answers.

### ✅ Completed labs

| Lab | Track | Difficulty | Completed | Verification hash |
|---|---|---|---|---|
| **Primeros pasos #1: tu primer log** (`intro-logs-1`) | Blue Team | Basic | 2026-10-16 | `DEA7CF63898492AC` |
| **Primeros pasos #2: leyendo peticiones web** (`intro-http-1`) | Blue Team | Basic | 2026-10-16 | `8BD8F0898DB41D94` |

Certificates can be verified at **academiaspg.com/verify** using the hash above.

### 🔄 In progress
- **Primeros pasos #3: tu primera alerta** (EDR alert triage) — certificate pending.

### 🧠 What I learned

**Lab 1: Reading my first log**
- What a log is and why it's the foundation of SOC work.
- Searching and filtering log files from the command line.

**Lab 2: Reading web requests**
- Reading web server access logs: IP address, timestamp, request path, status code and user-agent.
- Using `grep` to filter by HTTP status code (e.g., separating `200` successful responses from `404` not-found).
- Spotting automated scanning: a single IP generating many requests, mostly `404`s, with a user-agent that belongs to a known scanning tool instead of a normal browser.
- Identifying the dangerous part of a scan: the few requests that returned `200`, which reveal sensitive pages that are actually exposed (such as administration panels) and need to be protected first.

**Lab 3: Triaging my first alert (in progress)**
- Reading an EDR alert as structured JSON (process, parent process, command line).
- The key question of triage: *does it make sense for this parent process to launch this child process?*
- Recognizing classic red flags, such as an Office application launching a scripting engine with hidden-window and encoded-command arguments.
- Mapping behavior to the **MITRE ATT&CK** framework (technique IDs follow the `T####.###` format) so analysts share a common language.

### 🛠️ Skills & tools
`Log analysis` · `grep` · `HTTP status codes` · `User-agent analysis` · `EDR alerts` · `JSON` · `MITRE ATT&CK` · `Triage`

### 🗺️ Next steps
- [ ] Finish the EDR alert lab and add its certificate
- [ ] Continue the Academia SPG Blue Team track
- [ ] TryHackMe SOC Level 1 path
- [ ] Practice with SIEM tools (Splunk / Wazuh)
- [ ] Combine with my cloud knowledge: [aws-cloud-learning-journey](https://github.com/DeyviLora/aws-cloud-learning-journey)

---

## 🇪🇸 Español

### Sobre este repositorio
Este repositorio documenta mi práctica en seguridad defensiva (Blue Team). Estoy avanzando en la ruta para principiantes de **Academia SPG**, donde cada laboratorio simula una tarea de un analista SOC junior: leer logs, investigar tráfico web sospechoso y clasificar alertas.

> 🔒 **Nota:** Intencionalmente **no publico flags ni soluciones paso a paso**, por respeto a la plataforma y a otros estudiantes. Este repositorio documenta *habilidades y conceptos*, no respuestas.

### ✅ Laboratorios completados

| Laboratorio | Track | Dificultad | Completado | Hash de verificación |
|---|---|---|---|---|
| **Primeros pasos #1: tu primer log** (`intro-logs-1`) | Blue Team | Básico | 2026-10-16 | `DEA7CF63898492AC` |
| **Primeros pasos #2: leyendo peticiones web** (`intro-http-1`) | Blue Team | Básico | 2026-10-16 | `8BD8F0898DB41D94` |

Los certificados se pueden verificar en **academiaspg.com/verify** con el hash indicado.

### 🔄 En progreso
- **Primeros pasos #3: tu primera alerta** (clasificación de una alerta EDR) — certificado pendiente.

### 🧠 Lo que aprendí

**Lab 1: Leyendo mi primer log**
- Qué es un log y por qué es la base del trabajo en un SOC.
- Buscar y filtrar archivos de log desde la línea de comandos.

**Lab 2: Leyendo peticiones web**
- Leer logs de acceso de un servidor web: dirección IP, fecha y hora, ruta solicitada, código de estado y user-agent.
- Usar `grep` para filtrar por código HTTP (por ejemplo, separar las respuestas `200` exitosas de los `404` de "no existe").
- Detectar un escaneo automatizado: una misma IP haciendo muchas peticiones, casi todas `404`, con un user-agent de una herramienta de escaneo conocida en lugar de un navegador normal.
- Identificar la parte peligrosa de un escaneo: las pocas peticiones que devolvieron `200`, que revelan páginas sensibles realmente expuestas (como paneles de administración) y que hay que proteger primero.

**Lab 3: Clasificando mi primera alerta (en progreso)**
- Leer una alerta de EDR en formato JSON (proceso, proceso padre, línea de comandos).
- La pregunta clave del triaje: *¿tiene sentido que este proceso padre lance a este proceso hijo?*
- Reconocer señales de alarma clásicas, como una aplicación de Office lanzando un motor de scripting con ventana oculta y comandos codificados.
- Mapear el comportamiento al marco **MITRE ATT&CK** (los IDs de técnica tienen el formato `T####.###`) para que los analistas compartan un lenguaje común.

### 🛠️ Habilidades y herramientas
`Análisis de logs` · `grep` · `Códigos HTTP` · `Análisis de user-agent` · `Alertas EDR` · `JSON` · `MITRE ATT&CK` · `Triaje`

### 🗺️ Próximos pasos
- [ ] Terminar el laboratorio de alerta EDR y agregar su certificado
- [ ] Continuar la ruta Blue Team de Academia SPG
- [ ] Ruta SOC Level 1 de TryHackMe
- [ ] Practicar con herramientas SIEM (Splunk / Wazuh)
- [ ] Combinarlo con mi base en la nube: [aws-cloud-learning-journey](https://github.com/DeyviLora/aws-cloud-learning-journey)

---

## 📎 Evidence | Evidencia
<!-- Upload the certificate images to a /certificates folder and uncomment: -->
<!-- ![intro-logs-1](certificates/intro-logs-1.png) -->
<!-- ![intro-http-1](certificates/intro-http-1.png) -->

## 📫 Contact | Contacto
- GitHub: [DeyviLora](https://github.com/DeyviLora)
- LinkedIn: _add your link / agrega tu enlace_
