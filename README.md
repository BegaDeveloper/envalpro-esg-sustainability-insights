# 🌿 EnvalPro – ESG App for Sustainability Insights & Renovation Cost (Germany)

## 🚀 Introduction

**EnvalPro** is an **ESG (Environmental, Social, and Governance)** analytics platform built to help individuals, companies, and organizations evaluate and improve the sustainability performance of their **buildings, locations, and assets**.
The system provides deep insights into environmental impact, energy efficiency, and compliance with ESG standards — while also estimating **renovation and upgrade costs** required to achieve sustainability goals.

The purpose of EnvalPro is to **empower users to make data-driven, sustainable investment decisions**. By combining environmental analytics, cost modeling, and predictive algorithms, the app serves as a powerful decision-support tool for sustainability professionals, investors, and facility managers across Germany.

---

## 🧠 What the App Does

EnvalPro acts as a **comprehensive sustainability evaluation platform**, combining environmental data analysis with financial modeling.
Users can input property details or location data, and the system generates a detailed ESG report that includes:

* 🌍 **Environmental Impact Assessment** – Energy usage, emissions, and ecological footprint.
* 🏠 **Renovation Cost Estimation** – Calculates projected costs for upgrading to green standards.
* 🧾 **Compliance Scoring** – Benchmarks properties against EU and German ESG regulations.
* 📊 **Sustainability Insights Dashboard** – Interactive visualizations and recommendations.
* ⚙️ **AI-Based Predictive Models** – Suggests optimal improvement paths based on cost-benefit ratios.

With its intuitive UI and robust analytics engine, EnvalPro bridges the gap between **financial planning and environmental responsibility**.

---

## 🧩 Technologies Used

| Layer                        | Stack / Tools                                                                                         | Description                                                             |
| ---------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| **Frontend**                 | **Angular 17**, **RxJS**, **Angular Material**, **SCSS**                                              | Built the complete ESG analytics and reporting dashboard.               |
| **Backend**                  | **Python FastAPI**, **Pandas**, **NumPy**, **Scikit-Learn**                                           | Handled ESG data processing, sustainability scoring, and cost modeling. |
| **Database**                 | **PostgreSQL (Cloud SQL)**                                                                            | Stored property data, sustainability metrics, and compliance records.   |
| **Cloud / Infrastructure**   | **Google Cloud Platform (GCP)** – **App Engine**, **Cloud Storage**, **Cloud Functions**, **AI APIs** | Provided hosting, computation, and model deployment.                    |
| **Version Control / DevOps** | **GitHub Actions**, **Docker**, **CI/CD pipelines**                                                   | Automated builds, testing, and containerized deployments.               |

---

## 💻 My Role & Contributions

I served as the **Team Lead and Software Architect** for the EnvalPro project — overseeing the architecture, development flow, and implementation strategy across both the frontend and backend teams.
In addition to leading the team, I also contributed directly to the **frontend (Angular)** and coordinated **integration between the FastAPI backend and GCP services**.

Key leadership and technical contributions:

* Designed the **full system architecture**, defining communication patterns between Angular and FastAPI.
* Led a cross-functional team of frontend, backend, and data engineers, ensuring efficient collaboration.
* Developed **Angular modules and reusable components** for dashboards, charts, and report generation.
* Designed the **FastAPI endpoints** and data structures for ESG scoring, renovation cost estimation, and property modeling.
* Integrated **Google Cloud AI services** for environmental data analysis and automated recommendations.
* Established **code standards, CI/CD pipelines, and deployment strategies** on GCP.
* Ensured alignment with **ESG and EU data security requirements**, including GDPR compliance.

---

## ⚙️ Key Technical Highlights I Implemented

### 🧩 1. ESG Scoring & Cost Modeling Engine (FastAPI)

Led the backend architecture for a **dynamic ESG scoring algorithm** that combines sustainability metrics with renovation cost estimation.

Implemented:

* Weighted scoring model evaluating **E (environmental)**, **S (social)**, and **G (governance)** pillars.
* Cost prediction using **linear regression** and **domain-based heuristics** for renovation types (energy efficiency, insulation, solar installations, etc.).
* RESTful endpoints exposing ESG reports and cost breakdowns to the Angular frontend.

```python
@app.post("/esg/score")
def calculate_esg_score(data: ESGInput):
    env_score = model_env.predict(data.env_factors)
    soc_score = model_soc.predict(data.soc_factors)
    gov_score = model_gov.predict(data.gov_factors)
    cost_estimate = renovation_model.predict(data.property_features)
    return {"esg_score": (env_score + soc_score + gov_score) / 3, "cost_estimate": cost_estimate}
```

This engine powered all sustainability insights displayed in the frontend dashboard.

---

### ⚙️ 2. Angular ESG Dashboard Architecture

Architected a **modular Angular app** that allows users to visualize sustainability data interactively:

* Used **RxJS Observables and NgRx-like state management** for real-time updates.
* Integrated **Angular Material charts and D3.js visualizations** for ESG indicators and cost trends.
* Developed **filter panels, scorecards, and map overlays** for property-based insights.
* Built a **PDF report generator** that exports ESG summaries for clients and auditors.

The frontend was optimized for responsiveness and clarity, providing executives and ESG managers with an intuitive decision interface.

---

### ⚙️ 3. Integration & Cloud Infrastructure (GCP)

* Deployed both Angular and FastAPI services on **Google Cloud App Engine**.
* Used **Cloud Functions** for asynchronous tasks like report generation and model training.
* Configured **Cloud Storage** for storing uploaded documents, energy reports, and result datasets.
* Implemented **GCP logging and monitoring** for uptime and performance tracking.

This setup ensured scalability, low latency, and compliance with data privacy laws in the EU.

---

## 🧩 What We Built

* **ESG Scoring Engine** – Evaluates environmental, social, and governance performance dynamically.
* **Renovation Cost Predictor** – Estimates upgrade costs based on property type, size, and energy rating.
* **Interactive Analytics Dashboard** – Displays scores, trends, and recommendations.
* **PDF Report Generator** – Creates exportable sustainability and compliance reports.
* **Team Collaboration Tools** – Role-based dashboards for analysts, managers, and auditors.

---

## 🏁 Outcome

EnvalPro became a **leading ESG evaluation tool** used across Germany to assess sustainability performance and investment feasibility.
The platform helped clients **reduce analysis time by 60%**, **improve ESG compliance visibility**, and **quantify renovation impacts** with precision.

As the **Software Architect and Team Lead**, I successfully delivered a production-grade system that combines **environmental intelligence with financial analytics**, setting a new standard for ESG decision support tools.
