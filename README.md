# Jailbreaking&LLM: Analisi a due livelli

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20Scikit--Learn%20%7C%20Seaborn-brightgreen)
![Hugging%20Face](https://img.shields.io/badge/Hugging%20Face-%F0%9F%A4%97-yellow)
![](https://img.shields.io/badge/Transformer-all--MiniLM--L6--v2-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## Motivazioni

L'obiettivo del presente progetto è analizzare un dataset di prompt e costruire
un classificatore capace di distinguere tra **prompt safe** e **prompt malevoli**.

L'analisi confronta due approcci distinti:

- **Approccio statistico** basato su feature strutturali del prompt  
  (lunghezza, numero di parole, punteggiatura, keyword sospette, ecc.)
- **Approccio semantico** basato su **embeddings** generati da modelli di linguaggio

Il progetto mostra come l'approccio semantico sia più efficace nel riconoscere
prompt malevoli, riducendo significativamente i **false negatives**
rispetto al modello basato su feature statistiche.

---

## Metodologia
- Pulizia e preparazione del dataset
- Feature engineering (livello 1)
- Classificazione statistica
- Generazione embeddings (livello 2)
- Classificazione semantica
- Analisi degli errori e clustering dei prompt malevoli

---

## Risultati
- Migliore recall per la classe *malicious*
- Riduzione dei false negatives
- Individuazione di famiglie di attacchi jailbreak tramite clustering

---

## Strumenti
- Python ( Pandas, Numpy, Scikit-learn, Seaborn / Matplotlib )
- Sentence Transformers (all-MiniLM-L6-v2)
