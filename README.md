# Supervised machine learning for compressing the solar simulation data
Here we are trying to use supervised neural network for compressing MURaM simulation of solar atmosphere. The goal is to try and compress the fits cube from the simulation to a smaller size using ML.

In this directory there are a couple of notebooks with different sizes of neural networks and different aproaches in normalization of targeted physical parameters to explore how it influences the compression of the data.

- The notebooks are named **nn-compression_{type of normalization}_{compressed X times (bytes)}.ipynb**
- The compression ratio was calculated as: (no. of bytes in all targets) / (no. of parameters of neural network $\times$ 4)
- As it follows the best performing model is the one that compresses the size the lest, which is 5.3 times. In the results we will show plots of $p$ - pressure and $B_z$ - magnetic field in z direction. We will show $p$ because it has the lowest relative error and $B_z$ because it has the largest from all the physical parameters trough all the models
- Next to the model sizes we also investigated how normalization of $B$ and $p$ influenced the learning of models. We have only done this for 55.1 and 224.8 models, which are not the best performing ones :/

## Results
### 5.3 compression
### 17.2 compression
### 55.1 compression + arcsinh norm
### 224.8 compression + log norm



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
