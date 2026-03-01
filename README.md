# 🇪🇸 Analiza i predviđanje energetskog balansa Španije

Ovaj projekat predstavlja sveobuhvatnu analizu elektroenergetskog sistema Španije sa fokusom na odnos između potražnje za električnom energijom i proizvodnje iz obnovljivih izvora (vetar i sunce).

## 📌 Cilj projekta

Glavni cilj je razvoj preciznih modela mašinskog učenja za predviđanje energetskog balansa na osnovu meteoroloških podataka iz pet ključnih gradova:
Madrid
Barcelona
Valencia
Seville
Bilbao

Analiza je podeljena u dve celine:
### 1️⃣ Analiza potražnje (Demand Side)

Ispituje se uticaj temperature i sezonalnih faktora na ukupno opterećenje mreže.

### 2️⃣ Analiza ponude (Supply Side)

Analizira se zavisnost proizvodnje energije vetra i sunca od atmosferskih parametara (brzina vetra, oblačnost, vlažnost vazduha).

## 🔍 Ključni nalazi analize
### 🔹 1. Dinamika potrošnje (Load)

Termalni odziv – “U-kriva”
Uočena je nelinearna zavisnost između temperature i potrošnje. Potrošnja raste pri ekstremnim temperaturama:
  - ispod 15°C (grejanje)
  - iznad 25°C (hlađenje)

Sezonalnost
Januar je mesec sa najvećim kontrastima – beleži:
  - godišnje maksimume tokom hladnih talasa
  - značajne minimume tokom praznika (1. i 6. januar)

Dnevni profil
Izražen je večernji pik potrošnje oko 19:00h.

### 🔹 2. Proizvodnja iz obnovljivih izvora

Varijabilnost vetra
Proizvodnja vetroelektrana pokazuje visoku volatilnost i snažnu korelaciju sa brzinom vetra, naročito u severnim regionima (Bilbao).

Efikasnost solarne energije
Proizvodnja solarnih elektrana snažno zavisi od:

stepena oblačnosti

vlažnosti vazduha

Sezonski vrhunac proizvodnje beleži se tokom jula.

Komplementarnost izvora
Analizirano je kako energija vetra nadoknađuje pad solarne proizvodnje nakon zalaska sunca, čime se povećava stabilnost sistema.

## 🤖 Mašinsko učenje (Modeling)

Korišćena su dva napredna algoritma radi povećanja robusnosti i pouzdanosti predikcija:

  - XGBoost
  - Random Forest
## 🛠️ Tehnološki stack

Jezik: Python

Obrada podataka: Pandas, NumPy

Vizuelizacija: Matplotlib, Seaborn

ML biblioteke: Scikit-learn, XGBoost

## 📈 Rezultati i zaključak

Integracijom modela potražnje i modela proizvodnje razvijen je sistem koji:

  - predviđa ukupnu potrošnju električne energije

  - procenjuje koliki deo te potrošnje može biti pokriven iz obnovljivih izvora u realnom vremenu

Ovakav pristup omogućava:

  - optimizaciju rada termoelektrana

  - efikasnije upravljanje mrežom

   -smanjenje emisije CO₂
