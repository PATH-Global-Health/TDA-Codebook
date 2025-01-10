# Codebook for Enhanced Case Management

### start_time

- **Label**: nan
- **Type**: start

### deviceid

- **Label**: nan
- **Type**: deviceid

### today

- **Label**: nan
- **Type**: today

### end_time

- **Label**: nan
- **Type**: end

### into

- **Label**: Malaria HRP Study in Ethiopia – Second phase
  Targeted drug administration in migrant workers
  Enhanced case management questionnaire
- **Type**: note

<details>
<summary><h2>Section 1:  Identification of participant and farm (group)</h2></summary>

- **Type**: begin group

### interviewer_scanned_qr_code

- **Label**: 1.1. Interviewer ID
- **Type**: barcode

### interviewer_manual_qr_code

- **Label**: 1.2. Enter manually if scanning not possible:
- **Type**: text
- **Relevant**: interviewer_scanned_qr_code = null

### interviewer_qr_code

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(interviewer_scanned_qr_code=null, interviewer_manual_qr_code, interviewer_scanned_qr_code)

### date

- **Label**: 1.3. Date
- **Type**: date

### case_detection_type

- **Label**: 1.4. Type of case detection
- **Type**: select_one case_detection_type
- **Choices**:
  - 1: Passive case detection at fix health post
  - 2: Active case detection (active fever screening at farms)

### fixed_post

- **Label**: 1.5. Farm where fix health post is
- **Type**: select_one fixed_posts
- **Relevant**: case_detection_type=1
- **Choices**:
  - 79: Mihret Amare (Block 23)
  - 94: Tesfa Worku
  - 12: Aliyas Star (Block 23)
  - 45: Eyayu Gossa
  - 4: Abebe Wuletaw
  - 29: Birhan Dessalegn (Block 18)

### current_farm_camp

- **Label**: 1.6. Name of farm camp where patient is currently working
- **Type**: select_one farm_camp
- **Relevant**: case_detection_type=1
- **Choices**:
  - 1000: Abayneh Zerfu
  - 2: Abdul Nur Juhar
  - 3000: Abebe Tessema
  - 4: Abebe Wuletaw
  - 5: Abera Bekele
  - 6: Abiderafi Agri. Develop.
  - 7000: Abitew Tefera
  - 8: Adamu Baynessagn
  - 9: Aderajew Asmamaw
  - 10000: Afera Mengistu
  - 11000: Ahmed Ibrahim
  - 13: Aliyas Star (Block 10)
  - 12: Aliyas Star (Block 23)
  - 14: Amsalu Alemu
  - 15: Asefa Mekonnen
  - 16: Asmamaw Sisay
  - 17: Atsede Atalel
  - 18: Atsede Shiferaw
  - 19: Awuraris Getaneh
  - 20000: Ayanaw Gashanaw
  - 21: Ayelign Habtie (Block 26)
  - 22000: Ayelign Habtie (Block29)
  - 23000: Ayelign Yenehun
  - 24: Ayenachew Sisay
  - 25: Ayenew Bazezew
  - 26: Ayineshet Worku
  - 27000: Bata Trading
  - 29: Birhan Dessalegn (Block 18)
  - 28000: Birhan Dessalegn (Block16)
  - 30000: Birhanie Gebru
  - 31000: Birhanie Mulusew and His friends
  - 32000: Bossena Kassi
  - 33: BS agriclture
  - 34000: Chekilu Bayehu
  - 35000: Colonel Temesgen Digndigie
  - 38: Demoz Adigeh
  - 36000: Dessie Ayele (Block16)
  - 37000: Dessie Ayele (Block31)
  - 39: Destaw Muchie
  - 40: Dr. Amsalu Debebe
  - 41: Edget Metema
  - 42: Emawos Agri. Develop.
  - 43: Eneye Birillie
  - 44000: Eneyew Belete
  - 45: Eyayu Gossa
  - 46000: Fatuma Yimam
  - 47000: Fisseha Habtie (Block29)
  - 49000: Fisseha Habtie (Hectares23)
  - 48000: Fisseha Habtie (Hectares27)
  - 50000: Gashaw Bizu
  - 51000: Gebremedhin Tesfaye
  - 52: Geger Agri. Develop.
  - 53: Getachew Tezera
  - 54: Getiye Gebru
  - 55: Guadie Alem
  - 104: Habtu Tsidu
  - 56000: Habtamu Get
  - 57000: Habtamu Woretaw
  - 59: Haile Gebremariam
  - 60: Hailemariam Melesse
  - 61000: Hussen Ahmed
  - 62: Jejaw Abrha
  - 63: Kessete Wubetu
  - 64: Kililu Woldu
  - 65000: Mahibereselassie A/Gedam
  - 66000: Mamuye Bilata
  - 67: Mariye Mengistu
  - 71: Mastewal Mazengia (Block 26)
  - 70000: Mastewal Mazengia (Block28)
  - 69: Mastewal Mazengia (Hectares 37.5)
  - 68000: Mastewal Mazengia (Hectares51)
  - 72: Mekonnen Goshe
  - 73: Mekuanint Kassie
  - 74: Melaku Dires
  - 75000: Melikie and Enana
  - 76: Melkie Taddesse
  - 77: Mezgebe Abrha
  - 79: Mihret Amare (Block 23)
  - 78000: Mihret Amare (Block29)
  - 80: Mohammed Awol
  - 81: Mulugeta Semie
  - 82: Mulugeta Zewdu
  - 83: Nigussie Mekonnen
  - 84: Sadik Nur
  - 85: Selamsew Wubetu
  - 89: Shaleka Raday Legesse
  - 86: Sintayehu Alemu
  - 87: Sisay Birhan
  - 88: Sisay Tesfahun
  - 90: Temesgen Setargew
  - 91: Terefe Ayalew
  - 93: Terefe Dargie (Block 22)
  - 92: Terefe Dargie (Block 25)
  - 94: Tesfa Worku
  - 95: Tewdros Alemayehu
  - 96: Workneh Kassie and His friends
  - 97: Workneh Maru
  - 98: Yibeltal Tesfaye
  - 99: Yibralem Belay
  - 100: Yilma Ferede
  - 101: Yitayew Beyene
  - 102: Zeleke Wubetu
  - 58000: Zenaw Wagaw
  - 777000: Other (specify)

### current_farm_camp_other

- **Label**: Specify
- **Type**: text
- **Relevant**: current_farm_camp=777000

### study_arm

- **Label**: Study arm
- **Type**: select_one study_arm
- **Relevant**: case_detection_type=2
- **Choices**:
  - 1: Intervention 1: 2 rounds TDA
  - 2: Intervention 2: 3 rounds TDA
  - 3: Control

### active_case_farm

- **Label**: 1.7. Farm where active case detection is being conducted
- **Type**: select_one farm_camp
- **Relevant**: case_detection_type=2
- **Choices**:
  - 1000: Abayneh Zerfu
  - 2: Abdul Nur Juhar
  - 3000: Abebe Tessema
  - 4: Abebe Wuletaw
  - 5: Abera Bekele
  - 6: Abiderafi Agri. Develop.
  - 7000: Abitew Tefera
  - 8: Adamu Baynessagn
  - 9: Aderajew Asmamaw
  - 10000: Afera Mengistu
  - 11000: Ahmed Ibrahim
  - 13: Aliyas Star (Block 10)
  - 12: Aliyas Star (Block 23)
  - 14: Amsalu Alemu
  - 15: Asefa Mekonnen
  - 16: Asmamaw Sisay
  - 17: Atsede Atalel
  - 18: Atsede Shiferaw
  - 19: Awuraris Getaneh
  - 20000: Ayanaw Gashanaw
  - 21: Ayelign Habtie (Block 26)
  - 22000: Ayelign Habtie (Block29)
  - 23000: Ayelign Yenehun
  - 24: Ayenachew Sisay
  - 25: Ayenew Bazezew
  - 26: Ayineshet Worku
  - 27000: Bata Trading
  - 29: Birhan Dessalegn (Block 18)
  - 28000: Birhan Dessalegn (Block16)
  - 30000: Birhanie Gebru
  - 31000: Birhanie Mulusew and His friends
  - 32000: Bossena Kassi
  - 33: BS agriclture
  - 34000: Chekilu Bayehu
  - 35000: Colonel Temesgen Digndigie
  - 38: Demoz Adigeh
  - 36000: Dessie Ayele (Block16)
  - 37000: Dessie Ayele (Block31)
  - 39: Destaw Muchie
  - 40: Dr. Amsalu Debebe
  - 41: Edget Metema
  - 42: Emawos Agri. Develop.
  - 43: Eneye Birillie
  - 44000: Eneyew Belete
  - 45: Eyayu Gossa
  - 46000: Fatuma Yimam
  - 47000: Fisseha Habtie (Block29)
  - 49000: Fisseha Habtie (Hectares23)
  - 48000: Fisseha Habtie (Hectares27)
  - 50000: Gashaw Bizu
  - 51000: Gebremedhin Tesfaye
  - 52: Geger Agri. Develop.
  - 53: Getachew Tezera
  - 54: Getiye Gebru
  - 55: Guadie Alem
  - 104: Habtu Tsidu
  - 56000: Habtamu Get
  - 57000: Habtamu Woretaw
  - 59: Haile Gebremariam
  - 60: Hailemariam Melesse
  - 61000: Hussen Ahmed
  - 62: Jejaw Abrha
  - 63: Kessete Wubetu
  - 64: Kililu Woldu
  - 65000: Mahibereselassie A/Gedam
  - 66000: Mamuye Bilata
  - 67: Mariye Mengistu
  - 71: Mastewal Mazengia (Block 26)
  - 70000: Mastewal Mazengia (Block28)
  - 69: Mastewal Mazengia (Hectares 37.5)
  - 68000: Mastewal Mazengia (Hectares51)
  - 72: Mekonnen Goshe
  - 73: Mekuanint Kassie
  - 74: Melaku Dires
  - 75000: Melikie and Enana
  - 76: Melkie Taddesse
  - 77: Mezgebe Abrha
  - 79: Mihret Amare (Block 23)
  - 78000: Mihret Amare (Block29)
  - 80: Mohammed Awol
  - 81: Mulugeta Semie
  - 82: Mulugeta Zewdu
  - 83: Nigussie Mekonnen
  - 84: Sadik Nur
  - 85: Selamsew Wubetu
  - 89: Shaleka Raday Legesse
  - 86: Sintayehu Alemu
  - 87: Sisay Birhan
  - 88: Sisay Tesfahun
  - 90: Temesgen Setargew
  - 91: Terefe Ayalew
  - 93: Terefe Dargie (Block 22)
  - 92: Terefe Dargie (Block 25)
  - 94: Tesfa Worku
  - 95: Tewdros Alemayehu
  - 96: Workneh Kassie and His friends
  - 97: Workneh Maru
  - 98: Yibeltal Tesfaye
  - 99: Yibralem Belay
  - 100: Yilma Ferede
  - 101: Yitayew Beyene
  - 102: Zeleke Wubetu
  - 58000: Zenaw Wagaw
  - 777000: Other (specify)

### gender

- **Label**: 1.8. Patient’s gender
- **Type**: select_one gender
- **Choices**:
  - 1: Male
  - 2: Female

### gender_text

- **Label**: nan
- **Type**: calculate
- **Calculate**: jr:choice-name(gender,'gender')

### age

- **Label**: 1.9. Participant age (complete years)
- **Type**: integer

### has_study_id

- **Label**: 1.10. Does this patient have a Study ID?
- **Type**: select_one has_study_id
- **Relevant**: current_farm_camp<500 or case_detection_type=2
- **Choices**:
  - 0: No
  - 1: Yes
  - 2: Yes, but he/she lost it

### study_scanned_qr_code

- **Label**: 1.11. Scan study ID
- **Type**: barcode
- **Relevant**: has_study_id=1

### study_manual_qr_code

- **Label**: 1.12. Manually enter Study ID:
- **Type**: text
- **Relevant**: has_study_id=1 and study_scanned_qr_code = null

### study_qr_code

- **Label**: nan
- **Type**: calculate
- **Relevant**: has_study_id=1
- **Calculate**: if(study_scanned_qr_code=null, study_manual_qr_code, study_scanned_qr_code)

### s1_n1

- **Label**: Interviewer ID (Q1.1) should not be the same as participant's study ID (Q1.11).
- **Type**: note
- **Relevant**: study_qr_code!=null and interviewer_qr_code!=null and study_qr_code=interviewer_qr_code

### received_tda_round

- **Label**: 1.13. Has the patient received at least one round of targeted drug administration?
- **Type**: select_one yes_no_dr
- **Relevant**: has_study_id=1 or has_study_id=2
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Doesn't know / Doesn't remember

### tda_start_date

- **Label**: 1.14. First day of treatment of the most recent TDA
- **Type**: date
- **Relevant**: received_tda_round=1

### tda_start_day

- **Label**: nan
- **Type**: calculate
- **Relevant**: received_tda_round=1
- **Calculate**: round(decimal-date-time(today()) - decimal-date-time(tda_start_date))

### remember_tda_last_date

- **Label**: Do you remember the last day of treatment of the most recent TDA

(Ask the patient if he/she took the second and third doses of the TDA and when)

- **Type**: select_one yes_no
- **Relevant**: received_tda_round=1
- **Choices**:
  - 1: Yes
  - 0: No

### tda_last_date

- **Label**: 1.15. Last day of treatment of the most recent TDA

- **Type**: date
- **Relevant**: remember_tda_last_date=1

</details>

<details>
<summary><h2>Section 2:  Fever and malaria (group)</h2></summary>

- **Type**: begin group

### fever_since_last_study_visit

- **Label**: 2.1. Does the patient report having had fever since the previous study visit?
- **Type**: select_one yes_no
- **Relevant**: case_detection_type=2 and (has_study_id=1 or has_study_id=2)
- **Choices**:
  - 1: Yes
  - 0: No

### fever_last_48h

- **Label**: 2.2. Does the patient report fever in the last 48 hours?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### axillary_temperature

- **Label**: 2.3. Axillary temperature
- **Type**: decimal

### recall_fever_start_date

- **Label**: Do you recall the date when the fever started?
- **Type**: select_one yes_no
- **Relevant**: fever_since_last_study_visit=1 or fever_last_48h=1 or axillary_temperature>=37recall_fever_start_date5
- **Choices**:
  - 1: Yes
  - 0: No

### fever_start_date

- **Label**: 2.4. Date fever started
- **Type**: date
- **Relevant**: recall_fever_start_date=1

### rdt_conducted

- **Label**: 2.5. Is a malaria rapid diagnostic test (RDT) conducted?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### rdt_result

- **Label**: 2.6. RDT result
- **Type**: select_one rdt_result
- **Relevant**: rdt_conducted=1
- **Choices**:
  - 1: Negative
  - 2: P. falciparum
  - 3: P. vivax
  - 4: Mixed (Pf+Pv)
  - 5: Invalid

### repeat_rdt

- **Label**: 2.6a. Repeat RDT
- **Type**: select_one rdt_result
- **Relevant**: rdt_result=5
- **Choices**:
  - 1: Negative
  - 2: P. falciparum
  - 3: P. vivax
  - 4: Mixed (Pf+Pv)
  - 5: Invalid

### treatment

- **Label**: 2.7. Antimalarial treatment administered
- **Type**: select_multiple treatment
- **Relevant**: rdt_result=2 or rdt_result=3 or rdt_result=4 or repeat_rdt=2 or repeat_rdt=3 or repeat_rdt=4
- **Choices**:
  - 1: Artemether-Lumefantrine (AL)
  - 2: Radical cure Primaquine
  - 3: Single low-dose Primaquine
  - 4: Chloroquine
  - 5: Dihydroartemisinin-Piperaquine
  - 777: Other (specify)

### treatment_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(treatment,'777')

### severe_malaria_symptoms

- **Label**: 2.8. Does the patient have signs or symptoms of severe malaria?
- **Type**: select_one yes_no
- **Relevant**: rdt_conducted=1
- **Choices**:
  - 1: Yes
  - 0: No

### referred_for_malaria_management

- **Label**: 2.9. Was the patient referred to a health facility for malaria case management?
- **Type**: select_one yes_no
- **Relevant**: rdt_conducted=1
- **Choices**:
  - 1: Yes
  - 0: No

### s2_n1

- **Label**: Please call the study coordinator and fill out ORA’s Incident Report Form
- **Type**: note
- **Relevant**: referred_for_malaria_management=1 and tda_start_day<30

### s2_n2

- **Label**: Please refer patient to the health facility.
- **Type**: note
- **Relevant**: severe_malaria_symptoms=1 and referred_for_malaria_management=0

</details>

<details>
<summary><h2>Section 3:  Other illnesses or medical complaints  (group)</h2></summary>

- **Type**: begin group
- **Relevant**: current_farm_camp<500 or case_detection_type=2

### other_symptoms

- **Label**: 3.1. Does the patient have other symptoms or medical complaints?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### signs_symptoms

- **Label**: 3.2. Signs and symptoms
- **Type**: select_multiple signs_symptoms
- **Relevant**: other_symptoms=1
- **Choices**:
  - 1: Urticaria (hives)
  - 2: Pruritus (itching)
  - 3: Vomiting
  - 4: Diarrhea
  - 5: Loss of appetite
  - 6: Dizziness
  - 7: Convulsions
  - 8: Malaise
  - 9: Tiredness or drowsiness
  - 10: Headache
  - 11: Abdominal pain
  - 12: Palpitations or irregular heartbeat (arrhythmia)
  - 13: Angioedema (swelling of the face, mouth, etc.)
  - 14: Joint pain
  - 15: Blurred vision
  - 16: Airway obstruction
  - 17: Dyspnea
  - 777: Other (specify)

### signs_symptoms_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(signs_symptoms,'777')

### recall_symptoms_start_date

- **Label**: Do you recall the date when the signs and symptoms began?
- **Type**: select_one yes_no
- **Relevant**: other_symptoms=1
- **Choices**:
  - 1: Yes
  - 0: No

### symptoms_start_date

- **Label**: 3.3. Date signs/symptoms started
- **Type**: date
- **Relevant**: recall_symptoms_start_date=1

### symptoms_ongoing

- **Label**: 3.4. Are the signs/symptoms still ongoing?
- **Type**: select_one yes_no
- **Relevant**: other_symptoms=1
- **Choices**:
  - 1: Yes
  - 0: No

### symptoms_end_date

- **Label**: 3.5. Date signs/symptoms ended
- **Type**: date
- **Relevant**: symptoms_ongoing=0

### severity

- **Label**: 3.6. Severity
- **Type**: select_one severity
- **Relevant**: other_symptoms=1
- **Choices**:
  - 1: Mild (causing minimal discomfort and does not interfere with normal daily activities)
  - 2: Moderate (causes some interference with daily activities but does not cause significant discomfort or require extensive medical intervention)
  - 3: Severe (causes significant discomfort, interfering with daily life and requiring medical intervention)
  - 4: Serious adverse event (Life-threatening, requires hospitalization, or leads to significant disability or death)

### s3_n1

- **Label**: Please call the study coordinator and fill out ORA’s Incident Report Form
- **Type**: note
- **Relevant**: severity=4 and tda_start_day<30

### diagnosis

- **Label**: 3.7. Main diagnosis
- **Type**: select_one diagnosis
- **Relevant**: other_symptoms=1
- **Choices**:
  - 1: Potential drug adverse event
  - 2: Acute respiratory illness
  - 3: Gastroenteritis
  - 777: Other (specify)

### diagnosis_other

- **Label**: Specify
- **Type**: text
- **Relevant**: diagnosis=777

### patient_management

- **Label**: 3.8. Management of the patient
- **Type**: select_multiple patient_management
- **Relevant**: other_symptoms=1
- **Choices**:
  - 1: Paracetamol
  - 2: Patient referred to a health facility or hospital
  - 3: No specific treatment needed
  - 777: Other (specify)

### patient_management_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(patient_management,'777')

### s3_n2

- **Label**: Please call the study coordinator and fill out ORA’s Incident Report Form
- **Type**: note
- **Relevant**: selected(patient_management,'2') and tda_start_day<30

### concomitant_medications

- **Label**: 3.9. Other concomitant medication that the patient was already taking (other than dihydroartemisinin-piperaquine administered during the TDA)
- **Type**: text
- **Relevant**: other_symptoms=1

### additional_clinical_data

- **Label**: 3.10. Additional clinical data (if needed)
- **Type**: text
- **Relevant**: other_symptoms=1

</details>

### interviewer_comments

- **Label**: Any comments?
- **Type**: text
