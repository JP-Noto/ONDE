# ONDE AI R&D

**Laboratoire de recherche appliquée et développement : travail humain–IA.**
Devise : *CONNECT THE DOTS*.

> **Rang des travaux présentés : hypothèses et preuves de concept : rien de plus.**
> Ce dépôt présente le laboratoire : sa thèse, son problème, sa méthode. Il ne revendique aucun résultat démontré. « Démontré » exige un chiffre ; aucun chiffre n'existe encore.

*Le français fait foi. English readers: see [README.md](README.md) for an orientation page.*

---

## Ce que le labo est

ONDE AI R&D est un laboratoire de recherche appliquée *et* de développement : il produit des connaissances éprouvées et les livre en trois formes : **le mécanisme explique, le test contredit, le kit s'utilise**.

Il étudie comment travailler durablement avec une IA : un travail qui reste sous autorité humaine et dont la qualité se mesure. « Travail » couvre tout workflow humain–IA (créer, décider, organiser, apprendre) pas seulement la fabrication de livrables.

Méthode : problématiques vécues → hypothèses réfutables → pipeline à gates. Un praticien-chercheur, N=1, déclaré. Les résultats négatifs sont publiés.

## Le problème

Le travail assisté par IA échoue rarement par manque de puissance du modèle. Il échoue sur trois points :

**La durabilité.** Ce qui marche une session casse à la dixième, et casse encore au changement de génération de modèle. Les workflows ne se répètent pas ; ils se reconstruisent à chaque fois.

**L'autorité.** Le canon d'un projet glisse sans décision ; une proposition non validée devient référence par répétition ; la mémoire du projet enfle jusqu'à l'inutilisable, et l'humain, noyé, abdique de fait.

**La mesure.** La qualité du travail humain–IA se raconte au lieu de se mesurer : pas d'indicateur, pas de conditions d'échec, rien à contredire.

Ces échecs sont observables et reproductibles. Ils sont aujourd'hui traités comme des astuces de prompt. Le labo les traite comme des mécanismes : nommables, testables, réfutables.

## Le positionnement

> « L'IA propose, l'humain décide : informé, guidé, mis en état de bien décider. Chaque décision fait avancer le travail et laisse sa trace. La responsabilité est le prix ; la sécurité est le gain. Le workflow avance et se répète sous autorité humaine : personnel ou professionnel, même règle. »

## La méthode, en une ligne

```
réflexion → hypothèse → banc d'essai → terrain chercheur → auditable → utilisateurs réels → répliqué → doctrine
```

Le rang se gagne par l'usage, jamais auto-décerné. Détail : [`methode/PIPELINE.md`](methode/PIPELINE.md). L'appareil qui tient cette méthode : guichet,
registre, études, protocoles, dépôts : a un nom : **[ACTA](methode/ACTA.md)**.

## Contenu du dépôt

| Pièce | Ce qu'elle dit |
|---|---|
| [`PRESENTATION.md`](PRESENTATION.md) | La présentation complète du laboratoire : posture, problème, utilité, méthode, objets d'étude, périmètre, feuille de route. |
| [`methode/PIPELINE.md`](methode/PIPELINE.md) | Le pipeline de recherche à gates (v2.1) : sept étages, deux espèces de gates, boucles, péremption, éthique. |
| [`methode/PROTOCOLE-CQM.md`](methode/PROTOCOLE-CQM.md) | Les critères de qualité minimum de chaque gate : écrits avant le passage, vérifiables mécaniquement, symétriques. |
| [`methode/PROTOCOLE-PROJETS.md`](methode/PROTOCOLE-PROJETS.md) | Le protocole des projets de production : WIP → STAGING → LIVE → GELÉ → ARCHIVÉ, gates P1/P2. |
| [`methode/GUICHET.md`](methode/GUICHET.md) | Le guichet des problématiques : entrée unique du pipeline : dépôt standardisé, triage automatique, validation humaine. |
| [`methode/LEXIQUE.md`](methode/LEXIQUE.md) | Le vocabulaire du labo : une entrée, une ligne, un domicile. |
| [`methode/ACTA.md`](methode/ACTA.md) | L'appareil de méthode du laboratoire : guichet, journal, registre, études, protocoles, dépôts : ce qui fabrique et juge ce que les corpus publient. |
| [`methode/REGISTRE-HYPOTHESES.md`](methode/REGISTRE-HYPOTHESES.md) | La vue des rangs réels : hypothèses H1–H6, socle crédité, dettes ouvertes déclarées, et l'état du registre interne (rév. 16, jusqu'à H(T)). |
| [`ROADMAP.md`](ROADMAP.md) | La feuille de route et les chantiers de mesure déclarés. |

## Objets d'étude

Chaque objet d'étude vit dans son propre dépôt : ce dépôt-ci pointe, il ne duplique pas. **Les quatre dépôts de la famille sont publics** : LIVING REFERENCE depuis le 2026-08-06 ; MYSTANCE, WORKING REFERENCE et ce portail depuis le 2026-08-11 (chaque CHANGELOG fait foi).

**N° 1 — [LIVING REFERENCE](https://github.com/JP-Noto/LIVING-REFERENCE)** (axe autorité) : un système de références vivantes pour le travail assisté par IA : de la proposition à la référence par validation, double valeur, tamis de trace, validation partielle par facettes, glissement, tests de dérive D1–D5. Sept fiches : le socle fonde, les mécanismes construisent, la garde vérifie. **Dépôt initial : 2026-07-21** · statut : brouillon public (Public Draft) · le CHANGELOG du corpus fait foi pour les versions.

**N° 2 — [MYSTANCE](https://github.com/JP-Noto/MYSTANCE)** (axe humain) : la couche humaine des systèmes d'IA : régler la relation plutôt que la dominer. Paramètre cardinal : le niveau d'assistance (quatre niveaux nommés : MÉDIATION · APPUI · COLLABORATION · GÉNÉRATION) ; invariant proposé : *le niveau module combien l'IA propose, jamais qui décide*. Cinq mécanismes : niveau d'assistance, posture, motif « 3 + libre », templates verrouillés, nommage du compagnon. **Dépôt initial : 2026-08-02, à jour au 2026-08-11** (la carte des couches y accueille WORKING REFERENCE) · statut : brouillon public (Public Draft) · rangs de preuve tenus dans sa SPEC (rien de mesuré ni répliqué à ce jour) · le CHANGELOG du corpus fait foi pour les versions.

**N° 3 — [WORKING REFERENCE](https://github.com/JP-Noto/WORKING-REFERENCE)** (axe exécution) : la référence qui travaille : un corpus
n'est pas un document qu'on lit, c'est une **fonction qu'on appelle** : une **constante** (l'invariant
gagné par gates, ce qui doit survivre à un changement de génération de modèle) plus des **variables**,
l'instanciation **décidée** par la couche de référence selon l'état déclaré du travail, **servie**
(jamais chargée en bloc) et **scellée** (chaque décision de service traçable). Le média est une
variable. C'est la généralisation exécutable de LIVING REFERENCE, et la réponse structurelle à l'axe
durabilité du problème. **Dépôt initial : 2026-08-11** · statut : brouillon public (Public Draft) ·
rang : **hypothèse** (H(T) au registre), dit tel quel · le CHANGELOG du corpus fait foi pour les
versions. Domicile canonique : <https://github.com/JP-Noto/WORKING-REFERENCE>
(dépôt public depuis le 2026-08-11).

**Les quatre couches** (aucune redondance entre elles) :

| Couche | Gouverne |
|---|---|
| Un OS d'IA (tiers) | le système : lois, fichiers, boucles, frontières |
| LIVING REFERENCE | le statut du savoir : ce qui est validé, ce qui fait canon |
| WORKING REFERENCE | le service de la référence : ce qui monte à l'appel, servi et scellé |
| MYSTANCE | la place de l'humain : la relation paramétrée, la souveraineté |

## Antériorité

Deux enveloppes e-Soleau INPI horodatent ces travaux, empreintes SHA-256 aux récépissés :
**DSO2026026503** (21/07/2026 (LIVING REFERENCE) · **DSO2026028969** (11/08/2026) MYSTANCE 0.3,
WORKING REFERENCE 0.1.6, et le laboratoire lui-même, fond et vitrine).

## Les gardes du labo

- **Crédit ≠ preuve** : l'adoption par un tiers établit la transférabilité, jamais la validité.
- **Récence ≠ qualité** : la ressemblance aux N derniers n'est pas un critère de traversée.
- **Notes = signal** : les évaluations de la communauté déclenchent un examen ; elles ne sont jamais la métrique.
- **« Démontré » exige un chiffre** : plafond de vocabulaire : « preuve de concept » tant qu'aucune mesure n'existe.
- **Résultats négatifs publiés** : un labo qui ne publie que ses succès n'est pas un labo.

## Statut de ce dépôt

Brouillon public (Public Draft) — dépôt public depuis le 2026-08-11, consigné au [CHANGELOG](CHANGELOG.md). Ancrer n'est pas publier : l'antériorité est tenue par les enveloppes e-Soleau, la publication par ce dépôt. Les versions suivent le CHANGELOG.

## Licence et citation

Contenu sous [CC BY-NC-SA 4.0](LICENSE.md). Pour citer : [`CITATION.cff`](CITATION.cff).

---

*Julien-Pierre NOTO · ONDE AI R&D · laboratoire fondé le 2026-07-13 · Rang des travaux : hypothèses et preuves de concept.*
