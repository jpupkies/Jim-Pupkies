# Gemini — Decision Suppression Under Downstream Irreversibility

## Overview
This notebook demonstrates a portfolio-grade AI system designed to **refuse to act when downstream decisions are asymmetric, irreversible, or high-cost**, even if model confidence is high. Unlike conventional pipelines that act whenever confidence exceeds a threshold, this notebook separates model uncertainty, data uncertainty, and decision risk to enforce deliberate abstention.

It answers the portfolio question:  
> *“What happens when the system should not decide?”*

## Key Components

### 1. Decision Context and Irreversibility
- Defines a decision space including confidence, reversibility, blast radius, and recovery cost.  
- Establishes **irreversibility as a first-class system attribute**, independent of prediction confidence.

### 2. Model Uncertainty
- Quantifies predictive uncertainty using confidence dispersion and entropy-based proxies.  
- Keeps uncertainty metrics independent from downstream impact.

### 3. Data Uncertainty
- Captures input sparsity, signal conflict, and proxy quality as a separate risk axis.  
- Ensures that fragility of the underlying data is explicitly considered.

### 4. Downstream Irreversibility Scoring
- Computes a structured irreversibility score combining recovery cost, blast radius, and reversibility.  
- Highlights cases where acting could cause irreversible damage.

### 5. Decision Risk Composition
- Combines model uncertainty, data uncertainty, and irreversibility into a **composite decision risk surface**.  
- Prevents collapsing multiple signals into a single opaque metric.

### 6. Suppression, Deferral, and Escalation
- Implements policies that determine when to:
  - **DECIDE**  
  - **DEFER**  
  - **ESCALATE**  
  - **SUPPRESS**
- Treats abstention as a designed success outcome rather than a failure.

### 7. Stress Testing
- Surfaces counterintuitive boundary cases (e.g., high confidence + high irreversibility) to validate policy enforcement.  
- Ensures that the system behaves safely under extreme conditions.

### 8. Portfolio-Grade Visualization
- Scatter plots display model confidence vs irreversibility.  
- `SUPPRESS` decisions are overlaid as `X` markers, making abstention **explicit and auditable**.  

### 9. Executable Guardrails
- Terminal assertion ensures that suppression occurs in practice.  
- Fails the notebook if abstention never triggers, enforcing design intent.

## Portfolio Takeaways
- Demonstrates **engineering judgment beyond predictive outputs**.  
- Shows that **high confidence does not override downstream risk**, reinforcing safe, reliable, and auditable decision-making.  
- Treats abstention as a **first-class system behavior**, aligning with real-world production design principles.  
- Provides a clear, inspectable framework for **human-in-the-loop escalation, deferral, and suppression**.

This notebook complements the existing Gemini portfolio by filling the gap for **irreversibility-aware decision suppression**, illustrating how AI systems can explicitly refuse to act when consequences are too high.
