
# Enhancing Pharmacovigilance: Predicting Adverse Drug Interactions Using MedLLAMA

**Term:** Spring 2025  
**Team:** Team Green  
**Advisor:** Prof. Div Pithadia | Department: ECECS | Tagliatela College of Engineering

---

## 👩‍🎓 Students
- Yash Raythatha
- Ayushi Jar
- Saurabh
- Ayush Prajapati

---

## #️⃣ Keywords
MLOps, Python, Fine-tuning, Drug Interaction Prediction, Healthcare AI, Google Colab, medalpaca-7b, Hugging face, Gradio, Parameter efficient finetuning.

---

## 💻 Project Abstract
Drug interactions are a major cause of hospitalizations and adverse health outcomes. Current tools often lack accessibility and interpretability. This project bridges the gap using data science combined with clinical knowledge and large language models (LLMs).

We developed an AI-powered model to predict potential side effects caused by commonly prescribed drug combinations and generate clinically relevant, human-understandable summaries using the fine-tuned MedLLAMA model.

---

## 🫧 Background
Clinical decision-making tools that assess drug-drug interactions often provide limited or overly technical outputs. Our goal was to enhance accessibility and clinical relevance by developing an AI-driven platform capable of offering reliable, easy-to-interpret interaction information using modern machine learning methods.

---

## 📋 High-Level Requirements
- Develop a machine learning model capable of predicting and explaining drug-drug interactions.
- Fine-tune a large language model (LLAMA-7B) with curated datasets.
- Build a user-friendly Gradio-based web interface for clinicians and researchers.
- Deploy a publicly accessible version for broader testing and feedback.

---

## 📋 Functional Requirements
- Merge and preprocess multiple datasets related to drug-drug interactions.
- Fine-tune MedLLAMA 7B model using expanded dataset.
- Develop a Gradio-based web application for users to input drug pairs.
- Provide human-readable interaction descriptions, mechanisms, and severity levels.

---

## ✅ Non-Functional Requirements
- The system must be cloud deployable.
- Model inference must be GPU-optimized using 4-bit quantization.
- Web interface should be responsive and mobile-accessible.
- Secure API for future integration with EHR (Electronic Health Record) systems.

---

## ✨ Key Features
- **Interactive UI**: Easy-to-use Gradio interface for clinicians and researchers.
- **Clinical-Grade Predictions**: Human-readable interaction descriptions generated from fine-tuned MedLLAMA model.
- **Interaction Management Tips**: The output not only explains the interaction, but also **provides actionable advice** on what medical measures should be taken if two drugs are consumed together (e.g., dose adjustment, monitoring symptoms, alternative medication suggestions).

---

## ✍🏼 Conceptual Design
The project pipeline is as follows:
- Merge data from DDI Inter and PubChem.
- Expand the dataset using LLM.
- Preprocess and curate high-quality human-readable side effect data.
- Fine-tune the MedLLaMA-7B model using LoRA for parameter-efficient training.
- Deploy using a Gradio interface for user interaction.

All modeling, training, and experimentation were conducted using **Google Colab**.

---

## 🛠️ Technical Design
- **Base Model:** `medalpaca/medalpaca-7b (LLAMA-7B)`
- **Fine-tuning Strategy:** LoRA (Low-Rank Adaptation), 4-bit quantization for resource efficiency
- **Frameworks and Libraries:** Hugging Face Transformers, PEFT, Accelerate, Gradio
- **Deployment:** Gradio (or custom server hosting)

---

## 📦 Required Resources
- Google Colab (GPU enabled)
- PyTorch (4-bit compatible version)
- Hugging Face Transformers and PEFT libraries
- Gradio for web-based UI
- Jupyter for data preprocessing and testing

---

## 🏁 Project Plan & Milestones

| Week | Milestone/Activity | Deliverables/Features |
|:----|:--------------------|:----------------------|
| 1    | Define Scope and Requirements | Finalized project scope and high-level objectives |
| 2    | Dataset Collection | Sourced DDI Inter and PubChem datasets |
| 3    | Dataset Merging | Merged datasets and initial validation |
| 4    | Dataset Expansion | Used ChatGPT-4.0 for side effect generation |
| 5    | Preprocessing | Cleaned and structured expanded dataset |
| 6    | Model Setup | Prepared MedLLaMA-7B base model on Colab |
| 7    | Fine-tuning Strategy Finalization | Integrated LoRA + 4-bit quantization strategies |
| 8    | Fine-tuning Model | Conducted parameter-efficient fine-tuning |
| 9    | Evaluation and Metrics Analysis | Measured perplexity, manual quality checks |
| 10   | UI Development | Built Gradio-based user interface |
| 11   | Integration and Testing | Connected model output to UI, tested workflows |
| 12   | Final Deployment and Demo | Hosted project on Hugging Face Spaces / Web server |

---

## 🧪 Test Cases
- Validate model output for a wide range of drug pairs.
- Check output readability, accuracy of predicted side effects, and medical plausibility.
- Load-testing of the web interface under concurrent users.

---

## 👩🏻‍🏫 Installation Instructions

**Minimum Requirements:**
- Google Colab account with GPU access
- Installed libraries (via `requirements.txt`) including Gradio, transformers, peft, accelerate

**Steps to Run Locally (Optional for Further Development):**

```bash
git clone <this-repo-link>
cd project-directory
pip install -r requirements.txt
```
---

## 💡 Tips for Best Usage
- Use Google Colab with GPU enabled (`Runtime > Change Runtime Type > GPU`) for smooth model loading and interaction.
- Ensure a stable internet connection while loading large models.
- For deployments, prefer Hugging Face Spaces or GPU-backed servers for better inference speeds.
- Validate unknown drug combinations with medical experts before clinical usage.

---

### 👩🏻‍💻🧑🏻‍💻 Collaborators

[//]: # ( readme: collaborators -start )
<table>
<tr>
    <td align="center">
        <a href="https://github.com/digitaldiv">
            <img src="https://avatars.githubusercontent.com/u/1842870?v=4" width="100;" alt="Div Pithadia"/>
            <br />
            <sub><b>Div Pithadia</b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/chargershub">
            <img src="https://avatars.githubusercontent.com/u/160267476?v=4" width="100;" alt="Chargers hub"/>
            <br />
            <sub><b>Chargers Hub</b></sub>
        </a>
    </td></tr>
</table>
