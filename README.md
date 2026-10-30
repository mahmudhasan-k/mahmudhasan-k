# Hi there, I'm Mahmud Hasan 👋

### **Applied AI & Reinforcement Learning Builder · Full-Stack LLM Systems · Dynamic Process Control**

[![Live App - gochalo.vercel.app](https://img.shields.io/badge/Live_App-gochalo.vercel.app-009688?style=for-the-badge&logo=vercel&logoColor=white)](https://gochalo.vercel.app/)
[![GitHub Repo - Gochalo](https://img.shields.io/badge/GitHub_Repo-Gochalo_(গোছালো)-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mahmudhasan-k/gochalo)
[![LinkedIn - Mahmud Hasan](https://img.shields.io/badge/LinkedIn-mahmudhasan--k-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mahmudhasan-k/)
[![Email - Contact Me](https://img.shields.io/badge/Email-Outlook-0078D4?style=for-the-badge&logo=microsoft-outlook&logoColor=white)](mailto:hello@mahmudhasan@outlook.com)

---

## ⚡ About Me

I build **reliable, production-grade AI systems** and train **Reinforcement Learning (RL) controllers** for complex dynamical environments. Rather than shipping fragile demos, I focus on systems that hold up under real-world constraints—whether that means deterministic verification gates for Large Language Models or constraint-aware policy optimization for continuous process control.

* 🧠 **Reinforcement Learning & Control:** Designing and tuning deep RL policies (**PPO, SAC, TD3, DDPG, DQN**) for continuous-state dynamical systems using **Gymnasium**, **PC-Gym**, **Stable-Baselines3**, and **PyTorch**.
* 🛠️ **Production LLM Engineering:** Creator of [**Gochalo (গোছালো)**](https://gochalo.vercel.app/) ([Source Code](https://github.com/mahmudhasan-k/gochalo)), a bilingual (English + বাংলা) procedural intelligence workspace that transforms messy notices, flyers, links, and questions into verified, interactive action plans.
* 🔬 **Core Engineering Philosophy:** High test coverage ($630+$ automated checks), strict schema contracts, graceful degradation under API faults, and smooth human-centered interfaces.

---

## 🧰 Technical Arsenal

![Python 3.12](https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-React_19-3178C6?style=flat-square&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688?style=flat-square&logo=fastapi&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-Structured_AI-4285F4?style=flat-square&logo=google&logoColor=white)
![PyTorch & RL](https://img.shields.io/badge/RL-Gymnasium_%7C_SB3_%7C_PC--Gym-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL_%2B_RLS-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Render_%26_Vercel-2496ED?style=flat-square&logo=docker&logoColor=white)

### 🤖 Reinforcement Learning & Process Control

* **Policy Gradient & Actor-Critic Methods:** Proximal Policy Optimization (**PPO**), Soft Actor-Critic (**SAC**), Twin Delayed DDPG (**TD3**), Advantage Actor-Critic (**A2C**), Deep Q-Networks (**DQN**).
* **Continuous Dynamical Control:** Setpoint tracking across multi-step trajectories, actuator smoothness & control-effort regularization ($\Delta u$ minimization), hard/soft operational constraint satisfaction, and non-stationary disturbance rejection.
* **Environment & Training Engineering:** Custom `Gymnasium` / `PC-Gym` wrappers, observation & reward normalization (`VecNormalize`), action-space scaling, frame/history stacking for partial observability, and hyperparameter optimization with **Optuna**.

### 🌐 Full-Stack AI & Cloud Engineering

* **LLM & Extraction Pipelines:** `google-genai` SDK, constrained JSON schema compilation, quote-first source verification, multi-key quota/transient failover (`429`/`503`), OCR vision pipelines, and SSRF-guarded Jina web extraction.
* **Frontend & Local-First Storage:** React 19, Vite, TypeScript, local-first **IndexedDB** workspaces, **Clerk** Google OAuth, and **Supabase PostgreSQL** with Row-Level Security (RLS).
* **Testing & Verification:** `pytest`, `Vitest`, React Testing Library, `PGlite` database contract testing, and mocked transport verification.

---

## 🚀 Flagship Production Project

### [Gochalo · গোছালো — Bilingual AI Action-Planning Workspace](https://gochalo.vercel.app/)

🔗 **Live App:** [https://gochalo.vercel.app/](https://gochalo.vercel.app/) · 💻 **GitHub Repository:** [https://github.com/mahmudhasan-k/gochalo](https://github.com/mahmudhasan-k/gochalo)

> *A little order for everyday life. Turn questions, notices, photos, and public links into structured, verifiable next steps in English or বাংলা.*

Real-world circulars, visa procedures, scholarship announcements, and government notices bury critical dates, fees, and document rules inside dense paragraphs or image flyers. **Gochalo** converts unstructured inputs into a deterministic **6-category execution workspace** (**Overview, Actionable Steps, Deadlines, Fees, Required Documents, and Others/Contradictions**).

* **Multi-Modal Input Engine:** Supports direct procedural Q&A (*Ask & Plan*), **Gemini Vision** notice OCR (`PNG`/`JPEG`), guarded **Jina Reader** public URL extraction, and raw text analysis.
* **Two-Layer Verification & Graceful Degradation:** Combines local deterministic checks (verbatim quotation matching, numeric fidelity, and scope verification) with an independent semantic review pass and resilient fallback (`deterministic_review_fallback`).
* **Built for Execution:** Interactive checklists with progress tracking, custom personal task injection, `.ics` calendar export anchored to `Asia/Dhaka`, print/copy views, and offline-capable **IndexedDB** storage with optional **Clerk + Supabase** cloud sync.
* **Battle-Tested Codebase:** Backed by **$470+$ backend `pytest` checks (plus $405$ subtests)** and **$160+$ frontend `Vitest` tests**, deployed across **Vercel** and **Render**.

---

## 🧪 Current Research & Engineering Focus

### Autonomous Process Control via Deep Reinforcement Learning (`PC-Gym` / `Gymnasium`)

Currently developing and benchmarking sample-efficient RL controllers for nonlinear, multivariable chemical and dynamical process systems (preparing for the **ICChE 2026 PC-Gym Reinforcement Learning Control Challenge**):

| Optimization Objective | Engineering Approach |
| :--- | :--- |
| **Setpoint Tracking ($30\%$)** | Designing dense history-augmented state representations ($s_t, e_t = y_{\text{sp}} - y_t$) with off-policy (**SAC**, **TD3**) and on-policy (**PPO**) actor-critic architectures. |
| **Constraint Satisfaction ($30\%$)** | Stress-testing learned policies against hard safety bounds and operational envelopes without modifying underlying environment reward functions. |
| **Control Effort & Smoothness ($20\%$)** | Tuning policy network architectures and action-smoothing filters to prevent actuator chatter and minimize high-frequency control oscillations ($\Delta u$). |
| **Disturbance Rejection ($20\%$)** | Evaluating zero-shot policy robustness under unseen step disturbances, sensor noise, and dynamic setpoint transitions. |

---

## 📈 GitHub Activity & Connect

* 🌐 **Try Gochalo Live:** [https://gochalo.vercel.app/](https://gochalo.vercel.app/)
* 📦 **Flagship Repository:** [github.com/mahmudhasan-k/gochalo](https://github.com/mahmudhasan-k/gochalo)
* 💼 **LinkedIn:** [linkedin.com/in/mahmudhasan-k](https://www.linkedin.com/in/mahmudhasan-k/)
* 📫 **Email:** [hello.mahmudhasan@outlook.com](mailto:hello.mahmudhasan@outlook.com)

![Mahmud's GitHub Stats](https://github-readme-stats.vercel.app/api?username=mahmudhasan-k&show_icons=true&theme=tokyonight&hide_border=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=mahmudhasan-k&layout=compact&theme=tokyonight&hide_border=true)
