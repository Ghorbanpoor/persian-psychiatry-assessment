# persian-psychiatry-assessment
A Persian-language Python GUI for structured psychiatric intake and mental health assessment of first-time patients. Generates comprehensive Persian prompts to support clinical evaluation and differential diagnosis by psychiatrists.

## 📌 Overview

The Persian Psychiatry Assessment Assistant provides a graphical user interface (GUI) for collecting structured psychiatric history, documenting symptoms, and generating a comprehensive prompt for use with large language models (LLMs).

The application is designed to support psychiatrists and other qualified mental health professionals during initial patient interviews. It organizes patient-reported information into clinically relevant sections to facilitate review and further assessment.

**Important:** This application is a clinical support tool, not an autonomous diagnostic system. It does not replace professional judgment, direct patient interviews, medical examinations, or evidence-based diagnostic procedures.

## ✨ Features

- 🇮🇷 Persian-language graphical user interface.
- 🪪 Collection of basic patient information.
- 🗣️ Chief complaint and history of presenting symptoms.
- 🌧️ Screening questions related to depressive symptoms.
- ⚡ Assessment of possible manic and hypomanic symptoms.
- 😰 Anxiety symptoms and panic attacks.
- 🔄 Obsessive-compulsive symptoms.
- 👁️ Psychotic experiences, including hallucinations and delusions.
- 🧩 Trauma-related symptoms and stressors.
- 😴 Sleep, appetite, energy, and physical symptoms.
- 🚨 Initial assessment of suicidal thoughts, plans, intent, and self-harm history.
- 🏥 Previous psychiatric treatment and medical history.
- 💊 Current medications, allergies, and neurological history.
- 🍃 Substance use and possible withdrawal history.
- 👨‍👩‍👧 Family psychiatric history and social support.
- 🩺 Mental status examination fields for clinician observations.
- 📋 Automatic generation of a structured Persian clinical prompt.
- 📥 Export of the generated prompt as a UTF-8 text file.
- ☁️ Compatible with GitHub Codespaces.

## 🛠️ Technologies

The project uses the following technologies:

- **Python** — application logic and data processing.
- **Streamlit** — interactive web-based GUI.
- **HTML and CSS** — interface styling and right-to-left text alignment.
- **Large Language Models (optional)** — external AI-assisted analysis using the generated prompt.

The current implementation generates prompts locally within the application. An external AI service is not required to generate or download the prompt.

## 📂 Project Structure

```text
persian-psychiatry-assessment/
│
├── app.py
├── requirements.txt
└── README.md
```

### File Descriptions

- `app.py`: Main Streamlit application, patient intake form, assessment sections, safety alerts, and prompt generation.
- `requirements.txt`: Python dependencies.
- `README.md`: Project documentation and setup instructions.

## 🚀 Getting Started

### Prerequisites

You need one of the following environments:

- A GitHub account with access to GitHub Codespaces.
- A local computer with Python installed.
- A terminal capable of installing Python packages.

GitHub Codespaces is recommended for users who want to run the application without configuring a local Python environment.

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/persian-psychiatry-assessment.git
cd persian-psychiatry-assessment
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Create the Requirements File

Create a file named `requirements.txt` containing:

```text
streamlit>=1.40,<2.0
```

### 3. Install Dependencies

Run the following command in the terminal:

```bash
python -m pip install -r requirements.txt
```

### 4. Run the Application

Start the Streamlit application:

```bash
python -m streamlit run app.py --server.address 0.0.0.0
```

Streamlit will start a local web server, usually on port `8501`.

If you are using GitHub Codespaces, open the **Ports** panel and access port `8501` using the provided URL.

## ☁️ Running on GitHub Codespaces

1. Open this repository on GitHub.
2. Select **Code**.
3. Open the **Codespaces** tab.
4. Create a new Codespace.
5. Wait for the development environment to initialize.
6. Open the terminal.
7. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

8. Start the application:

   ```bash
   streamlit run app.py --server.address 0.0.0.0
   ```

9. Open the forwarded port `8501` to use the application in your browser.

## 📝 How to Use

### Step 1: Enter Patient Information

Complete the relevant sections of the intake form. The application includes fields for demographic information, chief complaint, symptom history, medical history, medication use, family history, and social circumstances.

Only collect information that is clinically necessary and appropriate for the intended use.

### Step 2: Assess Psychiatric Symptoms

Document the patient's reported symptoms, their duration, severity, progression, and impact on daily functioning.

Available sections cover depressive symptoms, manic and hypomanic symptoms, anxiety, panic attacks, obsessive-compulsive symptoms, psychotic experiences, trauma-related symptoms, sleep, and substance use.

### Step 3: Review Safety Information

Complete the initial safety assessment, including relevant questions about suicidal thoughts, plans, intent, access to means, previous attempts, self-harm, and potential harm to others.

The automated alerts are preliminary indicators only. They do not constitute a validated suicide risk assessment and must not be used to rule out risk.

If there is an immediate risk of serious harm, prioritize urgent professional assessment and appropriate emergency procedures rather than continuing routine form completion.

### Step 4: Record the Mental Status Examination

Qualified clinicians can document observations concerning appearance, behavior, speech, mood, affect, thought processes, perception, orientation, cognition, insight, and judgment.

Patient-reported symptoms should be distinguished from findings directly observed by the clinician.

### Step 5: Generate the Persian Prompt

Click the prompt-generation button to create a structured Persian prompt containing the information entered into the form.

The generated prompt instructs an AI model to:

- Summarize the clinical history.
- Identify reported symptoms and functional impairment.
- Discuss possible differential diagnoses.
- Identify supporting and contradictory evidence.
- Highlight missing information.
- Suggest follow-up interview questions.
- Consider medical, medication-related, and substance-related causes.
- Review reported safety concerns.
- Identify areas requiring further professional evaluation.

### Step 6: Copy or Download the Prompt

Review the generated prompt and download it as a UTF-8 text file.

If you choose to use an external AI service, review its privacy and security requirements before transferring any patient information.

## 🧠 Clinical Scope

The application is intended to support the organization of information gathered during an initial psychiatric assessment.

Potential areas for clinical review include:

- Depressive disorders.
- Bipolar and related disorders.
- Anxiety disorders.
- Panic disorder.
- Obsessive-compulsive and related disorders.
- Trauma- and stressor-related disorders.
- Psychotic disorders.
- Substance-related disorders.
- Sleep-related concerns.
- Possible medical or neurological contributors to psychiatric symptoms.
- Other conditions identified by the treating clinician.

These categories are not diagnoses generated or confirmed by the application. The presence, absence, and significance of any disorder must be established through an appropriate clinical assessment.

The current application does not implement a validated diagnostic interview, a standardized diagnostic scoring system, or an independently validated clinical decision-support algorithm.

## 🔐 Privacy and Data Protection

Psychiatric information is highly sensitive. Protecting patient confidentiality is essential.

The application should be used in accordance with applicable healthcare privacy laws, professional standards, and institutional policies.

Recommended precautions:

- Avoid entering names, national identification numbers, phone numbers, addresses, or other unnecessary identifiers.
- Use a coded patient reference when appropriate.
- Obtain informed consent where required before using external AI services.
- Do not submit identifiable patient information to public AI services without appropriate authorization and safeguards.
- Restrict access to the application and any exported files.
- Store patient records only in approved, access-controlled environments.
- Use secure transmission and storage methods.
- Establish appropriate retention and deletion policies.
- Review third-party service terms and data-processing arrangements before integration.

**Privacy limitation:** The current version is a prototype. It does not provide a dedicated electronic health record system, user authentication, role-based access control, encrypted patient database, audit logging, or automated deletion policies. Do not treat a public GitHub repository or publicly accessible Codespace as a secure clinical record system.

## ⚠️ Clinical Safety Disclaimer

This software is provided for informational, educational, and clinical workflow support purposes.

It is not intended to:

- Provide an independent psychiatric diagnosis.
- Replace a psychiatrist or other qualified healthcare professional.
- Determine that a patient is safe solely from questionnaire responses.
- Prescribe medications or recommend individualized medication doses.
- Replace emergency services or crisis intervention.
- Serve as a validated medical device or diagnostic instrument.

Automated alerts are based on selected form responses and are not a substitute for comprehensive clinical risk assessment.

Clinical decisions must be made by appropriately qualified professionals using the complete clinical context.

## 🔧 Limitations

The current version has the following limitations:

1. The application relies on information entered by the user.
2. It does not independently verify the accuracy of patient responses.
3. It does not connect to an AI model automatically.
4. It does not calculate validated diagnostic scores.
5. It does not provide a validated risk prediction model.
6. It does not automatically distinguish all psychiatric disorders.
7. It does not include a secure, persistent patient database.
8. It does not provide clinical user authentication or access management.
9. It does not replace a structured diagnostic interview or medical examination.
10. Its clinical content and workflow require expert review before real-world clinical deployment.

## 🛣️ Future Development

Potential future improvements include:

- [ ] Adaptive interviews based on previous answers.
- [ ] More comprehensive structured diagnostic interviews.
- [ ] Validated screening instruments where licensing and usage requirements permit.
- [ ] More detailed symptom timelines and episode tracking.
- [ ] Clinician-reviewed differential diagnosis reports.
- [ ] Optional integration with an approved AI API.
- [ ] PDF clinical report generation.
- [ ] Secure patient record management.
- [ ] Authentication and role-based access control.
- [ ] Audit logging and controlled data retention.
- [ ] Improved mobile responsiveness.
- [ ] Multilingual support.
- [ ] Clinical usability testing and formal validation.

Any future diagnostic or risk-assessment functionality should undergo appropriate clinical validation and safety review before being used to inform patient care.

## 🤝 Contributing

Contributions are welcome, particularly in the following areas:

- Improving the Persian-language interface.
- Enhancing accessibility and usability.
- Improving the organization of psychiatric history.
- Reviewing clinical terminology with qualified professionals.
- Adding privacy and security controls.
- Improving software testing and documentation.

To contribute:

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Test the application.
5. Submit a pull request describing your improvements.

Clinical content changes should be reviewed by qualified mental health professionals.

## 📄 License

No license has been specified yet.

Before distributing or reusing this project, add an appropriate open-source license if you intend to permit others to use, modify, or distribute the code. Without an explicit license, the default copyright rules generally apply.

## 👨‍💻 Author

**Project:** Persian Psychiatry Assessment Assistant

**Primary language:** Python

**Interface language:** Persian (Farsi)

**Application framework:** Streamlit

## ⭐ Acknowledgments

This project explores the use of Python-based interfaces and language models to organize psychiatric intake information and support clinician-led assessment.

The goal is to improve the structure and accessibility of clinical documentation while preserving professional responsibility, patient safety, and confidentiality.

---

**Disclaimer:** This project is a prototype and is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the judgment of a qualified healthcare professional for clinical decisions.
