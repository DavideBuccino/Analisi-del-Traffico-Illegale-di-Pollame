🐔💣 Chickens Under Surveillance: Analisi del Traffico Illegale di Pollame
In questo progetto, sviluppato con l’ausilio delle lezioni YouTube del Dott. Pietro Savastano, ho combinato Python e data visualization per esplorare uno scenario surreale quanto stimolante: il traffico internazionale di polli correlato ai crimini registrati nei diversi paesi.
📌 Strumenti utilizzati:
- Librerie Python: pandas, seaborn, matplotlib, os
- Fonti dati:
- FAO (scambi commerciali di animali vivi)
- UNODC (United Nations Office on Drugs and Crime — statistiche sui crimini)

🧪 Step operativi:
- 📂 Data Preprocessing:
- Importazione e filtraggio del dataset FAO per isolare transazioni legate al pollo (chickens.csv)
- Pulizia del dataset ONU (theft.xlsx) per estrarre il conteggio dei crimini per nazione e anno
- Uniformazione dei nomi delle colonne (Area → Country, ecc.) per preparare la join tra i due dataset
- 🔄 Merge & Analisi quantitativa:
- Creazione del dataframe criminal_traffic tramite merge su Country e Year
- Estrazione delle variabili chiave:
- value (valore monetario delle transazioni di polli)
- count (numero di crimini registrati)
- Generazione della metrica CCM (value × count, poi normalizzata / 1.000.000) per stimare il potenziale impatto economico nei paesi con alti tassi criminali
- 🧽 Filtraggio finale & Visualizzazione:
- Selezione dei dati dal 2013 in poi e solo per quantità esportate (Export Quantity)
- Ordinamento sulla base della metrica CCM
- Costruzione di pivot table per analisi per continente e paese
- 🕵️‍♂️ Output operativo:
- I dati sono stati segmentati per continenti: Africa, Americas, Asia, Europe, Oceania
- Creazione di una cartella per ogni “agente segreto” usando la libreria os, in modo da fornire report mirati per ciascuna regione

🎯 Obiettivo del progetto:
Comunicare agli “agenti segreti dei dati” i paesi più sospetti per traffico di pollame, incrociando esportazioni e incidenza criminale — il tutto in modo strutturato, visualizzabile e filtrabile.
📊 Un esercizio didattico che unisce ETL, analisi quantitativa e storytelling creativo con i superpoteri di Python, in particolar modo della libreria Pandas.
