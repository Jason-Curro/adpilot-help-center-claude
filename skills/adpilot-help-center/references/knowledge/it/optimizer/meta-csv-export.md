---
id: "meta-csv-export"
title: "Esportare un report da Meta Ads Manager"
description: "Preparare il report destinato all’Optimizer di AdPilot."
category: "optimizer"
feature: "optimizer"
audience: "merchant"
difficulty: "beginner"
language: "it"
plans: ["PRO"]
keywords: ["meta", "ads manager", "export", "csv", "report"]
last_reviewed: "2026-11-17"
translation_id: "meta-csv-export"
related: ["csv-requirements", "upload-csv"]
---

# Esportare un report da Meta Ads Manager

## Preparare il report in Meta
L'interfaccia di Meta Ads Manager può cambiare. I passaggi seguenti riprendono le istruzioni presenti attualmente in AdPilot:

1. Apri **Meta Ads Manager** e raggiungi l'area Rapporti (Report / Report personalizzato).
2. Scegli l'intervallo delle date; AdPilot suggerisce dati recenti, per esempio **7–30 giorni**.
3. Seleziona la campagna da analizzare e il livello **Gruppo di inserzioni**; prepara **un file per ogni campagna**.
4. Includi le metriche in [Formato CSV e colonne obbligatorie](../optimizer/csv-requirements.md), in particolare il **valore acquisti** (non il ROAS).
5. Controlla se il report offre davvero la colonna **Pubblico/Interesse** o una voce compatibile. AdPilot la richiede, ma Meta potrebbe non mostrarla nel report standard: non inventare o rinominare dati non equivalenti.
6. Esporta in formato **CSV**, non Excel `.xlsx`, e controlla intestazioni e formato numerico.
7. Conserva il file sul dispositivo fino al caricamento in AdPilot.

Se Meta usa etichette diverse, confronta le intestazioni esportate con [Formato CSV e colonne obbligatorie](../optimizer/csv-requirements.md). Il campo Pubblico/Interesse è obbligatorio per l'importazione attuale. Se manca nel report autentico esportato da Meta, chiedi indicazioni all'assistenza AdPilot senza improvvisare un campo sostitutivo.

Non inviare report pubblicitari privati in una chat pubblica. Vedi [Caricare un CSV nell’Optimizer](../optimizer/upload-csv.md).
