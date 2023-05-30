# ⭐ Znalec/Expert SW, HW, Security, Multimedia

## ⚖️ Zákony, Vyhlášky a Nariadenia
1. [**Zákon o znalcoch**, tlmočníkoch a prekladateľoch **382/2014**](https://www.slov-lex.sk/pravne-predpisy/SK/ZZ/2004/382/)  
2. [**Vyhláška Ministerstva spravodlivosti 228/2018**, ktorou sa vykonáva zákon 382/2014 o znalcoch](https://www.slov-lex.sk/pravne-predpisy/SK/ZZ/2018/228/20180801)   
3. [**Vyhláška o odmenách**, náhradných výdavkoch a náhradach za stratu času pre znalcov **491/2004 Z. z.**](https://www.slov-lex.sk/pravne-predpisy/SK/ZZ/2004/491/)    

4. [**GDPR Nariadenie Európskeho parlamentu a Rady (EÚ) 2016/679** z 27. apríla 2016 o ochrane fyzických osôb pri spracúvaní osobných údajov a o voľnom pohybe takýchto údajov](https://eur-lex.europa.eu/legal-content/SK/ALL/?uri=CELEX%3A32016R0679)  
5. [**Zákon o ochrane osobných údajov** a o zmene a doplnení niektorých zákonov **18/2018 Z. z.**](https://www.slov-lex.sk/pravne-predpisy/SK/ZZ/2018/18/)  
6. [**Zákon o ochrane osobných údajov** a o zmene a doplnení niektorých zákonov **122/2013 Z. z.**](https://www.slov-lex.sk/pravne-predpisy/SK/ZZ/2013/122/20140415)  

7. [**Autorský zákon 185/2015 Z. z.**](https://www.slov-lex.sk/pravne-predpisy/SK/ZZ/2015/185/)  
8. [**Trestný Zákon č. 300/2005** a konkrétne **§ 347**](https://www.slov-lex.sk/pravne-predpisy/SK/ZZ/2005/300/)

## 🔬 Nástroje na forenznú analýzu mobilných telefónov a inteligentných zariadení
1. **Cellebrite UFED**  
2. **MOBILedit Forensic**  
3. Magnet AXIOM
4. Oxygen Forensic® Detective

Register IČO organizácií vrátane znalcov Štatistický Úrad: https://zber.statistics.sk/sk/register-organizacii?_sk_susr_isis_pub_organisations_register_portlet_OrganisationsRegisterPortlet_INSTANCE_puzm_navigationType=SEARCH_VIEW

## Tipy
- Upraviť si email na znalec@nieco.sk  
- Využiť ponuku lepšieho poistenia znalca Vladimir Maxa, má lepšie zmluvné podmienky s Generali  
- Doplniť si do profilu Identifikačné údaje zamestnávateľa, treba napísať pani alena.cirbusova@justice.sk  

## 📴 Základný postup pri forenznej analýze
1. Vybrať SIM kartu (nie SD/micro SD kartu)
2. Mať nastavený letový/letecký režim, aby nedošlo k neoprávnenej manipulácii s dátami na zariadení 
3. Povoliť vývojársky (developer) režim pri Android zariadeniach (5-6x tap/click na Číslo zostav/code build)
4. Zapnúť ladenie (Debug) USB 
5. Pripojiť k PC
6. Cez forenzný nástroj vytvoriť logickú alebo fyzickú extrakciu

**Logická metóda** je relatívne rýchly spôsob, ako priamo extrahovať **dáta z používateľských súborov**. Veľkosť extrahovaných údajov je menšia, pretože údaje sa **nezískavajú z pamäte flash**. Nevýhodou tejto metódy však je, že **nedokáže obnoviť zmazané dáta/položky z mobilného zariadenia**. 

**Fyzická metóda** pozostáva z prístupu k flash pamäti mobilného telefónu a extrakcie údajov z tohto priestoru. V tomto prípade sa **pristupuje priamo k flash pamäti**, aby sa získali existujúce údaje a zachytili sa aj vymazané údaje. Na prístup k flash pamäti nástroje **používajú bootloader** na obídenie bezpečnostnej záplaty mobilného zariadenia. Keď máme extrakciu hotovú, môžeme podľa požiadaviek zadávateľa skúmať či sa v telefóne nachádzajú dáta, ktoré by mohli nasvedčovať spáchaniu trestného činu (napr. zbrane, drogy, nahota atd.).

## 🧰 Ďalšie nástroje znalca pre forenzné skúmanie PC
1. Autopsy
2. **Cellebrite Inspector**
3. **FTK Imager**
4. Magnet AXIOM
5. Oxygen Forensic® Detective

## 💻 Základný postup pri forenznom skúmaní PC
1. Aby sa zabránilo možnej zmene dát počas znaleckého skúmania na pamäťovom médiu je potrebné použiť opatrenie pre ochranu proti zápisu zo strany OS **(tzv. Write-Blocker)**, buď vo forme špeciálneho softvéru alebo ako hardvérového zariadenia
2. **Akékoľvek úkony s dôkazným materiálom v súdnom konaní sa môžu vykonávať iba na jeho kópiách**
3. Vytvoriť **bitovú kópiu média** (HDD, SSD) tzv. **obraz (image)**
4. Verifikovať vytvorený obraz a originálne médium s použitím vhodného **hašovacieho (hash funkcie) algoritmu** a zdokumentovanie získanej hodnoty hash-u
5. **Bitovú kópiu** pripájať **len v read-only** móde

### 🧮 Analýza Dát
a) Konfiguračné súbory OS - Configuration Files  
b) **Používatelia a používateľské skupiny** - Users and Groups  
c) **Súbory s heslami** - Password Files  
d) **Log súbory** - Logs (System Events, Audit Record, Application Events, Command History, Recently Accessed Files)  
e) **Aplikačné súbory** - Application Files (napr. priamo spustiteľné súbory, ikony, audio súbory danej aplikácie a pod.)  
f) **Dátové súbory** - Data Files (napr. dokumenty z textových editorov, tabuľkových procesorov, grafické súbory, video súbory a pod.)  
g) Swap súbory - Swap Files (súbory používané OS pre rozšírenie veľkosti operačnej pamäte)  
h) Dump súbory - Dump Files (súbory používané v niektorých typoch OS k automatickému uloženiu obsahu pamäte v prípade výskytu chybového stavu)  
i) Hibernačné súbory - Hibernation Files (súbory vytvárané pre zachytenie aktuálneho stavu OS pred vypnutím počítača, typické použitie najmä pre prenosné počítače)  
j) Dočasné súbory - Temporary Files  

Obnova vymazaných dát alebo len výberovej skupiny dát (napr. len grafické súbory, video súbory a pod.) zo súborových systémov jednotlivých dátových nosičov (hard diskov a ďalších médií) pomocou viacerých nezávislých softvérových nástrojov (teda s použitím viacerých rôznych algoritmov) a ich následná analýza
Po ukončení práce (analytickej fázy) na kópii obrazu, opätovne verifikovať túto pracovnú kópiu s originálnym obrazom a znovu zadokumentovať získané hodnoty hash-u.
