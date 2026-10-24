# 📡 رَصد | Rasd — CDR Investigation Platform

> **AR:** منصة تحقيق في بيانات الاتصالات (CDR): تتبّع الأحداث، ربط المكالمات والأنشطة ذات الصلة، واستخراج المؤشرات لدعم المحقق — مع ضوابط جنائية كاملة (Hashing، سلسلة الحيازة، سجل تدقيق).
>
> **EN:** A platform for investigating Call Detail Records (CDR): tracking events, linking related calls and activity, and extracting indicators for investigators — with full forensic controls (hashing, chain of custody, audit log).

👥 Team project · **My role: DFIR + Security + Reporting**

---

## 🏗️ Stack
| Layer | Tech |
|---|---|
| Backend | FastAPI |
| Databases | PostgreSQL · Neo4j (relationship graph) |
| Frontend | React · TypeScript · Vite |
| Infra | Docker Compose |

## 🔍 Features
- Records, Timeline, Evidence Map, Case Analysis, Reports
- Communication relationships & device-switching analysis
- **Forensic Bridge** — imports forensic output into the backend

## 🛡️ My Contribution (DFIR · Security · Reporting)
- Evidence acquisition & **SHA-256 hashing** + integrity check
- **Chain of custody** & **audit log**
- Authentication, roles & permissions, case-data protection
- Investigation findings & **report generation**
- Results validation

![Forensic Bridge](screenshots/forensic-bridge.png)

## 🚀 Run
```bash
docker compose -f infra/docker-compose.yml up -d   # databases
uvicorn app.main:app --reload                      # backend
npm install && npm run dev                         # frontend
```
> ✏️ Adjust paths to the repo layout.

## 📸 Screenshots
| Timeline | Evidence Map | Report |
|---|---|---|
| ![](screenshots/timeline.png) | ![](screenshots/evidence-map.png) | ![](screenshots/report.png) |

> 🔒 Uses a synthetic dataset only — no real subscriber data.

## 👩‍💻 Author
**Sahla Hassan | سهلة حسن** — DFIR / Security
[Portfolio](https://sahla-hassan.github.io) · [LinkedIn](https://linkedin.com/in/sahla-hassan)

