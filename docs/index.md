# AI Red Teaming Methodology

## **Phase 1: Reconnaissance & Scoping**

- **1.1. Defining Test Objectives & Scope**
    - 1.1.1. Identifying Business Risks & Threat Models
    - 1.1.2. Establishing Rules of Engagement
- **1.2. Model Fingerprinting**
    - 1.2.1. Identifying the Base Model (e.g., GPT, Llama, Gemini, Mistral)
    - 1.2.2. Deducing Model Size and Version
    - 1.2.3. Probing for Fine-Tuning or Specialization
- **1.3. System & Architectural Analysis**
    - 1.3.1. Eliciting the System Prompt & Meta-Instructions
    - 1.3.2. Identifying Integrated Systems (RAG, API Endpoints, Tools)
    - 1.3.3. Mapping the Application's Data Flow

## **Phase 2: Profiling & Boundary Testing**

- **2.1. Personality & Tone Baselining**
    - 2.1.1. Assessing Default Persona (Formal, Creative, Verbose)
    - 2.1.2. Probing for Emotional and Empathetic Responses
- **2.2. Instruction Following & Reasoning Fidelity**
    - 2.2.1. Testing Compliance with Complex, Multi-Constraint Prompts
    - 2.2.2. Evaluating Logical and Deductive Reasoning Capabilities
- **2.3. Ethical & Safety Boundary Probing**
    - 2.3.1. Testing Gray-Area Ethical Dilemmas
    - 2.3.2. Identifying the Threshold for Mildly Manipulative Requests
- **2.4. Refusal Pattern Analysis**
    - 2.4.1. Differentiating Between Soft vs. Hard Refusals
    - 2.4.2. Cataloging Justifications for Refusals

## **Phase 3: Initial Exploitation (Direct Jailbreaking TTPs)**

- **3.1. Persona & Role-Playing Attacks**
    - 3.1.1. Standard Persona Hijacking (e.g., DAN - "Do Anything Now")
    - 3.1.2. Authority Figure & Expert Impersonation
- **3.2. Instruction Overriding & Prefix Injection**
    - 3.2.1. Forcing Start-of-Response Affirmatives (e.g., "Sure, I can help...")
    - 3.2.2. "Ignore Previous Instructions" Style Overrides
    - 3.2.3. Payload Splitting and Reconstruction
- **3.3. Contextual Misdirection & Obfuscation**
    - 3.3.1. Character & Encoding Manipulation
    - 3.3.2. Fictional & Hypothetical Scenario Framing
- **3.4. Known Vulnerability Prompting (Adversarial Suffixes)**
    - 3.4.1. Appending Universal Adversarial Suffixes (e.g., GCG Attacks)
    - 3.4.2. Using Common Syntax Breakers (e.g., "=====")
    - 3.4.3. Leveraging Known Prompt Injection Templates

## **Phase 4: Advanced Manipulation & Evasion (Conversational Hacking)**

- **4.1. Iterative Refinement & Goal Hijacking**
    - 4.1.1. Gradual Escalation of Request Severity
    - 4.1.2. Pivoting from Safe to Unsafe Contexts
- **4.2. Multi-Turn Deception & Context Poisoning**
    - 4.2.1. Long-Context Fatigue & Safety Decay
    - 4.2.2. Embedding Malicious Logic in User History
- **4.3. Chain-of-Thought (CoT) Exploitation**
    - 4.3.1. Direct CoT for Decomposing Forbidden Tasks
    - 4.3.2. Reverse CoT for Safety Policy Analysis
- **4.4. Cognitive Hazard & State Manipulation Attacks**
    - 4.4.1. Gaslighting & Truth-Deterioration Probing
    - 4.4.2. Emotional Manipulation for Safety Override

## **Phase 5: Post-Exploitation & Objective Achievement**

- **5.1. Harmful Content Generation**
    - 5.1.1. Misinformation & Disinformation Campaigns
    - 5.1.2. Malicious Code & Exploit Generation
    - 5.1.3. Phishing & Social Engineering Content Crafting
- **5.2. Sensitive Information Elicitation**
    - 5.2.1. Extracting PII from Training Data or Context
    - 5.2.2. Deducing System Configurations or Internal Knowledge
- **5.3. Agentic System & Tool Hijacking**
    - 5.3.1. Abusing Integrated APIs and Functions
    - 5.3.2. Exploiting RAG Systems for Data Exfiltration
    - 5.3.3. Indirect Prompt Injection via Retrieved Documents

## **Phase 6: Analysis, Reporting & Remediation**

- **6.1. Vulnerability Cataloging & Severity Rating**
    - 6.1.1. Mapping Vulnerabilities to OWASP Top 10 for LLMs
    - 6.1.2. Assigning CVSS-Equivalent Scoring for AI Risks
- **6.2. Exploit Reliability & Persistence Testing**
    - 6.2.1. Measuring Success Rates Across Model Iterations
    - 6.2.2. Testing "One-Shot" vs. Multi-Turn Consistency
- **6.3. Impact Analysis & Risk Quantification**
    - 6.3.1. Estimating Potential Financial and Reputational Damage
    - 6.3.2. Evaluating Compliance and Legal Implications
- **6.4. Defensive Measures & Remediation Recommendations**
    - 6.4.1. System Prompt Hardening
    - 6.4.2. Input/Output Filtering and Guardrails
    - 6.4.3. Recommendations for Model Fine-Tuning