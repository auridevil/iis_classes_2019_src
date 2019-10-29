---
marp: true
title: Corso Gestione Progetti 2019
description: Corso di aggiornamento gestione progetti per i docenti del Istituto Tecnico Vallauri
theme: gaia
class: invert
paginate: true
_paginate: false
---

![bg](./assets/asoggetti-cfKC0UOZHJo-unsplash.jpg)

# <!--fit--> Corso IIS Vallauri - gestione progetti 2019


https://github.com/auridevil/iis_classes_2019_src
https://gest-progetti-iis.netlify.com/

<style scoped>a { color: #eee; }</style>

---
## Aureliano Bergese (fullstack@mondora)
![width:200px](./assets/auri.png)
Explorer
Functional Programming enthusiast
Father of 2
Professional Scrum Product Owner

---
### <!--fit--> Software nel 2019
---
# SUBJECTS (cosa)
- progetto: ciò che dobbiamo realizzare
- prodotto: uno o più progetti, volti a fornire un servizio unificato
- valore: benefit fornito dal prodotto
- revenue: guadagno fornito dal prodotto al proprietario
---
# STAKEHOLDERS (chi)


- team: chi lavora al progetto
- utenti finali: chi usa il prodotto
- clienti: chi commissiona il progetto
- funder: chi mette i soldi per il progetto
---

# ENVIRONMENTS (dove)
- dev: per i programmatori del team
- test: per i tester del team
- integration: per le altre entità che concorrono al progetto 
- demo: per mostrare le funzionalità al cliente / funder
- preproduction: per i tester del prodotto
- production: per gli utenti finali
---
### <!--fit--> Versionamento
---
# Un VCS traccia la storia dei cambiamenti di persone e team che lavorano insieme ad un progetto.
Un DVCS lo fa in maniera distribuita.

---
# Perchè? per rispondere alle domande:
- quali modifiche sono state fatte?
- chi ha fatto le modifiche?
- quando sono state fatte le modifiche?
- perchè sono state richieste le modifiche?
---

![Marp bg 90%](./assets/vcschart.png)

---
### <!--fit--> GIT
---
(Distributed) Version Control System
(git = idiota) 

Linus Torvalds 2005
Junio Hamano v1 (attualmente mantainer)

Basato su **checksum** di file e folder (per la velocità)

---
# Repository
Un repository (repo) o git-project è l'insieme di file e folder associati ad un progetto. Comprende anche lo storico delle modifiche.

---
# Crea nuovo (locale)
```bash
git init
```
---
# Clona esistente (remoto)
```bash
git clone https://github.com/auridevil/iis_classes_2019_src.git
cd iis_classes_2019
```
---
# Branching
un branch è un ramo dell'albertatura della storia del codice
il branch principale è **master**
![width:900px](./assets/branch1.png)

---
Tutti i branch del repo
```bash
mox@urania$ git branch
  branchdemo
* master
(END)
```

Cambia branch attivo
```bash
git checkout branchdemo
```
---

Crea nuovo branch
```bash
git branch funzionalita1425
```

Crea nuovo branch e utilizza
```bash
git checkout -b funzionalita1425
```

---
# Aggiungi
L'aggiunta di un set di modifiche è in due fasi: staging e commit.
**git add** aggiunge alcune modifiche allo stage 

Aggiungi modifica di un file
```bash
git add PITCHME.md
```

---

Aggiungi tutte le modifiche 
``` bash
git add .
```
Aggiungi modifiche di un folder
```bash
git add assets/*
```
NB la cancellazione è una modifica. Solitamente il renaming / move è considerata cancellazione + aggiunta.

---
**git commit** salva lo snapshot delle modifiche (sul branch correente) e completa il tracciamento

commit con editor 
``` bash
git commit
```
commit inline
``` bash
git commit -m "this is a inline commit message"
```

---
# Commit message (best practices)
- usare l'imperativo
- max 50 chars
- no punti finali
- dichiarare le modifiche fatte ad alto livello
- includere eventuali riferimenti a documentazione (e.g. jira code, tiketing...)
  
---
```bash
git commit -m "[type][branch] What is done "
```
type è il tipo di modifica:
- feat: funzionalità nuova
- fix: correzione errore
- chore: piccola sistemazione
- test: copertura del codice
- doc: documentazione

Se il branch è master, si esclude dal commit message.

---
# Status
```bash
mox@urania$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   game.txt
```
---
# Merge
Combina le modifiche fatte su due branch differenti. E' direzionale: merge **of** un branch **into** un'altro branch.

---
---
# Git as-a-service
- [Git Hub](https://www.github.com)
- [Git Lab](https://about.gitlab.com)
- [Bitbucket](https://bitbucket.org/)
# Tools
- [Atlassian Sourcetree](https://www.sourcetreeapp.com/)
- [Visual Studio Code](https://code.visualstudio.com/Download)
---


---
![Marp bg 90%](https://raw.githubusercontent.com/marp-team/marp/master/marp.png)

---

![bg](#123)
![](#fff)

##### <!--fit--> [@marp-team/marp-cli](https://github.com/marp-team/marp-cli) + [Netlify](https://www.netlify.com/) | [Now](https://zeit.co/now)

##### <!--fit--> 👉 The easiest way to host<br />your Marp deck on the web

---

![bg right 70%](https://www.netlify.com/img/press/logos/logomark.svg)

## **[Netlify](https://www.netlify.com/)**

#### Ready to write & host your deck!

[![Deploy to Netlify w:300](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/yhatt/marp-cli-example)

---

![bg right 70%](https://assets.zeit.co/image/upload/front/assets/design/now-black.svg)

## **[Now](https://zeit.co/now)**

#### Host your deck by just running `now`!

```bash
now
```

---

### <!--fit--> :ok_hand:

---

![bg 40% opacity blur](https://avatars1.githubusercontent.com/u/3993388?v=4)

### Created by Yuki Hattori ([@yhatt](https://github.com/yhatt))

https://github.com/yhatt/marp-cli-example
