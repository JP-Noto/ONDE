# ONDE AI R&D

**Laboratoire de recherche appliquée et développement : travail humain–IA.**

Devise : *CONNECT THE DOTS*.

> **Rang des travaux présentés : hypothèses, preuves de concept, et une doctrine.**
> Ce dépôt publie la méthode du laboratoire, dans ses grandes lignes.

*Le français fait foi. English readers: see [README.md](README.md).*

---

## Ce que le labo est

ONDE AI R&D est un laboratoire de recherche appliquée et de développement. Il étudie comment travailler durablement avec une IA : un travail qui reste sous autorité humaine et dont la qualité se mesure. « Travail » couvre tout workflow humain–IA (créer, décider, organiser, apprendre), pas seulement la fabrication de livrables.

Il produit des connaissances mises à l'épreuve, toujours par paire : un mécanisme nommé, qui explique ; un test écrit d'avance, qui peut le contredire. Sa méthode : des problématiques vécues, des hypothèses réfutables, un pipeline à gates. Un praticien-chercheur, N=1, déclaré. Tout se consigne ; tout ne se publie pas.

## Le problème

Le travail assisté par IA échoue rarement par manque de puissance du modèle. Il échoue sur trois points.

**La durabilité.** Ce qui marche une session casse souvent à la dixième, et à nouveau au changement de génération de modèle ; les workflows se reconstruisent. La question du labo : qu'est-ce qui se répète, et qu'est-ce qui survit à un changement de génération ?

**L'autorité.** Le canon d'un projet glisse sans décision ; une proposition non validée devient référence par répétition ; la mémoire enfle, et l'humain finit par abdiquer de fait. La question du labo : comment une référence se gagne-t-elle par décision humaine, et comment le reste-t-elle ?

**La mesure.** La qualité du travail humain–IA se raconte plus qu'elle ne se mesure : peu d'indicateurs, peu de conditions d'échec. La question du labo : quel indicateur, et quelles conditions d'échec écrites avant la mesure ? L'indicateur candidat : les itérations correctives par livrable validé.

Ces trois problèmes sont observables et reproductibles. Le labo les aborde comme des mécanismes : nommables, testables, réfutables.

## Le positionnement

> « L'IA propose, l'humain décide : informé, guidé, mis en état de bien décider. Chaque décision fait avancer le travail et laisse sa trace. La responsabilité est le prix ; la sécurité de la décision est le gain. Le workflow avance et se répète sous autorité humaine : personnel ou professionnel, même règle. »

## La méthode, en une ligne

```
réflexion → hypothèse → banc d'essai → terrain chercheur → auditable → utilisateurs réels → répliqué → doctrine
```

Le rang se gagne par l'usage, jamais auto-décerné.
Le pipeline à gates n'est pas une trouvaille du labo ; ce qui lui est propre, c'est le contenu de chaque étage et les critères de chaque passage.
L'appareil qui tient cette méthode s'appelle ACTA : un guichet, entrée unique où toute problématique, celles du fondateur comprises, reçoit un verdict humain ; un journal ; un registre ; des protocoles.
Il est décrit dans [`methode/PIPELINE.md`](methode/PIPELINE.md).

## Ce que ce dépôt publie

| Pièce | Ce qu'elle dit |
|---|---|
| [`methode/PIPELINE.md`](methode/PIPELINE.md) | Le pipeline de recherche, dans ses grandes lignes : huit étages, deux espèces de gates, ce qui tient la méthode. |
| [`methode/REGISTRE-HYPOTHESES.md`](methode/REGISTRE-HYPOTHESES.md) | La vue des rangs : chaque hypothèse, son rang réel, sa gate suivante. |

Derrière ces grandes lignes : les critères de chaque gate, le guichet, le lexique, et les corpus en développement. Ils s'ouvrent sur invitation, dans le cadre d'une collaboration, sous clause de confidentialité (NDA).

## La famille

Le labo publie sa méthode, dans ses grandes lignes, en accès ouvert. Ses corpus, eux, se développent à leur rang : un corpus est public à partir du rang auditable, et se développe en privé en deçà.

| Date | Événement |
|---|---|
| 21 juillet 2026 | LIVING REFERENCE, première version |
| 6 août | LIVING REFERENCE rendu public |
| 11 août | MYSTANCE et WORKING REFERENCE |
| 20 août | SOUNDNESS |
| 5 septembre | VIGILANCE |
| 10 septembre | proposition d'un outil porté au public, regroupant l'ensemble des corpus |

**[LIVING REFERENCE](https://github.com/JP-Noto/LIVING-REFERENCE)**, public : le statut du savoir dans un projet assisté par IA, de la proposition à la référence par validation.
**Doctrine** : en usage depuis juillet 2026, répliqué par ses utilisateurs déclarés, chacun de son côté sur un système distinct de celui de l'auteur, et resté inchangé à travers un changement de génération de modèle.
Un re-test peut être demandé si l'usage le montre ; il n'est pas systématique.
Repris comme pièce d'architecture par un OS tiers ; chaque décision y fait référence et laisse sa trace.

Les quatre autres corpus se développent en privé :

- **MYSTANCE**, la couche humaine : régler la relation humain–IA plutôt que la dominer ; le niveau d'assistance module combien l'IA propose, jamais qui décide.
- **WORKING REFERENCE**, la couche d'exécution : un corpus n'est pas un document qu'on lit, c'est une fonction qu'on appelle ; une constante gagnée par gates, servie et scellée.
- **SOUNDNESS**, la naissance du savoir extrait de documents : la fiche ne dit rien que la pièce ne fonde.
- **VIGILANCE**, l'économie de l'attention : le système vérifie tout, l'humain tranche sur les seules exceptions.

Ils s'ouvrent sur invitation, dans le cadre d'une collaboration, sous clause de confidentialité (NDA). Contact par le [profil](https://github.com/JP-Noto).

## La séquence

Elle n'a pas de date. Terrain chercheur, puis auditable (le corpus devient public), puis utilisateurs réels, puis réplication par des tiers qui déploient depuis le corpus seul. Une pièce sort quand elle est finie, avec son protocole et ses limites.

## Les gardes du labo

- **L'usage déclaré donne le rang, la mesure dit combien** : un mécanisme est démontré en usage quand ses utilisateurs déclarés l'ont adopté ; comme un moteur, démarré, il tourne. L'effet sur l'indicateur est une autre affirmation, mesurée ensuite.
- **Récence n'est pas qualité** : la ressemblance aux derniers travaux n'est pas un critère de traversée.
- **Notes = signal** : les évaluations déclenchent un examen ; elles ne sont jamais la métrique.
- **Tout se consigne, tout ne se publie pas** : ce qui est publié sert une démonstration ou une réflexion, sans obligation de calendrier.

## Licence et citation

Contenu sous [CC BY-NC-SA 4.0](LICENSE.md). Pour citer : [`CITATION.cff`](CITATION.cff). Contributions : [`CONTRIBUTING.md`](CONTRIBUTING.md).

---

*Julien-Pierre NOTO · ONDE AI R&D · laboratoire fondé le 13 juillet 2026.*
