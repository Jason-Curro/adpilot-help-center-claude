---
id: "csv-errors"
title: "Risolvere gli errori di importazione CSV"
description: "Capire perché il file CSV viene rifiutato."
category: "troubleshooting"
feature: "troubleshooting"
audience: "merchant"
difficulty: "beginner"
language: "it"
plans: ["PRO"]
keywords: ["csv", "error", "missing column", "encoding", "file"]
last_reviewed: "2026-11-17"
translation_id: "csv-errors"
related: ["csv-requirements", "upload-csv"]
---

# Risolvere gli errori di importazione CSV

## Controlli iniziali
Se l'Optimizer rifiuta un report, verifica prima i requisiti di [Formato CSV e colonne obbligatorie](../optimizer/csv-requirements.md). Il messaggio esatto aiuta a individuare il problema.

| Messaggio o sintomo | Cosa controllare |
| --- | --- |
| Nessun file selezionato | Seleziona il CSV prima di inviare. |
| File `.csv` richiesto | Esporta CSV, non `.xlsx` né un foglio rinominato. |
| Troppo piccolo / vuoto | Esporta dati reali; minimo 1 KiB. |
| Troppo grande | Riduci l'intervallo; massimo 10 MiB. |
| Codifica non supportata | Salva in UTF-8, non UTF-16. |
| Separatore non supportato | Usa virgola o punto e virgola. |
| Colonne mancanti | Confronta le intestazioni con le 13 categorie obbligatorie. |
| Troppe righe / colonne | Massimo 50.000 righe di dati e 200 colonne. |
| Nessuna riga valida | Verifica che ci siano dati utilizzabili oltre all'intestazione. |
| Non è un CSV di testo valido | Esporta un CSV pulito direttamente da Meta Ads Manager. |

## Se il caricamento riesce ma i valori sono sbagliati
1. Confronta spesa e acquisti totali in AdPilot con lo stesso periodo in Meta Ads Manager.
2. Riesporta **una sola campagna per file**, con numeri semplici e senza separatori delle migliaia.
3. Verifica che la colonna **valore acquisti** non contenga il ROAS e che le informazioni su pubblico/interesse siano autentiche.
4. Se le cifre sono ancora diverse, **non applicare** i suggerimenti e contatta l'assistenza AdPilot senza pubblicare il report privato.

## Procedura consigliata
1. Riesporta il report originale con le colonne richieste.
2. Se necessario, controlla codifica e separatori con un editor di testo.
3. Dopo la correzione, prova il caricamento **una volta**.
4. Se il messaggio persiste, annotalo per il supporto invece di condividere il file originale in chat.

Per la procedura completa, leggi [Caricare un CSV nell’Optimizer](../optimizer/upload-csv.md).
