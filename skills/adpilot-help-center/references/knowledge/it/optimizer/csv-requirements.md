---
id: "csv-requirements"
title: "Formato CSV e colonne obbligatorie"
description: "Dimensioni, codifica, separatori e campi obbligatori del report."
category: "optimizer"
feature: "optimizer"
audience: "merchant"
difficulty: "beginner"
language: "it"
plans: ["PRO"]
keywords: ["csv", "utf8", "semicolon", "columns", "headers", "limit"]
last_reviewed: "2026-11-17"
translation_id: "csv-requirements"
related: ["csv-errors"]
---

# Formato CSV e colonne obbligatorie

## Requisiti del file
L'Optimizer accetta file **`.csv`**, testo **UTF-8** (anche con BOM UTF-8), separatore **virgola** o **punto e virgola**, dimensione da **1 KiB a 10 MiB**, massimo **50.000 righe di dati** e **200 colonne**.

File `.xlsx`, codifica UTF-16 e separatori diversi non sono supportati. I CSV senza dati utilizzabili vengono rifiutati.

## Colonne obbligatorie
Il report deve contenere tutte le 13 categorie seguenti; AdPilot riconosce diverse varianti italiane e inglesi delle intestazioni:

| Dato | Esempio inglese | Esempio italiano |
| --- | --- | --- |
| Campagna | Campaign name | Nome della campagna |
| Gruppo di inserzioni | Ad set name | Nome del gruppo di inserzioni |
| Pubblico / interesse | Audience/Interest | Pubblico/Interesse |
| Spesa | Amount spent | Importo speso |
| Impression | Impressions | Impression |
| Copertura | Reach | Copertura |
| Frequenza | Frequency | Frequenza |
| Clic | Link clicks | Clic sul link |
| Percentuale clic | CTR | CTR |
| Costo per clic | CPC | CPC |
| Costo per mille | CPM | CPM |
| Acquisti | Purchases | Acquisti |
| Valore acquisti | Purchase value | Valore conversione acquisti |

Sono necessari sia **Acquisti** sia **Valore acquisti** come campi distinti. Se AdPilot segnala colonne assenti, consulta [Risolvere gli errori di importazione CSV](../troubleshooting/csv-errors.md) e controlla le intestazioni originali.

## Preparare dati affidabili
- Esporta **una sola campagna per file CSV**. Evita report che uniscono più campagne, soprattutto se condividono nomi identici per i gruppi di inserzioni.
- Usa numeri senza separatori delle migliaia: per esempio **1234.56** (CSV separato da virgole) oppure **1234,56** (CSV separato da punti e virgola). Evita formati come `1,234.56` o `1.234,56`: potrebbero essere interpretati male.
- Se possibile, mantieni i campi testuali su una riga; i ritorni a capo dentro celle CSV fra virgolette potrebbero non essere importati correttamente.
- Per il **valore degli acquisti** usa il valore reale delle conversioni, **non il ROAS degli acquisti**: sono metriche diverse.
- Mantieni periodo e valuta coerenti e confronta i totali con Meta prima di applicare le raccomandazioni AI.

La colonna **Pubblico/Interesse** è obbligatoria per l'importazione attuale. I report standard di Meta potrebbero non offrire un campo equivalente. **Non rinominare colonne non pertinenti né inventare valori di targeting** per superare il controllo. Se manca il campo nel report autentico, contatta l'assistenza AdPilot per verificare un formato compatibile.
