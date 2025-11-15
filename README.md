# Intelligent Book Marketing Copywriting System
**A Note on This Repository**

Please note that this project was developed as part of a formal, collaborative academic program with industry partners. Due to the nature of this partnership, the full source code is not publicly available. This repository serves as a professional portfolio piece to document and showcase the project's conceptual architecture, the AI workflow, and my technical role in its development and testing.

## 1. High-Level Summary

This project is a prototype for an "Intelligent Book Marketing Copywriting System," designed to bridge the gap between authors, publishers, and consumers.

The system leverages advanced AI prompting techniques, specifically Tree-of-Thoughts (ToT), to move beyond generic summaries. It aims to generate creative, emotionally resonant, and market-aware copywriting that effectively communicates a book's core value and enhances its connection with the target audience.

## 2. Context & Objective

* **Context:** This project was a key component of the "Digital Humanities Interdisciplinary Talent and Smart Leadership Program," developed in collaboration with publishing industry partners (e.g., Yuan-Liou Publishing Co.).

* **Problem:** Traditional marketing copy can be time-consuming to write and often fails to capture the unique essence of a book in a way that resonates with modern consumers.

* **Objective:** To create a "Humanity AI" system that assists marketing and editorial teams by:

    * Generating high-quality, creative copy at scale.
    
    * Using data-driven methods (ToT, predictive models) to evaluate and refine copy.
    
    * Strengthening the brand story and its connection with consumers.

## 3. My Role

As the primary developer and tester for this prototype, I was responsible for implementing the core system and validating its complex AI workflow. My key contributions include:

* **Prototype Development:** Built the functional proof-of-concept (PoC), architecting the entire end-to-end pipeline from book input to final copy generation.

* **ToT Implementation:** Wrote the Python scripts to engineer the ToT prompting structure. This involved designing the multi-step generation, evaluation, and selection logic.

* **System Integration:** Coded the integration between the core Large Language Model (LLM) and the "Hot-Selling Prediction Model" to create an automated evaluation loop.

* **Testing & Validation:** Conducted tests on the system's output, comparing the AI-generated copy against linguistic structures (Swales' "move" theory) and expert criteria.

## 4. System Architecture & Flow

The core innovation of this system is its use of a Tree-of-Thoughts (ToT) framework, which mimics a human's deliberate creative process of drafting, evaluating, and refining ideas.

<img width="9576" height="3084" alt="文案系統" src="https://github.com/user-attachments/assets/1d5627e2-78e4-4316-bc77-1bae26cf0e4c" />

**System Workflow Explained:**

* **Input (Book Content):** The system receives the raw content of a book (e.g., manuscript, summary, author's notes).

* **LLM + ToT Generation:**

  * Unlike a simple one-shot prompt, the system breaks down the writing task into distinct linguistic "moves" (based on Swales, 2011).
  
  * For each step (e.g., writing a hook, establishing a niche, creating a call-to-action), the LLM is prompted to generate three distinct versions (thoughts).

* **Automated Evaluation & Selection:**

  * **Self-Correction:** The system uses a dual-evaluation mechanism for each set of three versions:
  
      * **LLM as Evaluator:** The LLM itself assesses the three options based on creativity and relevance.
      
      * **Predictive Model:** A "Hot-Selling Prediction Model" provides a quantitative score on each option's potential marketability.
  
  * The system selects the "best" version from the three generated.

* **Iterative Refinement:**

  * The "best" version from the previous step is "passed" to the next step, serving as the foundation for the next "move."
  
  * This process repeats (Generate 3 -> Evaluate -> Select 1 -> Pass to next step) until a complete, multi-part marketing copy is constructed.

* **HITL (Human-in-the-Loop) Feedback:**

  * The final, AI-generated copy is presented to human experts (e.g., editors from Yuan-Liou Publishing).

  * Their professional feedback and evaluation are captured to refine both the LLM prompts and the predictive model's accuracy.

* **Output (Final Marketing Copy):** The system outputs a highly refined, structurally sound, and market-tested piece of marketing copy.

## 5. Key Highlights

* **ToT Framework:** This is the project's main highlight. Instead of basic prompting, this system uses a deliberate, branching logic (generate, evaluate, select) to achieve superior creative and strategic output.

* **Linguistic Theory Integration:** The system's generation process is grounded in academic linguistic theory (Swales' "moves"), ensuring the final copy is not just creative but also structurally persuasive.

* **Dual-Evaluation Mechanism:** Combines qualitative (LLM) and quantitative (Predictive Model) feedback at each step, creating a robust self-correction and optimization loop.

* **Industry Collaboration:** This prototype was designed in direct collaboration with publishing experts, ensuring its output is tailored to real-world industry needs.

## 6. Technology Stack 

* **Core Models:** LLMs

* **Core Techniques:** ToT Prompt Engineering, Predictive Modeling
