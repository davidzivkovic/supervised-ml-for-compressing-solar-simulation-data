# supervised-ml-for-compressing-solar-simulation-data
Using supervised neural network for compressing MURaM simulation of solar atmosphere. The goal is to try and compress the fits cube from the simulation to a smaller size using ML.

# 🔍 Analiza prodaje — Predikcija prihoda

Projekat predviđanja mesečnih prihoda korišćenjem machine learning modela na osnovu istorijskih podataka o prodaji.

## 📋 Sadržaj
- [Opis projekta](#opis-projekta)
- [Instalacija](#instalacija)
- [Rezultati](#rezultati)

---

## 📌 Opis projekta

Cilj projekta je izgradnja modela koji predviđa prihode za naredni mesec na osnovu:
- Istorijskih podataka o prodaji (2020–2024)
- Sezonskih trendova
- Kategorija proizvoda

## 🛠️ Tehnologije

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Scikit-learn](https://img.shields.io/badge/ScikitLearn-1.3-orange)

## ⚙️ Instalacija

```bash
git clone https://github.com/username/ime-projekta.git
cd ime-projekta
pip install -r requirements.txt
```

## 📁 Struktura projekta

```
├── data/
│   ├── raw/          # Originalni podaci
│   └── processed/    # Obrađeni podaci
├── notebooks/
│   └── analiza.ipynb
├── images/
│   └── plot.png
└── README.md
```

## 📊 Rezultati

Model postiže **R² = 0.94** na test skupu.

### Predikcija vs stvarne vrednosti

<p align="center">
  <img src="images/plot.png" width="700">
</p>

### Važnost featera

<p align="center">
  <img src="images/feature_importance.png" width="600">
</p>

## 🚀 Pokretanje

```bash
jupyter notebook notebooks/analiza.ipynb
```

## 📝 Zaključak

Random Forest model pokazuje najbolje rezultate sa RMSE od 1.240€.
Sezonalnost i kategorija proizvoda su najuticajniji faktori.

---

## 👤 Autor

**Ime Prezime** — [GitHub](https://github.com/username) · [LinkedIn](https://linkedin.com/in/username)
