# Simulazioni dell'algoritmo ibrido VQE per la soluzione di problemi di ottimizzazione combinatoria

Tesi di Petru Marcel Marincas per la laurea triennale in **Informatica dell'Università degli Studi di Bologna**, anno accademico 2023/2024.

## Introduzione

L'obbiettivo di questa tesi è l'implementazione e l'analisi dell'algoritmo ibrido VQE per la soluzione del Traveling Salesman Problem (TSP) e del Knapsack Problem (KP). Si tratta di un algoritmo che fa uso di un circuito quantistico in combinazione con un ottimizzatore classico ed è una soluzione promettente che potrebbe essere già efficiente ed utilizzabile per problemi di ottimizzazione combinatoria di dimensioni ridotte nell'era NISQ (Noisy Intermediate-Scale Quantum).

## Struttura del repository

Il repository è strutturato come segue:

- `src/`: contiene il codice sorgente dell'algoritmo ibrido VQE per la soluzione del TSP e del KP.
- `thesis/`: contiene il PDF della tesi.

## Tecnologie utilizzate

Il linguaggio utilizzato per l'implementazione è **Python** ed il framework di sviluppo è **Qiskit**.

In particolare nel progetto sviluppato abbiamo fatto uso delle seguenti versioni:

| Pacchetto     | Versione |
|---------------|----------|
| Qiskit        | 1.3.2    |
| Qiskit Aer    | 0.15.1   |

## Il codice sorgente

Il codice sorgente è diviso in due parti principali:
- **Metodi classici**: implementazione di algoritmi classici per la soluzione del TSP e del KP.
  - Questo serve per introdurre i problemi, indicare quali sono i risultati ottimali che si possono ottenere e creare dei metri di paragone futuri per valutare l'efficacia dell'algoritmo ibrido VQE.
  - Si tratterà dapprima di una descrizione del formalismo matematico della programmazione lineare intera nella descrizione di questi programmi, per poi passare alla descrizione degli algoritmi classici esatti ed euristici e, in buona parte dei casi, una loro implementazione in Python con l'uso di librerie come NumPy e Matplotlib per la visualizzazione dei risultati.
- **Metodi quantistici**: implementazione dell'algoritmo ibrido VQE per la soluzione del TSP e del KP.
  - Andremo ad introdurre l'algoritmo VQE, passo per passo, descrivendo il circuito quantistico e l'ottimizzatore classico utilizzato.
  - Si procederà con l'implementazione dell'algoritmo in Python con l'uso di Qiskit e si valuterà l'efficacia dell'algoritmo ibrido VQE confrontando i risultati ottenuti con quelli dei metodi classici.
    - Realisticamente, non ci si aspetta che l'algoritmo ibrido VQE sia più efficiente dei metodi classici per problemi di dimensioni ridotte, ma si vuole valutare se l'algoritmo è già utilizzabile e se è possibile ottenere risultati accettabili in tempi ragionevoli.
  - Infine, si discuteranno i risultati ottenuti e si proporranno possibili sviluppi futuri.

Il codice sorgente sarà disponibile come **Jupyter Notebook**.

Verranno sia caricate una versione statica dei notebook, in formato PDF, sia una versione interattiva, in formato `.ipynb`, che potrà essere eseguita in locale o su **Google Colab**.

