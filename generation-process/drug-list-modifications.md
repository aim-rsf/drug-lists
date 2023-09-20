# Drug List Modifications

For reproducibility purposes the code lists generated and their review processes have been outlined below. The modifications are as per clinician's advice (Jenny Cooper) to ensure removal of misclassified, erroneous drugs and maintaining balance between specificity and sensitivity in term sets.

As a combination of method 1 & 2 has been used to create the lists, there is some variation in documentation (for example, method 2 will contain the snomedizer R package query syntax). Below are the completed lists.

The steps included will roughly follow the following structure:
- snomedizer query (if used)
- generic drug list
- brand drug list
- modifications (removals and additions from clinicians review)
- additional notes

---
## Anticonvulsants 

```
#SNOMEDIZER QUERY:
concept_find(ecl = "<<763158003 : 127489000 |Has active ingredient (attribute) | = <<255632006", limit= 1200)$idAndFsnTerm
```

### 1. Generic drug list:
None

### 2. Brand drug list:
- Alzain
- Arbil MR
- Ativan
- Axalid
- Belvo
- Briviact
- Bromazepam
- Buccolam
- Carbagen
- Carbamazepine
- Celontin
- Centrax
- Chlordiazepoxide
- Clobazam
- Clomethiazole
- Clonazepam
- Convulex
- Dalmane
- Depakote
- Desitrend
- Desizon
- Diacomit
- Diazemuls
- Diazepam
- Dibro-Be
- Dilantin
- Dormicum
- Emeside
- Epanutin
- Epesri
- Epimaz
- Epistatus
- Ethosuximide
- Felbamate
- Felbatol
- Frisium
- Fycompa
- Gabapentin
- Gabitril
- Genlev
- Heminevrin
- Hypnovel
- Inovelon
- Keppra
- Kevesy
- Kigabeq
- Klonopin
- Lamictal
- Lamotrigine
- Lecaent
- Levetiracetam
- Librium
- Liskantin
- Loprazolam
- Lorazepam
- Lormetazepam
- Lyrica
- Magnesium sulfate
- Matever
- Midazolam
- Miprosed
- Mogadon
- Mysoline
- Neurontin
- Nitrazepam
- Nootropil
- Orimeten
- Ospolot
- Oxazepam
- Oxcarbazepine
- Ozalin
- Paraldehyde
- Perampanel
- Perizam
- Petinutin
- Phenobarbital
- Phenytoin
- Piracetam
- Pregabalin
- Primidone
- Pro-Epanutin
- Rewisca
- Rivotril
- Rohypnol
- Sabril
- Somnite
- Stesolid
- Sultiame
- Syonell
- Taloxa
- Tapclob
- Tegretol
- Temazepam
- Tensium
- Teril Retard
- Tiagabine
- Topamax
- Topiramate
- Tranxene
- Trileptal
- Trobalt
- Valclair
- Valproic acid
- Vigabatrin
- Vimpat
- Xanax
- Zacco
- Zarontin
- Zonegran
- Zonisamide
- Brivaracetam
- Cannabidiol
- Epidiolex
- Epidyolex
- Sativex
- Cenobamate
- Ontozry
- Eslicarbazepine
- Zebinix
- Arupsan
- fenfluramine
- fintepla
- Lacosamide
- vimpat
- Rufinamide
- Inovelon
- Sodium valproate
- Epilim
- Episenta
- Orlept
- Dyzantil
- Depakin
- Epival CR
- stiripentol
- Diacomit
- fosphenytoin
- epanutin


### 3. Modifications:

#### Removals:

- Thiamine
- Athiam
- Benerva
- Thiadose
- ThiamEss
- Tyvera, 
- Paracetamol
- pyridoxine
- Numark Epsom Salts
- Gabapentin creams/gel
- Nasal spray
- Alcohols ointments
- inhaler/inhalation powders
- Ipratropium/nebuliser/'neb'/(typos: nebuilser)
- Enema
- Tropium
- Magnesium sulfate powder/mixture/paste/oralx - unsure about intravenous/injections as I can see they can be used as anti-convulsant?
- Miprose
- Oils
- Temazepam
        
#### Additions:

Using BNF:

- Brivaracetam
- Cannabidiol
- Epidiolex
- Epidyolex
- Sativex
- Cenobamate
- Ontozry
- Eslicarbazepine
- Zebinix
- Arupsan
- fenfluramine
- fintepla
- Lacosamide
- vimpat
- Rufinamide
- Inovelon
- Sodium valproate
- Epilim
- Episenta
- Orlept
- Dyzantil
- Depakin
- Epival CR
- stiripentol
- Diacomit
- fosphenytoin
- epanutin

#### Removals at review stage:
- Dexfenfluramine - different to fenfluramine (which is an anticonvusant) with different indication
- Oral Benzodiazepines,
- Chlordiazepoxide - it is anticonvulsant but not licensed to be used except for in alcohol withdrawal regimes
- Librium, limbritol libraxin (chlordiazepoxide brands)
- Clomethiazole (Heminevrin brand)
- Alprazolam (Xanax brand name)
- Bromazepam - not BNF licensed for seizure control
- Lexotan (bromazepam brands)
- Flurazepam - like temazepam - used for sleep rather than seizure prevention
- Flunitrazepam - as per flurazepman and temazepam
- Dalmane (flurazepam brand)
- Loprazolam (Dormonoct brand)
- Nitrazepam - (mogadon, Somnite brand)
- Lormetazepam - (loramet, noctamid brand)
- Oxazepam (oxanid)
- Chlorazepate (tranxene brand)
- Lorazepam - orally
- Diazepam orally (tensium brand)
- Dormicum oral midazolam
- Izinova - bowel prep
- Magnesium - cutaneous or orally
- Belladonna alkaloids with phenobarbital aluminium hydroxide and magnesium trisilicate
- Orimeten - a steroid
- Potassium chloride 0.075% (potassium 5mmol/500ml) / Glucose 10% / Calcium gluconate 0.21% / Sodium chloride 0.029% / Magnesium sulfate 0.025% - fluid replacement solution

---
## Antipsychotics

### 1. Generic drug list:
- **1st Gen:**
  - Chlorpromazine
  - Fluphenazine
  - Levomepromazine
  - Pericyazine
  - Prochlorperazine
  - Promazine
  - Trifluoperazine
  - Butyrophenones
  - Droperidol
  - haloperidol
  - Thioxanthenes
  - zuclopenthixol
  - Diphenylbutylpiperidines
  - Substituted benzamides
- **2st Gen:**
  - Amisulpride
  - Aripiprazole
  - Asenapine
  - Cariprazine
  - Clozapine
  - Lurasidone
  - Olanzapine
  - Paliperidone
  - Quetiapine
  - Risperidone
  - Loxapine
    
    
### 2. Brand drug list:
- **1st Gen:**
  - Chlorazin
  - Largactil
  - Moditen
  - Modecate
  - Nozinan
  - Levinan
  - Neulactil
  - Stemetil
  - Buccastem
  - Prazine
  - Stelazine
  - Terrazine
  - benperidol
  - Anquil
  - Benquil
  - Xomolix
  - Serenace
  - Haldol
  - Halkid
  - Dozic
  - flupentixol
  - Depixol
  - Psytixol
  - Fluanxol
  - Clopixol
  - Ciatyl
  - pimozide
  - Orap
  - Sulpiride
  - Dolmatil
  - Sulpitil
- **2nd Gen:**
  - Solian
  - Abilify
  - Arpoya
  - Sycrest
  - Reagila
  - Zaponex
  - Clozaril
  - Denzapine
  - Latuda
  - Zyprexa
  - Zalasta
  - Arkolamyl
  - Zypadhera
  - Xeplion
  - Trevicta
  - Byannli
  - Invega
  - Seroquel
  - Atrolak
  - Biquelle
  - Brancico
  - Mintreleq
  - Psyquet
  - Seroquel
  - Sondate
  - Zaluron
  - Ebesque
  - Seotiapim
  - Tenprolide
  - Zaluron
  - Okedi
  - Risperdal
  - Loxapac
  - Adasuve

### 3. Modifications

#### Removals:
- low dose prochlorperazine (commonly used for nausea rather than antipsychotics)
- Tranquilin (methylphenidate, used for ADHD)
        
#### Additions:
- None

---
## Benzodiazepines

### 1. Generic drug list:
- Alprazolam
- Chlordiazepoxide
- Clobazam
- Clonazepam
- Diazepam
- Flurazepam
- Loprazolam
- Lorazepam
- Lormetazepam
- Midazolam
- Nitrazepam
- Oxazepam
- Remimazolam
- Temazepam
    
### 2. Brand drug list:
- Xanax
- Librium
- Tropium
- Librax (Capsules)
- Frisium
- Perizam
- Tapclob
- Zacco
- Rivotril
- Klonopin
- Valclair
- Tensium
- Stesolid
- Diazemuls
- Dalmane
- Ativan
- Dormicum
- Hypnovel
- Miprosed
- Ozalin
- Epistatus
- Buccolam
- Somnite
- Mogadon
- Rohypnol
- Byfavo

### 3. Modifications:

#### Removals:
- Titropium bromide (inhalers)
#### Additions:
- key drugs matching string 'zolam', 'zepam'

*Side note: Interest in creating subset of drug list only including oral (rectal and injected versions tend to be used for rapid sedation or epileptic fits)*

---
## Dementia

### 1. Generic drug list:
- Cholinesterase inhibitors: Donepezil, Galantamine
- acetylcholinesterase inhibitors: Rivastigmine
- NMDA receptor antagonists: Memantine
    
### 2. Brand drug list:
- Aricept
- Reminyl
- Galzemic
- Gatalin
- Gazylan
- Lotprosin
- Luventa
- Zeebral
- Acumor
- Consion
- Elmino
- Gaalin
- Galsya
- Exilian
- Kerstipon
- Nimvastid
- Voleze
- Erastig
- Almuriva
- Alzest
- Eluden
- Prometax
- Somniton
- Valios
- Alzhok
- Ebixa
- Marixino
- Nemdatine


### 3. Modifications:

#### Removals:
- None

#### Additions:
- None

---
## Galantamine

### 1. Generic drug list:
    Galantamine
    
### 2. Brand drug list:
- Reminyl
- Galzemic
- Gatalin
- Gazylan
- Lotprosin
- Luventa
- Zeebral
- Acumor
- Consion
- Elmino
- Gaalin
- Galsya

### 3. Modifications:

#### Removals:
- None
        
#### Additions:
- None 

---
## Lithium

### 1. Generic drug list:
- Lithium
    
### 2. Brand drug list:
- Lithium carbonate
- Priadel
- Camcolit
- Lithonate
- Liskonum
- Lithium Chloride
- Li-liquid (or liliquid)
- Lithium Citrate
- Litarex

### 3. Modifications:

#### Removals:
- Efalith ointment
- Lithium succinate ointment
- Lithium Carbonicum (homeopathic meds)
- any other creams/ointments

#### Additions:
- None 

---
## Metformin

### 1. Generic drug list:
- Metformin
- Axpinet
- Bolamyn
- Diagemet
- Glucient
- Glucophage
- Glucorex
- Glyformin
- Jesacrin
- Meijumet
- Metabet
- Metformin
- Metsol
- Metuxtan
- Sukkarto
- Yaltormin
- Avandamet
- Competact
- Janumet
    
### 2. Brand drug list:
    
- Metformin
- Diagemet XL
- Yaltormin SR
- Glucient SR
- Avandamet
- Axpinet
- Janumet
- Sukkarto SR
- Glucophage SR
- Meijumet
- Glucophage
- Competact
- Yaltormin SR
- Jesacrin
- Metsol
- Glyformin
- Metabet SR
- Glucorex SR
- Bolamyn SR
- Pioglitazone%Metformin combination
- Metuxtan SR

Note: % wildcard  to indicate string pattern between the two drugs

### 3. Modifications:
#### Removals:
- Any ointments, creams, inhalers

#### Additions:
-  Eucreas
- Jentadueto
- Komboglyze
- Synjardy
- Vipdomet
- Vokanamet
- Xigduo

---
## Mirtazapine

### 1. Generic drug list:
- Mirtazapine
    
### 2. Brand drug list:
- Zispin

### 3. Modifications:

#### Removals:
- None

#### Additions:
- None 

    
---
## Monoamine Oxidase Inhibitors (MAOIs)


### 1. Generic drug list:
- Tranylcypromine
- Isocarboxazid
- Phenelzine
- Nardil
    
### 2. Brand drug list:
- TBC


### 3. Modifications:
#### Removals:
- None
#### Additions:
- Additional brand names added by manual search on drugs appearing on Code Builder 


---
## Rivastigmine

```
#SNOMED QUERY:
concept_find(ecl="<<763158003 : 127489000 |Has active ingredient (attribute) | =   <<395868008",limit=140)$idAndFsnTerm
```

### 1. Generic drug list:
- Rivastigmine
    
### 2. Brand drug list:
- Nimvastid
- Erastig
- Eluden
- Rivastigmine
- Prometax
- Almuriva
- Exelon
- Kerstipon
- Alzest
- Somniton
- Voleze


### 3. Modifications:

#### Removals:
- None

#### Additions:
- None 


---
## SNRIs (Serotonin and norepinephrine reuptake inhibitors)

### 1. Generic drug list:
- Venlafaxine
- Bupropion
- Desvenlafaxine
- Duloxetine
- Milnacipran
    
### 2. Brand drug list:
- Alventa
- Amphero
- Apclaven
- Bonilux
- Depefex
- Efexor, (Effexor)
- Foraven
- Majoven
- Mentaven
- Politid
- Ranfaxine
- Rodomel
- Tardcaps
- Tifaxin
- Tonpular
- Trixat
- Vaxalin
- Venaxx
- Vencarm
- Venlablue
- Venlafaxine
- Venlaneo
- Venlasov
- Vensir
- Venzip
- Vexarin
- Winfex
- ViePax
- Venladex
- Sunveniz
- Venlalic
- Zyban
- Dutor
- Yentreve
- Cymbalta
- Depalta
- Duciltia


### 3. Modifications:

#### Removals:
- Naltrexone with bupropion, buproprion (used for smoking cessation)

####Additions:
- None 


---
## Strong Opioids

#### 1. Generic drug list:
- Morphine
- Buprenorphine
- Dipipanone hydrochloride
- Diamorphine hydrochloride
- Alfentanil
- fentanyl
- remifentanil
- Metha  hydrochloride
- Oxyco
- morphine
- Pentazocine
- Papaveretum
- dihydrocodeine tartrate
- Pethidine hydrochloride
- Tapentadol
- Tramadol hydrochloride

#### 2. Brand drug list:
- alfentanil
- rapifen
- butrans
- bunov
- bupeaze
- buplast
- bupramyl
- buprenorphine
- busiete
- butec
- buvidal
- carlosafine
- espranor
- gabup
- hapoctasin
- natzon
- panitaz
- prefibin
- prenotrix
- rebrikel
- reletrans
- relevtec
- sevodyne
- sixmo
- suboxone
- subutex
- temgesic
- tephine
- transtec
- turgeon
- zubsolv
- diamorphine
- ayendi
- dhc continus
- dihydrocodeine
- df 118 forte
- diconal
- dipipanone
- abstral
- actiq
- breakyl
- cynril
- durogesic
- effentora
- fencino
- fenhuma
- fentalis
- fentanyl
- instanyl
- ionsys
- matrifen
- mezolar
- mylafent
- opiodur
- osmach
- osmanil
- pecfent
- recivit
- sublimaze
- tilofyl
- victanyl
- yemex
- methadone
- metharose
- methadose
- synastone
- physeptone
- eptadone
- actimorph
- chloroform
- cyclimorph
- depodur
- filnarine
- kaolin and morphine
- mst continus
- mxl
- morcap
- morphgesic
- morphine
- oramorph
- rhotard morphine
- sevredol
- zomorph
- abtard
- candox
- carexil
- dolocodon pr
- ixyldone
- leveraxo
- longtec
- lynlor
- onexila xl
- oxeltra
- oxycontin
- oxynorm
- oxyact
- oxycodone
- oxylan
- oxypro
- proladone
- reltebon
- renocontin
- shortec
- zomestine
- papaveretum
- aspav
- pentazocine
- fortral
- pamergan
- pethidine
- ultiva
- remifentanil
- ationdo sr
- palexia
- tapimio
- tapentadol


### 3. Modifications:

#### Removals:
- Chloroform
- apomorphine
- Ammonium chloride morphine mix
- BeneFoot medical shoe
- OptiSmooth Mitro XL catheter
- Panoxylan (acne treatment gel)
- Hydroxyprogesterone
- dihydrocodeine (and co-dydramol, df 118, dhc continus brand names)
- kaolin
- Mgn-3 arabinoxylan
- morphine gel (for topical pain relief of a wound)
- diocalm Morphine hcl and activated attapulgite and attapulgite
- Chalk morphine aromat
- Peppermint oil mixtures
- Ipecacuanha


#### Additions:
- fortagesic -(combination)  Fortagesic Tablet (Sanofi-Synthelabo Ltd) Paracetamol/Pentazocine Hydrochloride Tablet Oral
- omnopon - Omnopon 10mg Tablet (Roche Products Ltd) Codeine Phosphate/Papaverine Hydrochloride/Morphine Hydrochloride 10mg Tablet Oral
- oxyargin - Oxyargin 40mg/20mg modified-release tablets (Mylan) Oxyargin 40mg/20mg modified-release tablets Modified-release tablet Oral Naloxone hydrochloride/ Oxycodone hydrochloride 20.000mg + 40.000mg
- Myloxifin- Myloxifin 40mg/20mg modified-release tablets (Zentiva) Myloxifin 40mg/20mg modified-release tablets Modified-release tablet Oral Naloxone hydrochloride/ Oxycodone hydrochloride 20.000mg + 40.000mg
- Targinact -Targinact 40mg/20mg modified-release tablets (Napp Pharmaceuticals Ltd) Modified-release tablet Oral Naloxone hydrochloride/ Oxycodone hydrochloride 20.000mg + 40.000mg
- cigarettes (as it does seem to be a (unconventional) method of giving opioids as analgesia/ to wean people off heroin)


---
## Tricyclic Antidepressants
*-pramine and -tryptiline are typical suffixes.*

### 1. Generic drug list:
- clomipramine hydrochloride
- imipramine hydrochloride
- amitriptyline hydrochloride
- dosulepin hydrochloride
- doxepin
- mianserin hydrochloride
- trazodone hydrochloride
- trimipramine
- lofepramine
- nortriptyline
- Vortioxetine,

### 2. Brand drug list:
- Clomipramine
- Anafranil
- Imipramine
- Tofranil
- amitriptyline
- Triptafen
- Lentizol
- Dosulepin
- Dothapax
- Prepadine
- Prothiaden
- Thaden
- Sinequan
- Sinepin
- Xepin
- Mianserin
- Molipaxin
- Trazodone
- Surmontil
- Feprapax
- Gamanil
- Lomont
- Motival
- Allegron
- Motipress


### 3. Modifications:

#### Removals:
- flupentixol
- melitracen
- Depixol
- Psytixol
- Fluanxol
- Brintellix (antipsychotics)
- 'creams' (used for eczema)
- ointments


#### Additions:
- None

---
## Weak Opioids

### 1. Generic drug list:
- Codeine phosphate
- Dihydrocodeine tartrate
- Meptazinol


### 2. Brand drug list:
- panadol ultra
- ibuprofen and codeine
- co-codamol
- migraine relief
- codafen continus
- paracodol
- solpadeine
- bepro
- kapake insts
- zipamol plus
- panadol ultra
- kaodene
- tylex
- solpadol
- medocodene
- solpaflex
- terpin
- emcozin
- galcodine
- kapake
- zapain
- codipar
- pulmo bailly
- feminax
- nurofen plus
- cuprofen plus
- migraleve
- codeine
- dhc continus
- dihydrocodeine
- df 118 forte
- meptid
- aceon
- brimisol
- dromadol
- invodol
- larapam
- mabron
- maneo
- marol
- maxitram
- nobligan
- oldaram
- tilodol
- tradorec
- tramacet
- tramadol
- tramake
- tramquel
- tramulief
- trapadex
- zamadol
- zeridame
- zydol
- zytram


### 3. Modifications:

#### Removals:
- Chloroform
- apomorphine
- Ammonium chloride morphine mix
- BeneFoot medical shoe
- OptiSmooth Mitro XL catheter
- Panoxylan (acne treatment gel)
- cough mixtures
- Hydroxyprogesterone
- %marol% strings excluding ^Marol$ expression.

#### Additions:
- None

#### Removals at review stage:

These are not opioids or they are used primarily as cough suppressants (in low doses):
- benylin - cough mixture
- menthol
- terpin
- codeine linctus - cough mixture
- mixture
- syrup
- kaolin
- pastille
- chloroxylenol - anti septic
- Dextromethorphan
- Brompheniramine /codeine
- promethazine
- phensedyl
- pseudoephedrin
- Dimotane With Codeine Elixir
- codeine 5mg/5ml or 6.75mg/ml
- feminax express and ultra - just NSAID no opioid.
- galcodine - cough mixture
- Kaodene - loperamide
- migraleve ultra - sumitriptan

#### Combinations added at review stage:
- codamin - combination Codanin Tablet (Wyeth Consumer Healthcare) Codeine Phosphate/Paracetamol Tablet
- Dypracet- combination Dypracet 20mg/500mg tablets (Auden McKenzie (Pharma Division) Ltd) Dihydrocodeine tartrate/Paracetamol Tablet Oral
- Eroset - combination Eroset 500mg/10mg tablets (M & A Pharmachem Ltd) Paracetamol/Dihydrocodeine tartrate 500mg + 10mg Tablet Oral
- formulix - combination Formulix Oral solution (Cilag Pharmaceuticals Ltd) Codeine Phosphate/Paracetamol Oral Solution Oral
- galake - combination Galake 10mg/500mg tablets (Galen Ltd)Paracetamol/Dihydrocodeine tartrate500mg + 10mgTabletOral
- syndol - combination Generic Syndol caplets Caffeine/Paracetamol/Codeine phosphate/Doxylamine succinate 30mg + 450mg + 10mg + 5mg Tablet Oral
- hypon and parahypon - Hypon Tablet (Wellcome Medical Division) Calcium Carbonate/Caffeine Citrate/Citric Acid/Codeine Phosphate/Aspirin Tablet Oral
- omnopon tablet - Omnopon 10mg Tablet (Roche Products Ltd) Codeine Phosphate/Papaverine Hydrochloride/Morphine Hydrochloride 10mg Tablet Oral
- painex - Painex caplets (Sandoz Ltd) Paracetamol/Doxylamine succinate/Caffeine/Codeine phosphate 450mg + 5mg + 30mg + 10mg Tablet Oral
- panadeine - Panadeine Tablet (GlaxoSmithKline UK Ltd) Paracetamol/Codeine phosphate 500mg + 8mg Tablet Oral
- parake - Parake Tablet (Galen Ltd) Paracetamol/Codeine phosphate 500mg + 8mg Tablet Oral
- paramol Paramol soluble tablets (SSL International Plc) Dihydrocodeine tartrate/Paracetamol 7.46mg + 500mg Effervescent tablet Oral
- syndol = Syndol caplets (Sanofi) Paracetamol/Doxylamine succinate/Caffeine/Codeine phosphate 450mg + 5mg + 30mg + 10mg Tablet Oral
- veganin - Veganin tablets (Omega Pharma Ltd) Tablet Oral Caffeine/ Codeine phosphate/ Paracetamol 30.000mg + 8.000mg + 500.000mg
