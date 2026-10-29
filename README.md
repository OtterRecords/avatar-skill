# Avatar

**Ton avatar à partir de tes vrais échanges.** Un skill Claude qui fouille tes appels, tes DM et tes notes pour en sortir les mots exacts de tes clients, et qui te laisse écrire la synthèse toi-même.

1. Ton avatar se trouve dans tes vrais échanges, pas dans l'imagination d'une IA.
2. L'IA va chercher la matière : les mots exacts de tes clients, avec leur source.
3. La synthèse, c'est toi qui l'écris, à la main.

---

## Pourquoi ce skill n'écrit pas ton avatar

Demande à une IA « décris mon client idéal » : elle te rendra un portrait générique, plausible, et faux. Elle n'a jamais parlé à tes clients.

Ce skill fait l'inverse. Il ne sert qu'à aller chercher la matière, dans tes vrais échanges, avec la source de chaque phrase. C'est le principe de mon coach : **écris toi-même la synthèse de ta cible, l'IA ne sert qu'à aller chercher la matière.** Si l'IA écrit la synthèse, tu lis un avatar plausible au lieu de comprendre ton client. C'est en l'écrivant toi-même que tu l'intègres, et que tu sauras parler comme lui dans tes hooks, ta page, tes messages.

Si tu lui demandes d'écrire la synthèse à ta place, il refuse, et il te dit pourquoi.

## Ce qu'il fait

1. **Il te demande où sont tes échanges** : transcripts d'appels, DM exportés, notes, mails, réponses à un formulaire. Sans échanges, il ne fabrique rien.
2. **Il extrait les mots exacts** de tes prospects et clients (jamais les tiens), mot pour mot, chacun avec sa source.
3. **Il les range dans six tiroirs** : situation, douleurs, désirs, peurs, croyances, déclencheurs.
4. **Il signale ce qui revient** chez plusieurs personnes, et **les trous** : les tiroirs vides ou trop maigres, avec la question à poser au prochain échange pour les remplir.
5. **Il te donne la grille des 8 questions**, à remplir à la main.
6. **Il relit tes réponses si tu veux**, sans les réécrire : il vérifie qu'elles s'appuient sur la matière et pointe ce qui vient de ta tête.

## La grille des 8 questions

1. Qui est-ce, en une phrase, avec ses mots à lui ?
2. Qu'est-ce qui le bloque aujourd'hui, concrètement ?
3. Qu'a-t-il déjà essayé, et pourquoi ça n'a pas marché ?
4. À quoi ressemble sa vie quand c'est réglé ?
5. De quoi a-t-il peur s'il se lance ?
6. Qu'est-ce qu'il croit, qui le freine ?
7. Qu'est-ce qui le fait passer à l'action maintenant ?
8. Quelle phrase de lui pourrais-tu mettre telle quelle en haut de ta page ?

---

## Installation

### Dans Claude Code

```bash
git clone https://github.com/OtterRecords/avatar-skill.git
mkdir -p ~/.claude/skills
cp -r avatar-skill/avatar ~/.claude/skills/
```

Relance Claude Code, puis tape `/avatar`. Tu peux aussi écrire « aide-moi à faire mon avatar à partir de mes appels » : Claude reconnaît le skill tout seul. Donne-lui le dossier où sont tes transcripts, il les lit tous.

### Dans Claude.ai

Selon ton offre Claude, tu peux ajouter tes propres skills dans les réglages.

1. Télécharge ce dépôt (bouton **Code**, puis **Download ZIP**) et décompresse-le.
2. Compresse **seulement le dossier `avatar`** en `.zip` (clic droit, puis Compresser). Le zip doit contenir le dossier `avatar` avec `SKILL.md` dedans.
3. Dans Claude.ai, ouvre les réglages, la partie des Skills, et téléverse ce zip.
4. Dans une conversation, joins tes transcripts ou tes DM exportés, et écris « fais-moi la matière de mon avatar ».

Si ton offre ne permet pas d'ajouter un skill : crée un **Projet**, colle le contenu de `avatar/SKILL.md` dans ses instructions, et ajoute tes échanges dans ses fichiers.

### Dans ChatGPT ou tout autre outil

Pas d'installation : copie le prompt ci-dessous dans une nouvelle conversation, puis joins tes échanges ou colle-les à la place de la dernière ligne. Le même prompt est dans `prompt.txt`.

```
Tu vas m'aider à construire la matière de mon avatar client à partir de mes vrais échanges avec mes prospects et mes clients. Ton rôle est d'aller chercher et de classer leurs mots exacts. Tu n'écris pas la synthèse : c'est moi qui l'écrirai, à la main.

MES ÉCHANGES
Je te les donne juste en dessous, en fichiers joints ou collés (transcripts d'appels, DM, notes, mails). S'il n'y a rien, demande-les-moi avant de commencer, et n'invente rien en attendant.

CE QUE TU FAIS
1. Relève uniquement les phrases de mes prospects et clients, jamais les miennes.
2. Recopie-les mot pour mot. Tu peux couper avec [...], jamais reformuler.
3. Note la source de chaque citation : le fichier, la date ou le numéro de l'échange.
4. Range chaque citation dans un seul de ces six tiroirs :
- SITUATION : où il en est aujourd'hui, son activité, son quotidien, ses outils ;
- DOULEURS : ce qui le gêne, le fatigue ou lui coûte, maintenant ;
- DÉSIRS : ce qu'il veut, à quoi ressemble sa vie quand c'est réglé ;
- PEURS : ce qu'il redoute s'il se lance, ou s'il ne fait rien ;
- CROYANCES : ce qu'il tient pour vrai, surtout ce qui le freine ;
- DÉCLENCHEURS : ce qui l'a fait chercher une solution maintenant.
5. Ajoute une partie CE QUI REVIENT : les mots ou les idées qui reviennent chez plusieurs personnes, avec le nombre de fois et les sources.
6. Ajoute une partie LES TROUS : chaque tiroir vide ou nourri par une seule personne, avec une question ouverte à poser au prochain échange pour le remplir.

LES RÈGLES
- Aucune citation inventée, même pour remplir un tiroir vide. Un trou se nomme, il ne se comble pas.
- Si un passage de transcript est douteux ou si on ne sait pas qui parle, écris [transcription douteuse] au lieu de deviner.
- Désigne les gens par leur source, pas par leur nom.

À LA FIN
Donne-moi cette grille, telle quelle, et dis-moi d'y répondre moi-même, à la main, en m'appuyant sur au moins une citation par réponse :
1. Qui est-ce, en une phrase, avec ses mots à lui ?
2. Qu'est-ce qui le bloque aujourd'hui, concrètement ?
3. Qu'a-t-il déjà essayé, et pourquoi ça n'a pas marché ?
4. À quoi ressemble sa vie quand c'est réglé ?
5. De quoi a-t-il peur s'il se lance ?
6. Qu'est-ce qu'il croit, qui le freine ?
7. Qu'est-ce qui le fait passer à l'action maintenant ?
8. Quelle phrase de lui pourrais-tu mettre telle quelle en haut de ta page ?

CE QUE TU REFUSES
Si je te demande d'écrire l'avatar, la synthèse ou les réponses à ma place, refuse et rappelle-moi pourquoi : si l'IA écrit la synthèse, je lis un avatar plausible au lieu de comprendre mon client. C'est en l'écrivant moi-même que je l'intègre, et que je saurai parler comme lui dans mes hooks, ma page, mes messages. Propose plutôt de me ressortir la matière d'un tiroir, de chercher une citation, ou de relire ce que j'ai écrit sans le réécrire.

MES ÉCHANGES
[COLLE TES ÉCHANGES ICI, OU JOINS TES FICHIERS]
```

---

## Tes données

Tes transcripts et tes DM contiennent des données personnelles. Le skill ne les envoie nulle part ailleurs que dans ta conversation avec Claude, désigne les gens par leur source plutôt que par leur nom, et ne cite que ce qui sert l'avatar. Vérifie les réglages de confidentialité de l'outil que tu utilises avant d'y déposer des échanges de clients.

## Ce que contient ce dépôt

```
avatar/
  SKILL.md    le skill : les échanges, l'extraction, les six tiroirs, les trous, la grille, le refus
prompt.txt    la version sans installation (ChatGPT ou autre)
README.md     ce fichier
LICENSE       MIT
```

Licence MIT : tu peux l'utiliser, le modifier et le partager librement.

---

Fait par Victor, qui implémente l'IA dans les business.

- Instagram : https://www.instagram.com/victorvitalyy_/
- L'avatar en page web : https://avatar-victor.vercel.app
