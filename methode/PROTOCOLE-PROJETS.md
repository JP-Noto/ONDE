# ONDE AI R&D · PROTOCOLE DES PROJETS v0.1

*Vue publique : instantané du 2026-08-02, non resynchronisé depuis : la cassette interne du
laboratoire fait foi, et elle a avancé (registre en révision 16 au 2026-08-11). Resynchronisation
complète : gate déclarée avant toute mise en public ([CHANGELOG](../CHANGELOG.md), 0.3.0).*

*Version publiée du protocole en vigueur (validé en juillet 2026). Complète [PIPELINE.md](PIPELINE.md) : le pipeline fait circuler des hypothèses et des mécanismes ; ce protocole gouverne les transitions de statut des PROJETS de production. Réutilise la checklist E-5 et le format gate-décision.*

---

## 1. Objet et périmètre

- S'applique aux projets de production du studio adossé au labo. Les objets du labo (kits, mécanismes) relèvent du pipeline et citent l'étage du pipeline dans leur STATUS.md, jamais le vocabulaire ci-dessous (un vocabulaire par nature d'objet, pas de double statut).
- Vocabulaire projet : `WIP → STAGING → LIVE → GELÉ → ARCHIVÉ`.
- Source de vérité : `STATUS.md` à la racine du projet. Vue : `_INDEX.md` généré à chaque modification d'un STATUS.md, daté en en-tête, jetable et régénérable.
- Règle d'hygiène héritée : si administrer une gate coûte plus que ce qu'elle garde, c'est la gate qu'on répare.

## 2. Gate P1 — WIP → STAGING (gate-décision, 3 vérifications)

1. **Mécanismes IA embarqués** : passés banc d'essai, OU explicitement déclarés hors-pipeline dans le STATUS.md. Aucun mécanisme ne se valide par contrebande via un projet.
2. **Conditions d'usage réel écrites** : qui utilise, sur quel périmètre, dans quelle fenêtre.
3. **Risque opérationnel borné** : impact maximal sur l'activité réelle défini ; tiers impliqués informés de ce qui change pour eux.

GO/NO-GO daté, signé, motivé en une phrase : consigné au journal.

## 3. Gate P2 — STAGING → LIVE (gate-décision, 2 vérifications)

1. **Checklist E-5 passée** (première exposition de tiers : cas exact qu'elle couvre).
2. **Chemin de retour défini** : que se passe-t-il si le LIVE échoue, qui décide du retrait, en combien de temps. Un projet sans rollback n'est pas prêt, il est pressé.

GO/NO-GO idem.

## 4. GELÉ et ARCHIVÉ, rien de neuf, tout hérité

- **GELÉ** : revue de boucle « suspendre », ou péremption — **N = 3 mois** sans activité (valeur unique, partagée avec le pipeline). Réactivation : GELÉ → statut antérieur par gate-décision.
- **ARCHIVÉ** : abandon acté, motif consigné. Comme au § 5 du pipeline, la sortie se documente : un projet qui meurt en silence n'enseigne rien.

## 5. Annexe A — gabarit STATUS.md (projet de production)

    # STATUS
    statut: WIP | STAGING | LIVE | GELÉ | ARCHIVÉ
    depuis: AAAA-MM-JJ
    gate: P1 | P2 | hors gate (initialisation)
    hors-pipeline: [mécanismes embarqués non passés au banc, ou "aucun"]
    registre: [référence au registre des hypothèses si applicable]
    note: [une ligne max : pourquoi ce statut maintenant]

## 6. Annexe B · gabarit STATUS.md (objet de labo)

    # STATUS
    etage: hypothèse | banc-essai | terrain-chercheur | auditable |
           utilisateurs-réels | répliqué | doctrine | réfuté | suspendu
    depuis: AAAA-MM-JJ
    gate: [dernière gate franchie, réf. fiche d'expérience si gate-mesure]
    registre: [entrée du registre des hypothèses]
    note: [une ligne max]

---

*Six lignes par STATUS.md, pas plus. Tout ce qui dépasse appartient au projet, pas au marqueur.*
