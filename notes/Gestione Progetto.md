---
title: Gestione Progetto
created: '2019-11-21T07:50:44.588Z'
modified: '2019-11-28T08:26:30.319Z'
---

# Gestione Progetto 

### 21/11/2019
Fonte: https://web.archive.org/web/20161121145226/http://rypress.com:80/tutorials/git/index

Git è un sistema di **versioning**, tiene traccia di ciascun cambiamento che avviene nel tuo progetto e da chi vengono fatti.
Prima di Git era il classico fare un progetto e ri/nominarlo
(prova visual studio code)


```bash
Git --versione= da la versione
``````

```bash
ls-la= mostra i file nascosti
``````

```bash
git init= inizializzo la repo di git
``````

```bash
git status= mostra le modifiche e resto fatte
```

```bash
Untracked file= un file non è sotto un controllo della versione. Per ignorare dei file dal tracciamento come i-_.class etc
```

```bash
git add nome= monitoro quel file "staging"
```

```bash
git commit -m"messagio"= così facendo abbiamo creato uno snapshot
```

```bash
git config --global user.mail "mail"
git config --global user.name "nome"
così posso fare il commit
```

```bash
git log= creo il log
```

```bash
git log --oneline= la si vede in maniera "più semplificata" con solo il commento 
```

### 28/11/2019
**UNDOING CHANGES**

```bash
git checkout id= fa vedere i contenuti della vecchia versione
```
head è il puntatore all'ultimo commit, facendo un checkout ad un vecchio torno ad un vecchio punto e così facendo non vedo più i commit avvenuti dopo

```bash
git checkout master= torno al commit corrente
```

```bash
git tag -a nome tag -m "messaggio"
```

```bash
git revert tag/id= torno effettivamente a quel commit e posso modificare senza problemi (solo con quello precedente)
```
