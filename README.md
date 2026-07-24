# Between-the-lines

# Tra le righe del catalogo: 
**Analisi esplorativa dei metadati bibliografici, dinamiche di genere ed evoluzione temporale**

## DOI
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)
METTI IL DOIIIII

## Descrizione

### In cosa consiste il progetto?

Il progetto consiste nella pulizia e analisi esplorativa di un dataset di metadati bibliografici. 

L'obiettivo principale di questo progetto è la pulizia e riordino, con finalità di analisi e pubblicazione aperta. Le domande di ricerca proposte andranno ad analizzare la distribuzione di genere, esplorare l'evoluzione dei temi trattati nel tempo all'interno delle pubblicazioni dal 1900 ad oggi, e se siano occorse variazioni significative ed identificare se esiste una relazione tra gli editori e riviste rispetto alle licenze utilizzate.

### Quali sono i risultati?

- **Analizzare** la distribuzione di genere all'interno delle pubblicazioni presenti nel dataset.
- **Esplorare** l'evoluzione dei temi trattati nel tempo all'interno delle pubblicazioni, e se ci siano state delle variazioni significative.
- **Identificare** se esiste una relazione tra gli editori e riviste rispetto alle licenze Open Access.

## Fonte dei dati

### Descrizione dei dati
Il dataset contiene le informazioni catalografiche delle pubblicazioni, tra cui identificativi, titoli, autori, genere dell'autore, editori, anni di pubblicazione e consistenza delle pagine.

| Variabile           | Tipo     |	Definizione                      | Esempio |
| :-------            | :---     | :---------                        | :------ |
|id                   |object    |chiave identificativa              |0	http://www.wikidata.org/entity/Q136384321|
|titolo               |object    |titolo dell'opera                  |Si tocca Corfù. Viaggi in Levante
|autori               |object    | autore e/o curatore               |Giacomo Caputo (maschio)
|data_pubblicazione   |	object   | data di pubblicazione             |1931
|argomenti            |	object   |temi trattati                      |bibliografia; bibliotecario
|basi_dati            |	object   |provenienza dei dati               |Scopus; Arts and Humanities Citation Index;
|doi_disponibili      |	object   |DOI dell'opera                     |10.53223/SINAPPSI_2024-01-5
|editori              |	object   |editore responsabile               |Idest
|licenze_rivista      |	object   |licenze dell'opera                 |Creative Commons Attribution-NonCommercial-NoD...
| rivista             |	object   |rivista di pubblicazione           |AIB studi
|edizione             |	object   |numero/anno di edizione            |543
|volume               |	object   |numero di volume                   |90
|pagine               |	object   |intervallo di pagine o pagina singola   |18
|url_disponibili      |	object   |eventuali siti correlati                |http://www.ricerchedisconfine.info/index.htm

### Citazione e link alle fonti dei dati utilizzati
I dati sono in formato CSV.
- **Link alla fonte:** https://raw.githubusercontent.com/dhdmch/2025-2026/refs/heads/main/data/lispod/data.csv

## Metodi e strumenti

Il progetto è stato sviluppato in un ambiente Google Colab utilizzando il linguaggio di programmazione Python. Lo strumento principale utilizzato per la manipolazione, l'analisi e la visualizzazione dei dati è la libreria Pandas.

### Le operazioni includono:

- Caricamento e ispezione dei dati (df.info(), df.describe());
- Bonifica e normalizzazione dei dati (conversione in Int64, gestione dei dati nulli);
- Creazione di nuove variabili (pubblicazione_prima, volume_info, pagina_inizio, autore_sesso);
- Analisi esplorativa tramite aggregazioni (value_counts()) e visualizzazioni tramite diversi grafici;
- Analisi esplicativa focalizzata sull'evoluzione per decennio di genere, pubblicazioni e analisi dell'uso delle licenze;

### Strumenti utilizzati:
- **Linguaggio di programmazione:** Python
- **Ambiente di sviluppo:** Notebook Colab
- **Librerie per l'analisi dati e la manipolazione:** `pandas`, `numpy`
- **Librerie per la visualizzazione grafica:** `matplotlib`
- **Controllo versione e Open Science:** GitHub, Zenodo

## Responsabili
- **Ambra Martiri** -  Autore/Studentessa

## Licenza

I dati di input e il codice di output (incluso in questo Notebook) sono rilasciati sotto licenza CC0 1.0 Universal.
