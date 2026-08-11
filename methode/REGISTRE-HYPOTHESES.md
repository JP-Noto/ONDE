# REGISTRE DES HYPOTHÈSES · ONDE AI R&D

*Version publiée du registre : la vue des **rangs réels**. Ce registre recense, il ne redéfinit rien : chaque mécanisme vit dans sa fiche (corpus LIVING REFERENCE, dépôt distinct : <https://github.com/JP-Noto/LIVING-REFERENCE>, public depuis le 2026-08-06). Règle du pipeline : le rang se gagne par l'usage, jamais auto-décerné.*

## État du registre interne au 2026-08-11

Le registre interne du laboratoire est à sa **révision 16** : **33 dépôts** reçus au guichet,
hypothèses lettrées jusqu'à **H(T)**. Ce document public en présente le socle et les mécanismes
historiques (vue du 2026-08-02) ; parmi les inscriptions récentes : **H(S)**, les invariants vivent
dans l'exécuteur, et **H(T)**, la **doctrine-fonction**, généralisation de LIVING REFERENCE (la
référence comme fonction : constante + variables, instanciation décidée, servie, scellée), domiciliée
dans le corpus **WORKING REFERENCE** (objet d'étude n° 3). La vue détaillée lettre à lettre sera
resynchronisée avant toute mise en public.

## Rappel de l'échelle (pipeline à gates)

réflexion → hypothèse → banc d'essai → terrain chercheur → auditable → utilisateurs réels → répliqué → **doctrine (glissante)**

**Aucun mécanisme n'a aujourd'hui le rang de doctrine. Tous sont candidats.**

*Note de tenue : aucun rang « doctrine » n'est permanent. C'est un **canon glissant** : stable pour un horizon de génération déclaré, avec re-test obligatoire à la prochaine génération majeure ; à défaut, retombée à « répliqué ». Définition et critère de génération : [PROTOCOLE-CQM.md](PROTOCOLE-CQM.md), gate 7.*

## Règle des deux rangs de reprise

- **Crédit au lineage** : un système tiers cite publiquement l'origine du concept (crédit daté, transfert consenti). Reconnaissance de filiation intellectuelle, pas une preuve d'usage.
- **Adoption architecturale** : le mécanisme est une pièce structurelle du système : le retirer changerait le système. Seule la **double valeur** a ce rang.

Toute formulation « trois mécanismes repris / déployés / en production » est un rang usurpé : la revendication exacte est **une adoption architecturale + trois crédits au lineage**.

## Le socle

| Hypothèse | Rang | Reprise externe |
|---|---|---|
| Double valeur (axiome : avancer + tracer, « une pierre deux coups ») | preuve de concept | **adoption architecturale** (mécanisme central d'un AIOS tiers) + crédit au lineage |
| Validation utilisateur (rien ne fait autorité sans validation humaine) | preuve de concept | crédit au lineage |
| Cycle de statuts (maturité × portée × fraîcheur) | preuve de concept | crédit au lineage |

Garde permanente : *crédit ≠ preuve*, et adoption par un utilisateur unique et apparenté ≠ réplication par des inconnus.

## Les mécanismes propres · cœur de la revendication

| Hypothèse | Rang | Prochain gate |
|---|---|---|
| **H1 · Glissement** (fenêtre + invariants + rappel, coût constant) | preuve de concept | terrain chercheur → auditable |
| **H2 · Héritage par facettes / validation partielle** (validation scopée ; requalifiée sur revue de champ : le patron formel (libération humaine scopée + héritage du couvert) est établi depuis 1984 (Military Message Systems) au plan du contrôle d'accès ; H2 est un **transfert** de ce patron au plan du contexte de production humain–IA, le résidu propre (facettes sémantiques déclarées + héritage-contexte) restant sans précédent trouvé) | preuve de concept | terrain chercheur → auditable |
| **H3 · Tamis de trace (trace sieve)** (borne la double valeur) | preuve de concept | terrain chercheur → auditable |
| **H4 · Transversalité** (2 dimensions × 3 barreaux : chat nu · agentique · OS) | hypothèse | banc d'essai (les 3 barreaux) |
| **H5 · Gate d'interface** | hypothèse | banc d'essai |
| **H6 · Cold consolidation** (économie de la trace : `hot`/`cold`, `cool`/`warm`, [LEXIQUE](LEXIQUE.md)) : chaque trace est *hot* (sous les yeux, coûte de l'attention) ou *cold* (rangée, récupérable, coût nul) ; une trace non consultée dans une fenêtre W **refroidit** vers un froid **réversible**, on la **réchauffe** au besoin, rien n'est supprimé. **Réfutable** : *si* on refroidit toute trace non consultée dans W vers un froid réversible, *alors* le coût d'attention/validation reste borné **sans perte d'auditabilité ni d'antériorité**, mesuré par (a) corpus *hot* stationnaire dans le temps · (b) **warm-rate** faible et stable · (c) zéro trace *cold* devenue non vérifiable. **Réfutée si** : le *hot* regrossit malgré la gate · warm-rate élevé (on refroidit du vivant) · un refroidissement casse une preuve d'antériorité. Troisième face de H1 (glisser) et H3 (tamiser) : **glisser / tamiser / consolider**. | hypothèse | banc d'essai : définir W, le format *cold* réversible, la gate `cool`/`warm` ; poser l'indicateur coût/valeur (le warm-rate) avant la première mesure |

## Les mécanismes du labo sur lui-même

| Hypothèse | Rang | Prochain gate |
|---|---|---|
| **Guichet des problématiques** : *si un dépôt standardisé (template unique) + triage automatique (complétude, E-5, recevabilité sur critères publiés) + validation humaine, alors moins de problématiques perdues et des réponses tenues, mesuré par : délai moyen de réponse datée · taux de dépôts recevables · nombre de problématiques converties en hypothèses.* Première instrumentation de H5. | hypothèse (instrument mis en service en interne ; la mise en service ne promeut pas le rang) | banc d'essai : les premiers dépôts réels |
| **Ancrage de chaque affirmation** : chaque champ factuel d'une fiche porte un lien vers sa pièce (log, document, hash) ; une affirmation non étayée devient détectable mécaniquement. | hypothèse (réserve : scalabilité hors du cas de l'auteur non testée) | banc d'essai : lot de fiches ancrées champ par champ vs règle « une occurrence » (ligne de base avant/après, indicateurs fixés avant première mesure) |
| **Disclaimer d'antériorité** : obligatoire sur toute hypothèse tant que la recherche (interne + externe) n'est pas faite et consignée ; les réinventions se détectent avant inscription plutôt qu'après. | hypothèse (caution : « prouvée » le jour même par l'agent producteur du constat, pas une réplication ; plafonnée à hypothèse sans regard extérieur) | banc d'essai : compter les « ça existait déjà » découverts avant vs après inscription. Compteur ouvert : 1 détecté avant, 0 après. N=1, agent non indépendant : ne promeut pas le rang. |
| **Pièce opposable ↔ fiche dérivée** : toute fiche dérivée porte un lien systématique et versionné vers sa pièce source opposable ; la fiche n'usurpe jamais la pièce. Crédit d'antériorité obligatoire : structure = Karpathy « LLM Wiki » · mécanisme = RAG grounding/citation. Apport revendicable : application au domaine + preuve N=1 réel, jamais l'invention du principe. | hypothèse (réserves attachées : E-5 au banc) | banc d'essai sur un corpus de projet réel, sous condition E-5 : anonymisation avant tout exemple concret |

## La garde

| Élément | Rang |
|---|---|
| Tests de dérive D1–D5 (dont D2 et D4, propres au modèle) | preuve de concept ; s'applique aussi au corpus lui-même |

## Dettes ouvertes déclarées

*Déclarées comme dettes, pas masquées comme absences, conformément à « résultats négatifs publiés comme les positifs ».*

| Dette | Nature | Se referme quand |
|---|---|---|
| **Économie de la trace non mesurée** | Aucun indicateur ne compare coût de la trace/validation et valeur récupérée. La supériorité de la méthode reste affirmée, pas mesurée. Touche H1/H3 et la double valeur. Instrument candidat inscrit : H6 · Cold consolidation, dont le *warm-rate* est cet indicateur coût/valeur. | Un indicateur coût/valeur est fixé **avant** la première mesure du banc H1/H3/H6, puis mesuré. |
| **Aucun cas d'échec documenté** | Rien n'a atteint le terrain ; « zéro échec » n'est pas une force mais une immaturité (rien n'a encore été exposé à la réfutation). | Première fiche d'expérience de banc/terrain incluant ses résultats négatifs. |
| **Passage à l'échelle (au-delà du N=1)** | La validation humaine peut devenir un goulot ; pas de réponse quantitative en N=1. | Terrain avec utilisateurs réels + réplicants (gates « utilisateurs réels » / « répliqué »). |
| **La chaîne de traçabilité s'arrête au juge** | En métrologie, aucun étalon ne se déclare juste : chaque maillon se raccorde au maillon supérieur, incertitude déclarée à chaque étage. Ici : la production est étalonnée contre le référentiel (D1–D5), le référentiel est validé par la décision humaine, **la décision humaine n'est raccordée à rien** : la chaîne se termine sur un instrument non étalonné qui se déclare juste. Corollaire : D1–D5 testent la production, rien ne teste la décision. Une décision erronée du juge est invisible aux cinq tests, et une production qui s'y conforme est déclarée *saine* : le dispositif convertit une erreur du juge en conformité certifiée. | Un **raccordement** existe : juge externe non-auteur sur un échantillon de **décisions** (pas de productions), au gate « auditable ». À défaut : **incertitude du juge déclarée**, comme les trois dettes ci-dessus. Ne se referme pas par une auto-évaluation, ni par un agent instruit de contredire, ni par un test D6 (un test de plus contre le *même* référentiel allonge le maillon du bas, il ne raccorde rien). |

## Objets d'étude et leurs registres propres

Ce registre tient les rangs du pipeline du labo. Chaque corpus tient en outre ses rangs de preuve dans sa propre SPEC : **WORKING REFERENCE** (objet d'étude n° 3, dépôt initial 2026-08-11) sur l'échelle du pipeline : tout y est au rang hypothèse, verdict cité ligne à ligne. **MYSTANCE** (objet d'étude n° 2, dépôt initial 2026-08-02, à jour en 0.3) tient les siens dans sa SPEC ; échelle : *précédent d'usage* (au moins une occurrence réelle, datée, non mesurée) · *spécifié* (règle écrite, aucun déploiement) · *mesuré* · *répliqué*. À ce jour : motif « 3 + libre » et posture au rang *précédent d'usage* ; tout le reste *spécifié* ; **rien de mesuré ni répliqué**. Deux échelles, une même discipline : le rang se gagne par l'usage, et le vocabulaire ne dépasse jamais la preuve.

## Profils

| Profil | Rang |
|---|---|
| SLIDING CANON | preuve de concept en usage réel (N=1, non mesuré) |

---

*ONDE AI R&D. À la promotion d'un mécanisme (gate franchie), mettre à jour la ligne ici + le statut dans la fiche : les deux, sinon dérive D4.*
