# CyberQuant 🛡️📊

> **Continuous Cyber Risk Quantification & Security Investment Optimization**  
> *Transforming raw security telemetry, threat intelligence, and control posture into explainable financial risk metrics and budget-optimal security decisions.*

[![Live Demo](https://img.shields.io/badge/Demo-Live%20Prototype-0ea5e9?style=for-the-badge&logo=netlify)](https://cyberquant.netlify.app)
[![Architecture](https://img.shields.io/badge/Architecture-Zero--Dependency%20Vanilla%20ES6-10b981?style=for-the-badge)](./app.js)
[![Platform](https://img.shields.io/badge/Platform-Web%20%7C%20Cross--Browser-6366f1?style=for-the-badge)](./index.html)
[![Status](https://img.shields.io/badge/Status-Prototype%20%2F%20Hackathon%20Edition-f59e0b?style=for-the-badge)]()

---

## 📌 Executive Summary

Traditional vulnerability management relies on isolated technical scores (like CVSS) that fail to convey business impact or assist executives in allocating capital. A CVSS 9.8 vulnerability on an isolated internal server does not carry the same risk as an actively exploited flaw on an internet-facing payment pipeline.

**CyberQuant** bridges the communication divide between CISOs, security engineers, and the CFO/Board. It models cyber risk as an actuarial, financial equation—quantifying exposure into **Estimated Annual Loss (₹ Cr)** and utilizing a **constrained mathematical optimizer** to recommend the highest-ROI security investments under strict budgetary limits.

---

## 🌟 Key Capabilities

### 1. 📐 Mathematical Risk Quantification Engine
Instead of subjective low/medium/high matrices, CyberQuant applies a structured, transparent residual risk formulation:

$$\text{Residual Risk} = \text{Likelihood} \times \text{Impact} \times \text{Exposure} \times (1 - \text{Control Effectiveness})$$

- **Likelihood**: Technical severity (CVSS), exploit availability, observed in-the-wild exploitation (e.g., CISA KEV / threat feeds).
- **Impact**: Asset criticality, revenue dependency, hourly downtime costs, regulatory/data sensitivity.
- **Exposure**: Internet-facing vs. internal private boundary.
- **Controls**: Compensating controls (WAF, EDR, MFA, Segmentation, Backups) evaluated against assessed coverage and effectiveness.
- Output is normalized to an intuitive `0–100` residual-risk index paired with monetary Annual Loss Expectancy.

### 2. 💡 0/1 Constrained Security Investment Optimizer
Security leaders often have fixed budgets and dozens of competing control requests. CyberQuant solves an algorithmic knapsack selection problem across candidate security investments:
- **Objective**: Maximize total expected risk reduction.
- **Constraint**: Total deployment cost $\le$ Available capital budget.
- **Diminishing Returns Modeling**: Penalizes overlapping tool deployments to reflect real-world defense-in-depth synergies and redundancies.

### 3. 🧪 Real-Time Scenario Simulator & Stress-Testing
Allows decision-makers to stress-test their risk posture before committing funds:
- Dynamic sliders for **Investment Budget**, **Threat Level**, **Control Efficacy**, and **Gross Business Impact**.
- Instant recalculation of residual risk, avoided financial loss, and recommended control configurations.

### 4. ⚡ Dynamic Threat Simulation Engine
- Test how zero-day disclosures or active attack campaigns dynamically impact enterprise risk.
- Trigger real-time simulations (e.g., active weaponization against the Payment Gateway) to see immediate telemetry recalculations ($72 \to 91$ risk spike) and automated action triage.

### 5. 🤖 AI Risk Analyst (Decision Support)
- Evidence-based risk explanations formatted for executive consumption.
- Contextual triage articulating *why* an asset became critical, affected upstream business services, and human-in-the-loop remediation advice.

### 6. 🚀 9-Stage Guided Onboarding Workflow
- Structured organization onboarding with support for live CSV imports (or instant synthetic data generation).
- Built-in schema validation for asset inventories, CVE lists, business services, and security controls.

### 7. 📄 Board & Executive Reporting
- Print-ready and exportable cyber risk posture summaries designed for executive committee and board reviews.

---

## 🖥️ Live Demo & Quickstart

### 🌐 Online Demo
Access the live deployed prototype directly:  
👉 **[cyberquant.netlify.app](https://cyberquant.netlify.app)**

### 💻 Running Locally (Zero Dependencies)
CyberQuant is built entirely with pure web standards. No Node.js, `npm install`, build runners, or backend servers are required.

1. **Clone the repository**:
   ```bash
   git clone https://github.com/BasicPanther/CyberQuant.git
   cd CyberQuant
   ```

2. **Run**:
   - Double-click `index.html` or open it in any modern browser (Chrome, Edge, Firefox, Safari).
   - Alternatively, serve with any local HTTP server:
     ```bash
     npx serve .
     # or
     python -m http.server 8000
     ```

---

## 🧭 Evaluator & Demo Path

To experience the full capability in under 3 minutes:

1. **Explore Existing Enterprise**:
   - Select **Existing Company** to load *FinServe Technologies*.
   - Review the **Enterprise Risk Trend**, **Top Business Risks**, and **Annualized Financial Exposure**.
2. **Simulate a Threat Event**:
   - Click **Simulate New Threat Event** on the Overview or Threat Intelligence tab.
   - Observe the live recalculation: Payment Gateway risk spikes from $72 \to 91$, and enterprise loss exposure expands.
3. **Inspect the AI Risk Analyst**:
   - Navigate to **AI Risk Analyst** to review the explainable root-cause evidence and recommended compensatory mitigations.
4. **Run the Investment Optimizer**:
   - Switch to **Investment Optimizer**, enter an available budget (e.g., `₹100L`), and click **Optimize Budget**.
   - Review the algorithmically selected portfolio, expected risk reduction ($42\%$), and estimated loss avoided ($\text{₹2.6 Cr}$).
5. **Simulate Scenarios**:
   - Open **Scenario Simulator** to adjust threat intensity, control coverage, or budget constraints to stress-test your risk thresholds.
6. **Test the Onboarding Flow**:
   - Return to the landing page and choose **New Company** to walk through the 9-stage onboarding workflow, CSV template generation, and validation engine.

---

## 🏗️ Architecture & Technology Stack

| Layer | Implementation | Details |
|---|---|---|
| **Frontend Framework** | Vanilla ES6+ JavaScript | Zero external runtime dependencies; lightweight, blazingly fast execution |
| **Styling & Theme** | Custom Modern CSS3 | Deep space / cybersecurity theme with custom design tokens, responsive CSS Grid & Flexbox |
| **Visualizations** | Native SVG & CSS Data Visualizations | Real-time trend vectors, risk matrices, and responsive telemetry bars |
| **Optimization Engine** | Combinatorial Power Set Evaluation | Evaluates all $2^8 = 256$ investment combinations with overlap mitigation curves |
| **Data Ingestion** | Native FileReader & CSV Parser | Client-side validation against required schema headers |

---

## 📁 Repository Structure

```
CyberQuant/
├── index.html        # Single-page application entry point & root container
├── styles.css        # Cyber security themed design tokens, grid & typography
├── app.js            # Reactive application logic, risk engine & optimizer
├── .gitignore        # Standard ignore patterns
└── README.md         # Documentation & architecture breakdown
```

---

## 🔒 Governance & Ethical Note

CyberQuant is designed as a **decision-support platform** that operates under human-in-the-loop oversight. All risk models, financial parameters, and investment recommendations are transparent, explainable, and configurable to match institutional risk tolerance.

---

## 📄 License

Distributed under the [MIT License](LICENSE). Built for the Smart India Hackathon (SIH) prototype showcase.
