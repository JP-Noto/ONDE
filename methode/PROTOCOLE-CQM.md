# PROTOCOLE CQM · les critères de chaque gate

*Vue publique : instantané du 2026-08-02, non resynchronisé depuis : la cassette interne du
laboratoire fait foi, et elle a avancé (registre en révision 16 au 2026-08-11). Resynchronisation
complète : gate déclarée avant toute mise en public ([CHANGELOG](../CHANGELOG.md), 0.3.0).*

*Version publiée du protocole en vigueur au laboratoire (validé en juillet 2026). Ce protocole définit **les vérifications**, pas les valeurs chiffrées : fixer des seuils sans données serait de l'invention. Chaque valeur marquée `[à fixer]` se fixe **avant la première mesure concernée, jamais après**. Domicile des étages : [PIPELINE.md](PIPELINE.md).*

Trois propriétés non négociables :

1. **Écrits avant le passage.** Une gate dont les critères s'écrivent au moment de juger n'est pas une gate.
2. **Vérifiables mécaniquement.** Pas d'adjectif — chaque critère est un test qu'un tiers peut passer (présence d'un champ, résultat d'un grep, existence d'un artefact daté).
3. **Symétriques.** Les livrables du labo et les contributions communautaires passent exactement les mêmes gates. Un privilège d'auteur invaliderait le protocole.

À chaque gate s'ajoute la **checklist E-5** (données personnelles/RGPD · consentement · divulgation des liens · potentiel de détournement · charge et risque utilisateur) : cinq cases, pas une bureaucratie.

## Gate 1 · réflexion → hypothèse *(gate-décision)*

- [ ] Une **prédiction observable** est énoncée (que verrait-on si c'est vrai ? si c'est faux ?).
- [ ] La **filiation** est posée : antécédents internes datés liés ; art antérieur externe nommé, ou « non trouvé » consigné avec la recherche faite.
- [ ] **Règle d'ancrage** : au moins une occurrence datée et vérifiable citée, ou entrée marquée « anticipation » (ne franchira pas la gate 3 sans occurrence).
- [ ] Un **domicile unique** est assigné ; les autres documents lieront.
- [ ] Zéro adjectif dans la formulation des critères de succès.
- [ ] GO consigné en une ligne : daté, signé, motivé.

## Gate 2 · hypothèse → banc d'essai *(entrée de gate-mesure)*

- [ ] Le **protocole du banc est écrit avant le run** : quoi observer, sur quels cas construits, combien `[à fixer]`.
- [ ] Ce qui compterait comme **échec** est énoncé d'avance, et l'étage de renvoi en cas d'échec (hypothèse).
- [ ] La mécanique est **spécifiée assez pour être éprouvée** : déclaration de profil complète, règles machine-lisibles.
- [ ] Les **scénarios d'abus** sont définis (rubber-stamping, contournement de gate, réapparition d'un rejeté).
- [ ] Si simulation : **les limites sont écrites dans la fiche** : le banc falsifie la mécanique, ne valide jamais la valeur ; biais des juges-LLM déclarés.

## Gate 3 · banc d'essai → terrain chercheur *(gate-mesure)*

- [ ] **Fiche d'expérience du banc consignée au cahier** : date, hypothèse, version du protocole, résultat, itérations correctives, décision.
- [ ] Le terrain d'observation est identifié, et déclaré comme non-preuve (opérateur = auteur).
- [ ] Les **deux pistes** sont définies (A : barreau ③ AIOS · B : barreau ①/② UI nue) avec leur fenêtre bornée `[à fixer]`.
- [ ] Une hypothèse née d'anticipation cite désormais **au moins une occurrence observée** (règle d'ancrage, sinon elle reste au banc).

## Gate 4 · terrain chercheur → auditable *(gate-mesure + revue éthique n° 1)*

- [ ] **Fiches des deux pistes consignées** ; une divergence A/B est publiée comme falsification de H4, pas lissée.
- [ ] **Piste complète** : statuts affichés partout, validations consignées (qui, quoi, périmètre, écarté et pourquoi), rejets avec raisons.
- [ ] **Chaque revendication porte son étage** : grep de contrôle : « démontré » sans chiffre = blocage ; vocabulaire au-dessus du rang = blocage.
- [ ] **D1–D5 passés sur le corpus lui-même**, résultat consigné.
- [ ] **Les résultats négatifs** du banc et du terrain sont consignés au registre et listés ; ceux qui sont publiés le sont avec la borne du tri déclarée : le récit n'est écrit que pour ce qui a changé une décision, jamais selon ce qui flatte.
- [ ] CHANGELOG à jour, licence et attribution posées, filiation (LINEAGE) à jour.
- [ ] Zéro adjectif comme critère dans les textes normatifs : grep de contrôle.
- [ ] **Revue éthique n° 1 tenue** (première exposition de tiers en aval), consignée.

## Gate 5 · auditable → utilisateurs réels *(gate-décision)*

- [ ] Le **kit est déployable par un tiers sans l'auteur** : test réel : une personne hors labo réussit l'amorçage en suivant le seul corpus publié, sans échange avec l'auteur ; son parcours est consigné.
- [ ] Le **plan de recrutement des sujets est écrit** : d'où viennent les dix premiers inconnus, par quel canal, avec quel message : les canaux liés au labo étiquetés comme tels.
- [ ] Le **protocole de mesure est publié avant les mesures** : baseline, qui classe créatif/correctif (un tiers, jamais le praticien seul), seuils `[à fixer]`, durée `[à fixer]`.
- [ ] Le **kit est auto-rapporteur** : le rapport de réplication se génère pendant l'usage.
- [ ] Un **canal de retour** existe (issues) avec engagement de délai `[à fixer]` : l'autorité de validation qui ne répond pas se fait forker.

## Gate 6 · utilisateurs réels → répliqué *(gate-mesure)*

- [ ] **≥ X `[à fixer]` réplications indépendantes** sur **≥ Y `[à fixer]` workflows distincts** — indépendant se déclare : tout lien avec l'auteur (familial, commercial, de collaboration) est divulgué et disqualifie la réplication comme indépendante ; les répliquants venus d'un canal lié au labo sont comptés mais distingués.
- [ ] Seuls les **rapports de réplication** comptent : le scoring priorise, ne fait jamais franchir ; une faille d'audit renvoie à hypothèse.
- [ ] La **métrique atteint son seuil prédéclaré** (gate 5) sur la durée prédéclarée.

## Gate 7 · répliqué → doctrine (canon glissant, stable pour un horizon déclaré) *(gate-décision finale)*

- [ ] Le mécanisme a **survécu à ≥ 1 changement de génération de modèle sans révision** : définition opérationnelle de « stable ». **Ce qui compte comme génération** (révisable) : le modèle en production pour ce mécanisme **change de famille** OU **franchit un saut de version majeure annoncé par le fournisseur** (ex. 4.x → 5.0), journalisé à sa date. **Clause de jugement** : un modèle de même version dont le comportement change de façon démontrée au banc peut être déclaré événement de génération, avec raison journalisée : la règle propose, l'humain décide.
- [ ] **Doctrine ≠ permanent** : le rang porte une **fenêtre de fraîcheur déclarée** et un **déclencheur de révision** à la prochaine génération majeure (canon glissant). À l'échéance non re-testée, le rang **retombe à « répliqué »** (fraîcheur périmée), publié comme tel.
- [ ] Chaque génération majeure supplémentaire survécue **allonge l'horizon déclaré** (sévérité accumulée — Mayo).
- [ ] Les **résultats négatifs** rencontrés en route sont consignés avec les positifs, listés, et publiés pour partie selon la même borne.
- [ ] **Revue contradictoire** : au moins un examinateur qui n'est pas l'auteur signe le passage (quatre yeux).

## Boucles et péremption

Chaque échec renvoie à l'étage défini par sa gate ; **revue de boucle** consignée (*continuer / pivoter / suspendre*) : jugement humain, pas compteur. Péremption : **3 mois** sans activité → `suspendu` (valeur unique, partagée avec le [protocole des projets](PROTOCOLE-PROJETS.md)). `Réfuté` et `suspendu` se publient comme les positifs.

## Inspirations à sourcer avant publication du protocole au rang auditable

Pré-enregistrement (type OSF / Registered Reports), revue par les pairs, gates de release open source (politiques de gel type Debian, semver). **Sources à vérifier et dater au moment de cette publication, pas encore citées, conformément à la règle de filiation (« ne sont pas cités tant qu'ils ne le sont pas »).**

---

*ONDE AI R&D. Les `[à fixer]` se fixent avant la première mesure concernée.*
