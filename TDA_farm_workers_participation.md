# Codebook for Farm Workers' Participation Form

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

- **Label**: Malaria HRP Study in Ethiopia- Second phase
  Farm Workers' Participation form
  Survey and TDA
- **Type**: note

### info

- **Label**: INSTRUCTIONS: This form should be filled only ONCE PER STUDY VISIT PER FARM and at the end of all activities in the farm camp .

This form should be filled and send by the TDA team.

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

### date

- **Label**: 4. Date
- **Type**: date

### activity_filter

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(study_arm=1,20,if(study_arm=2, 19, 40))

### study_activity

- **Label**: 5. Enter the study activity
- **Type**: select_one study_activity
- **Choices**:
  - 1: TDA1
  - 2: TDA 2
  - 3: TDA 3

### current_farm_workers

- **Label**: 6. How many farm workers are currently working in this farm
- **Type**: integer

### farm_workers_not_in_study

- **Label**: 7. How many farm workers currently working in this farm were not found in the study visit(s)?
- **Type**: integer
