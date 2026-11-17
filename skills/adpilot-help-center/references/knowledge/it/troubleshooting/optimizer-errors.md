---
id: "optimizer-errors"
title: "Risolvere i problemi dell’Optimizer"
description: "Controlli su piano, campagne, attese e report."
category: "troubleshooting"
feature: "troubleshooting"
audience: "merchant"
difficulty: "beginner"
language: "it"
plans: ["PRO"]
keywords: ["optimizer", "error", "locked", "csv", "cooldown"]
last_reviewed: "2026-11-17"
translation_id: "optimizer-errors"
related: ["csv-requirements", "optimization-cooldown", "csv-errors", "error-reference"]
---

# Risolvere i problemi dell’Optimizer

## Se l'ottimizzazione non è disponibile
1. Controlla che il piano attivo sia **Pro**: Free e Starter non possono creare nuovi round.
2. Apri **Campagne** e seleziona una proposta AI salvata. L'ottimizzazione parte dalla campagna, non da un report isolato.
3. Verifica se per quella campagna compare un'attesa di **72 ore**.
4. Controlla il CSV in [Formato CSV e colonne obbligatorie](../optimizer/csv-requirements.md).
5. Se l'elaborazione restituisce un codice di riferimento, annotalo con l'orario approssimativo.

## Se i suggerimenti sembrano errati
Confronta spesa, acquisti, valore degli acquisti, intervallo delle date e suddivisione campagne/gruppi con il report Meta originale. Non applicare automaticamente un suggerimento AI che contraddica i dati reali o le regole pubblicitarie.

Vedi [Quando posso ottimizzare di nuovo?](../optimizer/optimization-cooldown.md), [Risolvere gli errori di importazione CSV](../troubleshooting/csv-errors.md) e [Che cosa significa ERR-XXXXXX?](../troubleshooting/error-reference.md).
