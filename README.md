# SDLC_and_Usecase_diagram_of_AutoApply
# AutoApply — SDLC Model Selection

## About AutoApply

**AutoApply** is an AI-based job application system built around a four-agent pipeline:

**Job Parser → Resume Analyzer → Matcher → Writer**

The system processes job descriptions and applicant information through specialized AI agents to produce tailored application outputs.

---

## Use Case Overview

The basic use case can be represented as:

```text
                    ┌──────────────────────┐
                    │      AutoApply       │
                    │                      │
Applicant ─────────►│  Provide Job Details │
                    │          │           │
                    │          ▼           │
                    │   ┌──────────────┐   │
                    │   │  Job Parser  │   │
                    │   └──────┬───────┘   │
                    │          ▼           │
                    │   ┌──────────────┐   │
                    │   │    Resume    │   │
                    │   │   Analyzer   │   │
                    │   └──────┬───────┘   │
                    │          ▼           │
                    │   ┌──────────────┐   │
                    │   │    Matcher   │   │
                    │   └──────┬───────┘   │
                    │          ▼           │
                    │   ┌──────────────┐   │
                    │   │    Writer    │   │
                    │   └──────┬───────┘   │
                    │          ▼           │
                    │  Tailored Application│
                    │       Output         │
                    └──────────────────────┘
```

The applicant provides the required information, while AutoApply processes it through the four-agent pipeline to generate the final output.

---

## SDLC Model Selection

For AutoApply, six SDLC models were evaluated:

* Waterfall
* V-Shaped
* Iterative
* Spiral
* Agile
* Prototype

The models were compared based on criteria that are particularly important for an AI-driven system.

### Comparison

| Criteria                         | Waterfall | V-Shaped | Iterative | Spiral |  Agile | Prototype |
| -------------------------------- | --------: | -------: | --------: | -----: | -----: | --------: |
| Requirement Flexibility          |        No |       No |       Yes |    Yes |    Yes |       Yes |
| AI Output Adaptability           |        No |       No |       Yes |     No |    Yes |       Yes |
| Continuous Testing & Integration |        No |      Yes |       Yes |    Yes |    Yes |        No |
| Risk Management & AI Reliability |        No |       No |        No |    Yes |    Yes |        No |
| User Feedback & Early Delivery   |        No |       No |       Yes |    Yes |    Yes |       Yes |
| Efficiency & Low Overhead        |       Yes |       No |       Yes |     No |    Yes |        No |
| Fast Delivery                    |        No |       No |       Yes |     No |    Yes |       Yes |
| **Overall Score**                |     **3** |    **6** |    **23** | **20** | **30** |    **17** |

### Result

**Agile achieved the highest score: 30/30.**

---

## Why Agile Was Selected

Agile was selected because the core of AutoApply is a **four-agent AI pipeline** that requires iterative development and continuous testing.

Each agent can be developed and tested independently before being integrated into the complete system:

**Job Parser → Resume Analyzer → Matcher → Writer**

This structure fits naturally with Agile's incremental and sprint-based development approach.

### 1. Requirement Flexibility

AI-based systems often require changes after observing actual outputs. The requirements of AutoApply can evolve as different prompts, inputs, and AI responses are tested.

Agile allows these requirements to be refined throughout development instead of fixing them entirely at the beginning.

### 2. AI Output Adaptability

The output of a language model is not completely predictable in advance. Responses may be inconsistent, incomplete, or differently structured than expected.

Agile allows the team to:

**Test → Observe → Improve → Retest**

This makes it suitable for continuously tuning prompts, agent behavior, and output handling.

### 3. Continuous Testing & Integration

Each AI agent can be tested individually and then integrated step by step.

This makes it possible to identify problems early rather than waiting until the entire system is completed.

### 4. AI Reliability & Risk Handling

For AutoApply, the major technical concern is the **reliability of AI-generated output**, rather than risks such as bot detection because the system uses **pasted job descriptions instead of live web scraping**.

Agile supports continuous testing and refinement, making it possible to address reliability issues as they appear.

### 5. Early and Incremental Delivery

The project can be developed through working increments:

**Single Agent → Two-Agent Chain → Full Pipeline → Frontend → Tracker**

Each increment provides a working part of the system while allowing the team to gather feedback and improve the next stage.

---

## Final Justification

Agile is the most suitable SDLC model for AutoApply because the project requires **flexibility, iterative development, continuous testing, AI-output refinement, and incremental delivery**.

Unlike traditional models that depend heavily on fixed requirements established at the beginning, Agile allows AutoApply to evolve as the team learns more from actual AI outputs and system testing.

> **The project therefore adopts Agile as its SDLC model, with an overall score of 30/30 in the comparison.**

---

## Group 10

* **AHMAD IBRAHIM NAHIAN** — 24524203065
* **MAHATHIR MOHAMMAD** — 24524203179
* **MD. HASIBUL HASAN TALUKDAR** — 23524202003
* **MD. AKIMO ISLAM SAD** — 24524203135
