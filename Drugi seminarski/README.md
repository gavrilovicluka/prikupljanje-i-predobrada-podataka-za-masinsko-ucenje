# Uticaj kvaliteta i predobrade slika na performanse modela za klasifikaciju bolesti na listovima biljaka

Ovaj repozitorijum sadrzi seminarski rad iz predmeta **Prikupljanje i predobrada podataka za masinsko ucenje**, na master akademskim studijama Elektronskog fakulteta u Nisu, koji istrazuje uticaj razlicitih tehnika predobrade slika na performanse konvolucione neuronske mreze (CNN) u zadatku klasifikacije bolesti biljaka.

## 📊 Dataset

Za istrazivanje je koriscen [PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset), koji sadrzi slike listova biljaka sa razlicitim bolestima i zdravim klasama.

Potrebno je preuzeti skup podataka i smestiti ga u folder `.\data`.

## 🔬 Eksperimenti

Sprovedeno je ukupno **5 eksperimenata** sa razlicitim tokovima predobrade:

- baseline (resize + normalizacija)
- denoising (Gaussian + Median filter)
- transformacije prostora boja (LAB)
- segmentacija pozadine
- kompletna augmentacija (geometrijska + fotometrijska + CutMix)

## ⚙️ Instalacija biblioteka

- Kreiranje virtuelnog okruzenja: `python -m venv .venv`
- Aktivacija (Windows PowerShell): `.\.venv\Scripts\Activate.ps1`
- Nakon aktivacije, u terminalu treba da se pojavi prefiks `(.venv)`
- Instalacija potrebnih biblioteka: `pip install -r requirements.txt`