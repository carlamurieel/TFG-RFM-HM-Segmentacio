# TFG — Segmentació de clients i predicció de churn al sector retail

**Treball Final de Grau** — Grau d'Estadística UB-UPC  
**Autora**: Carla Muriel Maillo
**Director**: Dr. Jordi Cortes  
**Convocatòria**: Juny 2026

## Descripció

Aquest repositori conté el codi font complet del Treball Final de Grau:

> **Segmentació de clients i predicció de churn en el sector retail: una aplicació al dataset d'H&M Group**

El treball desenvolupa un sistema integrat d'anàlisi de la cartera de clients d'H&M aplicant:
- Construcció de variables RFM (Recency, Frequency, Monetary)
- Segmentació no supervisada amb K-means (K = 4)
- Predicció de churn amb Regressió Logística i Random Forest
- Playbook estratègic d'accions diferenciades per segment

## Estructura del repositori

```
TFG-RFM-HM-Segmentacio/
├── 01_preproces_RFM.ipynb       # Capítol I: preprocés i RFM
├── 02_kmeans_segmentacio.ipynb  # Capítol II: K-means
├── 03_churn_prediction.ipynb    # Capítol III: predicció de churn
├── requirements.txt              # Dependències Python
└── README.md                     # Aquest fitxer
```

## Dataset

Les dades provenen de la competició pública **H&M Personalized Fashion Recommendations** (Kaggle, 2022):

🔗 https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations

El dataset **NO es distribueix** en aquest repositori per qüestions de mida i llicència. Cal descarregar-lo directament de Kaggle i col·locar-lo a la carpeta `data/`.

## Requisits

- Python 3.13
- Llibreries: pandas, numpy, scikit-learn, matplotlib
- Maquinari mínim recomanat: 16 GB de RAM

Per instal·lar les dependències:

```bash
pip install -r requirements.txt
```

## Reproductibilitat

Tots els notebooks utilitzen llavor aleatòria fixada (`random_state=42`) per garantir la reproductibilitat exacta dels resultats numèrics i de les figures del TFG.

## Resultats principals

- **994.320 clients** actius segmentats en 4 grups (Champions, En Risc, Compradors Recents, Hibernants)
- **Hopkins H = 0,9951**: validació de clusterabilitat
- **AUC = 0,779** (Random Forest) per a la predicció de churn
- **790 Champions amb risc de churn** identificats com a subpoblació crítica

## Llicència

MIT License — vegeu el fitxer LICENSE.

## Contacte

Per a qualsevol qüestió sobre el codi o els resultats, contacteu a:
📧 [carlaamuriel3@gmail.com]
