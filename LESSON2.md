---
marp: true
title: Software Development Lifecycle
description: Software Development Lifecycle - Hints & Insights - Lesson2
theme: gaia
class: invert
paginate: true
_paginate: false
---

![bg](./assets/brett-jordan-MFLNpz5FZRk-unsplash.jpg)

# <!--fit--> Software Development Lifecycle

# <!--fit--> Lesson 2

<style scoped>a { color: #eee; }</style>

---

![bg](./assets/luke-chesser-pJadQetzTkI-unsplash.jpg)

# Sommario - Modulo 2

1. Bootstrap di un progetto
2. Pianificare lo sviluppo
3. Ruoli
4. Step
5. Documentazione
6. Dev-Ops

---

![bg](./assets/luke-chesser-CxBx_J3yp9g-unsplash.jpg)

### <!--fit--> Bootstrap di un progetto

---

# Repository e versionamento

- creazione repo su GitHub (o similare)
- clonare repo sulla propria macchina
- aggiungere collaboratori
- impostare eventuali webhook

---

# Scelta del linguaggio e delle tecnologie

Variabili:

- Conoscenza del team
- Tempo a disposizione
- Espressività
- Dominio
- Librerie dedicate
- Trends e stimolo dei devs

---

# Numeri di versione

Seguire le regole di semantic versioning [semver](https://semver.org/)

### <!--fit--> MAJOR.MINOR.PATCH (e.g. 2.4.12)

MAJOR: versione con cambiamenti incompatibili (breaking change)
MINOR: versione con nuove funzionalità, retrocompatibile
PATCH: versione con bug fixes e func fixes

1.0.0 è la prima versione matura, non la prima rilasciata
Si incrementa la versione quando del codice nuovo entra in _master_

---

# Documentazione in project

Sono file nella root del progetto, solitamente scritti in linguaggio Markdown:

- CHANGELOG
- README
- CONTRIBUTING

E' bene redarli e tenerli aggiornati fin dal principio.

(continua)

---

# CHANGELOG

Traccia lo storico delle funzionalità su _master_, associato al numero di versione e la data.

```
## [0.3.0] - 2021-31-02
### Added
- IT translation from [@schillaci](https://github.com/ttskill).
- force API to be async in params from [@auridevil](https://github.com/auridevil).
### Fixed
- Delay in microservices discovery from [@converge](https://github.com/converge)

## [0.2.9] - 2021-28-02
### Fixed
...
```

---

# README

- Cosa serve il progetto (short)
- I passi per far "partire" il progetto (comp)
- I passi per eseguire i test unitari (comp)
- Come interagire con il sw
- Chi ha scritto il progetto e con che licenza è rilasciato il sorgente
- Varie info aggiuntive

---

# CONTRIBUTING

- Messaggi di commit
- Branch naming
- Come fare un fork & pull
- Cosa è necessario per sottomettere una pull-request
- Livello minimo di coverage richiesto
- Convenzioni di codice / stile
- Filosofia dietro al progetto

---

# BOILERPLATE

E' utile tenere un repository boilerplate per i propri progetti, da cui partire velocemente a lavorare (con la documentazione in progetto, i folder per i sorgenti e i test, il gitignore, et cetera).

Una volta clonato il _boilerplate project_, cambiare origin:

```bash
$ git remote rm origin
$ git remote add origin git@github.com:auridevil/newprojectcool.git
$ git config master.remote origin
$ git config master.merge refs/heads/master
```

---

![bg](./assets/luke-chesser-CxBx_J3yp9g-unsplash.jpg)

### <!--fit--> Pianificare lo sviluppo

## Da dove iniziare

---

Top Down

---

Bottom Up

---

Core First

---

Data Mock

---

![bg](./assets/luke-chesser-CxBx_J3yp9g-unsplash.jpg)

### <!--fit--> Ruoli

## Chi fa cosa

---

Analista

---

DEV

---

Frontend developer

---

Backend developer

---

Fullstack developer

---

Web developer

---

DB developer

---

Tester

---

Project Manager

---

Ops

---

Dev-Ops

---

DBA

---

Cliente

---

![bg](./assets/luke-chesser-CxBx_J3yp9g-unsplash.jpg)

### <!--fit--> Step di Progetto

## Come si è sempre fatto

---

Raccolta Requisiti

---

Analisi
(output funzionale)

---

Design
(output tecnica)

---

Sviluppo
(output codice)

---

Test

---

Validazione

---

Rilascio

---

Mantenimento

---

Evolutive

---

![bg](./assets/luke-chesser-CxBx_J3yp9g-unsplash.jpg)

### <!--fit--> Documentazione

---

Scelte Tecniche

---

Manuale utente

---

Manuale di manutezione

---

Mappa infrastrutturale

---

Documentazione del codice

---

Commenti

---

Codice leggibile

---

Readme & Markdown

---

![bg](https://freenaturestock.s3.amazonaws.com/1533.jpg)

### <!--fit--> :ok_hand:

---

![bg](https://freenaturestock.s3.amazonaws.com/1533.jpg)

### Created by Aureliano Bergese

https://github.com/auridevil/
https://twitter.com/elmozzo
https://www.instagram.com/elmozzo_buendia/
https://medium.com/@elmozzo

This work is licensed under a [Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
