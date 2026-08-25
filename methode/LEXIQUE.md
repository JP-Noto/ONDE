# LEXIQUE · ONDE AI R&D

*Vue publique : instantané du 2026-08-02, non resynchronisé depuis : la cassette interne du
laboratoire fait foi, et elle a avancé (registre en révision 16 au 2026-08-11). Resynchronisation
complète : gate déclarée avant toute mise en public ([CHANGELOG](../CHANGELOG.md), 0.3.0).*

*Version publiée. Règle du lexique : il **lit, il ne redéfinit pas** : chaque entrée tient en une ligne et pointe son domicile ; en cas d'écart, le domicile fait foi. Les domiciles « SPEC » renvoient au corpus LIVING REFERENCE (dépôt distinct : <https://github.com/JP-Noto/LIVING-REFERENCE>, public depuis le 2026-08-06).*

## Convention de première mention (règle de rédaction)

- **On forge en anglais d'abord.** Le terme **anglais est canonique** et doit coller au concept au plus près ; le français suit. On pense le concept en anglais, on choisit le mot le plus fidèle, puis on traduit.
- **Description « 1 + 1 = 2 ».** Tout concept coiné se décrit en **une phrase concise et totalement intelligible**, sans glose savante ni appel à l'autorité.
- **Portée bornée.** La règle ne vise que les termes que le corpus **invente ou détourne** (ceux du présent lexique). La langue courante reste supposée, sinon régression infinie, et le lexique attrape sa propre enflure.
- **Première mention = glose + lien.** À sa première occurrence dans un document, un terme coiné porte une glose courte puis un lien vers son ancre au LEXIQUE, jamais une redéfinition complète. Le LEXIQUE fait foi ; la glose est la mention accessible.
- **Un concept, un nom.** Avant de forger, vérifier qu'aucun terme réservé n'est déjà pris. *Cas fondateur : `cool` / `refroidir` (économie de la trace) a été choisi pour ne pas entrer en collision avec `freeze` / `geler` (verrouillage-document) : deux concepts, deux mots.*

## La méthode (domicile : SPEC du corpus LIVING REFERENCE)

- **Proposition** : toute production de l'IA ; n'engage rien.
- **Validation** : décision explicite de l'utilisateur : quoi, jusqu'où, sur quoi.
- **Référence** : proposition validée ; guide dans les limites exactes de sa validation.
- **Les trois axes** : maturité (engage ?), portée (où, sur quoi ?), fraîcheur (jusqu'à quand ?).
- **Récence** : le fait d'être le plus récent ; jamais un critère d'admission (l'admission = validation), ne classe que parmi les validés ; ≠ fraîcheur.
- **Canon glissant** : le seul concept de fenêtre : les N derniers validés + invariants, qui glisse à chaque validation. *« Canon flottant » = ancien nom, déprécié.*
- **Unité de continuité** : la maille dans laquelle la fenêtre glisse (scène, chapitre, chantier…), déclarée par le profil ; type + unité suffisent, aucun jugement de pertinence.
- **Invariant** : élément dont la disparition changerait une décision à venir ; borné par la nécessité, pas par le nombre.
- **Rappel / référence invitée** : retour au contexte par décision explicite, le temps d'une étape ; ne promeut rien.
- **Validation partielle / héritage par facettes** : une validation partielle ne couvre que des facettes nommées d'un vocabulaire clos ; l'aval n'hérite que du couvert.
- **Tamis de trace** *(EN : trace sieve)* : trace si et seulement si un axe bouge, ou si la perte ferait refaire ; sinon rien. *« Frein de trace » : ancien nom, déprécié (un frein ralentit, un tamis trie).*
- **Tests de dérive D1–D5** : les cinq conditions d'échec vérifiables ; s'appliquent au corpus lui-même.
- **Profil / déclaration de conformité** : un domaine déclare cinq champs : N, unité de continuité, invariance, révision, facettes.

## Le pipeline du labo (domicile : [PIPELINE.md](PIPELINE.md))

- **Réflexion** : intuition consignée, datée ; aucun engagement.
- **Hypothèse** : formulation testable : une prédiction observable est énoncée.
- **Banc d'essai** : cas construits par le labo, N petit, utilisateur simulé si utile ; **falsifie la mécanique, ne valide jamais la valeur**. *Préclinique : n'autorise que l'étage suivant.*
- **Terrain chercheur** : usage en production réelle par le praticien-chercheur (N=1 déclaré), deux pistes : A (barreau ③ AIOS) · B (barreau ①/② UI nue) ; les deux doivent passer, une divergence = H4 falsifiée.
- **Auditable** : la gate de publication : téléchargeable parce que vérifiable (piste complète, étage affiché, CQM passés), pas parce que prouvé. Précondition de l'aval : plan de recrutement écrit.
- **Utilisateurs réels** : des inconnus déploient depuis le corpus publié seul, sans l'auteur ; trois canaux : scoring = signal · réplication = mesure · audit = falsification.
- **Répliqué** : ≥ X réplications indépendantes sur ≥ Y workflows distincts (X, Y au [PROTOCOLE-CQM](PROTOCOLE-CQM.md)).
- **Doctrine (glissante)** : statut terminal, **gagné**, **jamais permanent** : répliqué + survie à ≥ 1 changement de génération de modèle sans révision ; porte une **fenêtre de fraîcheur déclarée** et un re-test à la prochaine génération majeure : à défaut, retombée à « répliqué ». Jamais auto-décerné. Aucun élément ne l'a atteint.
- **Génération (de modèle)** : le modèle en production change de **famille** ou franchit un **saut de version majeure annoncé par le fournisseur**, journalisé à sa date ; clause de jugement : un même numéro au comportement démontré changé peut être déclaré événement de génération, avec raison.
- **Gate** : passage d'étage : validation explicite contre des CQM écrits avant le passage. Deux espèces : **gate-décision** (une ligne datée, signée, motivée) · **gate-mesure** (fiche d'expérience au cahier : banc d'essai, terrain chercheur, répliqué).
- **Revue de boucle** : à chaque échec renvoyé : décision consignée *continuer / pivoter / suspendre* ; péremption **3 mois** sans activité → `suspendu` ; `réfuté` et `suspendu` se publient.
- **Cahier d'expériences** : une fiche par run ; domicile de la métrique centrale : sans lui, elle n'existe pas.
- **Gate d'interface** : la gate aux frontières entre projets : ne traverse que du validé, dans ses limites, contraintes vérifiées (hypothèse H5).
- **CQM** : critères de qualité minimum d'une gate : écrits avant tout passage, vérifiables mécaniquement, sans adjectif, symétriques (labo et communauté passent les mêmes).
- **Métrique centrale** : itérations correctives par livrable validé ; les itérations créatives ne comptent pas (écarter trois variations sur quatre, c'est le travail).
- **Barreaux d'environnement** *(EN : environment rungs)* — trois **classes définies par le régime de contrôle** (qui garde la main), jamais par un produit : **① chat nu** (l'humain tape tout, l'IA répond du texte, trace manuelle) · **② agentique de bureau** (l'IA agit sur fichiers/outils locaux, l'humain valide chaque geste) · **③ OS complet** (l'IA opère dans l'OS sous délégation *standing*, plusieurs pas sans validation geste-à-geste). Les bras de H4. Chaque barreau est une **classe peuplée d'un panel** (plusieurs produits, pas un). **Extensible par le critère seul** : un ④ barreau ne naît que d'un **régime de contrôle réellement nouveau** (ex. multi-agents sans humain dans la boucle), jamais d'un nouveau produit. **À ne pas confondre avec le *niveau d'utilisateur*** (débutant / intermédiaire / avancé) : axe **orthogonal**, corrélé (③ ~ utilisateur avancé) mais distinct. **On numérote l'environnement ; la personne est un tag.**
- **Terrain d'observation** : un projet réel où la méthode se pratique ; **jamais une preuve** (l'opérateur est l'auteur).
- **Science impliquée** : praticien-chercheur, N=1, déclaré ; une force si elle est dite, une faille si elle est implicite.

## Les livrables et les rôles (domiciles : [PIPELINE.md](PIPELINE.md) ; [GUICHET.md](GUICHET.md))

- **Mécanisme / test / kit** : les trois formes de livrable : **le mécanisme explique, le test contredit, le kit s'utilise**. Un mécanisme sans test n'est qu'un récit ; un kit sans mécanisme n'est qu'une recette.
- **Les trois rôles** : **utilisateur** (se sert du kit, dans ses limites) · **chercheur** (audite les mécanismes et les tests) · **constructeur** (dépose au guichet, propose, modifie). Une même personne peut tenir plusieurs rôles, jamais dans le même geste.
- **Les trois portes du guichet** : un dépôt entre par une seule porte : **problématique** (un problème constaté) · **proposition d'amélioration** (une solution suggérée) · **modification réalisée** (un changement déjà fait, soumis à validation). Même fiche, même traitement, fondateur compris.
- **Règle d'ancrage** : **« montre une occurrence, ou reste au banc »** : rien n'entre au pipeline sans au moins une occurrence datée et vérifiable ; l'idée sans trace attend au banc d'essai.

## Les mots réservés et le cycle des documents

- **Orchestration / orchestrer** *(mot **réservé**)* — **exclusivement** la question de recherche : « l'orchestration est-elle réalisable par un ensemble de doctrines et de calibrages, plutôt que par le système ? » (objet d'étude candidat, étage réflexion ; antériorité obligatoire : terme saturé côté industrie). **Ne s'emploie jamais pour la conduite d'un plan.**
- **Pilotage / piloter** : la conduite du plan : fronts, tempo, ordre de marche.
- **Gel / geler** *(EN : **freeze**)* : état d'un document dont le contenu ne se modifie plus par édition. Toute idée nouvelle entre par le pipeline, jamais par édition du gelé. *Ne pas confondre avec `cool` / `refroidir` (déplacer une **trace** vers le froid). Le gel verrouille l'écriture d'un document ; le refroidissement range l'attention d'une trace. Deux axes.*
- **Dégel versionné** *(EN : **versioned unfreeze**)* — une **procédure**, pas une réouverture : (1) archiver la version gelée **à l'octet près** (hash vérifié), (2) réviser un **périmètre borné et déclaré**, (3) **re-geler** avec incrément de version. *Registre Debian (freeze/unfreeze). Traduire par un simple « unfreeze » perdrait les trois obligations : un lecteur comprendrait « on rouvre », pas « on amende sous contrainte ».*

## L'économie de la trace · hot / cold (domicile : [REGISTRE-HYPOTHESES.md](REGISTRE-HYPOTHESES.md), H6)

*Concept « 1 + 1 = 2 » : chaque trace est soit sous les yeux, soit rangée, jamais supprimée.*

- <a id="hot"></a>**hot** *(FR : chaud)* : une trace **sous les yeux**, activement relue ou citée ; le seul état qui **coûte de l'attention**.
- <a id="cold"></a>**cold** *(FR : froid)* — une trace **rangée hors de la vue courante** : coût d'attention nul, mais **conservée et vérifiable**, récupérable à tout instant. Le froid n'est pas la suppression.
- <a id="cool"></a>**cool** *(FR : refroidir)* : faire passer une trace de *hot* à *cold* quand elle cesse d'être consultée (mouvement **graduel** et **réversible**). **≠ `geler`** (qui verrouille un document contre l'édition).
- <a id="warm"></a>**warm** *(FR : réchauffer)* : ramener une trace de *cold* à *hot* le jour où on en a besoin. Le **taux de réchauffement (warm-rate)** est l'**indicateur coût/valeur** de la trace : bas et stable → le refroidissement était juste ; élevé → on refroidit du vivant, la fenêtre est trop agressive.

## Les gardes

- **Crédit ≠ preuve** : l'adoption par un tiers établit la transférabilité, jamais la validité.
- **Récence ≠ qualité** : la ressemblance aux N derniers n'est pas un critère de traversée ; statut + périmètre + contraintes + CQM le sont.
- **Notes = signal** : les évaluations de la communauté déclenchent un examen ; elles ne sont jamais la métrique.
- **« Démontré » exige un chiffre** : plafond de vocabulaire : « preuve de concept » tant qu'aucune mesure n'existe.
- **Ce qui marche et ce qui ne marche pas, notés pareil, publiés pour partie** : on ne montre pas que les succès. Ce qui est publié est choisi, jamais selon ce qui flatte, et on dit comment on choisit : tout résultat négatif est consigné et listé, le récit n'est écrit que pour ce qui a changé une décision.

---

*ONDE AI R&D.*
