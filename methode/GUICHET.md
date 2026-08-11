# GUICHET DES PROBLÉMATIQUES · ONDE AI R&D

*Vue publique : instantané du 2026-08-02, non resynchronisé depuis : la cassette interne du
laboratoire fait foi, et elle a avancé (registre en révision 16 au 2026-08-11). Resynchronisation
complète : gate déclarée avant toute mise en public ([CHANGELOG](../CHANGELOG.md), 0.3.0).*

*Version publiée (guichet validé et en service en interne depuis juillet 2026 ; **le dépôt public n'est pas encore ouvert** : il ouvrira avec les règles de contribution, voir [ROADMAP](../ROADMAP.md)). C'est l'entrée unique du pipeline et une incarnation de H5 (gate d'interface). Distinction tenue : la validation met l'instrument en service ; le guichet reste inscrit au registre **au rang hypothèse** — il se teste comme les autres, par les premiers dépôts réels, et le rang se gagne par l'usage.*

## Principe

Toute problématique (du fondateur, d'un constructeur, d'un contributeur, d'un utilisateur) entre par **le même dépôt standardisé**. Un template unique, une moulinette de triage, une validation humaine. Personne ne passe par la fenêtre, pas même le fondateur.

## Les trois portes (qui dépose)

1. **Porte labo** : le chercheur et ceux qui travaillent officiellement avec le labo (contributeurs-chercheurs nommés, profil R&D terrain).
2. **Porte utilisateur** : quiconque utilise les mécanismes, kits et profils du labo, dans n'importe quel environnement (chat nu, agentique, AIOS).
3. **Porte constructeur** : un bâtisseur de système (un AIOS ou tout autre) qui a relevé des problématiques dans son produit ou chez ses utilisateurs, y compris des problématiques auxquelles il a déjà réfléchi : ses hypothèses arrivent comme propositions attachées au dépôt, bienvenues, et passent les gates comme les autres.

**Les portes disent QUI dépose ; les sources disent D'OÙ vient la problématique** (terrain / pratique / anticipation). Les deux dimensions se croisent librement : un constructeur peut déposer une anticipation, un utilisateur une friction de pratique. Même template, même moulinette, mêmes gates pour les trois portes.

## Le dépôt · fiche unique

Trois types de dépôt sur la même fiche : **problématique** · **proposition d'amélioration** · **modification réalisée**. Champs obligatoires : date/heure · déposant + lien déclaré · type · source (1/2/3) · sujet en une phrase · l'observation (l'occurrence concrète) · l'enjeu · l'échéance s'il y en a une · déjà tenté/fait · hypothèses proposées (facultatif) · données sensibles (oui/non).

## La moulinette · triage automatique, validation humaine

À réception, un traitement automatique produit trois choses :

1. **Contrôle de complétude** : champs manquants signalés.
2. **Flag éthique** : passage de la checklist E-5 (données personnelles, consentement, divulgation, détournement, charge) : tout point levé est marqué pour revue humaine.
3. **Score de recevabilité** : calculé sur critères publiés : occurrence observée citée (ou dépôt marqué « anticipation pure ») · sujet unique par dépôt · absence de contradiction interne · enjeu explicite. Trois bandes : **recevable** · **à reformuler** (réponse type automatique, motivée point par point) · **irrecevable motivé**.

**Garde non négociable : le score propose, il ne bloque jamais.** Toute réponse automatique indique la voie d'appel humaine. La machine trie, l'humain décide : le guichet applique le positionnement du labo à sa propre porte. Un score est une proposition : le traiter comme une validation serait une dérive D4.

## Priorité de traitement

Deux dimensions, jamais confondues :
- **La provenance fixe la plausibilité** (terrain et pratique ancrées ; anticipation sous règle d'ancrage).
- **L'enjeu et l'échéance fixent le rang de traitement** : une problématique bloquante de production avec client ou délai passe devant une anticipation à froid.

## Ce que le labo s'engage à rendre

Pour tout dépôt recevable : un **accusé daté** · l'inscription au **journal de traitement** · la formulation en hypothèse réfutable (ou le motif de non-conversion) · une **réponse datée** : décision de traitement, position dans la file, prochaine étape. Une contribution recevable entre au rang hypothèse et passe les mêmes gates ; le banc d'essai mesure ensuite sa **scalabilité** : tient-elle au-delà du cas de son auteur ? Règle : critères publiés, délais tenus, sinon les déposants forkent, et ils auront raison.

## Le profil du contributeur-chercheur (porte labo)

Profil **R&D terrain** — *research & development engineering* : la fusion du chercheur et du praticien. On instruit avec rigueur ET on a les mains dans un système réel. Tout contributeur qui rejoint la porte labo est attendu sur cette double posture.

## Ce que le guichet n'est pas

Pas un tribunal des idées (la réflexion libre reste libre — seul le *dépôt* est formalisé) · pas un SAV (le labo instruit des mécanismes, il ne dépanne pas un projet) · pas une file d'attente opaque (journal consultable, réponses datées).
