# Izbor atributa (Feature Selection)

Ovaj repozitorijum sadrzi seminarski rad iz predmeta **Prikupljanje i predobrada podataka za masinsko ucenje**, na master akademskim studijama Elektronskog fakulteta u Nisu, koji istrazuje uticaj razlicitih tehnika izbora karakteristika na modele masinskog ucenja.

## 📊 Dataset

Za istrazivanje je koriscen [SECOM Dataset](https://www.kaggle.com/datasets/paresh2047/uci-semcom), koji sadrzi podatke iz procesa proizvodnje poluprovodnika.

Potrebno je preuzeti skup podataka i smestiti ga u folder `.\data`.

## 🔬 Eksperimenti

U okviru eksperimenta su obradjene su sledece metode za selekciju karakteristika:

1. Filter metode
    - Variance Threshold
    - Chi-Square
    - Pearson Correlation
    - Mutual Information
    - Fisher's Score

2. Embedded metode
    - LASSO (L1 Logistic Regression)
    - Ridge (L2 Logistic Regression)
    - ElasticNet (L1 + L2)
    - Decision Tree (Gini importance)
    - ExtraTrees (ensemble feature importance)

3. Wrapper metode
    - RFE (Recursive Feature Elimination)
    - SFS (Sequential Forward Selection)
    - SBE (Sequential Backward Elimination)

4. Hibridne metode
    - Variance -> Mutual Information -> RFE
    - Variance -> Chi2 -> RFE

## ⚙️ Podesavanje okruzenja i instalacija biblioteka

- Kreiranje virtuelnog okruzenja: `python -m venv .venv`
- Aktivacija (Windows PowerShell): `.\.venv\Scripts\Activate.ps1`
- Nakon aktivacije, u terminalu treba da se pojavi prefiks `(.venv)`
- Instalacija potrebnih biblioteka: `pip install -r requirements.txt`