# RakhtSakhi Twin — Project Charter

## 1. What are we building?
A web-based decision support tool that forecasts a simulated Indian woman's
14-day risk of entering moderate anaemia (Hb < 10.9 g/dL), so a clinician
can prioritize who gets the next scarce Hb test.

## 2. Who uses it?
- Primary user: Clinic nurse / community health worker
- Secondary user: Doctor (reviews high-risk cases)
- NOT for: General public, patients self-diagnosing

## 3. What does it do?
- Shows a ranked worklist of patients by risk
- Explains WHY a patient is high risk (top 3 factors)
- Allows what-if simulation ("what if she takes iron daily?")
- Recommends: "Prioritize Hb test" or "Schedule follow-up"

## 4. What it NEVER does?
- Never diagnoses anaemia
- Never prescribes iron dosage
- Never claims definite Hb value
- Never uses real patient data
- Never replaces a blood test

## 5. What data does it use?
- Synthetic EHR (age, baseline Hb, cycle history, diet)
- Synthetic daily observations (sleep, fatigue, adherence, symptoms)
- NO real patients. NO wearables. NO sensors.

## 6. Prediction target
Binary: Will this patient enter moderate anaemia (Hb < 10.9 g/dL)
within the next 14 days? (Yes / No)

## 7. Success criteria for hackathon
- Working web app runs locally via Docker
- Risk prediction with SHAP explanation
- Clinician dashboard with worklist + what-if
- 20-min demo video
- Public GitHub repo with README + architecture