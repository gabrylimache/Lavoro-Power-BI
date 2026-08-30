Valentino Starace, Limache Gabriele, Manarini Andrea, Endaya Zeus, Bertarelli Manuel
# power-bi-food-sales-dashboard
End-to-end Power BI sales analytics project featuring data cleaning, star schema modeling, DAX measures, interactive dashboards and technical documentation.
# Power BI Food Sales Analytics

## Descrizione del progetto

Questo repository contiene un progetto completo di **Business Intelligence sviluppato in Microsoft Power BI** per analizzare le vendite di una società simulata operante nel settore della distribuzione alimentare.

Il progetto è stato realizzato partendo da un dataset reperito su **Kaggle**, successivamente analizzato, pulito, corretto e arricchito per renderlo coerente con gli obiettivi di reporting.

Il lavoro comprende l'intero processo di sviluppo di una soluzione BI:

- analisi e pulizia dei dati;
- correzione delle categorie prodotto;
- ricostruzione della struttura geografica;
- modellazione dei dati;
- creazione di una tabella calendario;
- sviluppo di misure DAX;
- progettazione di dashboard interattive;
- implementazione di filtri e funzionalità di drill down;
- realizzazione della documentazione tecnica;
- creazione del manuale utente.

---

## Obiettivi di business

Il report è stato progettato per rispondere alle seguenti domande:

- Qual è il valore complessivo delle vendite?
- Come cambiano ricavi e quantità nel tempo?
- Quali categorie prodotto generano il maggiore fatturato?
- Quali continenti, paesi e città presentano le performance migliori?
- Qual è la differenza tra andamento dei ricavi e andamento dei volumi?
- Come si confrontano i risultati con il mese e l'anno precedente?
- Quali classi di prodotto contribuiscono maggiormente alle vendite?

---

## Dataset

Il dataset finale utilizzato per il report presenta le seguenti caratteristiche:

- **18.000 transazioni di vendita**
- periodo analizzato: **2023-2025**
- **163 città**
- **72 paesi**
- **6 continenti**
- dimensioni dedicate a prodotti, categorie, clienti, dipendenti, città, paesi e date

> **Nota sulla provenienza dei dati**
>
> Il dataset iniziale è stato reperito su Kaggle. Alcune classificazioni dei prodotti, informazioni geografiche e transazioni di vendita sono state corrette, arricchite o generate in modo controllato per ottenere uno scenario dimostrativo coerente su tre anni.
>
> I dati non rappresentano le prestazioni di una società reale e vengono utilizzati esclusivamente a scopo didattico e di portfolio.

---

## Problemi individuati nei dati iniziali

Durante l'analisi preliminare sono state rilevate diverse incoerenze.

### Categorie prodotto errate

Alcuni prodotti erano associati a categorie non coerenti con il loro nome.

Esempi:

- prodotti a base di frutta secca associati alla categoria `Meat`;
- prodotti vegetali associati alla categoria `Poultry`;
- vini e bevande associati a categorie non pertinenti;
- prodotti non alimentari inseriti in categorie alimentari.

### Struttura geografica incoerente

La tabella iniziale delle città conteneva prevalentemente città statunitensi, successivamente associate a paesi internazionali non coerenti.

Esempi di combinazioni errate:

```text
Chicago, Norway
Montgomery, Bulgaria
Minneapolis, Rwanda
