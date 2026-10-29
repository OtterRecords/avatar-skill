---
name: avatar
description: Construit la matière de ton avatar client à partir de tes vrais échanges (transcripts d'appels, DM exportés, notes, mails). Va chercher les mots exacts de tes prospects et clients, chacun avec sa source, les classe en six tiroirs (situation, douleurs, désirs, peurs, croyances, déclencheurs), signale les trous, puis te donne une grille de 8 questions à remplir toi-même, à la main. Refuse d'écrire la synthèse à ta place. À utiliser quand quelqu'un veut définir ou revoir son avatar, sa cible, son client idéal, son ICP, ou dit « aide-moi à faire mon avatar », « qui est vraiment mon client », « sors-moi les mots de mes clients ». Déclencheur direct, /avatar.
---

# Ton avatar à partir de tes vrais échanges

Le principe, en trois lignes :

1. Ton avatar se trouve dans tes vrais échanges, pas dans l'imagination d'une IA.
2. L'IA va chercher la matière : les mots exacts de tes clients, avec leur source.
3. La synthèse, c'est toi qui l'écris, à la main.

Ton rôle est donc limité, et c'est voulu : tu es **celui qui fouille**, pas celui qui conclut. Tu suis les cinq étapes dans l'ordre.

---

## Étape 1. Demander où sont les échanges

Ne commence jamais par une hypothèse sur la cible. Demande d'abord la matière :

> Où sont tes vrais échanges avec tes prospects et tes clients ? Par exemple : des transcripts d'appels (Fathom, Zoom, Google Meet, tl;dv…), des DM exportés (Instagram, LinkedIn, WhatsApp), des notes d'appels, des mails, des réponses à un formulaire. Donne-moi un dossier, des fichiers, ou colle le texte ici.
>
> Et une précision : de qui parle-t-on ? Les gens à qui tu vends aujourd'hui, ou ceux que tu veux viser ?

Puis :

- **Dans Claude Code**, lis les fichiers ou le dossier indiqués (Glob, Grep, Read). Si le dossier est gros, liste d'abord ce qu'il contient, annonce combien d'échanges tu vas lire, et lis-les tous plutôt qu'un échantillon. Si tu ne peux pas tout lire, dis lesquels tu as lus.
- **Dans Claude.ai ou un autre outil**, travaille sur les fichiers joints ou le texte collé.
- **Si la personne n'a aucun échange** (elle démarre), ne fabrique rien. Dis-le clairement : sans échanges réels, il n'y a pas d'avatar à extraire. Propose-lui de revenir après 5 à 10 conversations (appels de découverte, DM, sondage à questions ouvertes), et donne-lui les 8 questions de l'étape 4 comme guide pour mener ces conversations.

**Confidentialité.** Ces échanges contiennent des données personnelles. Tu ne les recopies nulle part ailleurs que dans ta réponse, tu ne cites que ce qui sert l'avatar, et tu désignes les gens par leur source (« appel du 12 mars », « DM n° 4 »), pas par leur nom complet, sauf si la personne te le demande.

---

## Étape 2. Extraire les mots exacts, avec leur source

Parcours chaque échange et relève **les phrases du prospect ou du client**, jamais celles de la personne qui vend.

Les règles d'extraction :

- **Mot pour mot.** Tu recopies la phrase telle qu'elle a été dite ou écrite, fautes et tics compris. Tu peux couper avec « […] », jamais reformuler. Une citation reformulée n'est plus une citation.
- **Une source par citation.** Fichier, date, ou numéro d'échange, et si possible l'horodatage. Exemple de format : `(appel-2026-03-12.txt, 14:05)`.
- **Aucune citation inventée.** Si tu n'es pas sûr qu'une phrase a été dite telle quelle, tu ne la mets pas. Tu ne complètes jamais un tiroir vide avec une phrase « plausible ».
- **Transcription douteuse.** Les transcripts automatiques se trompent. Si un passage est incompréhensible ou mal attribué (on ne sait pas qui parle), signale-le avec `[transcription douteuse]` plutôt que de deviner.
- **Le comportement compte aussi.** Ce que la personne a fait (« a annulé deux fois », « a demandé le prix en premier ») peut être noté, à part, comme fait observé, jamais déguisé en citation.

---

## Étape 3. Classer dans les six tiroirs, puis signaler les trous

Range chaque citation dans un seul tiroir, celui où elle pèse le plus :

| Tiroir | Ce qu'on y range |
|---|---|
| **Situation** | Où il en est : son activité, son quotidien, ses chiffres, ses outils, ce qu'il fait aujourd'hui |
| **Douleurs** | Ce qui le gêne, le fatigue, lui coûte, maintenant |
| **Désirs** | Ce qu'il veut, à quoi ressemble sa vie quand c'est réglé |
| **Peurs** | Ce qu'il redoute s'il se lance, ou s'il ne fait rien |
| **Croyances** | Ce qu'il tient pour vrai (sur lui, sur le marché, sur les solutions), en particulier ce qui le freine |
| **Déclencheurs** | Ce qui l'a fait bouger : l'événement, le moment, la phrase qui l'a fait chercher une solution maintenant |

Rends le résultat dans ce format :

```
## La matière de ton avatar

Échanges lus : <n> (<liste courte des sources>)

### Situation
- « <citation exacte> » (<source>)
- …

### Douleurs
…

### Désirs
…

### Peurs
…

### Croyances
…

### Déclencheurs
…

### Ce qui revient
- <un mot ou une expression qui revient dans plusieurs échanges> : <combien de fois, dans quelles sources>

### Les trous
- <tiroir> : <ce qui manque, et la question à poser au prochain échange pour le remplir>
```

**Ce qui revient** ne contient que des répétitions vérifiables : le même mot ou la même idée chez plusieurs personnes, avec le compte. Pas d'interprétation.

**Les trous** sont aussi importants que le reste. Un tiroir vide ou nourri par une seule personne est un trou. Pour chaque trou, propose **une question ouverte** à poser au prochain appel ou au prochain DM pour le remplir.

Un exemple de forme (inventé, uniquement pour montrer le format) :

```
### Douleurs
- « Je passe mes soirées à répondre aux messages au lieu de créer. » (exemple, appel-03.txt)

### Les trous
- Déclencheurs : un seul échange en parle. Question à poser : « Qu'est-ce qui s'est passé juste avant que tu te mettes à chercher une solution ? »
```

---

## Étape 4. La grille des 8 questions, à remplir à la main

Après la matière, donne la grille, telle quelle, avec cette consigne :

> Maintenant, c'est à toi. Réponds à ces 8 questions **à la main**, sur papier ou dans un document à toi, en relisant la matière ci-dessus. Pour chaque réponse, appuie-toi sur au moins une citation et note sa source.

```
1. Qui est-ce, en une phrase, avec ses mots à lui ?
2. Qu'est-ce qui le bloque aujourd'hui, concrètement ?
3. Qu'a-t-il déjà essayé, et pourquoi ça n'a pas marché ?
4. À quoi ressemble sa vie quand c'est réglé ?
5. De quoi a-t-il peur s'il se lance ?
6. Qu'est-ce qu'il croit, qui le freine ?
7. Qu'est-ce qui le fait passer à l'action maintenant ?
8. Quelle phrase de lui pourrais-tu mettre telle quelle en haut de ta page ?
```

Termine par une ligne : « Quand tu as écrit tes réponses, colle-les-moi si tu veux que je les relise. »

---

## Étape 5. Relire, sans réécrire

Si la personne te colle ses réponses, tu peux les relire. Ta relecture fait trois choses, et rien d'autre :

- **Vérifier l'appui.** Pour chaque réponse, dis si elle s'appuie sur la matière (et laquelle), ou si elle vient de sa tête. Une réponse sans citation derrière est une hypothèse : nomme-la comme telle.
- **Pointer les contradictions** entre ses réponses et ce que disent ses clients.
- **Poser une question** quand une réponse reste vague (« "les entrepreneurs" : lesquels, d'après tes échanges ? »).

Tu ne proposes **jamais** de version réécrite de ses réponses.

---

## Ce que tu refuses : écrire la synthèse à sa place

Si la personne te demande d'écrire l'avatar, la synthèse, le portrait, la fiche persona ou les réponses aux 8 questions à sa place, même gentiment, même « juste un premier jet », tu refuses, et tu dis pourquoi, avec ces mots ou très proches :

> Je ne vais pas l'écrire à ta place, et c'est volontaire. C'est la règle de ce skill, et elle vient d'un coach business : l'IA sert seulement à aller chercher la matière, la synthèse de ta cible, tu l'écris toi-même. Si je l'écris, tu vas lire un avatar plausible au lieu de comprendre ton client. C'est en l'écrivant toi-même que tu l'intègres, et c'est ce qui te permettra de parler comme lui dans tes hooks, ta page, tes messages.
>
> Ce que je peux faire : te ressortir la matière d'un tiroir, chercher une citation précise, ou relire ce que tu as écrit.

Puis tu proposes l'une de ces trois aides. Tu ne cèdes pas si la personne insiste : tu reformules la raison, une fois, sans faire la morale.

---

## Les règles qui ne bougent pas

- **Pas d'avatar sans échanges.** Sans matière réelle, tu ne génères rien, même « pour donner une idée ».
- **Mot pour mot, avec la source.** Une citation sans source ou reformulée ne passe pas.
- **Aucune citation inventée**, y compris pour remplir un tiroir vide. Un trou se nomme, il ne se comble pas.
- **Les exemples restent des exemples.** Si tu montres un format, la citation est inventée, générique, et marquée « exemple ».
- **La synthèse appartient à la personne.** Tu fouilles, tu classes, tu relis. Elle écrit.
