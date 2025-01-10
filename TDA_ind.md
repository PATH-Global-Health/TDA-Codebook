# Codebook for baseline and endline survey

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
  Targeted drug administration in farm workers
  Individual survey questionnaire
- **Type**: note

<details>
<summary><h2>Section 1: Identification of interviewer and farm (group)</h2></summary>

- **Type**: begin group

### s1_n1

- **Label**: Section 1: Identification of interviewer and farm
- **Type**: note

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

### study_arm

- **Label**: 1.4. Study arm
- **Type**: select_one study_arm
- **Choices**:
  - 1: Intervention 1: 2 rounds TDA
  - 2: Intervention 2: 3 rounds TDA
  - 3: Control

### farm_camp_code

- **Label**: 1.5. Name of farm camp
- **Type**: select_one farm_camp
- **Choices**:
  - 1000: Abayneh Zerfu - (Asefa Mekonnen)
  - 2: Abdul Nur Juhar - (Nega Juar)
  - 3000: Abebe Tessema
  - 4: Abebe Wuletaw - (Aragie Mirkuzie)
  - 5: Abera Bekele - (Sitotaw Agegnehu)
  - 6: Abiderafi Agri. Develop. - (Teku G/selasie)
  - 7000: Abitew Tefera
  - 8: Adamu Baynessagn - (Samuel Ayalew)
  - 9: Aderajew Asmamaw - (Gashaw Adisu)
  - 10000: Afera Mengistu - (Afera)
  - 11000: Ahmed Ibrahim - (Ahmed Ibrahim)
  - 13: Aliyas Star (Block 10) - (Birhanu Abebe)
  - 12: Aliyas Star (Block 23) - (Endalk Adane)
  - 14: Amsalu Alemu - (Muluye Endalew)
  - 15: Asefa Mekonnen - (Endris Kassahun)
  - 16: Asmamaw Sisay - (Asmamaw Sisay)
  - 17: Atsede Atalel - (Bewuket Yenealem Baye)
  - 18: Atsede Shiferaw - (Azanaw Adigo Negashe)
  - 19: Awuraris Getaneh - (Tsegaye Ngusie)
  - 20000: Ayanaw Gashanaw - (Ayanaw)
  - 21: Ayelign Habtie (Block 26) - (Fikiremichael Ayelign)
  - 22000: Ayelign Habtie (Block29) - (Ayelign Habtie)
  - 23000: Ayelign Yenehun - (Ayelign Yenehun)
  - 24: Ayenachew Sisay - (Adane Ayalew)
  - 25: Ayenew Bazezew - (Habetamu Gidey)
  - 26: Ayineshet Worku - (Eyayaw Getawn)
  - 27000: Bata Trading
  - 29: Birhan Dessalegn (Block 18) - (Tesifaye Weday Meniberu)
  - 28000: Birhan Dessalegn (Block16) - (Tesfaye)
  - 30000: Birhanie Gebru - (Habitu)
  - 31000: Birhanie Mulusew and His friends - (Birhanie)
  - 32000: Bossena Kassi - (Bossena)
  - 33: BS agriclture - (Muz Mihretie Ferede)
  - 34000: Chekilu Bayehu - (Chekilu Bayehu)
  - 35000: Colonel Temesgen Digndigie
  - 38: Demoz Adigeh - (Bisetegen Ashagra Tasew)
  - 36000: Dessie Ayele (Block16) - (Dessie)
  - 37000: Dessie Ayele (Block31) - (Dessie)
  - 39: Destaw Muchie - (Abebu Mengistie)
  - 40: Dr. Amsalu Debebe - (Gebire Debas Demeke)
  - 41: Edget Metema - (Dessie Achenef)
  - 42: Emawos Agri. Develop. - (Muz Miheret)
  - 43: Eneye Birillie - (Solomon Belay)
  - 44000: Eneyew Belete - (Eneyew)
  - 45: Eyayu Gossa - (Asfaw Eyayu)
  - 46000: Fatuma Yimam - (Biruke)
  - 47000: Fisseha Habtie (Block29) - (Fisseha Habtie)
  - 49000: Fisseha Habtie (Hectares23) - (Fisseha Habtie)
  - 48000: Fisseha Habtie (Hectares27) - (Fisseha Habtie)
  - 50000: Gashaw Bizu - (Gashaw)
  - 51000: Gebremedhin Tesfaye - (Yerega)
  - 52: Geger Agri. Develop. - (Melkamu kasegen)
  - 53: Getachew Tezera - (Negash Zenaw)
  - 54: Getiye Gebru - (Mesfin Abeje Atanaw)
  - 55: Guadie Alem - (Moges Guadie)
  - 56000: Habtamu Get - (Habtamu)
  - 57000: Habtamu Woretaw - (Habtamu)
  - 104: Habtu Tsidu - (Belay Tadie)
  - 59: Haile Gebremariam - (Ferede Enyew)
  - 60: Hailemariam Melesse - (Surafel Fentahun )
  - 61000: Hussen Ahmed - (Hussen)
  - 62: Jejaw Abrha - (Abebe. Fantahun)
  - 63: Kessete Wubetu - (Wolde Aragie Yirdaw)
  - 64: Kililu Woldu - (Solomon Aderagew)
  - 65000: Mahibereselassie A/Gedam
  - 66000: Mamuye Bilata - (Gedefaw)
  - 67: Mariye Mengistu - (Wendimnew Getnet)
  - 71: Mastewal Mazengia (Block 26) - (Temesgen Atalay Gebeyehu)
  - 70000: Mastewal Mazengia (Block28) - (Mastewal Mazengia)
  - 69: Mastewal Mazengia (Hectares 37.5) - (Kiflie Mazengia)
  - 68000: Mastewal Mazengia (Hectares51) - (Mastewal Mazengia)
  - 72: Mekonnen Goshe - (Mandie Teketayi)
  - 73: Mekuanint Kassie - (Dejen Worku)
  - 74: Melaku Dires - (Nigus. Dejen)
  - 75000: Melikie and Enana
  - 76: Melkie Taddesse - (Ayanaw Alebel)
  - 77: Mezgebe Abrha - (Birara Mengistie)
  - 79: Mihret Amare (Block 23) - (Eshetu Muluken)
  - 78000: Mihret Amare (Block29) - (Mihret Amare)
  - 80: Mohammed Awol - (Mohamed Abole)
  - 81: Mulugeta Semie - (Kifilie Magenigiya Zenebe)
  - 82: Mulugeta Zewdu - (Solomon Woldie Desie)
  - 83: Nigussie Mekonnen - (Nigussie Mekonnen)
  - 777000: Other (specify)
  - 84: Sadik Nur - (Fitalew Tekilu)
  - 85: Selamsew Wubetu - (Workeneh Kibertu Bera)
  - 89: Shaleka Raday Legesse - (Marye Tilahun Kebede)
  - 86: Sintayehu Alemu - (Sintayehu Alemu)
  - 87: Sisay Birhan - (Kasahun Awoke Kebebew)
  - 88: Sisay Tesfahun - (Amsayaw Sisay Tesfahun)
  - 90: Temesgen Setargew - (Wube Getu)
  - 91: Terefe Ayalew - (Chilot Abye)
  - 93: Terefe Dargie (Block 22) - (Baye Alemiye)
  - 92: Terefe Dargie (Block 25) - (Terefe Dargie)
  - 94: Tesfa Worku - (Tsegachw Abebe Shumeye)
  - 95: Tewdros Alemayehu - (Benyam Negash)
  - 96: Workneh Kassie and His friends - (Moges Shumie)
  - 97: Workneh Maru - (Amsalu Marew)
  - 98: Yibeltal Tesfaye - (Nigus Getnet Alemu)
  - 99: Yibralem Belay - (Biniam Negash)
  - 100: Yilma Ferede - (Aragie Abebe)
  - 101: Yitayew Beyene - (Molla Asmare Askenawu)
  - 102: Zeleke Wubetu - (Mengaw Tadesse)
  - 58000: Zenaw Wagaw - (Zenaw Wagaw)

### farm_camp_name

- **Label**: nan
- **Type**: calculate
- **Calculate**: jr:choice-name(farm_camp_code,'farm_camp_code')

### survey_filter

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(round(decimal-date-time(today()) - decimal-date-time(date('2024-09-15')))<0,1,2)

### survey

- **Label**: 1.6. Survey
- **Type**: select_one survey
- **Choices**:
  - 1: Baseline
  - 2: Endline

</details>

<details>
<summary><h2>Section 2: Participant’s eligibility and consent (group)</h2></summary>

- **Type**: begin group

### s2_n1

- **Label**: Section 2: Participant’s eligibility and consent
- **Type**: note

### gender

- **Label**: 2.1. Participant gender
- **Type**: select_one gender
- **Choices**:
  - 1: Male
  - 2: Female

### age

- **Label**: 2.2. Participant age
- **Type**: integer

### s2_end_survey_2_2

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(age<14,1,0)

### s2_n2

- **Label**: This individual does not meet eligibility criteria to participate in the survey.

Please thank them for their time and end the interview.

- **Type**: note
- **Relevant**: s2_end_survey_2_2=1

### guardian_at_farm

- **Label**: 2.3. Is a parent or guardian at the farm and able to provide informed consent for the participant?
- **Type**: select_one yes_no
- **Relevant**: s2_end_survey_2_2 = 0 and age>=14 and age<18
- **Choices**:
  - 1: Yes
  - 0: No

### s2_end_survey_2_3

- **Label**: nan
- **Type**: calculate
- **Relevant**: s2_end_survey_2_2=0
- **Calculate**: if(age>=14 and age<18 andguardian_at_farm=0,1,0)

### s2_n3

- **Label**: This individual does not meet eligibility criteria to participate in the survey.

Please thank them for their time and end the interview.

- **Type**: note
- **Relevant**: s2_end_survey_2_3=1

### occupation

- **Label**: 2.4. What is your current primary occupation?
- **Type**: select_one occupation
- **Relevant**: s2_end_survey_2_3=0
- **Choices**:
  - 1: Seasonal agricultural worker
  - 2: Other (specify)

### occupation_other

- **Label**: Specify occupation
- **Type**: text
- **Relevant**: occupation=2

### s2_end_survey_2_4

- **Label**: nan
- **Type**: calculate
- **Relevant**: s2_end_survey_2_3=0
- **Calculate**: if(occupation=2,1,0)

### s2_n4

- **Label**: This individual does not meet eligibility criteria to participate in the survey.

Please thank them for their time and end the interview.

- **Type**: note
- **Relevant**: s2_end_survey_2_4=1

### time_at_farm

- **Label**: 2.5. How long have you been working in Delelo farm camps?
- **Type**: select_one time_at_farm
- **Relevant**: s2_end_survey_2_4=0
- **Choices**:
  - 1: Less than 4 weeks
  - 2: More than 4 weeks

### antimalarials_given_without_testing_last_4_weeks

- **Label**: 2.5a. In the last 4 weeks since you arrived in Delello, did you work in any farm camps where antimalarial drugs were given to all farm workers without testing?
- **Type**: select_one yes_no
- **Relevant**: time_at_farm=1
- **Choices**:
  - 1: Yes
  - 0: No

### s2_end_survey_2_5

- **Label**: nan
- **Type**: calculate
- **Relevant**: s2_end_survey_2_4=0
- **Calculate**: if(survey=2 and antimalarials_given_without_testing_last_4_weeks=0,1,0)

### s2_n5

- **Label**: This individual does not meet eligibility criteria to participate in the survey.

Please thank them for their time and end the interview.

- **Type**: note
- **Relevant**: s2_end_survey_2_5=1

### recent_arrival_date

- **Label**: 2.6. Date of most recent arrival at this farm
- **Type**: date
- **Relevant**: s2_end_survey_2_5=0

### is_recent_arrival_date_correct_1

- **Label**: nan
- **Type**: calculate
- **Relevant**: s2_end_survey_2_5=0
- **Calculate**: if(time_at_farm=1 and round(decimal-date-time(today()) - decimal-date-time(date(recent_arrival_date)))<=30,1,0)

### is_recent_arrival_date_correct_2

- **Label**: nan
- **Type**: calculate
- **Relevant**: s2_end_survey_2_5=0
- **Calculate**: if(time_at_farm=2 and round(decimal-date-time(today()) - decimal-date-time(date(recent_arrival_date)))>30,1,0)

### error_recent_arrival_date_1

- **Label**: Recent arrival date must be within the last 4 weeks.
- **Type**: note
- **Relevant**: time_at_farm=1 and is_recent_arrival_date_correct_1=0

### error_recent_arrival_date_2

- **Label**: Recent arrival date must be over 4 weeks ago.
- **Type**: note
- **Relevant**: time_at_farm=2 and is_recent_arrival_date_correct_2=0

### severely_ill

- **Label**: 2.6a. Is this participant severely ill?
- **Type**: select_one yes_no
- **Relevant**: s2_end_survey_2_5=0
- **Choices**:
  - 1: Yes
  - 0: No

### s2_end_survey_2_6_a

- **Label**: nan
- **Type**: calculate
- **Relevant**: s2_end_survey_2_5=0
- **Calculate**: if(severely_ill=1,1,0)

### s2_n6

- **Label**: This individual does not meet eligibility criteria to participate in the survey.

Please thank them for their time and end the interview.

- **Type**: note
- **Relevant**: s2_end_survey_2_6_a=1

### s2_n7

- **Label**: INFORMED CONSENT
  Read the information sheet and obtain consent from the participant and make sure they understand the information. The participant needs to sign TWO copies of the Informed consent/Assent Form, one will be given to him/her and the other one will be kept for study records.
- **Type**: note
- **Relevant**: s2_end_survey_2_6_a=0

### consent_today

- **Label**: 2.7. Has the participant provided consent to participate today?
- **Type**: select_one yes_no
- **Relevant**: s2_end_survey_2_6_a=0 and age>=18
- **Choices**:
  - 1: Yes
  - 0: No

### assent_today

- **Label**: 2.8. Has the participant provided assent to participate today?
- **Type**: select_one yes_no
- **Relevant**: s2_end_survey_2_6_a=0 and age>=14 and age<18
- **Choices**:
  - 1: Yes
  - 0: No

### guardian_consent_today

- **Label**: 2.9. Has the parent/legal guardian provided consent for the minor to participate today?
- **Type**: select_one yes_no
- **Relevant**: assent_today=1
- **Choices**:
  - 1: Yes
  - 0: No

### s2_end_survey_c

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(severely_ill=1,1,if(age<14,1,if(age>=14 and age<18 and guardian_at_farm=0,1,if(occupation=2,1,if(survey=2 and antimalarials_given_without_testing_last_4_weeks=0,1,if( age>=18 and consent_today=0,1,if(age>=14 and age<18 and assent_today=0,1,if(age>=14 and age<18 and assent_today=1 and guardian_consent_today=0,1,0))))))))

### sample_scanned_qr_code

- **Label**: 2.10. Assign a Sample QR code to the participant. Stick one copy on the Recruitment Form, another one on the Informed Consent, and the third one on the DBS card
- **Type**: barcode
- **Relevant**: s2_end_survey_c=0

### sample_manual_qr_code

- **Label**: 2.11. Manually enter Sample QR code number
- **Type**: text
- **Relevant**: s2_end_survey_c=0 and sample_scanned_qr_code=null

### sample_qr_code

- **Label**: nan
- **Type**: calculate
- **Relevant**: s2_end_survey_c=0
- **Calculate**: if(sample_scanned_qr_code=null, sample_manual_qr_code, sample_scanned_qr_code)

### label_recruitment_form

- **Label**: 2.12. Did you fill out and label the Recruitment Form with the participant’s Sample QR?
- **Type**: select_one yes_no
- **Relevant**: s2_end_survey_c=0
- **Choices**:
  - 1: Yes
  - 0: No

### label_informed_consent

- **Label**: 2.13. Did you label the Informed Consent with the participant’s Sample QR code?
- **Type**: select_one yes_no
- **Relevant**: s2_end_survey_c=0
- **Choices**:
  - 1: Yes
  - 0: No

### label_dbs_card

- **Label**: 2.14. Did you label the DBS card with the participant’s Sample QR code?
- **Type**: select_one yes_no
- **Relevant**: s2_end_survey_c=0
- **Choices**:
  - 1: Yes
  - 0: No

### has_study_id

- **Label**: 2.15. Does this participant already have a Study ID?
- **Type**: select_one yes_no_lt
- **Relevant**: s2_end_survey_c=0 and survey=2
- **Choices**:
  - 1: Yes
  - 0: No
  - 2: Yes, but he / she lost it

<details>
<summary><h2>Retrieve Study ID (group)</h2></summary>

- **Type**: begin group
- **Relevant**: has_study_id=2

### check_study_id_note

- **Label**: Retrieve Study ID using the SearchID app if participant was registered with his/her name/last name at previous TDA rounds.
- **Type**: note

### search_study_id

- **Label**: Search Study ID
- **Type**: text

</details>

### find_study_id

- **Label**: 2.15a. Have you been able to find the participant in the SearchID app and retrieve the Study ID that was previously assigned?
- **Type**: select_one yes_no
- **Relevant**: has_study_id=2
- **Choices**:
  - 1: Yes
  - 0: No

<details>
<summary><h2>Participant's Study ID (group)</h2></summary>

- **Type**: begin group
- **Relevant**: s2_end_survey_c=0 and (survey=1 or (survey=2 and has_study_id=1 ))

### s2_n8

- **Label**: Assign participant a Study ID and scan it
- **Type**: note
- **Relevant**: survey=1

### s2_n9

- **Label**: Scan participant’s Study ID
- **Type**: note
- **Relevant**: survey=2 and has_study_id=1

### study_scanned_qr_code

- **Label**: 2.16. Participant’s Study ID
- **Type**: barcode
- **Relevant**: (survey=1 or (survey=2 and has_study_id=1 ))

</details>

### study_manual_qr_code

- **Label**: 2.17. Manually enter Study ID
- **Type**: text
- **Relevant**: s2_end_survey_c=0 and (survey=1 or (survey=2 and (has_study_id=1 or find_study_id=1) )) and study_scanned_qr_code=null

### study_qr_code

- **Label**: nan
- **Type**: calculate
- **Relevant**: s2_end_survey_c=0
- **Calculate**: if(study_scanned_qr_code=null, study_manual_qr_code, study_scanned_qr_code)

### s2_n10

- **Label**: Interviewer ID (Q1.1) should not be the same as participant's study ID (Q2.16).
- **Type**: note
- **Relevant**: study_qr_code!=null and interviewer_qr_code!=null and study_qr_code=interviewer_qr_code

### returned_home_this_year

- **Label**: 2.18. Have you returned home any-time after first arriving at a farm since July?
- **Type**: select_one yes_no
- **Relevant**: s2_end_survey_c=0 and survey=2
- **Choices**:
  - 1: Yes
  - 0: No

### other_farms_july_to_now

- **Label**: 2.19. Have you worked at other farms between July and now?
- **Type**: select_one yes_no
- **Relevant**: s2_end_survey_c=0 and survey=2
- **Choices**:
  - 1: Yes
  - 0: No

### num_other_farms_since_july

- **Label**: 2.20. How many other farms have you worked at since July?
- **Type**: integer
- **Relevant**: other_farms_july_to_now=1

<details>
<summary><h2>Farms visited (repeat)</h2></summary>

- **Type**: begin repeat
- **Relevant**: num_other_farms_since_july>0

### pos

- **Label**: nan
- **Type**: calculate
- **Calculate**: position(..)

### other_farm

- **Label**: 2.21. Which farm?
- **Type**: select_one farm_camp
- **Relevant**: pos<=num_other_farms_since_july
- **Choices**:
  - 1000: Abayneh Zerfu - (Asefa Mekonnen)
  - 2: Abdul Nur Juhar - (Nega Juar)
  - 3000: Abebe Tessema
  - 4: Abebe Wuletaw - (Aragie Mirkuzie)
  - 5: Abera Bekele - (Sitotaw Agegnehu)
  - 6: Abiderafi Agri. Develop. - (Teku G/selasie)
  - 7000: Abitew Tefera
  - 8: Adamu Baynessagn - (Samuel Ayalew)
  - 9: Aderajew Asmamaw - (Gashaw Adisu)
  - 10000: Afera Mengistu - (Afera)
  - 11000: Ahmed Ibrahim - (Ahmed Ibrahim)
  - 13: Aliyas Star (Block 10) - (Birhanu Abebe)
  - 12: Aliyas Star (Block 23) - (Endalk Adane)
  - 14: Amsalu Alemu - (Muluye Endalew)
  - 15: Asefa Mekonnen - (Endris Kassahun)
  - 16: Asmamaw Sisay - (Asmamaw Sisay)
  - 17: Atsede Atalel - (Bewuket Yenealem Baye)
  - 18: Atsede Shiferaw - (Azanaw Adigo Negashe)
  - 19: Awuraris Getaneh - (Tsegaye Ngusie)
  - 20000: Ayanaw Gashanaw - (Ayanaw)
  - 21: Ayelign Habtie (Block 26) - (Fikiremichael Ayelign)
  - 22000: Ayelign Habtie (Block29) - (Ayelign Habtie)
  - 23000: Ayelign Yenehun - (Ayelign Yenehun)
  - 24: Ayenachew Sisay - (Adane Ayalew)
  - 25: Ayenew Bazezew - (Habetamu Gidey)
  - 26: Ayineshet Worku - (Eyayaw Getawn)
  - 27000: Bata Trading
  - 29: Birhan Dessalegn (Block 18) - (Tesifaye Weday Meniberu)
  - 28000: Birhan Dessalegn (Block16) - (Tesfaye)
  - 30000: Birhanie Gebru - (Habitu)
  - 31000: Birhanie Mulusew and His friends - (Birhanie)
  - 32000: Bossena Kassi - (Bossena)
  - 33: BS agriclture - (Muz Mihretie Ferede)
  - 34000: Chekilu Bayehu - (Chekilu Bayehu)
  - 35000: Colonel Temesgen Digndigie
  - 38: Demoz Adigeh - (Bisetegen Ashagra Tasew)
  - 36000: Dessie Ayele (Block16) - (Dessie)
  - 37000: Dessie Ayele (Block31) - (Dessie)
  - 39: Destaw Muchie - (Abebu Mengistie)
  - 40: Dr. Amsalu Debebe - (Gebire Debas Demeke)
  - 41: Edget Metema - (Dessie Achenef)
  - 42: Emawos Agri. Develop. - (Muz Miheret)
  - 43: Eneye Birillie - (Solomon Belay)
  - 44000: Eneyew Belete - (Eneyew)
  - 45: Eyayu Gossa - (Asfaw Eyayu)
  - 46000: Fatuma Yimam - (Biruke)
  - 47000: Fisseha Habtie (Block29) - (Fisseha Habtie)
  - 49000: Fisseha Habtie (Hectares23) - (Fisseha Habtie)
  - 48000: Fisseha Habtie (Hectares27) - (Fisseha Habtie)
  - 50000: Gashaw Bizu - (Gashaw)
  - 51000: Gebremedhin Tesfaye - (Yerega)
  - 52: Geger Agri. Develop. - (Melkamu kasegen)
  - 53: Getachew Tezera - (Negash Zenaw)
  - 54: Getiye Gebru - (Mesfin Abeje Atanaw)
  - 55: Guadie Alem - (Moges Guadie)
  - 56000: Habtamu Get - (Habtamu)
  - 57000: Habtamu Woretaw - (Habtamu)
  - 104: Habtu Tsidu - (Belay Tadie)
  - 59: Haile Gebremariam - (Ferede Enyew)
  - 60: Hailemariam Melesse - (Surafel Fentahun )
  - 61000: Hussen Ahmed - (Hussen)
  - 62: Jejaw Abrha - (Abebe. Fantahun)
  - 63: Kessete Wubetu - (Wolde Aragie Yirdaw)
  - 64: Kililu Woldu - (Solomon Aderagew)
  - 65000: Mahibereselassie A/Gedam
  - 66000: Mamuye Bilata - (Gedefaw)
  - 67: Mariye Mengistu - (Wendimnew Getnet)
  - 71: Mastewal Mazengia (Block 26) - (Temesgen Atalay Gebeyehu)
  - 70000: Mastewal Mazengia (Block28) - (Mastewal Mazengia)
  - 69: Mastewal Mazengia (Hectares 37.5) - (Kiflie Mazengia)
  - 68000: Mastewal Mazengia (Hectares51) - (Mastewal Mazengia)
  - 72: Mekonnen Goshe - (Mandie Teketayi)
  - 73: Mekuanint Kassie - (Dejen Worku)
  - 74: Melaku Dires - (Nigus. Dejen)
  - 75000: Melikie and Enana
  - 76: Melkie Taddesse - (Ayanaw Alebel)
  - 77: Mezgebe Abrha - (Birara Mengistie)
  - 79: Mihret Amare (Block 23) - (Eshetu Muluken)
  - 78000: Mihret Amare (Block29) - (Mihret Amare)
  - 80: Mohammed Awol - (Mohamed Abole)
  - 81: Mulugeta Semie - (Kifilie Magenigiya Zenebe)
  - 82: Mulugeta Zewdu - (Solomon Woldie Desie)
  - 83: Nigussie Mekonnen - (Nigussie Mekonnen)
  - 777000: Other (specify)
  - 84: Sadik Nur - (Fitalew Tekilu)
  - 85: Selamsew Wubetu - (Workeneh Kibertu Bera)
  - 89: Shaleka Raday Legesse - (Marye Tilahun Kebede)
  - 86: Sintayehu Alemu - (Sintayehu Alemu)
  - 87: Sisay Birhan - (Kasahun Awoke Kebebew)
  - 88: Sisay Tesfahun - (Amsayaw Sisay Tesfahun)
  - 90: Temesgen Setargew - (Wube Getu)
  - 91: Terefe Ayalew - (Chilot Abye)
  - 93: Terefe Dargie (Block 22) - (Baye Alemiye)
  - 92: Terefe Dargie (Block 25) - (Terefe Dargie)
  - 94: Tesfa Worku - (Tsegachw Abebe Shumeye)
  - 95: Tewdros Alemayehu - (Benyam Negash)
  - 96: Workneh Kassie and His friends - (Moges Shumie)
  - 97: Workneh Maru - (Amsalu Marew)
  - 98: Yibeltal Tesfaye - (Nigus Getnet Alemu)
  - 99: Yibralem Belay - (Biniam Negash)
  - 100: Yilma Ferede - (Aragie Abebe)
  - 101: Yitayew Beyene - (Molla Asmare Askenawu)
  - 102: Zeleke Wubetu - (Mengaw Tadesse)
  - 58000: Zenaw Wagaw - (Zenaw Wagaw)

### specify_other_farm

- **Label**: Specify names of other farm(s)
- **Type**: text
- **Relevant**: other_farm=777000

### other_farm_name

- **Label**: nan
- **Type**: calculate
- **Relevant**: pos<=num_other_farms_since_july
- **Calculate**: if(other_farm=777000, specify_other_farm, jr:choice-name(other_farm,'other_farm'))

### work_months_farm

- **Label**: 2.22. When did you work at ${other_farm_name}
- **Type**: select_multiple work_months_farm
- **Relevant**: pos<=num_other_farms_since_july
- **Choices**:
  - 1: July
  - 2: August
  - 3: September
  - 4: October
  - 5: November

### farms_visited_note_1

- **Label**: Data collection for farm ${other_farm_name} completed
- **Type**: note
- **Relevant**: pos<=num_other_farms_since_july

</details>

</details>

<details>
<summary><h2>Section 3:  Sociodemographic (group)</h2></summary>

- **Type**: begin group
- **Relevant**: s2_end_survey_c=0

### s3_n1

- **Label**: Section 3: Sociodemographic
- **Type**: note

### other_occupations

- **Label**: 3.1. Besides your current work as a seasonal worker, what other occupations do you do?
- **Type**: select_multiple other_occupation
- **Choices**:
  - 1: Agricultural worker in permanent residence area
  - 2: Cattle herder
  - 3: Professional/technical/managerial
  - 4: Teacher
  - 5: Student/learner
  - 6: Small business/retail
  - 7: Government staff
  - 8: Private security personnel
  - 9: Construction
  - 10: Housewife
  - 11: No other work
  - 777: Other: Specify:

### other_occupations_specify

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(other_occupations,'777')

### highest_education_level

- **Label**: 3.2. What is the highest level of education that the participant has completed?
- **Type**: select_one highest_education_level
- **Choices**:
  - 1: No formal education
  - 2: Primary school (1-6 grade)
  - 3: Secondary school (7-12 grade)
  - 4: University/College
  - 777: Other (specify)
  - 888: Don’t know

### highest_education_level_other

- **Label**: Specify
- **Type**: text
- **Relevant**: highest_education_level=777

### spoken_languages

- **Label**: 3.3. What languages do you speak and understand?
- **Type**: select_multiple language
- **Choices**:
  - 1: Amharic
  - 2: English
  - 3: Tigrigna
  - 4: Arabic
  - 777: Other (specify)

### spoken_languages_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(spoken_languages,'777')

### citizen

- **Label**: 3.4. Of what country are you a citizen?
- **Type**: select_one country
- **Choices**:
  - 1: Ethiopia
  - 2: Eritrea
  - 3: Djibouti
  - 4: Somalia
  - 5: Sudan
  - 6: South Sudan
  - 7: Kenya
  - 777: Other (specify)

### citizen_other

- **Label**: Specify
- **Type**: text
- **Relevant**: citizen=777

### years_in_ethiopia

- **Label**: 3.5. For how many years have you been in Ethiopia?
- **Type**: select_one years_in_ethiopia
- **Relevant**: citizen>1
- **Choices**:
  - 1: Less than one year
  - 2: One year or more

### main_residence_metema

- **Label**: 3.6. Is your main place of residence (i.e., where you maintain a household and live most of the year) in this district (Metema)?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### main_residence_kebele_metema

- **Label**: 3.7. What is your village (Kebele) of main residence within Metema district?
- **Type**: select_one kebele_in_metema
- **Relevant**: main_residence_metema=1
- **Choices**:
  - 1: Achera
  - 2: Agam Wuha
  - 3: Ashamit
  - 4: Awasa
  - 5: Das
  - 6: Delelo
  - 7: Diviko
  - 8: Gaje
  - 9: Genda-Weha
  - 10: Gubay
  - 11: Gundo
  - 12: Kemechela
  - 13: Kokit
  - 14: Kumer Aftit
  - 15: Kushara
  - 16: Lemlem Terara
  - 17: Lencha
  - 18: Meka
  - 19: Mender 6 7 8
  - 20: Mesha
  - 21: Shashige
  - 22: Shemelegra
  - 23: Shinfa
  - 24: Tagure
  - 25: Tumet
  - 26: Wondabeso
  - 27: Zebach-Bahir
  - 777: Other (Specify)

### main_residence_kebele_metema_specify

- **Label**: Specify
- **Type**: text
- **Relevant**: main_residence_kebele_metema=777

### main_residence_country

- **Label**: 3.8. If this district (Metema) is not your main place of residence, where is your main residence?

Country:

- **Type**: select_one country
- **Relevant**: main_residence_metema=0
- **Choices**:
  - 1: Ethiopia
  - 2: Eritrea
  - 3: Djibouti
  - 4: Somalia
  - 5: Sudan
  - 6: South Sudan
  - 7: Kenya
  - 777: Other (specify)

### main_residence_country_specify

- **Label**: Specify:
- **Type**: text
- **Relevant**: main_residence_country=777

### main_residence_region

- **Label**: 3.8. If this district (Metema) is not your main place of residence, where is your main residence?

Region:

- **Type**: select_one region
- **Relevant**: main_residence_metema=0
- **Choices**:
  - 1: Addis Ababa
  - 2: Afar
  - 3: Amhara
  - 4: Benishangul Gumuz
  - 5: Dire Dawa
  - 6: Gambela
  - 7: Harari
  - 8: Oromia
  - 9: Sidama
  - 10: Somali
  - 11: South West Ethiopia
  - 12: SNNP
  - 13: Tigray
  - 14: Maekel
  - 15: Anseba
  - 16: Gash-Barka
  - 17: Debub
  - 18: Northern Red Sea
  - 19: Southern Red Sea
  - 20: Djibouti City
  - 21: Ali Sabieh
  - 22: Arta
  - 23: Dikhil
  - 24: Tadjoura
  - 25: Obock
  - 26: Bakool (Hudur)
  - 27: Banadir (Mogadisho)
  - 28: Bari (Bosaso)
  - 29: Bay (Baidoa)
  - 30: Galgaduud (Dhusamareb)
  - 31: Gedo (Garbahaarreey)
  - 32: Hiiraan (Beledweyn)
  - 33: Lower Juba (Kismayo)
  - 34: Lower Shabelle (Merca)
  - 35: Middle Juba (Bu'ale)
  - 36: Middle Shebelle (Jowhar)
  - 37: Mudug (Galkayo)
  - 38: Nugal (Garowe)
  - 39: Awdal
  - 40: Maroodi Jeex
  - 41: Sahil
  - 42: Sanaag
  - 43: Sool
  - 44: Togdheer
  - 45: Khartoum
  - 46: North Kordofan
  - 47: Northern
  - 48: Kassala
  - 49: Blue Nile
  - 50: North Darfur
  - 51: South Darfur
  - 52: South Kordofan
  - 53: Al Jazirah
  - 54: White Nile
  - 55: River Nile
  - 56: Red Sea
  - 57: Al Qadarif
  - 58: Sennar
  - 59: West Darfur
  - 60: Central Darfur
  - 61: East Darfur
  - 62: West Kordofan
  - 63: Bahr el Ghazal
  - 64: Equatoria
  - 65: Greater Upper Nile
  - 66: Nairobi
  - 67: Central
  - 68: Coast
  - 69: Eastern
  - 70: North Eastern
  - 71: Nyanza
  - 72: Rift Valley
  - 73: Western
  - 777: Other (Specify)

### main_residence_region_specify

- **Label**: Specify:
- **Type**: text
- **Relevant**: main_residence_region=777

### main_residence_zone

- **Label**: 3.8. If this district (Metema) is not your main place of residence, where is your main residence?

Zone:

- **Type**: select_one zone
- **Relevant**: main_residence_country=1 and main_residence_region!=777
- **Choices**:
  - 1: North Western
  - 2: Central
  - 3: Eastern
  - 4: Southern
  - 5: Western
  - 6: South Eastern
  - 7: Mekelle
  - 8: Awsi /Zone 1
  - 9: Kilbati /Zone2
  - 10: Gabi /Zone 3
  - 11: Fanti /Zone 4
  - 12: Hari /Zone 5
  - 24: West Gondar
  - 23: Central Gondar
  - 13: North Gondar
  - 14: South Gondar
  - 15: North Wello
  - 16: South Wello
  - 17: North Shewa (AM)
  - 18: East Gojam
  - 19: West Gojam
  - 20: Wag Hamra
  - 21: Awi
  - 22: Oromia
  - 25: West Wellega
  - 26: East Wellega
  - 27: Ilu Aba Bora
  - 28: Jimma
  - 29: West Shewa
  - 30: North Shewa (OR)
  - 31: East Shewa
  - 32: Arsi
  - 33: West Hararge
  - 34: East Hararge
  - 35: Bale
  - 36: Borena
  - 37: South West Shewa
  - 38: Guji
  - 39: West Guji
  - 40: Buno Bedele
  - 41: West Arsi
  - 42: Kelem Wellega
  - 43: Horo Gudru Wellega
  - 44: Finfine Special
  - 45: East Bale
  - 46: Siti
  - 47: Fafan
  - 48: Jarar
  - 49: Erer
  - 50: Korahe
  - 51: Shabelle
  - 52: Doolo
  - 53: Afder
  - 54: Liban
  - 55: Nogob
  - 56: Daawa
  - 57: Metekel
  - 58: Assosa
  - 59: Kamashi
  - 60: Mao Komo Special
  - 61: Guraghe
  - 62: Hadiya
  - 63: Kembata Tembaro
  - 64: Gedeo
  - 65: Wolayita
  - 66: South Omo
  - 67: Gamo
  - 68: Alle
  - 69: Konso
  - 70: Halaba
  - 71: Gofa
  - 72: Basketo
  - 73: Siltie
  - 74: Amaro
  - 75: Burji
  - 76: Derashe
  - 77: Yem Special
  - 78: Sheka
  - 79: Kefa
  - 80: Bench Sheko
  - 81: Dawuro
  - 82: Mirab Omo
  - 83: Konta Special
  - 84: Nuwer
  - 85: Agnewak
  - 86: Majang
  - 87: Itang Special woreda
  - 88: Harari
  - 89: Region 14
  - 90: Dire Dawa urban
  - 91: Dire Dawa rural
  - 92: Sidama
  - 777: Other (Specify)

### main_residence_woreda

- **Label**: 3.8. If this district (Metema) is not your main place of residence, where is your main residence?

District (Woreda):

- **Type**: select_one woreda
- **Relevant**: main_residence_country=1 and main_residence_region<777
- **Choices**:
  - 1: Tahtay Adiyabo
  - 2: Laelay Adiabo
  - 3: Zana
  - 4: Tahtay Koraro
  - 5: Asgede
  - 6: Tselemti
  - 7: Sheraro town
  - 8: Indasilassie town
  - 9: Selekleka
  - 10: Seyemti Adyabo
  - 11: Adi Daero
  - 12: Adi Hageray
  - 13: Tsimbla
  - 14: Endabaguna town
  - 15: Dima (TG)
  - 16: May Tsebri town
  - 17: Chila
  - 18: Aheferom
  - 19: Edaga arbi
  - 20: Adwa
  - 21: Laelay Maychew
  - 22: Tahtay Mayechew
  - 23: Adet
  - 24: Kola Temben
  - 25: Naeder
  - 26: Abergele (TG)
  - 27: Abi Adi town
  - 28: Adwa town
  - 29: Axum town
  - 30: Rama
  - 31: Ahsea
  - 32: Egela
  - 33: Hahayle
  - 34: Endafelasi
  - 35: Emba Sieneti
  - 36: Enticho town
  - 37: Keyhe tekli
  - 38: Tanqua Melashe
  - 39: Gulo Mekeda
  - 40: Erob
  - 41: Saesie
  - 42: Ganta Afeshum
  - 43: Hawzen
  - 44: Kelete Awelallo
  - 45: Atsbi
  - 46: Adigrat town
  - 47: Wukro town
  - 48: Bizet
  - 49: Edaga Hamus town
  - 50: Hawzen town
  - 51: Freweyni town
  - 52: Tsaeda Emba
  - 53: Atsbi town
  - 54: Agulae
  - 55: Geraleta
  - 56: Zala Anbesa town
  - 57: Selewa
  - 58: Bora (TG)
  - 59: Neqsege
  - 60: Emba Alaje
  - 61: Endamehoni
  - 62: Raya Azebo
  - 63: Raya Alamata
  - 64: Ofla
  - 65: Maichew town
  - 66: Korem town
  - 67: Alamata town
  - 68: Mekhoni town
  - 69: Zata
  - 70: Chercher
  - 71: Kafta Humera
  - 72: Welkait
  - 73: Tsegede (TG)
  - 74: Setit Humera
  - 75: May Kadra
  - 76: Dansha town
  - 77: Awra (TG)
  - 78: Korarit
  - 79: May Gaba
  - 80: Saharti
  - 81: Enderta
  - 82: Hintalo
  - 83: Degua Temben
  - 84: Hagere Selam town
  - 85: Samre
  - 86: Adigudom
  - 87: Wajirat
  - 88: Mekelle
  - 89: Dubti
  - 90: Elidar
  - 91: Asayita
  - 92: Afambo
  - 93: Mile
  - 94: Chifra
  - 95: Dubti town
  - 96: Kori
  - 97: Adar
  - 98: Gerani
  - 99: Asayita town
  - 100: Samera Logiya town
  - 101: Erebti
  - 102: Kunneba
  - 103: Abaala
  - 104: Megale
  - 105: Berahile
  - 106: Dalol
  - 107: Afdera
  - 108: Bidu
  - 109: Abaala town
  - 110: Amibara
  - 111: Awash
  - 112: Gewane
  - 113: Dulecha
  - 114: Gelalu
  - 115: Arguba
  - 116: Hanruka
  - 117: Awash town
  - 118: Awra (AF)
  - 119: Euwa
  - 120: Teru
  - 121: Yalo
  - 122: Gulina
  - 123: Telalek
  - 124: Samurobi
  - 125: Dawe
  - 126: Dalefage
  - 127: Hadelela
  - 128: Addi Arekay
  - 129: Beyeda
  - 130: Janamora
  - 131: Debark
  - 132: Dabat
  - 133: Dabat town
  - 134: Telemt
  - 135: Debark town
  - 136: Ebenat
  - 137: Libokemekem
  - 138: Fogera
  - 139: Farta
  - 140: Lay Gayint
  - 141: Tach Gayint
  - 142: Semada
  - 143: East Esite
  - 144: Dera (AM)
  - 145: Debre Tabor town
  - 146: Andabet/ West Esite
  - 147: Guna Begemider
  - 148: Mena Meketewa
  - 149: Sede Muja
  - 150: Nefas Mewicha town
  - 151: Wegeda town
  - 152: Ebenat town
  - 153: Hamusit town
  - 154: Woreta town
  - 155: Mekan Eyesuse
  - 156: Adiss Zemen town
  - 157: Bugna
  - 158: Raya Kobo
  - 159: Gidan
  - 160: Meket
  - 161: Wadla
  - 162: Hara town
  - 163: Guba Lafto
  - 164: Habru
  - 165: Woldiya town
  - 166: Lasta
  - 167: Dawunt
  - 168: Gazo
  - 169: Angot
  - 170: Filakit town
  - 171: Gashena town
  - 172: Mersa town
  - 173: Lalibela town
  - 174: Kobo town
  - 175: Argoba
  - 176: Tenta
  - 177: Kutaber
  - 178: Ambasel
  - 179: Thehulederie
  - 180: Delanta
  - 181: Kalu
  - 182: Albuko
  - 183: Dessie Zuria
  - 184: Legambo
  - 185: Sayint
  - 186: Borena /Debresina
  - 187: Kelela
  - 188: Jama
  - 189: Were Ilu
  - 190: Wegde
  - 191: Kombolcha town
  - 192: Dessie town
  - 193: Mehal Sayint
  - 194: Legehida
  - 195: Mekdela
  - 196: Worebabu
  - 197: Wereilu town
  - 198: Wegel tena town
  - 199: Degolo town
  - 200: Kelala town
  - 201: Akeseta town
  - 202: Tulu Awlia
  - 203: Harbu town
  - 204: Mekane Selame
  - 205: Hike town
  - 206: Mida Woremo
  - 207: Merhabete
  - 208: Ensaro
  - 209: Moretna Jiru
  - 210: Menze Gera Midir
  - 211: Gishe Rabel
  - 212: Antsokiya
  - 213: Eferatana Gidem
  - 214: Menze Mama Midir
  - 215: Tarema Ber
  - 216: Mojan Wedera
  - 217: Kewet
  - 218: Angolelana Tera
  - 219: Assagirt
  - 220: Ankober
  - 221: Hagere Mariam
  - 222: Berehet
  - 223: Minjar Shenkora
  - 224: Basona Worena
  - 225: Debre Berhan town
  - 226: Menze Keya Gabriel
  - 227: Menze Lalo Midir
  - 228: Siya Debirna Wayu
  - 229: Tulefa town
  - 230: Arerti town
  - 231: Molale town
  - 232: Debre Sina town
  - 233: Shoa Robit
  - 234: Mehale Meda town
  - 235: Ataye town
  - 236: Aleme Ketma town
  - 237: Bibugn
  - 238: Hulet Ej Enese
  - 239: Goncha Siso Enebse
  - 240: Enebse Sarmder
  - 241: Enarj Enawga
  - 242: Enemay
  - 243: Debay Telatgen
  - 244: Debre Elias
  - 245: Michakel
  - 246: Guzamn
  - 247: Baso Liben
  - 248: Awabel
  - 249: Dejen
  - 250: Shebel Bernta
  - 251: Debre Markos town
  - 252: Senan
  - 253: Aneded
  - 254: Amanuel town
  - 255: Sedae
  - 256: Gundwoin town
  - 257: Debrework town
  - 258: Lumame town
  - 259: Merto Lemariyam town
  - 260: Mota Town
  - 261: Dejen town
  - 262: Bechena Town
  - 263: Semen Achefer
  - 264: Bahirdar Zuria
  - 265: Yilmana Densa
  - 266: Mecha
  - 267: Sekela
  - 268: Quarit
  - 269: Dega Damot
  - 270: Dembecha
  - 271: Jabi Tehnan
  - 272: Bure (AM)
  - 273: Wemberma
  - 274: Bahir Dar town
  - 275: Debub Achefer
  - 276: Finote Selam town
  - 277: Debub Mecha
  - 278: Shendi town
  - 279: Denbecha town
  - 280: Gonje
  - 281: Dure Bete
  - 282: Jiga town
  - 283: Merawi town
  - 284: Bure town
  - 285: Adete town
  - 286: Zequala
  - 287: Sekota
  - 288: Dehana
  - 289: Gaz Gibla
  - 290: Abergele (AM)
  - 291: Sahila
  - 292: Sekota town
  - 293: Tsagbeji
  - 294: Amde Work town
  - 295: Dangila
  - 296: Banja
  - 297: Ankasha
  - 298: Guangua
  - 299: Fagta Lakoma
  - 300: Jawi
  - 301: Guagusa Shikudad
  - 302: Ayehu Guwagusa
  - 303: Agew Gimija Bet
  - 304: Adiss Kidame town
  - 305: Tilili town
  - 306: Fendika town
  - 307: Injibara town
  - 308: Zigem
  - 309: Dangila town
  - 310: Chagni town
  - 311: Dewa Cheffa
  - 312: Bati
  - 313: Jilye Tumuga
  - 314: Artuma Fursi
  - 315: Dewa Harewa
  - 316: Kemisie town
  - 317: Chef Robit town
  - 318: Senbete town
  - 319: Bati Town
  - 320: Amba Giorgis town
  - 321: Shawra town
  - 322: Kolla Debba town
  - 323: Chilga 1
  - 324: Tegede
  - 325: Lay Armacho
  - 326: Wegera
  - 327: Gonder Zuria
  - 328: East Dembia
  - 329: Chilga 2
  - 330: Alefa
  - 331: West Belesa
  - 332: East Belesa
  - 333: Gondar town
  - 334: Masero Denb /Central Armacho
  - 335: Tach Armacho
  - 336: Takusa
  - 337: Kinfaz Begela
  - 338: West Dembiya
  - 339: Aykel town
  - 340: Adagn Ager Chaqo
  - 341: Mirab Armacho
  - 342: Metema
  - 343: Quara
  - 344: Midre Genet
  - 345: Metema Yohanes town
  - 346: Gendawuha town
  - 347: Mana Sibu
  - 348: Nejo
  - 349: Gimbi
  - 350: Lalo Asabi
  - 351: Kiltu Kara
  - 352: Boji Dirmeji
  - 353: Ayira
  - 354: Jarso (West Wellega)
  - 355: Gudetu Kondole
  - 356: Boji Chekorsa
  - 357: Babo
  - 358: Yubdo
  - 359: Gaji
  - 360: Haru
  - 361: Nole Kaba
  - 362: Begi
  - 363: Homa
  - 364: Sayo Nole
  - 365: Guliso
  - 366: Gimbi town
  - 367: Leta Sibu
  - 368: Mendi town
  - 369: Nejo town
  - 370: Limu (OR)
  - 371: Ibantu
  - 372: Gida Ayana
  - 373: Haro Limu
  - 374: Boneya Boshe
  - 375: Wayu Tuka
  - 376: Bila Seyo
  - 377: Gobu Seyo
  - 378: Sibu Sire
  - 379: Diga
  - 380: Sasiga
  - 381: Leka Dulecha
  - 382: Guto Gida
  - 383: Jimma Arjo
  - 384: Nunu Kumba
  - 385: Wama Hagalo
  - 386: Kiremu
  - 387: Nekemte town
  - 388: Darimu
  - 389: Alge Sachi
  - 390: Yayu
  - 391: Metu Zuria
  - 392: Ale
  - 393: Bure (OR)
  - 394: Sale Nono
  - 395: Becho (Ilu Aba Bora)
  - 396: Bilo Nopha
  - 397: Hurumu
  - 398: Didu
  - 399: Halu /Huka
  - 400: Metu town
  - 401: Dorani
  - 402: Limu Seka
  - 403: Limu Kosa
  - 404: Sekoru
  - 405: Tiro Afeta
  - 406: Kersa (Jimma)
  - 407: Mena (Jimma)
  - 408: Goma
  - 409: Gera
  - 410: Seka Chekorsa
  - 411: Dedo
  - 412: Omo Nada
  - 413: Sigmo
  - 414: Setema
  - 415: Shebe Sambo
  - 416: Chora (Jimma)
  - 417: Gumay
  - 418: Agaro town
  - 419: Jimma town
  - 420: Mancho
  - 421: Omo Beyam
  - 422: Botor Tolay
  - 423: Nono Benja
  - 424: Illu Galan
  - 425: Ginde Beret
  - 426: Jeldu
  - 427: Ambo Zuria
  - 428: Mida Kegn
  - 429: Cheliya
  - 430: Bako Tibe
  - 431: Dano
  - 432: Nono
  - 433: Tikur Enchini
  - 434: Dendi
  - 435: Ejere /Addis Alem
  - 436: Adda Berga
  - 437: Meta Robi
  - 438: Ambo town
  - 439: Abuna Ginde Beret
  - 440: Toke Kutaye
  - 441: Jibat
  - 442: Ifata
  - 443: Ejersa Lafo
  - 444: Cobi
  - 445: Meta Walkite
  - 446: Liban Jawi
  - 447: Wara Jarso
  - 448: Dera (OR)
  - 449: Hidabu Abote
  - 450: Kuyu
  - 451: Degem
  - 452: Gerar Jarso
  - 453: Debre Libanos
  - 454: Wuchale
  - 455: Abichugna Gne'a
  - 456: Kimbibit
  - 457: Fiche town
  - 458: Yaya Gulele
  - 459: Jida
  - 460: Aleltu
  - 461: Fentale
  - 462: Boset
  - 463: Adama
  - 464: Lome (OR)
  - 465: Gimbichu
  - 466: Ada'a
  - 467: Dugda
  - 468: Adama Tulu Jido Kombolcha
  - 469: Bishoftu town
  - 470: Bora (OR)
  - 471: Liben Chukala
  - 472: Adama town
  - 473: Mojo Town
  - 474: Metehara town
  - 475: Merti
  - 476: Aseko
  - 477: Golocha
  - 478: Jeju
  - 479: Dodota
  - 480: Ziway Dugda
  - 481: Hitosa
  - 482: Sude
  - 483: Chole
  - 484: Amigna
  - 485: Seru
  - 486: Robe
  - 487: Tena
  - 488: Shirka
  - 489: Degeluna Tijo
  - 490: Tiyo
  - 491: Munessa
  - 492: Limu Bilbilo
  - 493: Guna
  - 494: Sire
  - 495: Lude Hitosa
  - 496: Diksis
  - 497: Bele Gesgar
  - 498: Inkolo Wabe
  - 499: Asela town
  - 500: Shanan Kolu
  - 501: Bekoji town
  - 502: Mieso
  - 503: Doba
  - 504: Tulo (OR)
  - 505: Mesela
  - 506: Chiro town
  - 507: Anchar
  - 508: Goba Koricha
  - 509: Habro
  - 510: Daro Lebu
  - 511: Boke
  - 512: Kuni /Oda Bultum
  - 513: Gemechis
  - 514: Chiro Zuria
  - 515: Bedesa
  - 516: Hawi Gudina
  - 517: Gumbi Bordede
  - 518: Burqua Dhintu
  - 519: Babile town
  - 520: Kombolcha
  - 521: Jarso (East Hararghe)
  - 522: Gursum (OR)
  - 523: Babile (OR)
  - 524: Fedis
  - 525: Haro Maya
  - 526: Kurfa Chele
  - 527: Kersa (East Hararge)
  - 528: Meta
  - 529: Goro Gutu
  - 530: Deder
  - 531: Melka Balo
  - 532: Bedeno
  - 533: Midhaga Tola
  - 534: Chinaksen
  - 535: Girawa
  - 536: Golo Oda
  - 537: Meyu Muleke
  - 538: Haromaya town
  - 539: Goro Muti
  - 540: Deder town
  - 541: Kumbi
  - 542: Aweday town
  - 543: Agarfa
  - 544: Gasera
  - 545: Sinana
  - 546: Goba (OR)
  - 547: Harena Buluk
  - 548: Mena (Bale)
  - 549: Meda Welabu
  - 550: Berbere
  - 551: Gura Damole
  - 552: Goro (Bale)
  - 553: Robe Town
  - 554: Goba town
  - 555: Dinsho
  - 556: Yabelo
  - 557: Arero
  - 558: Moyale (OR)
  - 559: Dire
  - 560: Teltale
  - 561: Miyo
  - 562: Dilo
  - 563: Dhas
  - 564: Gomole
  - 565: Guchi
  - 566: Dubluk
  - 567: Elwaya
  - 568: Yabelo town
  - 569: Wachile
  - 570: Ameya
  - 571: Wenchi
  - 572: Waliso
  - 573: Dawo
  - 574: Ilu
  - 575: Kersana Malima
  - 576: Tole
  - 577: Becho (SW Shewa)
  - 578: Seden Sodo
  - 579: Woliso town
  - 580: Goro (SW Shewa)
  - 581: Sodo Daci
  - 582: Uraga
  - 583: Bore
  - 584: Adola
  - 585: Wadera
  - 586: Odo Shakiso
  - 587: Liben
  - 588: Dama
  - 589: Arda Jila
  - 590: Girja /Harenfema
  - 591: Ana Sora
  - 592: Saba Boru
  - 593: Gora Dola
  - 594: Negele town
  - 595: Aga Wayu
  - 596: Haro Walabu
  - 597: Adola town
  - 598: Gumi Idalo
  - 599: Shakiso town
  - 600: Bule Hora
  - 601: Kercha
  - 602: Hambela Wamena
  - 603: Abaya
  - 604: Dugda Dawa
  - 605: Gelana (West Guji)
  - 606: Melka Soda
  - 607: Bule Hora town
  - 608: Suro Berguda
  - 609: Birbirsa Kojowa
  - 610: Chora (Buno Bedele)
  - 611: Dega
  - 612: Dabo Hana
  - 613: Gechi
  - 614: Borecha
  - 615: Dedesa
  - 616: Meko
  - 617: Bedele town
  - 618: Bedele Zuria
  - 619: Chwaka
  - 620: Dodola town
  - 621: Siraro
  - 622: Shala
  - 623: Arsi Negele
  - 624: Kofele
  - 625: Kore
  - 626: Gedeb Asasa
  - 627: Dodola
  - 628: Kokosa
  - 629: Nenesebo
  - 630: Adaba
  - 631: Shashemene town
  - 632: Shashemene Zuria
  - 633: Heban Arsi
  - 634: Wondo
  - 635: Bishan Guracha
  - 636: Arsi Negele town
  - 637: Hawa Galan
  - 638: Yama Logi Welel
  - 639: Dale Wabera
  - 640: Gawo Kebe
  - 641: Sayo
  - 642: Denbi Dollo town
  - 643: Anfilo
  - 644: Dale Sadi
  - 645: Gidami
  - 646: Jimma Horo
  - 647: Lalo Kile
  - 648: Sedi Chenka
  - 649: Horo
  - 650: Shambu town
  - 651: Guduru
  - 652: Ababo
  - 653: Abay Chomen
  - 654: Jimma Genete
  - 655: Jimma Rare
  - 656: Jarte Jardega
  - 657: Amuru
  - 658: Abe Dongoro
  - 659: Choman Guduru
  - 660: Horo Buluk
  - 661: Burayu
  - 662: Lege Tafo-Lege Dadi town
  - 663: Sululta town
  - 664: Sebeta Hawas
  - 665: Dukem
  - 666: Sebeta town
  - 667: Bereh
  - 668: Akaki
  - 669: Sululta
  - 670: Welmera
  - 671: Mulo
  - 672: Sendafa town
  - 673: Holeta town
  - 674: Gelana (Finfine)
  - 675: Gololcha Bale
  - 676: Lege Hida
  - 677: Ginir
  - 678: Rayitu
  - 679: Seweyna
  - 680: Dawe Ketchen
  - 681: Ginir town
  - 682: Ayisha
  - 683: Dembel
  - 684: Shinile
  - 685: Erer (SM)
  - 686: Afdem
  - 687: Hadhagala
  - 688: Miesso
  - 689: Gota-Biki
  - 690: Gablalu
  - 691: Gursum (SM)
  - 692: Babile (SM)
  - 693: Shabeeley
  - 694: Aw-Bare
  - 695: Kebribeyah
  - 696: Harshin
  - 697: Tuliguled
  - 698: Goljano
  - 699: Jigjiga town
  - 700: Wajale town
  - 701: Kebribayah town
  - 702: Koran /Mulla
  - 703: Haroreys
  - 704: Harawo
  - 705: Degehamedo
  - 706: Degehabur
  - 707: Aware
  - 708: Gashamo
  - 709: Gunagado
  - 710: Bilcil-Bur
  - 711: Degahabur town
  - 712: Yocale
  - 713: Daror
  - 714: Burqod
  - 715: Ararso
  - 716: Dig
  - 717: Fik
  - 718: Salahad
  - 719: Hamero
  - 720: Lagahida
  - 721: Meyumuluka
  - 722: Qubi
  - 723: Yahob
  - 724: Wangey
  - 725: Shaygosh
  - 726: Kebridehar
  - 727: Shilabo
  - 728: Debeweyin
  - 729: Marsin
  - 730: Kebridehar town
  - 731: Goglo
  - 732: Lasdhankayre
  - 733: Higloley
  - 734: El-Ogaden
  - 735: Bodaley
  - 736: East Imi
  - 737: Adadle
  - 738: Danan
  - 739: Gode
  - 740: Kelafo
  - 741: Mustahil
  - 742: Ferfer
  - 743: Berocano
  - 744: Godey town
  - 745: Elale
  - 746: Aba-Korow
  - 747: Danod
  - 748: Bokh
  - 749: Galadi
  - 750: Warder
  - 751: Daratole
  - 752: Lehel-Yucub
  - 753: Galhamur
  - 754: Charati
  - 755: Elkare /Serer
  - 756: West Imi
  - 757: Hargele
  - 758: Barey
  - 759: Dolobay
  - 760: Raso
  - 761: Kohle /Qoxle
  - 762: God-God
  - 763: Filtu
  - 764: Dolo Ado
  - 765: Goro Baqaqsa
  - 766: Guradamole
  - 767: Deka Suftu
  - 768: Bokolmayo
  - 769: Ayun
  - 770: Elwayne
  - 771: Garbo
  - 772: Sagag
  - 773: Dihun
  - 774: Horshagah
  - 775: Hararey
  - 776: Moyale (SM)
  - 777: Hudet
  - 778: Mubarek
  - 779: Qada Duma
  - 780: Gilgel Beles town
  - 781: Dangur
  - 782: Guba
  - 783: Wembera
  - 784: Mandura
  - 785: Dibate
  - 786: Pawe
  - 787: Bulen
  - 788: Menge
  - 789: Kurmuk
  - 790: Assosa
  - 791: Sherkole
  - 792: Bambasi
  - 793: Bilidigilu
  - 794: Homosha
  - 795: Undulu
  - 796: Assosa town Administration
  - 797: Kamashi town
  - 798: Zayi
  - 799: Sedal
  - 800: Kamashi
  - 801: Dembe
  - 802: Mizyiga
  - 803: Maokomo Special
  - 804: Kebena
  - 805: Abeshege
  - 806: Ezha
  - 807: Gedebano Gutazer Welene
  - 808: Sodo
  - 809: Meskan
  - 810: Mareko
  - 811: Endiguagn
  - 812: Gumer
  - 813: Cheha
  - 814: Enemor Ener
  - 815: Muhur Na Aklil
  - 816: Geta
  - 817: Welkite town
  - 818: Butajira town
  - 819: Emdebir town
  - 820: Bui town
  - 821: Misrak Meskan
  - 822: Debub Sodo
  - 823: Enor Ener
  - 824: Misha
  - 825: Gombora
  - 826: Lemmo
  - 827: Shashogo
  - 828: Misrak Badawacho
  - 829: Soro
  - 830: Duna
  - 831: Analemmo
  - 832: Mirab Badowach
  - 833: Gibe
  - 834: Hosaena town
  - 835: Shone Town
  - 836: Gimbichu town
  - 837: Jajura town
  - 838: Ameka
  - 839: Siraro Badawacho
  - 840: Mirab Soro
  - 841: Tembaro
  - 842: Angacha
  - 843: Kediada Gambela
  - 844: Kacha Bira
  - 845: Hadero Tunto
  - 846: Doyogena
  - 847: Damboya
  - 848: Durame town
  - 849: Adilo
  - 850: Shinshincho town
  - 851: Hadero town
  - 852: Wenago
  - 853: Yirgachefe
  - 854: Kochere
  - 855: Bule
  - 856: Dila Zuria
  - 857: Gedeb
  - 858: Dila town
  - 859: Chelelektu town
  - 860: Rape
  - 861: Churso
  - 862: Gedeb town
  - 863: Yirgachefe town
  - 864: Boloso Sore
  - 865: Damot Gale
  - 866: Damot Woide
  - 867: Humbo
  - 868: Sodo Zuria
  - 869: Kindo Koyesha
  - 870: Ofa
  - 871: Boloso Bombe
  - 872: Damot Sore
  - 873: Kindo Daddaye
  - 874: Damot Pullasa
  - 875: Duguna Fango
  - 876: Sodo Town
  - 877: Areka town
  - 878: Boditi town
  - 879: Tebela town
  - 880: Gesuba town
  - 881: Gununo Hamus town
  - 882: Hobicha Abaya
  - 883: Kawo Koisha
  - 884: Abela Abaya
  - 885: Bayera Koisha
  - 886: Salamago
  - 887: South Ari
  - 888: North Ari
  - 889: Hamer
  - 890: Bena Tsemay
  - 891: Dasenech /Kuraz
  - 892: Malie
  - 893: Nyngatom
  - 894: Jinka town
  - 895: Boko Dawula
  - 896: Wub Ari
  - 897: Selamber town
  - 898: Boreda
  - 899: Mirab Abaya
  - 900: Chencha Zuriya
  - 901: Ezo /Kogota
  - 902: Dita
  - 903: Daramalo
  - 904: Chencha
  - 905: Kemba
  - 906: Kemba town
  - 907: Gerese
  - 908: Bonke
  - 909: Arba Minch Zuria
  - 910: Gacho Baba
  - 911: Kucha Alpha
  - 912: Garda Marta
  - 913: Kucha
  - 914: Arba Minch town
  - 915: Alle Special
  - 916: Karat town
  - 917: Segen Zuria
  - 918: Karat Zuria
  - 919: Kena
  - 920: Kulito town
  - 921: Wera
  - 922: Atote Ulo
  - 923: Wera Djo
  - 924: Melekoza
  - 925: Denba Gofa
  - 926: Zala
  - 927: Uba Debre Tsehay
  - 928: Gezei Gofa
  - 929: O'yida
  - 930: Sawla town
  - 931: Bulike town
  - 932: Melo Gada
  - 933: Basketo SP Woreda
  - 934: Alicho Woriro
  - 935: Siltie
  - 936: Lanfero
  - 937: Mierab Azenet Berbere
  - 938: Dalocha
  - 939: Sankura
  - 940: Misrak Azenet Berbere
  - 941: Wulbareg
  - 942: Tora town
  - 943: Worabe town
  - 944: Kibet town
  - 945: Mito
  - 946: Misrak Siltie
  - 947: Amaro
  - 948: Burji Special
  - 949: Derashe Special
  - 950: Yem SP Woreda
  - 951: Anderacha
  - 952: Masha
  - 953: Yeki
  - 954: Tepi
  - 955: Masha town
  - 956: Saylem
  - 957: Gesha
  - 958: Gewata
  - 959: Gimbo
  - 960: Adiyio
  - 961: Tullo
  - 962: Cheta
  - 963: Decha
  - 964: Chena
  - 965: Bita
  - 966: Bonga town
  - 967: Goba (SP)
  - 968: Shisho Ande
  - 969: Wacha
  - 970: Sheko
  - 971: Gurafereda
  - 972: Debub Bench
  - 973: Shay Bench
  - 974: Semen Bench
  - 975: Gidi Bench
  - 976: Mizan Aman town
  - 977: Size town
  - 978: Tocha
  - 979: Mareka
  - 980: Loma
  - 981: Gena
  - 982: Isara
  - 983: Kachi
  - 984: Tercha Zuriya
  - 985: Mari Mansa
  - 986: Disa
  - 987: Zabagazo
  - 988: Tercha town
  - 989: Gesa town
  - 990: Gachit
  - 991: Menit Goldiye
  - 992: Gori Gesha
  - 993: Menit Shasha
  - 994: Bero
  - 995: Surma
  - 996: Maji
  - 997: Konta
  - 998: Akobo
  - 999: Lare
  - 1000: Jikawo
  - 1001: Wantawo
  - 1002: Makuey
  - 1003: Gambela National Park
  - 1004: Abobo
  - 1005: Gambela Zuria
  - 1006: Gog
  - 1007: Jore
  - 1008: Dima (GM)
  - 1009: Gambela town
  - 1010: Godere
  - 1011: Mengesh
  - 1012: Itang
  - 1013: Sofi
  - 1014: Shenkor
  - 1015: Jinela
  - 1016: Hakim
  - 1017: Erer (HR)
  - 1018: Dire Teyara
  - 1019: Amir Nur
  - 1020: Aboker
  - 1021: Abadir
  - 1022: Akaki Kality
  - 1023: Nifas Silk Lafto
  - 1024: Kolfe Keraniyo
  - 1025: Bole
  - 1026: Lideta
  - 1027: Kirkos
  - 1028: Yeka
  - 1029: Addis Ketema
  - 1030: Arada
  - 1031: Gulele
  - 1032: Lemi Kura
  - 1033: Sabian
  - 1034: Malka Jabti /M.Jebdu)
  - 1035: Legehare
  - 1036: Addis Ketema (DD)
  - 1037: Gende Kore
  - 1038: Dechatu
  - 1039: Hafat Issa
  - 1040: Kazira
  - 1041: Police Maret
  - 1042: Aseliso
  - 1043: Jeldessa
  - 1044: Wahil
  - 1045: Biyoawale
  - 1046: Shebe Dino
  - 1047: Hawassa Zuria
  - 1048: Arbegona
  - 1049: Dale
  - 1050: Aleta Wendo
  - 1051: Dara
  - 1052: Hulla
  - 1053: Bensa
  - 1054: Aroresa
  - 1055: Boricha
  - 1056: Gorche
  - 1057: Malga
  - 1058: Wonosho
  - 1059: Chire
  - 1060: Bursa
  - 1061: Aleta Chuko
  - 1062: Bona Zuria
  - 1063: Hawasa town
  - 1064: Wondo-Genet
  - 1065: Yirgalem town
  - 1066: Aleta Wondo town
  - 1067: Leku town
  - 1068: Hawela
  - 1069: Bura
  - 1070: Dara Otilicho
  - 1071: Teticha
  - 1072: Chirone
  - 1073: Shafamo
  - 1074: Chabe Gambeltu
  - 1075: Daye town
  - 1076: Hokko
  - 1077: Bilate Zuria
  - 1078: Darara
  - 1079: Daella
  - 1080: Chuko town
  - 1081: Wondo-Genet town
  - 1082: Loka Abaya
  - 7777: Other (Specify)

### main_residence_district_specify

- **Label**: 3.8. If this district (Metema) is not your main place of residence, where is your main residence?

District:

- **Type**: text
- **Relevant**: main_residence_country>1 or main_residence_region=777 or main_residence_woreda=7777

### main_residence_village

- **Label**: 3.8. If this district (Metema) is not your main place of residence, where is your main residence?

Village (Kebele):

- **Type**: text
- **Relevant**: main_residence_metema=0

### time_in_metema

- **Label**: 3.9. For how long have you been in this district (Metema) during this trip?
- **Type**: select_one time_in_metema
- **Relevant**: main_residence_metema=0
- **Choices**:
  - 1: Less than a month
  - 2: Between 1 and 3 months
  - 3: Between 3 and 6 months
  - 4: Between 6 months and 1 year
  - 5: More than 1 year
  - 888: Don’t know/don’t remember

</details>

<details>
<summary><h2>Section 4:  Living at the farm and malaria prevention (group)</h2></summary>

- **Type**: begin group
- **Relevant**: s2_end_survey_c=0

### s4_n1

- **Label**: Section 4: Living at the farm and malaria prevention

I’m going to ask you some questions about where do you sleep in this farm and malaria prevention

- **Type**: note

### sleep_structure

- **Label**: 4.1. What kind of structure do you sleep in at this farm?
- **Type**: select_one sleep_structure
- **Choices**:
  - 1: Informal structure (reed walls, thatch or tarp roof (Gibaza in Amharic)
  - 2: No structure, sleep outdoors
  - 3: Permanent traditional structure (mud walls, thatched roofs, corrugated iron and earth floors, open eaves, no ceiling and no screening)
  - 4: Modern structure (iron roof, burnt brick or cement walls and cement floor)
  - 5: Tent
  - 777: Other (specify)

### sleep_structure_other

- **Label**: Specify
- **Type**: text
- **Relevant**: sleep_structure=777

### ppl_in_sleeping_structure

- **Label**: 4.2. How many people live in your sleeping structure at this farm, including yourself?
- **Type**: integer
- **Relevant**: sleep_structure=1 or sleep_structure=3 or sleep_structure=4 or sleep_structure=5 or sleep_structure=7 or sleep_structure=777

### num_sleeping_places

- **Label**: 4.3. How many sleeping places are there in your sleeping structure at this farm?
- **Type**: integer
- **Relevant**: sleep_structure=1 or sleep_structure=3 or sleep_structure=4 or sleep_structure=5 or sleep_structure=7 or sleep_structure=777

### num_share_space

- **Label**: 4.4. With how many people do you share your sleeping space in your sleeping structure at this site?
- **Type**: integer
- **Relevant**: sleep_structure=1 or sleep_structure=3 or sleep_structure=4 or sleep_structure=5 or sleep_structure=7 or sleep_structure=777

### malaria_diagnosis_30d

- **Label**: 4.5. Have any of the people working with you at this farm been diagnosed with malaria (by rapid diagnostic test or microscopy) in the past 30 days?
- **Type**: select_one yes_no_dn
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Don't know

### bed_net_available

- **Label**: 4.6. Do you have a bed net available to use at this farm?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### net_sleep_last_night

- **Label**: 4.7. Did you sleep under a mosquito net last night?
- **Type**: select_one yes_no
- **Relevant**: bed_net_available=1
- **Choices**:
  - 1: Yes
  - 0: No

### no_net_reason

- **Label**: 4.8. If you did not sleep under any net last night, why not?
- **Type**: select_multiple no_net_reason
- **Relevant**: net_sleep_last_night=0
- **Choices**:
  - 1: No place/space to hang the net
  - 2: Net is uncomfortable / too hot
  - 3: Net does not fit the bed/sleeping arrangements
  - 4: Net is too large/heavy to carry when I travel
  - 5: Net is in poor condition
  - 6: There are no mosquitoes right now
  - 7: There is no malaria risk right now
  - 8: I slept outside
  - 777: Other (specify)
  - 888: Don’t know

### no_net_reason_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(no_net_reason,'777')

### mosquito_protection

- **Label**: 4.9. What other methods do you use to protect yourself against mosquito bites or malaria at this worksite?
- **Type**: select_multiple mosquito_protection
- **Choices**:
  - 1: Nothing
  - 2: Mosquito repellent
  - 3: Medicine/drugs to prevent malaria (specify medication)
  - 4: Fire/smoke
  - 5: Wearing long sleeves/clothes that covered skin
  - 888: Don’t know/don’t remember
  - 999: Decline to answer
  - 777: Other (specify)

### mosquito_protection_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(mosquito_protection,'777')

</details>

<details>
<summary><h2>Section 5:  Occupational travel, worksite conditions and malaria risk (group)</h2></summary>

- **Type**: begin group
- **Relevant**: s2_end_survey_c=0

### s5_n1

- **Label**: Section 5: Occupational travel, worksite conditions and malaria risk

Thank you for your answers. Now I would like to ask you some questions about your work at this farm, travels, and time you spend outdoors

- **Type**: note

### travel_origin

- **Label**: 5.1. Where did you travel from to come to this farm?
- **Type**: select_one travel_origin
- **Choices**:
  - 1: Main residence
  - 2: Another worksite, within Metema
  - 3: Another worksite, outside of Metema (specify)
  - 777: Other (specify)

### travel_origin_other_worksite

- **Label**: Specify another worksite, outside of Metema
- **Type**: text
- **Relevant**: travel_origin=3

### travel_origin_other

- **Label**: Specify
- **Type**: text
- **Relevant**: travel_origin=777

### work_months

- **Label**: 5.2. Over the entire year, what months do you usually work in this area?
- **Type**: select_multiple months
- **Choices**:
  - 1: January
  - 2: February
  - 3: March
  - 4: April
  - 5: May
  - 6: June
  - 7: July
  - 8: August
  - 9: September
  - 10: October
  - 11: November
  - 12: December

### work_rest_year

- **Label**: 5.3. Where do you work the remainder of the year?
- **Type**: select_one work_rest_year
- **Choices**:
  - 1: Main residence
  - 2: Another worksite, within Metema
  - 3: Another worksite, outside of Metema (specify)
  - 777: Other (specify)

### work_rest_year_other_worksite

- **Label**: Specify another worksite, outside of Metema
- **Type**: text
- **Relevant**: work_rest_year=3

### work_rest_year_other

- **Label**: Specify
- **Type**: text
- **Relevant**: work_rest_year=777

### annual_return_metema

- **Label**: 5.4. Do you return to this location (Metema) to work annually?
- **Type**: select_one annual_return_metema
- **Relevant**: main_residence_metema=0
- **Choices**:
  - 1: Yes, every year
  - 2: Some years, but it varies
  - 3: No, generally different locations between years
  - 4: This is my first time working at the site

### arrival_month

- **Label**: 5.5. What month did you arrive in Metema for work this year?
- **Type**: select_one months
- **Relevant**: main_residence_metema=0
- **Choices**:
  - 1: January
  - 2: February
  - 3: March
  - 4: April
  - 5: May
  - 6: June
  - 7: July
  - 8: August
  - 9: September
  - 10: October
  - 11: November
  - 12: December

### departure_month

- **Label**: 5.6. What month are you planning to depart from Metema this year?
- **Type**: select_multiple departure_month
- **Relevant**: main_residence_metema=0
- **Choices**:
  - 8: August
  - 9: September
  - 10: October
  - 11: November
  - 12: December
  - 13: January 2025
  - 14: February 2025
  - 88: Not yet decided
  - 777: Other (specify)

### departure_month_specify

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(departure_month,'777')

### returning_gz_dembia

- **Label**: 5.7. Are you returning to Gondar Zuria, East Dembia, Belesa, or Ebenet?
- **Type**: select_one yes_no
- **Relevant**: main_residence_metema=0
- **Choices**:
  - 1: Yes
  - 0: No

### residence_location_gondar_woreda

- **Label**: 5.7a. Where exactly is your place of residence in Gondar Zuria, East Dembia, Belesa, or Ebenet? **WOREDA**
- **Type**: select_one residence_location_gondar_woreda
- **Relevant**: returning_gz_dembia=1
- **Choices**:
  - 1: Gondar Zuria
  - 2: East Dembia
  - 3: Belesa
  - 4: Ebenet

### residence_location_gondar_kebele

- **Label**: 5.7a. Where exactly is your place of residence in Gondar Zuria, East Dembia, Belesa, or Ebenet? **KEBELE**
- **Type**: select_one residence_location_gondar_kebele
- **Relevant**: returning_gz_dembia=1
- **Choices**:
  - 1: Abowarca
  - 2: Abunesemera
  - 3: Ambachara
  - 4: Arbiytu
  - 5: Arewaya
  - 6: Ayeba
  - 7: B/Gembe
  - 8: Berhala
  - 9: Birbokes
  - 10: Chiher
  - 11: Chinchaye
  - 12: Dass
  - 13: Dawa
  - 14: Debesan tekara
  - 15: Debre selam
  - 16: Degola
  - 17: Denkeze
  - 18: Denzaze
  - 19: Ferka dangurie
  - 20: Gubaye
  - 21: Hamesafige jewana
  - 22: Jayera
  - 23: Liyeya Dugie
  - 24: Machia
  - 25: Manterno
  - 26: Menchir gebrial
  - 27: Menzero
  - 28: Merdo
  - 29: Meterha
  - 30: Sebeha gebrial
  - 31: Sehor gultoch
  - 32: Sehor sarwha
  - 33: Sendeba
  - 34: Shiha
  - 35: Shiwana
  - 36: Tiown seguaje
  - 37: Wuzaba
  - 38: Yemada
  - 39: Zantera
  - 40: Zengaje
  - 41: Abagualit
  - 42: Achera
  - 43: Addisige
  - 44: Arebia
  - 45: Atikilit
  - 46: Balangeb
  - 47: Barcha
  - 48: Buwa
  - 49: Debirzuria
  - 50: Dirmara
  - 51: Fenja
  - 52: Gana
  - 53: Gedawa
  - 54: Girarige
  - 55: Gubia
  - 56: Guramba Bata
  - 57: Guramba Mikial
  - 58: Jangua
  - 59: Jarjar
  - 60: Mekuamia
  - 61: Saliji
  - 62: Senbetdeber
  - 63: Serabadabilo
  - 64: Simano
  - 65: Sufankara
  - 66: Wawucha
  - 67: Weyinatana
  - 68: Wokerako
  - 69: Ababikela
  - 70: Abegelidy
  - 71: Abena
  - 72: Aderseg
  - 73: Akuha
  - 74: Alemshewa
  - 75: Amesteya
  - 76: Aquashmosh
  - 77: Balearbe
  - 78: Birkoche
  - 79: Debir Abajale
  - 80: Deregeha
  - 81: Embacheko
  - 82: Gelamatebeya
  - 83: Gunaguna
  - 84: Jeman
  - 85: Kita
  - 86: Lusina
  - 87: Mechena
  - 88: Niquara
  - 89: Sarawdi
  - 90: Selamaya
  - 91: Serekerna
  - 92: Shumige
  - 93: Tarassinba
  - 94: Tigagie
  - 95: Wagi
  - 96: Wariba
  - 97: Weftoma
  - 98: Wenberoch
  - 99: Wergaja
  - 100: Zeha
  - 101: Abayitera
  - 102: Abeye
  - 103: Achekan
  - 104: Addisalem
  - 105: Aderarua
  - 106: Aketie
  - 107: Amisteya
  - 108: Aniteleziba
  - 109: Arba Tsguar
  - 110: Arefa
  - 111: Asawagarie
  - 112: Ashekereterara
  - 113: Aybashika
  - 114: Ayiseg
  - 115: Azenedela
  - 116: Bursa
  - 117: Chama Korach
  - 118: Cherge
  - 119: Dahoch
  - 120: Deber Zana
  - 121: Debozige
  - 122: Degeb
  - 123: Dengora
  - 124: Diquna
  - 125: Fenta
  - 126: Ferfer
  - 127: Gabezi
  - 128: Gilemes
  - 129: Girarege
  - 130: Goga
  - 131: Gond
  - 132: Gonedebirareg
  - 133: Gowa Akotana
  - 134: Guhala Zuria
  - 135: Gulana
  - 136: Hamusit
  - 137: Jandab
  - 138: Kalay
  - 139: Kalay Sholit
  - 140: Kibeza
  - 141: Koza
  - 142: Lavamariam
  - 143: Macha
  - 144: Mentie
  - 145: Michewa
  - 146: Mukatera
  - 147: Sami
  - 148: Sera
  - 149: Shamishe
  - 150: Shura
  - 151: Tala
  - 152: Taretarua
  - 153: Taymen
  - 154: Tele
  - 155: Wareb
  - 156: Woyeba
  - 157: Wurara
  - 158: Zoz
  - 777: Other (Specify)

### residence_location_gondar_kebele_specify

- **Label**: Specify
- **Type**: text
- **Relevant**: residence_location_gondar_kebele=777

### where_live

- **Label**: Where exactly do you live?
- **Type**: text
- **Relevant**: returning_gz_dembia=1

### followup_residence_health

- **Label**: 5.7b. Would you be willing to participate in a follow up visit once you are back in your place of residence to check your health and malaria status?
- **Type**: select_one yes_no
- **Relevant**: returning_gz_dembia=1
- **Choices**:
  - 1: Yes
  - 0: No

### contact_number_for_visit

- **Label**: 5.7c. Could you provide us with your contact number so we can contact you to plan the visit?
- **Type**: text
- **Relevant**: followup_residence_health=1

### outdoor_sleep_last_month

- **Label**: 5.8. Have you slept outdoors (outside of any structure) in the last month?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### s5_n2

- **Label**: Please check your answer since in Q4.8 participant responded that they slept outside.
- **Type**: note
- **Relevant**: selected(no_net_reason,'8') and outdoor_sleep_last_month=0

### freq_outdoor_sleep_month

- **Label**: 5.9. How often did you sleep outside of any structure in the last month?
- **Type**: select_one freq_outdoor_sleep_month
- **Relevant**: outdoor_sleep_last_month=1
- **Choices**:
  - 1: Every night
  - 2: 5-6 nights per week
  - 3: 3-4 nights per week
  - 4: 1-2 nights per week
  - 5: Less than 1 night per week

### reason_outdoor_sleep

- **Label**: 5.10. Why did you sleep outside of any structure?
- **Type**: select_multiple reason_outdoor_sleep
- **Relevant**: outdoor_sleep_last_month=1
- **Choices**:
  - 1: Working at farm
  - 2: Guarding crops against wild animals
  - 3: It was too hot inside
  - 4: Not enough space inside
  - 5: Spending time with a partner
  - 6: No sleeping structure
  - 777: Other (specify)
  - 888: Don’t know / don’t remember
  - 999: Decline to answer

### reason_outdoor_sleep_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(reason_outdoor_sleep,'777')

### time_outside_evening

- **Label**: 5.11. Did you spend any time outside between the hours of 6pm and 6am in the last month?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### freq_time_outside_evening

- **Label**: 5.12. How often did you spend time outside between 6pm and 6am in the last month?
- **Type**: select_one freq_time_outside_evening
- **Relevant**: time_outside_evening=1
- **Choices**:
  - 1: Every night
  - 2: 5-6 nights per week
  - 3: 3-4 nights per week
  - 4: 1-2 nights per week
  - 5: Less than 1 night per week

### avg_hours_outside_evening

- **Label**: 5.13. On average, how many hours per day did you spend outside between 6pm and 6am in the last month?
- **Type**: integer
- **Relevant**: time_outside_evening=1

### reasons_outside_evening

- **Label**: 5.14. What are the reasons for spending time outside between the hours of 6pm and 6am?
- **Type**: select_multiple reasons_outside_evening
- **Relevant**: time_outside_evening=1
- **Choices**:
  - 1: Working at the farm (ploughing, weeding, harvesting)
  - 2: Traveling
  - 3: Guarding livestock
  - 4: It was too hot inside
  - 5: Leisure/bars/socialising with friends
  - 6: Spending time with a partner
  - 7: No space inside
  - 8: Cooking/eating
  - 9: No sleeping structure
  - 777: Other (specify)
  - 888: Doesn’t know
  - 999: Decline to answer

### reasons_outside_evening_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(reasons_outside_evening,'777')

### nights_outside_delelo

- **Label**: 5.15. In the last month, have you spent at least one night anywhere other than this kebele (Delelo)?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### num_places_last_month

- **Label**: 5.16. How many different places other than this kebele have you spent at least one night in the past month?
- **Type**: integer
- **Relevant**: nights_outside_delelo=1

</details>

<details>
<summary><h2>Section 6:  Malaria knowledge attitude practice (KAP) (group)</h2></summary>

- **Type**: begin group
- **Relevant**: s2_end_survey_c=0

### s6_n1

- **Label**: Section 6: Malaria knowledge attitude practice (KAP)
- **Type**: note

### heard_of_malaria

- **Label**: 6.1. Have you heard of malaria?
- **Type**: select_one yes_no_dn
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Don't know

### malaria_transmission

- **Label**: 6.2. In your opinion, how is malaria transmitted?
- **Type**: select_multiple malaria_transmission
- **Relevant**: heard_of_malaria=1 or heard_of_malaria=888
- **Choices**:
  - 1: Mosquito bites
  - 2: By water
  - 3: By air
  - 4: By eating contaminated food
  - 5: By eating immature sugarcane
  - 6: By fasting
  - 7: By touching a person with malaria
  - 8: By sleeping next to a person with malaria
  - 9: Staying/sleeping in the forest
  - 10: Bathing in river
  - 11: Poor hygiene
  - 12: Spirits
  - 777: Other (specify)
  - 888: Don’t know

### malaria_transmission_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(malaria_transmission,'777')

### malaria_symptoms

- **Label**: 6.3. What are the signs or symptoms of malaria?
- **Type**: select_multiple malaria_symptoms
- **Relevant**: heard_of_malaria=1 or heard_of_malaria=888
- **Choices**:
  - 1: Fever
  - 2: Headache
  - 3: Fatigue
  - 4: Dizziness
  - 5: Joint/muscular pain
  - 6: Chills
  - 7: Nausea/vomit
  - 8: Loss of appetite
  - 9: Diarrhea
  - 10: Coughing
  - 11: Rash
  - 12: Sweating
  - 777: Other (specify)
  - 888: Don’t know

### malaria_symptoms_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(malaria_symptoms,'777')

### malaria_prevention

- **Label**: 6.4. In your opinion, what are the ways that people can prevent getting infected with malaria?
- **Type**: select_multiple malaria_prevention
- **Relevant**: heard_of_malaria=1 or heard_of_malaria=888
- **Choices**:
  - 1: By using a bed net
  - 2: By using insecticide spray inside the house
  - 3: By using mosquito coil
  - 4: By using mosquito repellent
  - 5: By using chemoprophylaxis/medicine
  - 6: Clothes/insecticide-treated clothes
  - 7: By wearing covered or long clothing
  - 8: Fire/smoke
  - 9: Drink boiled water
  - 10: Traditional healer
  - 11: Stay out of the forest
  - 12: Cannot be prevented
  - 777: Other (specify)
  - 888: Don’t know
  - 999: Decline to answer

### malaria_prevention_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(malaria_prevention,'777')

### malaria_info_source

- **Label**: 6.5. What is your main source of information about malaria?
- **Type**: select_one malaria_info_source
- **Relevant**: heard_of_malaria=1 or heard_of_malaria=888
- **Choices**:
  - 1: Health Extension Worker
  - 2: Government Health facility (Health Center and Hospital)
  - 3: Private health provider
  - 4: Pharmacy
  - 5: Shop / market
  - 6: Teachers
  - 7: Religious leaders / monks
  - 8: Family members
  - 9: Co-workers
  - 10: Friends/neighbors
  - 11: Employers
  - 12: TV
  - 13: Radio
  - 14: Posters
  - 15: Leaflets/brochures
  - 777: Other (specify)
  - 888: Don’t know

### malaria_info_source_other

- **Label**: Specify
- **Type**: text
- **Relevant**: malaria_info_source=777

### malaria_testing_treatment

- **Label**: 6.6. Do you know where you can be tested and treated for malaria?
- **Type**: select_one yes_no
- **Relevant**: heard_of_malaria=1 or heard_of_malaria=888
- **Choices**:
  - 1: Yes
  - 0: No

### first_testing_place

- **Label**: 6.7. Where is the first place you would go to get tested and treated for malaria?
- **Type**: select_one first_testing_place
- **Relevant**: malaria_testing_treatment=1
- **Choices**:
  - 1: Health Extension worker/ Health post
  - 2: Mobile Health Team at farm
  - 3: Health center
  - 4: Government Hospital
  - 5: Private health provider
  - 6: Pharmacy
  - 7: Shop / market
  - 8: In the home only
  - 9: Traditional healer
  - 777: Other (specify)
  - 888: Don’t know/don’t remember

### first_testing_place_other

- **Label**: Specify
- **Type**: text
- **Relevant**: first_testing_place=777

### first_testing_place_name

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(selected(first_testing_place,'777'), first_testing_place_other, jr:choice-name(first_testing_place,'first_testing_place'))

### reason_first_testing_place

- **Label**: 6.8. Why would ${first_testing_place_name} be the first place you would go to get tested and treated for malaria?
- **Type**: select_multiple reason_first_testing_place
- **Relevant**: malaria_testing_treatment=1
- **Choices**:
  - 1: Quality of care is better
  - 2: I trust them
  - 3: Short waiting time
  - 4: Short travel distance
  - 5: The service time is convenient hours
  - 6: It’s cheaper (or free)
  - 777: Other (specify)
  - 888: Don’t know

### reason_first_testing_place_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(reason_first_testing_place,'777')

</details>

<details>
<summary><h2>Section 7:  History of fever and treatment seeking (group)</h2></summary>

- **Type**: begin group
- **Relevant**: s2_end_survey_c=0

### s7_n1

- **Label**: Section 7: History of fever and treatment seeking
- **Type**: note

### malaria_diagnosis_6months

- **Label**: 7.1. Have you been diagnosed (either RDT or microscopy) with malaria in the past 6 months?
- **Type**: select_one yes_no_dn
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Don't know

### fever_ill_2weeks

- **Label**: 7.2. Have you been ill with a fever in the past 2 weeks?
- **Type**: select_one yes_no_dn
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Don't know

### fever_location_metema

- **Label**: 7.2a. Think about the last time that you were sick with fever. Were you in Metema when you had this symptom?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### fever_treatment_advice

- **Label**: 7.3. The last time you had a fever in Metema, did you seek advice or treatment for the illness from any source?
- **Type**: select_one yes_no_dn
- **Relevant**: fever_location_metema=1
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Don't know

### reasons_no_treatment

- **Label**: 7.4. What are the reasons that you didn’t seek advice or treatment?
- **Type**: select_multiple reasons_no_treatment
- **Relevant**: fever_treatment_advice=0
- **Choices**:
  - 1: Waited for fever subsided
  - 2: No money for treatment
  - 3: No money for transport
  - 4: Not sure where to go
  - 5: Didn’t feel ill enough
  - 6: Couldn’t get time off work
  - 777: Other (specify)
  - 888: Don’t know/don’t remember

### reasons_no_treatment_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(reasons_no_treatment,'777')

### time_to_seek_treatment

- **Label**: 7.5. How long after the fever (or other signs) started did you first seek advice or treatment?
- **Type**: select_one time_to_seek_treatment
- **Relevant**: fever_treatment_advice=1
- **Choices**:
  - 1: Same day
  - 2: Day after
  - 3: Two days after
  - 4: Three or more days after
  - 888: Don’t know / Don’t remember

### first_treatment_place

- **Label**: 7.6. Where was the FIRST PLACE you sought advice or treatment?
- **Type**: select_one first_treatment_place
- **Relevant**: fever_treatment_advice=1
- **Choices**:
  - 1: Health Extension Worker/ health post
  - 2: Mobile Health Team at farm
  - 3: Health center
  - 4: Government hospital
  - 5: Private health provider
  - 6: Pharmacy
  - 7: Shop / market
  - 8: In the home only
  - 9: Traditional healer
  - 777: Other (specify)
  - 888: Don’t know/don’t remember

### first_treatment_place_other

- **Label**: Specify
- **Type**: text
- **Relevant**: first_treatment_place=777

### first_treatment_place_name

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(selected(first_treatment_place,'777'), first_treatment_place_other, jr:choice-name(first_treatment_place,'first_treatment_place'))

### reason_first_treatment_place

- **Label**: 7.7. Why did you seek advice or treatment at this place [${first_treatment_place_name}]?
- **Type**: select_multiple reason_first_treatment_place
- **Relevant**: fever_treatment_advice=1 and first_treatment_place!=888
- **Choices**:
  - 1: Quality of care is better
  - 2: I trust them
  - 3: Short wait time
  - 4: Short travel distance
  - 5: Convenient hours
  - 6: It’s cheaper (or free)
  - 777: Other (specify)
  - 888: Don’t know

### reason_first_treatment_place_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(reason_first_treatment_place,'777')

### km_to_first_place

- **Label**: 7.8. How many kilometers did you have to travel to reach ${first_treatment_place_name}?
- **Type**: integer
- **Relevant**: fever_treatment_advice=1 and first_treatment_place!=888

### walking_time_to_place

- **Label**: 7.9. How much time does it take you to travel to this place [${first_treatment_place_name}] walking?
- **Type**: select_one walking_time_to_place
- **Relevant**: fever_treatment_advice=1 and first_treatment_place!=888
- **Choices**:
  - 1: Less than 30 minutes
  - 2: Between 30 minutes and 1 hour
  - 3: Between 1 and 3 hours
  - 4: Between 3 and 6 hours
  - 5: More than 6 hours
  - 777: Other specify
  - 888: Don’t know

### walking_time_to_place_other

- **Label**: Specify
- **Type**: text
- **Relevant**: walking_time_to_place=777

### malaria_test_at_place

- **Label**: 7.10. Did you get a malaria blood test using a drop of blood from your finger (microscopy or RDT) at this place [${first_treatment_place_name}]?
- **Type**: select_one yes_no_dn
- **Relevant**: fever_treatment_advice=1 and first_treatment_place!=888
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Don't know

### test_result

- **Label**: 7.11. What was the result of the test?
- **Type**: select_one test_result
- **Relevant**: malaria_test_at_place=1
- **Choices**:
  - 1: P. falciparum
  - 2: P. vivax
  - 3: Mixed
  - 4: Positive (unknown parasite species)
  - 5: Negative
  - 888: Don’t know / don’t remember
  - 999: Decline to answer

### treatment_received

- **Label**: 7.12. What treatment, if any, did you receive from this place [${first_treatment_place_name}]?
- **Type**: select_multiple treatment_received
- **Relevant**: fever_treatment_advice=1 and first_treatment_place!=888
- **Choices**:
  - 1: Paracetamol
  - 2: Chloroquine
  - 3: Artemether-Lumefantrine (AL)
  - 4: DHA-PQ
  - 5: Primaquine
  - 6: Oral quinine
  - 7: Quinine injection
  - 8: Artesunate Injection
  - 9: Antibiotics (e.g. amoxicillin)
  - 10: Did not receive treatment
  - 11: Referred
  - 777: Other (specify)
  - 888: Don’t know / don’t remember

### treatment_received_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(treatment_received,'777')

</details>

<details>
<summary><h2>Section 8:  Targeted drug administration (group)</h2></summary>

- **Type**: begin group
- **Relevant**: s2_end_survey_c=0 and survey=2

### s8_n1

- **Label**: Section 8: Targeted drug administration
- **Type**: note

### received_antimalarials_without_test

- **Label**: 8.1. While working at the farms in Metema, did you ever received antimalarials without being tested as part of a campaign to all farmers in you farm?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### s8_end_section

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(received_antimalarials_without_test=0,1,0)

### reason_no_tda

- **Label**: 8.2. Why have you not received antimalarials?
- **Type**: select_one reason_no_tda
- **Relevant**: received_antimalarials_without_test=0
- **Choices**:
  - 1: The campaign didn’t happen at my farm
  - 2: Ineligible
  - 3: Refused the antimalarials
  - 4: Was not at the farm when antimalarials were administered
  - 777: Other (specify)

### reason_no_tda_other

- **Label**: Specify
- **Type**: text
- **Relevant**: reason_no_tda=777

### refusal_reason_tda

- **Label**: 8.3. Reason for refusal to take antimalarials
- **Type**: select_one refusal_reason_tda
- **Relevant**: reason_no_tda=3
- **Choices**:
  - 1: Doesn’t think it’s necessary to take a drug
  - 2: He/she’s healthy
  - 3: Doesn’t want to take a drug he doesn’t know
  - 4: Doesn’t want to take a drug without being tested
  - 5: Doesn’t believe the drugs prevent malaria
  - 6: Treatment is too long or complex
  - 7: Religious or cultural beliefs
  - 8: Interferes with other habits (e.g. alcohol consumption)
  - 9: Is afraid of adverse events
  - 10: Heard negative rumors about this drug
  - 11: Doesn’t trust the TDA team
  - 12: Doesn’t know what the drugs are for
  - 13: Is taking other drugs (not contra-indicated) and doesn’t want to take that many pills
  - 777: Other (specify)

### refusal_reason_tda_other

- **Label**: Specify
- **Type**: text
- **Relevant**: refusal_reason_tda=777

### s8_end_section_2

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(received_antimalarials_without_test=0 and (reason_no_tda=1 or reason_no_tda=2 or reason_no_tda=4 or reason_no_tda=777), 1, 0)

### tda_rounds_received

- **Label**: 8.4. How many different times did the study teams come to your farm and you received antimalarials without being tested as part of a campaign to all farmers in you farm?
- **Type**: select_one tda_rounds_received
- **Relevant**: s8_end_section=0 and s8_end_section_2=0
- **Choices**:
  - 1: One
  - 2: Two
  - 3: Three
  - 888: Don't Know

### tda_same_farm

- **Label**: 8.5. Were the different times administered at the same farm?
- **Type**: select_one yes_no_farm
- **Relevant**: tda_rounds_received=2 or tda_rounds_received=3
- **Choices**:
  - 1: Yes, they were received at the same farm
  - 2: No, they were received at different farms

### know_tda_purpose

- **Label**: 8.6. Do you know what the purpose of the antimalarial campaign is?
- **Type**: select_one know_tda_purpose
- **Relevant**: s8_end_section=0 and s8_end_section_2=0
- **Choices**:
  - 1: No, I don’t know what the purpose is
  - 2: Yes, to treat malaria
  - 3: Yes, to prevent malaria
  - 4: Yes, to treat and prevent malaria
  - 777: Yes, other (specify)

### know_tda_purpose_other

- **Label**: Specify
- **Type**: text
- **Relevant**: know_tda_purpose=777

### last_round_day1_observed

- **Label**: 8.7. During the last campaign, was the administration of the first dose (day 1) directly observed?
- **Type**: select_one yes_no
- **Relevant**: s8_end_section=0 and s8_end_section_2=0
- **Choices**:
  - 1: Yes
  - 0: No

### s8_n2

- **Label**: **Drug adherence**:

Provide information for the most recent time you received antimalarials as part of a campaign.

- **Type**: note
- **Relevant**: s8_end_section=0 and s8_end_section_2=0

### blister_pack_available

- **Label**: 8.8. Is the blister pack available?
- **Type**: select_one blister_pack_available
- **Relevant**: s8_end_section=0 and s8_end_section_2=0
- **Choices**:
  - 1: Yes - Blister pack is available and has been given to the team
  - 2: No - but participant is able to self-report how many pills were taken
  - 3: No - and participant is unable to report how many pills were taken
  - 777: Other (specify)

### blister_pack_available_other

- **Label**: Specify
- **Type**: text
- **Relevant**: blister_pack_available=777

### no_blister_pack_reason

- **Label**: 8.9. Why is the blister pack not available?
- **Type**: select_one no_blister_pack_reason
- **Relevant**: blister_pack_available=2 or blister_pack_available=3 or blister_pack_available=777
- **Choices**:
  - 1: Did not know blister pack had to be saved, so threw it away
  - 2: Cannot find blister pack
  - 3: Gave blister pack to someone else
  - 777: Other (specify)

### no_blister_pack_reason_other

- **Label**: Specify
- **Type**: text
- **Relevant**: no_blister_pack_reason=777

### finished_med_as_advised

- **Label**: 8.10. Did you finish all of the medication as advised by the person who gave it to you?
- **Type**: select_one yes_no_dn
- **Relevant**: s8_end_section=0 and s8_end_section_2=0
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Don't know

### total_pills_prescribed

- **Label**: 8.11. What was the total number of pills prescribed (given out)?

(Count blister pack if available or ask the participant to self-report)

- **Type**: integer
- **Relevant**: s8_end_section=0 and s8_end_section_2=0

### pills_taken

- **Label**: 8.12. How many pills did you take?

(Count from blister pack if available or ask the participant to self-report)

- **Type**: integer
- **Relevant**: s8_end_section=0 and s8_end_section_2=0

### pills_remaining

- **Label**: 8.13. How many pills are remaining on the blister pack?
- **Type**: integer
- **Relevant**: blister_pack_available=1

### unfinished_pills_reason

- **Label**: 8.14. Why did you not finish all the pills?
- **Type**: select_one unfinished_pills_reason
- **Relevant**: (pills_taken<9 and gender=1) or (pills_taken<24 and gender=2)
- **Choices**:
  - 1: It was too many pills
  - 2: It made me ill
  - 3: I lost the remainder
  - 4: I shared it with others
  - 5: I was not sick to start with
  - 6: I felt better
  - 7: I forgot to take the rest
  - 8: I saved them for another time when I am ill
  - 9: I didn’t understand the instructions provided by the team
  - 10: I don’t believe in this medication
  - 11: I didn’t like the taste
  - 12: The pills were too big
  - 13: I heard negative rumors about the medication
  - 777: Other (specify)
  - 888: Don’t know

### unfinished_pills_reason_other

- **Label**: Specify
- **Type**: text
- **Relevant**: unfinished_pills_reason=777

### adverse_events

- **Label**: 8.15. Did you experience any adverse events from the medication
- **Type**: select_one yes_no_dn
- **Relevant**: s8_end_section=0 and s8_end_section_2=0
- **Choices**:
  - 1: Yes
  - 0: No
  - 888: Don't know

### num_adverse_events

- **Label**: 8.16. How many adverse events/symptoms did you experience?
- **Type**: integer
- **Relevant**: adverse_events=1

<details>
<summary><h2>Adverse events (repeat)</h2></summary>

- **Type**: begin repeat
- **Relevant**: adverse_events=1

### s8_pos1

- **Label**: nan
- **Type**: calculate
- **Calculate**: position(..)

### adverse_event_type

- **Label**: 8.17. Type of adverse event/symptom
- **Type**: select_one adverse_event_type
- **Relevant**: s8_pos1<=num_adverse_events
- **Choices**:
  - 1: Skin reaction
  - 2: Alteration of heart rhythm (palpitations)
  - 3: Dizziness
  - 4: Vomiting
  - 5: Headache
  - 6: Joint pain
  - 7: Malaise
  - 8: Diarrhea
  - 777: Other (specify)

### adverse_event_type_other

- **Label**: Specify
- **Type**: text
- **Relevant**: adverse_event_type=777

### symptom_severity

- **Label**: 8.18. Severity of the symptom?
- **Type**: select_one symptom_severity
- **Relevant**: s8_pos1<=num_adverse_events
- **Choices**:
  - 1: Mild (causing minimal discomfort and does not interfere with normal daily activities)
  - 2: Moderate (causes some interference with daily activities but does not cause significant discomfort or require extensive medical intervention)
  - 3: Severe (causes significant discomfort, interfering with daily life and requiring medical intervention or hospitalization)
  - 4: Serious adverse event: Life-threatening, requires hospitalization, or leads to significant disability

### symptom_severity_note

- **Label**: Please call the study coordinator and fill out ORA's incident report form
- **Type**: note
- **Relevant**: symptom_severity=4

### symptom_duration

- **Label**: 8.19. How long did the symptom last for?
- **Type**: integer
- **Relevant**: s8_pos1<=num_adverse_events

### symptom_resolved

- **Label**: 8.20. Did the symptom resolve completely?
- **Type**: select_one symptom_resolved
- **Relevant**: s8_pos1<=num_adverse_events
- **Choices**:
  - 1: Yes, the symptom resolved
  - 0: No, the symptom is still ongoing

### alleviation_action

- **Label**: 8.21. What did you do to alleviate this adverse event
- **Type**: select_one alleviation_action
- **Relevant**: s8_pos1<=num_adverse_events
- **Choices**:
  - 1: Nothing
  - 2: Visited mobile health team, health extension worker or health facility
  - 3: Took modern medicines at home
  - 4: Took traditional medicines at home
  - 777: Other (specify)

### alleviation_action_other

- **Label**: Specify
- **Type**: text
- **Relevant**: alleviation_action=777

### s8_r1_n1

- **Label**: Data collection for adverse event #${s8_pos1} is complete.
- **Type**: note
- **Relevant**: s8_pos1<=num_adverse_events

</details>

### feelings_without_malaria_test

- **Label**: 8.22. How did you feel about being offered treatment for malaria without being tested?
- **Type**: select_one feelings_without_malaria_test
- **Relevant**: s8_end_section=0 and s8_end_section_2=0
- **Choices**:
  - 1: Very comfortable
  - 2: Moderately comfortable
  - 3: A little uncomfortable
  - 4: Very uncomfortable

### acceptance_improvements

- **Label**: 8.23. What would have made this intervention more acceptable to you and your co-workers?
- **Type**: select_multiple acceptance_improvements
- **Relevant**: s8_end_section=0 and s8_end_section_2=0
- **Choices**:
  - 1: Nothing, I felt comfortable
  - 2: Testing for malaria before treatment
  - 3: Distribution at a health facility
  - 4: Distribution by a nurse
  - 5: More information at the time of the distribution
  - 6: Visit at a time people are available
  - 777: Other (specify)

### acceptance_improvements_other

- **Label**: Specify
- **Type**: text
- **Relevant**: selected(acceptance_improvements,'777')

### participate_no_testing

- **Label**: 8.24. If you were offered the same intervention (malaria treatment without testing), would you participate?
- **Type**: select_one yes_no
- **Relevant**: s8_end_section=0 and s8_end_section_2=0
- **Choices**:
  - 1: Yes
  - 0: No

### no_participation_reason

- **Label**: 8.25. Why would you not participate again?
- **Type**: select_one no_participation_reason
- **Relevant**: participate_no_testing=0
- **Choices**:
  - 1: Don’t want to take medicine when not sick
  - 2: Don’t think medicine is effective
  - 3: Worried about side effects
  - 4: Worried about taking malaria medicine with other medicines
  - 5: Don’t like the taste of medicine
  - 777: Other (specify)

### no_participation_reason_other

- **Label**: Specify
- **Type**: text
- **Relevant**: no_participation_reason=777

</details>

<details>
<summary><h2>Section 9:  Sample collection  (group)</h2></summary>

- **Type**: begin group
- **Relevant**: s2_end_survey_c=0

### s9_n1

- **Label**: Section 9: Sample collection
- **Type**: note

### rdt_result

- **Label**: 9.1. RDT result
- **Type**: select_one rdt_result
- **Choices**:
  - 1: Negative
  - 2: Positive for P.falciparum only
  - 3: Positive for P. vivax only
  - 4: Positive for mixed (Pf + Pv)
  - 5: Invalid
  - 6: RDT not conducted

### no_rdt_reason

- **Label**: 9.2. Please specify why RDT was not conducted
- **Type**: select_one no_rdt_reason
- **Relevant**: rdt_result=6
- **Choices**:
  - 1: Participant refused
  - 2: Inadequate blood flow
  - 777: Other (specify)

### no_rdt_reason_other

- **Label**: Specify
- **Type**: text
- **Relevant**: no_rdt_reason=777

### repeat_rdt_result

- **Label**: 9.3. Repeat RDT result
- **Type**: select_one rdt_result
- **Relevant**: rdt_result=5
- **Choices**:
  - 1: Negative
  - 2: Positive for P.falciparum only
  - 3: Positive for P. vivax only
  - 4: Positive for mixed (Pf + Pv)
  - 5: Invalid
  - 6: RDT not conducted

### dbs_collected

- **Label**: 9.4. Was a DBS collected?
- **Type**: select_one yes_no
- **Choices**:
  - 1: Yes
  - 0: No

### no_dbs_reason

- **Label**: 9.5. Why was DBS not collected?
- **Type**: select_one no_dbs_reason
- **Relevant**: dbs_collected=0
- **Choices**:
  - 1: Inadequate blood flow
  - 2: Participant refused
  - 777: Other (specify)

### no_dbs_reason_other

- **Label**: Specify
- **Type**: text
- **Relevant**: no_dbs_reason=777

### dbs_labeled_packed

- **Label**: 9.6. Was the DBS card labeled with the Sample QR code and packed for storage?
- **Type**: select_one yes_no
- **Relevant**: dbs_collected=1
- **Choices**:
  - 1: Yes
  - 0: No

### treat

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(rdt_result=2 or rdt_result=3 or rdt_result=4 or repeat_rdt_result=2 or repeat_rdt_result=3 or repeat_rdt_result=4, 1, 0)

### n9_n2

- **Label**: **Participant treatment**

Use the job aid to assess if participant can receive antimalarial medication.

- **Type**: note
- **Relevant**: treat=1

### eligible_malaria_treatment

- **Label**: 9.7. Is the participant eligible for malaria treatment?

<span style="color:red">CHECK ALL CONTRAINDICATIONS BEFORE PROCEEDING</span>

- **Type**: select_one yes_no
- **Relevant**: treat=1
- **Choices**:
  - 1: Yes
  - 0: No

### s9_end_survey

- **Label**: nan
- **Type**: calculate
- **Relevant**: treat=1
- **Calculate**: if(
  (study_arm=3 or
  (survey=2 and (study_arm=1 or study_arm=2)))
  and eligible_malaria_treatment=0,1,0)

### show_9_8

- **Label**: nan
- **Type**: calculate
- **Relevant**: treat=1
- **Calculate**: if(survey=1 and (study_arm=1 or study_arm=2)
  and eligible_malaria_treatment=0,1,0)

### s9_n3

- **Label**: Refer to the health facility using the Referral form.
- **Type**: note
- **Relevant**: s9_end_survey=1

### not_eligible_reason

- **Label**: 9.8. If no, specify reason
- **Type**: select_one not_eligible_reason
- **Relevant**: show_9_8=1
- **Choices**:
  - 1: Refuses to take TDA (withdrew consent)
  - 2: Has contraindications

### contraindications

- **Label**: 9.9. Indicate contraindications
- **Type**: select_multiple contraindications
- **Relevant**: not_eligible_reason=2
- **Choices**:
  - 1: Has received anti-malarial drug in previous 2 weeks
  - 2: Taking concomitant contra-indicated medication
  - 3: Severe illness
  - 4: History of cardiac rhythm disturbances, bradycardia, or heart failure
  - 5: Allergy to DP component or other artemisinin derivatives
  - 6: Pregnancy

### dp_pq_treatment_4_male

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(survey=1 and (study_arm=1 or study_arm=2) and eligible_malaria_treatment=1 and gender=1 and (rdt_result=2 or repeat_rdt_result=2),1,0)

### note_dp_pq_treatment_4_male

- **Label**: 9.10. Treat participant with **DP** and **single low dose of Primaquine**
- **Type**: note
- **Relevant**: dp_pq_treatment_4_male=1

### dp_pq_radical_4_male

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(survey=1 and (study_arm=1 or study_arm=2) and eligible_malaria_treatment=1 and gender=1 and (rdt_result=3 or rdt_result=4 or repeat_rdt_result=3 or repeat_rdt_result=4),1,0)

### note_dp_pq_radical_4_male

- **Label**: 9.11. Treat participant with **DP** and **radical cure of Primaquine**
- **Type**: note
- **Relevant**: dp_pq_radical_4_male=1

### al_pq_treatment_4_male

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(
  (survey=1 and study_arm=3 and eligible_malaria_treatment=1 and gender=1 and (rdt_result=2 or repeat_rdt_result=2))
  or
  (survey=2 and eligible_malaria_treatment=1 and gender=1 and (rdt_result=2 or repeat_rdt_result=2)),1,0)

### note_al_pq_treatment_4_male

- **Label**: 9.12. Treat participant with **AL** and a **single low dose of Primaquine**
- **Type**: note
- **Relevant**: al_pq_treatment_4_male=1

### cq_pq_radical_4_male

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(
  (survey=1 and study_arm=3 and eligible_malaria_treatment=1 and gender=1 and ( rdt_result=3 or rdt_result=4 or repeat_rdt_result=3 or repeat_rdt_result))
  or
  (survey=2 and eligible_malaria_treatment=1 and gender=1 and ( rdt_result=3 or rdt_result=4 or repeat_rdt_result=3 or repeat_rdt_result)),
  1,0)

### note_cq_pq_radical_4_male

- **Label**: 9.13. Treat participant with **CQ** and a **radical cure of Primaquine**
- **Type**: note
- **Relevant**: cq_pq_radical_4_male=1

### al_treatment_4_female

- **Label**: nan
- **Type**: calculate
- **Calculate**: if( eligible_malaria_treatment=1 and gender=2 and (rdt_result=2 or rdt_result=4 or repeat_rdt_result=2 or repeat_rdt_result=4),1,0)

### note_al_treatment_4_female

- **Label**: 9.14. Treat participant with **AL**
- **Type**: note
- **Relevant**: al_treatment_4_female=1

### cq_treatment_4_female

- **Label**: nan
- **Type**: calculate
- **Calculate**: if( eligible_malaria_treatment=1 and gender=2 and (rdt_result=3 or repeat_rdt_result=3),1,0)

### note_cq_treatment_4_female

- **Label**: 9.15. Treat participant with **CQ**
- **Type**: note
- **Relevant**: cq_treatment_4_female=1

### antimalarial_given

- **Label**: 9.16. Was antimalarial provided?
- **Type**: select_one yes_no
- **Relevant**: eligible_malaria_treatment=1
- **Choices**:
  - 1: Yes
  - 0: No

### antimalarial_dose1_observed

- **Label**: 9.17. Was dose #1 directly observed?
- **Type**: select_one yes_no
- **Relevant**: antimalarial_given=1
- **Choices**:
  - 1: Yes
  - 0: No

</details>

### closing_statement

- **Label**: Closing statement

Thank you very much for answering these questions. Your answers will help us understand who gets malaria and why.

If you suspect you have symptoms of malaria in the future, such as having a fever or body aches, please go to the closest clinic when you feel sick and ask for a malaria test.

Do you have any questions for me about malaria or this research?

If you have any questions about this study in the future, please contact the Study Coordinator (show the participant where to find their phone numbers on the consent form)

- **Type**: note
- **Relevant**: s2_end_survey_c=0

### interviewer_comments

- **Label**: Any comments?
- **Type**: text

### study_qr_4_instance_name

- **Label**: nan
- **Type**: calculate
- **Calculate**: if(sample_qr_code=null,study_qr_code,sample_qr_code)
