# Vežbe za kolokvijum iz NAP-a (text mining)

Svaka sveska ima gotovu pripremu podataka (učitavanje, čišćenje, izlazna varijabla, odluka o kolonama, podela na trening i test).
Od ćelije **▶ OVDE KREĆEŠ** sve kucaš sam. Na dnu svake sveske je "dati kod" koji dobijaš na kolokvijumu.

Sveske se pokreću iz foldera `notebooks/`, a podaci se čitaju iz `../data` (SBERT model iz `../models`).

## Klasifikacija

| Sveska | Reprezentacija | Klasifikator | Podaci |
|---|---|---|---|
| K1 | TF-IDF | logistička regresija | McDonald's (profesorkin primer) |
| K2 | BoW + numeričke kolone | stablo odlučivanja | mobilne aplikacije, 3 klase |
| K3 | spaCy vektori reči (FunctionTransformer) | SVM + SMOTE | tvitovi avio-kompanijama |
| K4 | spaCy vektori reči (sopstvena klasa) | logistička regresija + SMOTE | TripAdvisor hoteli |
| K5 | BoW (TF) + one-hot `Branch` | SVM, linearni kernel | Disneyland (profesorkin primer 2) |
| K6 | TF-IDF | LR naspram stabla, pa podešeno stablo | E-Commerce odeća |
| K7 | TF-IDF + RobustScaler + one-hot | logistička regresija | Women's Clothing, uzorak 5000 |
| K8 | TF-IDF + MinMaxScaler | SVM, pa SVM + SMOTE | mobilne aplikacije, 4 klase |

## Klasterizacija

| Sveska | Reprezentacija | Podaci |
|---|---|---|
| C1 | spaCy vektori reči | Guardian (profesorkin primer) |
| C2 | SBERT all-MiniLM-L12-v2 | E-Commerce odeća (profesorkin primer 2) |
| C3 | po izboru, uz obrazloženje | Amazon komentari |
| C4 | spaCy vektori reči + provera sa rubrikom | BBC RSS vesti 2023 |
| C5 | SBERT + provera sa kategorijom | BBC arhiva 2004-2005 |

`models/` je u `.gitignore`, jer je model 130 MB i GitHub ga ne bi primio.
