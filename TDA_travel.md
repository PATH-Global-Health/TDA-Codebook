# Codebook for travel to highlands for workers in control arm form

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
  Targeted drug administration in migrant workers
  Travel to highlands for workers in control arm
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

### farm_camp_code

- **Label**: 1.4. Name of farm camp
- **Type**: select_one farm_camp
- **Choices**:
  - 2: Abdul Nur Juhar
  - 4: Abebe Wuletaw
  - 8: Adamu Baynessagn
  - 13: Aliyas Star (Block 10)
  - 18: Atsede Shiferaw
  - 19: Awuraris Getaneh
  - 21: Ayelign Habtie (Block 26)
  - 29: Birhan Dessalegn (Block 18)
  - 33: BS agriclture
  - 38: Demoz Adigeh
  - 40: Dr. Amsalu Debebe
  - 43: Eneye Birillie
  - 53: Getachew Tezera
  - 54: Getiye Gebru
  - 55: Guadie Alem
  - 59: Haile Gebremariam
  - 60: Hailemariam Melesse
  - 67: Mariye Mengistu
  - 74: Melaku Dires
  - 85: Selamsew Wubetu
  - 89: Shaleka Raday Legesse
  - 86: Sintayehu Alemu
  - 99: Yibralem Belay

### age

- **Label**: 1.5. Participant age
- **Type**: integer

### main_residence_metema

- **Label**: 1.6. Is your main place of residence (i.e., where you maintain a household and live most of the year) in this district (Metema)?
- **Type**: select_one yes_no
- **Relevant**: age>=14
- **Choices**:
  - 1: Yes
  - 0: No

### main_residence_country

- **Label**: 1.7. If this district (Metema) is not your main place of residence, where is your main residence?

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

- **Label**: 1.7. If this district (Metema) is not your main place of residence, where is your main residence?

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

- **Label**: 1.7. If this district (Metema) is not your main place of residence, where is your main residence?

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

- **Label**: 1.7. If this district (Metema) is not your main place of residence, where is your main residence?

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
  - 152: Ebenat town
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

- **Label**: 1.7. If this district (Metema) is not your main place of residence, where is your main residence?

District:

- **Type**: text
- **Relevant**: main_residence_country>1 or main_residence_region=777 or main_residence_woreda=7777

### main_residence_village

- **Label**: 1.7. If this district (Metema) is not your main place of residence, where is your main residence?

Village (Kebele):

- **Type**: text
- **Relevant**: main_residence_metema=0

### return_month

- **Label**: 1.8. What month are you planning to return home to Gondar Zuria, East Dembia, Belesa or Ebenet?
- **Type**: select_multiple return_month
- **Relevant**: main_residence_woreda=327 or main_residence_woreda=328 or main_residence_woreda=331 or main_residence_woreda=332 or main_residence_woreda=136 or main_residence_woreda=152
- **Choices**:
  - 1: October
  - 2: November
  - 3: December
  - 4: January 2025
  - 5: February 2025
  - 6: Not returning to Gondar Zuria, East Dembia, Belesa or Ebenet
  - 7: Not yet decided
  - 777: Other (specify)

### return_month_specify

- **Label**: Specify:
- **Type**: text
- **Relevant**: selected(return_month,'777')

### residence_location_kebele

- **Label**: 1.9. Where exactly is your place of residence in Gondar Zuria, East Dembia, Belesa or Ebenet?
- **Type**: text
- **Relevant**: selected(return_month,'1') or selected(return_month,'2') or selected(return_month,'3') or selected(return_month,'4') or selected(return_month,'5') or selected(return_month,'777')

### followup_residence_health

- **Label**: 1.10. Would you be willing to participate in a follow up visit once you are back in your place of residence to check your health and malaria status?
- **Type**: select_one yes_no
- **Relevant**: selected(return_month,'1') or selected(return_month,'2') or selected(return_month,'3') or selected(return_month,'4') or selected(return_month,'5') or selected(return_month,'777')
- **Choices**:
  - 1: Yes
  - 0: No

### contact_number_for_visit

- **Label**: 1.11. Could you provide us with your contact number so we can contact you to plan the visit?
- **Type**: text
- **Relevant**: followup_residence_health=1

### has_study_id

- **Label**: 1.12. Does this participant already have a Study ID?
- **Type**: select_one has_study_id
- **Relevant**: selected(return_month,'1') or selected(return_month,'2') or selected(return_month,'3') or selected(return_month,'4') or selected(return_month,'5') or selected(return_month,'777')
- **Choices**:
  - 0: No
  - 1: Yes
  - 2: Yes, but he/she lost it

### study_scanned_qr_code

- **Label**: 1.13. Scan study ID
- **Type**: barcode
- **Relevant**: has_study_id=1

### study_manual_qr_code

- **Label**: 1.14. Manually enter Study ID:
- **Type**: text
- **Relevant**: has_study_id=1 and study_scanned_qr_code = null

### study_qr_code

- **Label**: nan
- **Type**: calculate
- **Relevant**: has_study_id=1
- **Calculate**: if(study_scanned_qr_code=null, study_manual_qr_code, study_scanned_qr_code)

### interviewer_comments

- **Label**: Any comments?
- **Type**: text
