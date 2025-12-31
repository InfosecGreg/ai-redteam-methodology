# Phase 1: Reconnaissance & Scoping

## 1. Overview

Phase 1: Reconnaissance & Scoping is the foundational stage of the AI red teaming methodology, focused on establishing a deep understanding of the target system and the boundaries of the engagement. It encompasses the critical activities of defining business-aligned testing objectives, fingerprinting the underlying model architecture, and mapping the broader application ecosystem. This phase ensures that subsequent exploitation attempts are targeted, efficient, and respect the established rules of engagement.

## 2. Core Objectives

*   **Align Testing with Business Risk:** Identify the specific organizational hazards and high-impact threat models unique to the target application.
*   **Establish Operational Boundaries:** Define clear Rules of Engagement (RoE) to ensure testing is conducted safely and legally.
*   **De-anonymize the Target Model:** Determine the base model's identity, version, and specialized fine-tuning to select appropriate TTPs.
*   **Map the Architectural Surface:** Catalog integrated systems like RAG, external APIs, and internal data flows to identify complex attack vectors.

## 3. Strategic Importance

This phase is critical for maximizing ROI and minimizing operational friction. By aligning with stakeholders on objective risks (e.g., PII leakage vs. creative hallucination), the red team ensures that its findings provide actionable value. Furthermore, effective model fingerprinting and architectural mapping prevent "blind" testing, allowing researchers to skip ineffective generic prompts and focus on known weaknesses of the specific system architecture, thereby significantly increasing the depth of the final security assessment.

## 4. Methodology Approach

The approach during Phase 1 is primarily research-oriented and analytical, characterized by a "patient observer" mindset. Red teamers act as technical detectives, using a mix of direct probing and architectural deduction to peel back the layers of the AI application. The focus is on gathering high-quality intelligence rather than achieving immediate exploitation. This phase requires a deep understanding of the current AI threat landscape and the ability to extrapolate system behavior from subtle conversational cues.

## 5. Phase Components

*   **1.1 - Defining Test Objectives & Scope**: Covers the establishment of business-aligned risk profiles, threat modeling, and the formalization of rules of engagement to guide the testing process.
*   **1.2 - Model Fingerprinting**: Focuses on identifying the base model architecture, deducing its size/version, and probing for specialized fine-tuning that might alter its safety behavior.
*   **1.3 - System & Architectural Analysis**: Involves mapping the target's internal context, including eliciting system prompts, identifying integrated tools (e.g., RAG, APIs), and tracing application data flow.

---

## 6. Defensive Considerations & Mitigation

Strategic defense at this stage focuses on **Information Minimization** and **System Integrity Policy**:
*   **Inventory Disclosure Control:** Limit the availability of technical details regarding the specific model version or system prompt to external users to prevent targeted fingerprinting.
*   **Holistic Risk Orchestration:** Establish a centralized AI Risk Appetite framework that clearly defines what constitutes a "high-severity" finding before testing begins.
*   **Architectural Hardening:** Implement strict validation and sanitization between the LLM and its integrated tools (RAG, APIs) to reduce the surface area discovered during mapping.
*   **Access Control & Logging:** Ensure that all probing attempts during the "recon" stage are logged and monitored for patterns typical of pre-exploitation behavior.
