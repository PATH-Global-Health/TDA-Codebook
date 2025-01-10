# Codebook for Farm Questionnaire

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

- **Label**: Malaria HRP in Ethiopia – Second phase

Cross sectional surveys – Farm questionnaire

- **Type**: note

### interviewer_scanned_qr_code

- **Label**: 0. Interviewer ID
- **Type**: barcode

### interviewer_manual_qr_code

- **Label**: 1. Enter manually if scanning not possible:
- **Type**: text
- **Relevant**: interviewer_scanned_qr_code = null

### interviewer_qr_code

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(interviewer_scanned_qr_code=null, interviewer_manual_qr_code, interviewer_scanned_qr_code)

### study_arm

- **Label**: 2. Study arm
- **Type**: select_one study_arm
- **Choices**:
  - 1: Intervention 1: 2 rounds TDA
  - 2: Intervention 2: 3 rounds TDA
  - 3: Control

### farm_camp_code

- **Label**: 3. Name of farm camp
- **Type**: select_one farm_camp
- **Choices**:
  - 2: Abdul Nur Juhar
  - 4: Abebe Wuletaw
  - 5: Abera Bekele
  - 6: Abiderafi Agri. Develop.
  - 8: Adamu Baynessagn
  - 9: Aderajew Asmamaw
  - 13: Aliyas Star (Block 10)
  - 12: Aliyas Star (Block 23)
  - 14: Amsalu Alemu
  - 15: Asefa Mekonnen
  - 16: Asmamaw Sisay
  - 17: Atsede Atalel
  - 18: Atsede Shiferaw
  - 19: Awuraris Getaneh
  - 21: Ayelign Habtie (Block 26)
  - 24: Ayenachew Sisay
  - 25: Ayenew Bazezew
  - 26: Ayineshet Worku
  - 29: Birhan Dessalegn (Block 18)
  - 33: BS agriclture
  - 38: Demoz Adigeh
  - 39: Destaw Muchie
  - 40: Dr. Amsalu Debebe
  - 41: Edget Metema
  - 42: Emawos Agri. Develop.
  - 43: Eneye Birillie
  - 45: Eyayu Gossa
  - 52: Geger Agri. Develop.
  - 53: Getachew Tezera
  - 54: Getiye Gebru
  - 55: Guadie Alem
  - 104: Habtu Tsidu
  - 59: Haile Gebremariam
  - 60: Hailemariam Melesse
  - 62: Jejaw Abrha
  - 63: Kessete Wubetu
  - 64: Kililu Woldu
  - 67: Mariye Mengistu
  - 71: Mastewal Mazengia (Block 26)
  - 69: Mastewal Mazengia (Hectares 37.5)
  - 72: Mekonnen Goshe
  - 73: Mekuanint Kassie
  - 74: Melaku Dires
  - 76: Melkie Taddesse
  - 77: Mezgebe Abrha
  - 79: Mihret Amare (Block 23)
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

### farm_camp_name

- **Label**: nan
- **Type**: calculate
- **Calculate**: jr:choice-name(farm_camp_code,'farm_camp_code')

### farm_manager_name

- **Label**: 4. Name and last name of the farm manager
- **Type**: text

### respondent_last_name

- **Label**: 5. Name and last name of respondent
- **Type**: text

### respondent_role

- **Label**: 6. Role of the respondent
- **Type**: select_one role
- **Choices**:
  - 1: Farm owner
  - 2: Farm manager
  - 3: Farm delegate
  - 777: Other

### respondent_role_other

- **Label**: Specify role of the respondent
- **Type**: text
- **Relevant**: selected(respondent_role,'777')

### contact_info

- **Label**: 7. Contact information
- **Type**: text

### farm_agri_worker_count

- **Label**: 8. How many agricultural workers are there at this farm?
- **Type**: integer

### seasonal_migrant_worker_count

- **Label**: 9. How many of these agricultural workers are seasonal migrant agricultural workers?
- **Type**: integer

### crop

- **Label**: 10. What type of crop is cultivated at this farm
- **Type**: select_multiple crop
- **Choices**:
  - 1: Sesame
  - 2: Sorghum
  - 3: Cotton
  - 4: Soya beans
  - 777: Other (Specify)

### crop_specify

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(crop,'777')

### migrant_worker_sleep_structure

- **Label**: 11. In what type of sleeping structure do the seasonal migrant agricultural workers sleep in?
- **Type**: select_multiple sleep_structure
- **Choices**:
  - 1: Permanent traditional structure (mud walls, thatched roofs, Corrugated iron and earth floors, open eaves, no ceiling and no screening)
  - 2: Modern structure (iron roof, burnt brick or cement walls and cement floor)
  - 3: Informal structure (reed walls, thatch or tarp roof) (Gibaza)
  - 4: Tent
  - 5: No structure, sleep outdoors
  - 777: Other (Specify)

### migrant_worker_sleep_structure_specify

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(migrant_worker_sleep_structure,'777')

### last_wall_spray_date

- **Label**: 12. When was the last time that the interior walls of the sleeping structures at the farm were sprayed against mosquitos?
- **Type**: select_one last_wall_spray_date
- **Relevant**: selected(migrant_worker_sleep_structure,'1') or selected(migrant_worker_sleep_structure,'2') or selected(migrant_worker_sleep_structure,'3') or selected(migrant_worker_sleep_structure,'777')
- **Choices**:
  - 1: Never been sprayed
  - 2: Less than a year
  - 3: One year ago or longer
  - 888: Don't know
  - 999: Decline to answer

### no_spray_reason

- **Label**: 13. Why were the structures not sprayed with insecticide within the last 12 months?
- **Type**: select_multiple no_spray_reason
- **Relevant**: last_wall_spray_date=1 or last_wall_spray_date=3
- **Choices**:
  - 1: The  spray operators did not come
  - 2: We don't have any malaria in this village/neighborhood
  - 3: Spraying program not implemented here
  - 777: Other (specify)
  - 888: Don't know
  - 999: Decline to answer

### no_spray_reason_specify

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(no_spray_reason,'777')

### standing_water_nearby_farm

- **Label**: 14. Is there standing water nearby the farm?
- **Type**: select_one yes_no_dn
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Don't know

### gps

- **Label**: 15. GPS coordinates
- **Type**: geopoint

### interviewer_comments

- **Label**: Any comments?
- **Type**: text
