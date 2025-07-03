# 🚀 Custom Authentication Service – **Open Contribution Repo**

<!-- Intro Narration -->

Hey there! I’m **Yatharth Kumar Saxena**, and over the last 30 days I hand-crafted a production-grade authentication service (🌟 296 commits, 4 500+ lines of handwritten code). Now I’m opening the doors so the community can push it even further.

---

## 📑 **Table of Contents**

* 📖 **Introduction** ([#-introduction](#-introduction))
* 🛠️ **What Went In** ([#-what-went-in](#-what-went-in))
* 🧩 **Current Architecture** ([#-current-architecture](#-current-architecture))
* 🗂️ **Folder Structure** ([#-folder-structure](#-folder-structure))
* 🧑‍💻 **Open Contribution Areas** ([#-open-contribution-areas](#-open-contribution-areas))
* 🤝 **How to Contribute** ([#-how-to-contribute](#-how-to-contribute))
* ⚙️ **Tech Stack & Principles** ([#-tech-stack--principles](#-tech-stack--principles))
* 🎯 **Final Takeaway** ([#-🎯-final-takeaway](#-🎯-final-takeaway))

---

## 📖 **Introduction**

This repository is **purely** for external contributions. Think of it as the public workshop where we co-create new features, squash bugs, and polish the architecture. The original solo build lives [here](https://github.com/YatharthKumarSaxena/Custom_Authentication_Service_NodeJS).

> *“System fails. Design survives.”* — **YKS**

---

## 🛠️ **What Went In**

* ⏳ **30 days** of focused backend design & development.
* ✅ **296 commits** — every thought versioned.
* 📄 **4 500+ lines** of handwritten code (*excluding Express.js boilerplate*).
* 🧠 17 APIs · JWT auth · device-aware sessions · rate limiting · single-admin model.

---

## 🧩 **Current Architecture**

**Design Principles:** SOLID · DRY · YAGNI · KISS  
**Design Patterns:** Singleton · Factory · Template Method · Strategy · Chain-of-Responsibility

High-level design (HLD) and low-level design (LLD) diagrams are documented in the `/docs` folder. The service is microservice-ready and battle-tested for scalability.

---

## 🗂️ **Folder Structure**

> Total files: **175+** (source, configs, docs, tests)

| 📁 /folder       | 🏷️ Description                  |
| ---------------- | -------------------------------- |
| `configs/`       | 🛠️ Environment & token configs  |
| `controllers/`   | 🧩 Route logic & orchestration   |
| `middlewares/`   | 🔗 Auth, role, rate-limit chains |
| `models/`        | 🗄️ Mongoose schemas             |
| `rate-limiters/` | ⏱️ Custom limiter factories      |
| `services/`      | ⚙️ Business logic abstractions   |
| `utils/`         | 🧰 Helper utilities              |
| `docs/`          | 📚 HLD & LLD diagrams            |
| `README.md`      | 🗺️ You are here!                |

Every sub-folder contains its own `README.md` with deeper details. 📝

---

## 🧑‍💻 **Open Contribution Areas**

1. **OTP Verification Workflow** 📲  
   *Goal:* After sign-up, `isActive` stays **false** until user verifies a 6-digit OTP (email/SMS).  
   Controller should **wait up to 30 s** for verification; else user re-requests OTP.  
   Clean, modular design (consider pluggable microservice vs internal API).

2. **Forgot-Password API** 🔑  
   Secure token/OTP flow → password reset.

3. **Enhanced Logging** 📈  
   Structured logs, trace IDs, winston/pino integration.

4. **Performance & Reliability** ⚡  
   Caching, graceful shutdowns, horizontal scalability ideas.

5. **Bug Fixes / Refactors** 🐞  
   Anything that boosts maintainability, reliability, or availability.

Contributions **must** align with existing HLD/LLD and follow design principles.

---

## 🤝 **How to Contribute**

1. **Fork** this repo ➜ create a feature branch.  
2. Run `npm install` & rename `.env.sample` ➜ `.env`.  
3. Write clean, commented code + unit tests.  
4. Create a PR referencing an open issue.  
5. Fill out the PR template (design rationale, test evidence).

> **Note:** First-time OSS contributors welcome! 🙌

---

## ⚙️ **Tech Stack & Principles**

* **Node.js + Express.js** (REST)  
* **MongoDB/Mongoose** (TTL indexes for cleanup)  
* **JWT** (access & refresh)  
* **Cron** jobs (log & account cleanup)  
* **Rate Limiting** (device/user aware)  
* **Testing:** Jest + Supertest  

Design mantra: *clean code, clear contracts, scalable architecture.*

---

## 🎯 **Final Takeaway**

This project started as my personal deep-dive into system design. Now it’s **our playground** to experiment, learn, and craft production-ready auth-tech together. Your smallest PR or biggest refactor — everything counts.

Looking forward to your valuable contributions! 🙏
