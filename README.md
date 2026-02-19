<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:1f6feb&height=180&section=header&text=Chester%20Guan&fontSize=42&fontColor=e6edf3&fontAlignY=35&desc=healthcare%20AI%20%C2%B7%20systems%20builder%20%C2%B7%20Gainesville%20FL&descSize=16&descColor=8b949e&descAlignY=55&animation=fadeIn"/>

<div align="center">

<a href="https://scholar.google.com/citations?user=VsYXfV8AAAAJ"><img src="https://img.shields.io/badge/Google_Scholar-300+_citations-4285F4?style=flat&logo=googlescholar&logoColor=white"/></a>
<a href="https://twitter.com/Chester_Guan16"><img src="https://img.shields.io/badge/𝕏-Chester__Guan16-000000?style=flat&logo=x"/></a>
<a href="https://chesterguan.github.io/"><img src="https://img.shields.io/badge/Web-chesterguan.github.io-4285F4?style=flat&logo=googlechrome&logoColor=white"/></a>
<a href="mailto:ziyuan.guan@ufl.edu"><img src="https://img.shields.io/badge/UF-Dept.%20of%20Medicine-FA4616?style=flat"/></a>

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&multiline=true&repeat=true&width=700&height=80&lines=I+teach+machines+to+watch+over+patients.;Then+I+build+the+guardrails+so+you+can+trust+them." alt="Typing SVG" />

</div>

---

### Hey, I'm Chester.

I'm a researcher and engineer at the [University of Florida](https://ic3.center.ufl.edu/) — been here long enough to know the hospital WiFi passwords. I split my time between two labs: **IC3** (Intelligent Clinical Care Center) and **PRISMAp** (Precision & Intelligent Systems in Medicine).

The short version: I spent years training models to predict bad things before they happen — delirium, kidney failure, surgical complications. Published 25+ papers on it across [Nature Scientific Reports](https://www.nature.com/articles/s41598-025-22634-7), [JAMA Surgery](https://jamanetwork.com/journals/jamasurgery), [JMIR](https://medinform.jmir.org/), and ICLR workshops. 300+ citations. Multiple [NIH grants](https://reporter.nih.gov/) (R01, R21, K01, OT2) funded that work.

Then I realized: **predictions alone don't save anyone.** You need systems. Systems that clinicians actually use, that run in real time, that you can *prove* did the right thing. So now I build those too.

**MS in Electrical & Computer Engineering**, UF. Data Scientist III, Department of Medicine.

---

### What I've published

I like giving my models weird fruit names. Here's what came out of it:

| Paper | TL;DR | Scale |
|:------|:------|:------|
| [**MySurgeryRisk**](https://arxiv.org/abs/2506.21814) | "Will this surgery go wrong?" — multicenter validation | 508k surgeries, AUROC 0.95 |
| [**DeLLiriuM**](https://arxiv.org/abs/2410.17363) | LLM that predicts delirium from structured EHR | 104k patients, 195 hospitals |
| [**MANDARIN**](https://arxiv.org/abs/2503.06059) | Mixture-of-Experts for delirium + coma | 92k ICU patients |
| [**MANGO**](https://arxiv.org/abs/2412.17832) | Multimodal transformer for ICU acuity | Vitals + labs + notes fused |
| [**APRICOT-Mamba**](https://arxiv.org/abs/2311.02026) | State-space model for real-time ICU prediction | 75k patients, 147 hospitals |
| [**Temporal Cross-Attn**](https://arxiv.org/abs/2403.04012) | Dynamic EHR tokenization | ICLR 2024 Workshop |
| [**Federated Learning**](https://arxiv.org/abs/2404.06641) | Predict postop complications without sharing data | Multi-center, privacy-first |

<details>
<summary>more papers (25+ total) ...</summary>
<br/>

- **Risk-Specific Training Cohorts** — class imbalance in surgical prediction — *JAMA Surgery* (2024)
- **Transparent AI** — explainable postop complication interface (2024)
- **Global Contrastive Training** — multimodal EHR + language supervision (2024)
- **EHR Data Quality** — scoping review — *JMIR Med Inform* (2024)
- **Selective State Space Models** — brain dysfunction across cohorts (2024)
- **AKI Prediction** — external validation for non-critical care (2024)
- **ML + FHIR** — scoping review on FHIR-native ML systems — *JMIR Med Inform* (2023)
- **AI-Enhanced ICU** — pervasive sensing in critical care (2023)
- **Delirium from Ambient Signals** — noise and light as ICU predictors (2023)
- **Computable Phenotypes** — brain dysfunction characterization (2023)
- **AKI Multistate Analysis** — kidney injury trajectories — *Scientific Reports* (2023)
- **Acute Illness Phenotypes** — temporal clustering (2023)
- **Deep Interpolation Network** — physiologic time series (2020)

</details>

---

### What I'm building now

Predictions are nice. But I got tired of models sitting in Jupyter notebooks while clinicians still drown in paperwork. So now I build the infrastructure layer.

```
  ┌──────────────────────────────────────────┐
  │           ClinicClaw (coming soon)        │
  │     AI agents that do real clinical work  │
  │   ambient docs · smart orders · prior auth│
  ├──────────────────────────────────────────┤
  │              VERITAS                       │
  │     every agent action: checked, logged   │
  │  deny-by-default · SHA-256 audit chain    │
  ├──────────────────────────────────────────┤
  │            HAVEN Protocol                  │
  │    patients own their data. period.       │
  │   consent · provenance · value tracking   │
  ├──────────────────────────────────────────┤
  │          PSDL                              │
  │     clinical scenarios as code            │
  └──────────────────────────────────────────┘
```

<table>
<tr>
<td width="50%" valign="top">
<h4><a href="https://github.com/Chesterguan/HAVEN">HAVEN Protocol</a> &nbsp; <code>TypeSpec</code> &nbsp; v2.0</h4>
<p>Your blood test results train AI models you'll never see. You can't audit access. You can't set conditions. You don't share in the value. HAVEN fixes that.</p>
<ul>
<li>4 primitives: Health Asset, Consent, Provenance, Contribution</li>
<li>Content-addressed (SHA-256), Ed25519-signed</li>
<li>Silence = denial. Always.</li>
<li>FHIR R4 + OMOP CDM native</li>
<li>Formal specs, test vectors, 3 language whitepapers</li>
</ul>
<h4><a href="https://github.com/Chesterguan/PSDL">PSDL</a> &nbsp; <code>Python</code> &nbsp; ⭐ 9</h4>
<p>Clinical scenarios as code. Write a patient case once, run it everywhere, get deterministic results.</p>
</td>
<td width="50%" valign="top">
<h4>VERITAS &nbsp; <code>Rust</code> &nbsp; <em>(coming soon)</em></h4>
<p>Before an AI agent touches a patient record, VERITAS checks the policy, logs the action, and verifies the output. Every. Single. Time.</p>
<ul>
<li>Deny-by-default policy engine</li>
<li>SHA-256 hash-chained audit trail</li>
<li>5 healthcare scenarios, 58 tests</li>
<li><code>RequireApproval</code> = human stays in the loop</li>
</ul>
<h4>ClinicClaw &nbsp; <code>Rust</code> &nbsp; <em>(design phase)</em></h4>
<p>The actual hospital system. Real LLM calls, real FHIR, real clinical workflows — all governed by VERITAS.</p>
<h4><a href="https://github.com/Chesterguan/AesculTwin">AesculTwin</a> &nbsp; <code>TypeScript</code> &nbsp; ⭐ 2</h4>
<p>AI-powered surgeon assistance.</p>
</td>
</tr>
</table>

---

### How I think about this

```rust
impl Chester {
    fn day_job(&self) -> &str {
        "mass ECE @ UF · data scientist III · IC3 + PRISMAp"
    }

    fn things_i_care_about(&self) -> Vec<&str> {
        vec![
            "can you prove what your AI did?",
            "can the patient say no?",
            "does it work at 3am when the senior resident is asleep?",
            "would you trust it with your mom's chart?",
        ]
    }

    fn tools(&self) -> Vec<&str> {
        vec!["Rust", "Python", "TypeScript", "FHIR R4"]
    }

    fn funded_by(&self) -> Vec<&str> {
        vec!["NIH R01", "NIH R21", "NIH K01", "NIH OT2"]
    }
}
```

<div align="center">

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![FHIR](https://img.shields.io/badge/FHIR_R4-FF6B35?style=for-the-badge)

</div>

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Chesterguan&show_icons=true&theme=github_dark&hide_border=true&count_private=true&hide_title=true" alt="stats"/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Chesterguan&theme=github-dark-blue&hide_border=true" alt="streak"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Chesterguan&layout=compact&theme=github_dark&hide_border=true&langs_count=8" alt="langs"/>

</div>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:1f6feb&height=100&section=footer&animation=fadeIn"/>
