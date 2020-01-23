---
title: Git
created: '2019-11-21T07:50:44.588Z'
modified: '2020-01-23T07:50:25.236Z'
---

# Git 

### 21/11/2019
Fonte: https://web.archive.org/web/20161121145226/http://rypress.com:80/tutorials/git/index

Fonte: https://learngitbranching.js.org/

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
git revert tag/id= torno effettivamente a quel commit e posso modificare senza problemi (solo con quello precedente), ma creo un commit nuovo quindi non torno per davvero indietro
```
### 5/12/2019
```bash
git reset --hard= lascia i file "senza commit", ma tutti i file già esistenti modificati e senza commit li fa tornare all'ultimo commit
```

```bash
git clean -f= cancella i file "senza commit"
```
**BRANCHE**

E' una linea indipendente dallo sviluppo, puoi fare una "copia" dei file in un'altro luogo, modificarlo e se ti piace unirla al progetto originale

        O inizio
        |
        |
        O divisione
       /|
      / |
      0 |
      | | 
      | |  
      \ |  
       \|
        0 merge
        |

```bash
git branch= mostra i branch esistenti
```
**12/12/2019**

```bash
git branch nome= creo un branch
```

```bash
git checkout nome= passo nel branch desiderato
```

```bash
git checkout -b nome= passo direttamente nel branch
```

```bash
git merge nome= eseguo il merge, prima di questo devo passare nel master/nel branch "master" rispetto a quello con cui voglio fare il merge
```
```bash
git log --oneline --graph=mostra grafico dei commit con i branch
```
**19/12/2019**

```bash
git rebase= simile al merge ma prende un tot di commit e li copia da qualche parte 
```

```bash
git rebase nome= prende la roba aggiornata del master e la porta in bugfix
```

REMOTE 

```bash
git clone= crei una copia locale di una repo remota
```

```bash
git fetch= scarica gli aggiornamenti dalla repo remota 
```

```bash
git pull = fetch e merge uniti 
```

```bash 
git push= mette la roba in remoto
```


