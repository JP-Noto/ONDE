# ONDE AI R&D
## Laboratoire de recherche appliquée et développement · travail humain–IA
*Présentation (août 2026) Julien-Pierre NOTO. Statut : Public Draft.*

---

## Résumé

ONDE AI R&D est un laboratoire de R&D : recherche appliquée *et* développement : il produit des connaissances éprouvées et les livre en mécanismes, tests et kits. Il étudie comment travailler durablement avec une IA : un travail qui reste sous autorité humaine et dont la qualité se mesure. « Travail » couvre tout workflow humain–IA (créer, décider, organiser, apprendre) pas seulement la fabrication de livrables. Méthode : problématiques vécues → hypothèses réfutables → pipeline à gates. Un praticien-chercheur, N=1, déclaré. Les résultats négatifs sont publiés. Rang actuel des travaux : hypothèses et preuves de concept. L'un d'eux (la double valeur) est un mécanisme central de l'architecture d'un OS tiers.

## Posture

Le labo est adossé à une pratique réelle du travail avec l'IA ; le chercheur est lui-même utilisateur. C'est le dispositif d'observation : la posture dite « praticien-chercheur ». Vocabulaire tenu dans tout le document, trois rôles : l'**utilisateur** travaille avec l'IA, le **chercheur** instruit les hypothèses, le **constructeur** bâtit les systèmes. Les rôles sont des casquettes, pas des identités : une même personne peut en porter plusieurs, et **chacun choisit lesquelles**. Le rôle se lit à l'acte ; la spécialisation, au sujet. Trois sources de problématiques :

1. **le terrain** : un utilisateur bute : une problématique apparaît ;
2. **la pratique** : le chercheur bute dans son propre travail (le chercheur est lui aussi un utilisateur : N=1, déclaré) : une problématique apparaît ;
3. **l'anticipation** : le cas pensé à froid : « si on fait X, ça devrait donner Y, non ? » : une problématique apparaît, sans occurrence observée, encore.

Les sources décrivent des origines, pas des personnes : tout contributeur déclaré peut déposer une problématique par chacune des trois : un constructeur qui bute sur son architecture dépose en source 2 au même titre que le chercheur. Les problématiques n'ont pas toutes le même poids : la provenance fixe la plausibilité ; **l'enjeu et l'échéance fixent le rang de traitement** : une problématique bloquante de production, avec client ou délai, passe devant une anticipation à froid.

Deux règles bornent la troisième source. La provenance ne fixe jamais la validité : toute hypothèse passe les mêmes gates. Règle d'ancrage : une hypothèse née de la seule anticipation ne va pas au terrain sans citer une occurrence observée : **montre une occurrence, ou reste au banc**. Une ou plusieurs occurrences, sur un même projet ou sur plusieurs : une problématique peut être ciblée comme transversale. L'accès à un AIOS de production permet d'éprouver une idée en jours. Fait : la double valeur (aujourd'hui centrale dans un OS tiers) est née de la source 2, pas d'une demande utilisateur.

## Problème

Le travail assisté par IA échoue rarement par manque de puissance du modèle. Il échoue sur les trois points que le labo étudie :

**La durabilité.** Ce qui marche une session casse à la dixième, et casse encore au changement de génération de modèle. Les workflows ne se répètent pas ; ils se reconstruisent à chaque fois.

**L'autorité.** Le canon d'un projet glisse sans décision ; une proposition non validée devient référence par répétition ; la mémoire du projet enfle jusqu'à l'inutilisable, et l'humain, noyé, abdique de fait.

**La mesure.** La qualité du travail humain–IA se raconte au lieu de se mesurer : pas d'indicateur, pas de conditions d'échec, rien à contredire.

Ces échecs sont observables et reproductibles. Ils sont aujourd'hui traités comme des astuces de prompt. Le labo les traite comme des mécanismes : nommables, testables, réfutables.

## Utilité

**Utilisateur** : quiconque travaille avec une IA : des mécanismes pour tenir un référentiel sans dérive, valider sans se noyer, tracer sans s'alourdir. Applicables en chat nu, sans rien installer : la plupart des utilisateurs travaillent sans AIOS ; la transversalité (H4) existe pour eux.

**Constructeur** : tout AIOS : savoir quels mécanismes tiennent avant de les coder. Les tests de dérive D1–D5 sont implémentables. Fait : la double valeur (chaque interaction utile fait avancer le travail *et* laisse une trace) est un mécanisme central de l'architecture d'un AIOS en production. Pas un ajout d'interface : une pièce d'architecture, adoptée parce qu'elle résolvait une problématique réelle.

**Écosystème** : le savoir actuel sur le travail humain–IA est anecdotique, captif d'un outil, invérifiable, et casse à chaque génération de modèle. Le labo produit l'inverse : des connaissances réfutables, indépendantes des outils, testées dans la durée. Aucun vendeur n'a intérêt à produire cette couche : elle n'appartient à personne. Analogie : les règles de l'art du bâtiment : elles disent ce qui tient, indépendamment du constructeur.

## Positionnement

« L'IA propose, l'humain décide : informé, guidé, mis en état de bien décider. Chaque décision fait avancer le travail et laisse sa trace. La responsabilité est le prix ; la sécurité est le gain. Le workflow avance et se répète sous autorité humaine : personnel ou professionnel, même règle. »

## Méthode

L'appareil qui tient cette méthode a un nom : **ACTA** : le guichet des problématiques, le journal,
le registre des hypothèses, les études, les protocoles et les dépôts d'antériorité
([methode/ACTA.md](methode/ACTA.md)).

```
réflexion → hypothèse → banc d'essai → terrain chercheur → auditable → utilisateurs réels → répliqué → doctrine
```

- Toute problématique entre par un **dépôt standardisé** : template unique pour tous, fondateur compris : déposant, source, occurrence, enjeu, échéance. Triage automatique (complétude, critères éthiques, recevabilité sur critères publiés), puis validation humaine : le score propose, l'humain décide.
- Une idée devient hypothèse sous la forme : *si [mécanisme], alors [effet observable], mesuré par [indicateur]*. Sinon elle n'entre pas.
- Trois gates mesurées : banc d'essai, terrain chercheur, réplication. Indicateur principal : itérations correctives par livrable validé. Les autres gates : décision humaine consignée.
- Terrain chercheur : deux environnements obligatoires, AIOS et interface nue (une fenêtre de chat grand public, sans système installé). Un mécanisme qui ne tient que sur un seul a falsifié sa transversalité ; ce résultat se publie.
- L'échec à une gate renvoie à un étage défini. Une hypothèse inactive est suspendue. Réfutations et suspensions se publient.
- **Auditable** = téléchargeable, protocole complet, critères de réplication inclus. **Répliqué** = ≥ X réplications indépendantes sur ≥ Y workflows distincts. **Doctrine** = répliqué + a survécu à un changement de génération de modèle sans révision.
- Les scores utilisateurs sont des signaux. Seul le rapport de réplication fait monter.

## Objets d'étude

Le problème est général ; il s'instruit par objets d'étude : chacun attaque un axe du problème.

### N° 1 · LIVING REFERENCE (axe autorité)

Cinq hypothèses sur la tenue d'un référentiel de projet : **H1 glissement** (fenêtre + invariants + rappel, coût constant), **H2 héritage par facettes** (validation scopée, pas de précédent nommé trouvé), **H3 tamis de trace** (une trace n'est émise que si elle déplace un axe), **H4 transversalité** (du chat nu à l'AIOS), **H5 gate d'interface**. Un profil éprouvé : SLIDING CANON, rang preuve de concept en usage réel (N=1, non mesuré). Une batterie de tests de dérive D1–D5, appliquée au corpus lui-même. Lineage public (StreamingLLM, MemGPT, ADR, modèle bitemporel, Ranganathan) : la contribution revendiquée est la recontextualisation et l'assemblage, pas les primitives. État : **dépôt initial le 2026-07-21** (Public Draft ; le CHANGELOG du corpus fait foi pour les versions) ; stade preuve de concept. Domicile canonique : <https://github.com/JP-Noto/LIVING-REFERENCE> (dépôt public depuis le 2026-08-06). Le corpus vit dans son propre dépôt ; celui-ci pointe, il ne duplique pas.

### N° 2 · MYSTANCE (axe humain)

La couche humaine des systèmes d'IA : **régler la relation plutôt que la dominer**. Le réglage de la relation humain–IA prolifère sur le marché, mais sans norme : fragmenté, sans contrat publié, révocable sans préavis, et sans invariant. MYSTANCE propose de le normer : des paramètres explicites, visibles, tenus par l'utilisateur, garantis par des règles écrites et réfutables. Paramètre cardinal : le **niveau d'assistance**, quatre niveaux nommés à contrat comportemental (MÉDIATION · APPUI · COLLABORATION · GÉNÉRATION), échelle close aux deux bouts (jamais zéro médiation, jamais de production 100 % IA). Invariant proposé : *le niveau module combien l'IA propose, jamais qui décide.* Cinq mécanismes : niveau d'assistance, posture (quatre registres canoniques), motif « 3 + libre », templates verrouillés (clause contenant/contenu : le contenant est protégé, le contenu appartient à l'utilisateur), nommage du compagnon. État : **dépôt initial le 2026-08-02** (Public Draft ; le CHANGELOG du corpus fait foi). Rangs de preuve tenus dans sa SPEC : « précédent d'usage » ou « spécifié » selon le mécanisme : rien de mesuré ni répliqué à ce jour, dit tel quel. Domicile canonique : <https://github.com/JP-Noto/MYSTANCE> (dépôt public depuis le 2026-08-11). **À jour au 2026-08-11** : la carte des couches accueille WORKING REFERENCE, le hors-domaine multi-humains est
déclaré, l'échelle des niveaux porte son schéma.

### N° 3 · WORKING REFERENCE (axe exécution)

La référence qui travaille : **le corpus comme fonction**. Une **constante** (l'invariant gagné par
gates : ce qui doit survivre à un changement de génération de modèle sans révision) plus des
**variables**, l'instanciation **décidée** par la couche de référence d'après l'état déclaré du
travail en cours, **servie** (jamais chargée en bloc) et **scellée** (chaque décision de service
traçable, chaînée). Le média est une variable : un médium de plus coûte un générateur et un banc,
jamais une seconde couche de référence. Propriété mesurable centrale : le volume servi par appel ne
croît pas avec la taille du corpus. C'est la généralisation exécutable de LIVING REFERENCE : l'aîné,
testé contre la SPEC du cadet, est une instance partielle : son glissement passe les familles
constante/instanciation/service, mais il ne scelle pas ses décisions de service ; l'écart est
exactement l'apport. État : **dépôt initial le 2026-08-11** (Public Draft ; le CHANGELOG
du corpus fait foi pour les versions). Rang : **hypothèse**, H(T) au registre du laboratoire, chaque revendication du
corpus porte son rang. Domicile canonique : <https://github.com/JP-Noto/WORKING-REFERENCE> (dépôt public depuis le 2026-08-11).

## Existant

- Corpus LIVING REFERENCE (CC BY-NC-SA) : **dépôt initial fait le 2026-07-21** (Public Draft), **passage en dépôt public le 2026-08-06** ; le CHANGELOG du corpus fait foi.
- Corpus MYSTANCE (CC BY-NC-SA + clause contenant/contenu) : **dépôt initial fait le 2026-08-02** (dépôt privé, Public Draft) : SPEC, whitepaper, lineage vérifié sur textes originaux, journal d'antériorité à deux entrées datées (balayage savant + balayage produits 2023–2026), neuf fiches, premier template verrouillé.
- Trois concepts du socle sont intégrés au cadre d'un AIOS tiers en production : la double valeur (mécanisme central de l'architecture), la validation tracée et le cycle de statuts. Crédit ≠ preuve : l'adoption date et crédibilise, seules les gates font monter. *(Crédit externe et lien : à poser avant toute publication qui les mobilise.)*
- Accès à un AIOS de production : batteries de test en environnement AIOS réel.
- Guichet des problématiques : dépôt standardisé + triage + validation humaine (au rang hypothèse : il passe ses propres gates).
- Kit démonstrateur à ~80 % ; conçu pour produire son rapport de réplication comme sous-produit de l'usage.
- Un conteneur de projets réels : terrain d'observation, jamais preuve.
- **Antériorité horodatée** : deux enveloppes e-Soleau INPI : DSO2026026503 (21/07/2026, LIVING
  REFERENCE) · DSO2026028969 (11/08/2026, MYSTANCE 0.3 + WORKING REFERENCE 0.1.6 + le laboratoire,
  fond et vitrine), empreintes SHA-256 aux récépissés.
- **Appareil de méthode nommé** : ACTA (2026-08-10) : 33 dépôts au guichet, registre des hypothèses
  en révision 16, lettres jusqu'à H(T).

## Périmètre

- Le labo produit des mécanismes éprouvés, des tests et des kits. Il ne construit pas d'outil ni d'OS et n'héberge aucun utilisateur : c'est un choix de rôle, pas une frontière défensive.
- **La discipline du label fait sa valeur** : rien ne se prévaut d'un rang non atteint, ni un système du côté du labo, ni le labo du côté d'un déploiement. C'est cette retenue qui rend une certification crédible le jour où elle est décernée.
- Le périmètre va du chat nu à l'OS complet (H4) : la plupart des utilisateurs travaillent sans installer aucun système, donc les mécanismes doivent tenir partout. Un résultat obtenu sur un seul environnement n'engage que cet environnement ; qu'un mécanisme soit repris ailleurs, ou sans OS du tout, est un **cas de mesure attendu** : la convergence se fait par les mécanismes.

## Feuille de route

Publication du corpus au rang auditable (dépôt public, daté, citable) → seuils de mesure fixés avant toute première mesure → démonstrateur finalisé (trois environnements) → plan de recrutement des répliquants écrit avant l'ouverture → règles de contribution publiées avant l'ouverture (les contributions entrent au rang hypothèse, mêmes gates) → premières doctrines certifiées, ou premières réfutations publiées.

**Chantiers de mesure déclarés** : l'économie de la trace (coût de tracer/valider vs valeur récupérée : le tamis borne le coût, aucun indicateur ne le compare encore à la valeur) et le passage à l'échelle au-delà du N=1 (quand la validation humaine peut devenir un goulot). À instrumenter au banc d'essai (H1/H3) avant toute revendication de supériorité.

## Demande au lecteur

Lire le corpus quand il sera auditable. Contredire : chaque mécanisme publie ses conditions d'échec. Répliquer : le kit produit le rapport pendant l'usage. La réplication par des inconnus est la seule voie vers le rang doctrine.

---

*Julien-Pierre NOTO · ONDE AI R&D · Rang des travaux présentés : hypothèse et preuve de concept, rien de plus.*
