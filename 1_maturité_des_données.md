## Tableau de synthèse de maturité

Modèle: Échelle Gartner EIM/Gouvernance des données — 1=Conscient, 2=Réactif, 3=Proactif, 4=Maîtrisé, 5=Efficace. Remarque: le niveau 0 « Non conscient » existe chez Gartner mais n’est pas utilisé ici.

| Dimension | Niveau actuel (1-5) | Commentaires (forces/faiblesses) |
|---|---:|---|
| Gouvernance des données | 2 | Ownership et décisions fragmentés par département ; pas de modèle opératoire unifié ni de comité. |
| Qualité des données | 2 | La personnalisation dépend de données fiables, mais métadonnées obsolètes et événements incomplets réduisent la confiance. |
| Architecture des données | 3 | Lacs/BDs/cloud et temps réel solides ; principal manque: intégration inter-domaines. |
| Conformité (RGPD, CCPA, etc.) | 2 | Empreinte globale ; consentement, DSR, DPIA et processus de brèche 72h pas opérationnalisés partout. |
| Usage & Accessibilité | 3 | ML produit solide ; self‑service business limité, décisions ralenties. |
| Sécurité des données | 3 | Contrôles d’accès/sauvegarde/protection en place ; minimisation et PETs à renforcer. |
| Littératie data | 2 | Termes et docs hétérogènes ; compréhension des politiques inégale. |
| Intégration des données | 2 | Silos marketing/produit/contenu/ingénierie bloquent les analytics « parcours utilisateur ». |
| Analytics & BI | 3 | ML avancé ; BI d’entreprise fragmentée (datasets/KPIs) et définitions incohérentes. |

---

## Méthodologie d’évaluation (résumé)
- Collecte d’informations: ateliers, entretiens, sondages (en ligne) et revue d’artefacts (tableaux de bord, schémas, politiques).
- Cadre d’évaluation: échelle IMM 1–5 (alignée sur Gartner) couvrant capacités organisationnelles, pratiques de gestion des informations, et opérations de gouvernance.
- Facteurs de changement: appréciation de la capacité au changement (risques culturels, résistance) et, si l’usage d’outils collaboratifs est élevé, vérification de la « readiness » collaborative pour éviter la dérive en dépotoirs coûteux.
- Périmètre: cette évaluation est entreprise‑wide; des déclinaisons locales par fonction (R&D, finance, marketing) peuvent être produites avec les mêmes critères.

## Modèle organisationnel (contexte)
- Centralisé : une équipe, standards uniformes, risque d’engorgement.
- Intégré (embedded) : équipes data dans les domaines, décisions rapides, risque d’incohérence.
- CoE : standards centraux + correspondants métiers intégrés.

## Handoff
- Ce document capture les niveaux et observations.
- La Politique définit principes/rôles/contrôles.
- Le Plan décrit le déploiement, le pilote et les KPIs.

Note: le plan détaillé 60–90 jours et les KPIs sont dans le Plan de Mise en Œuvre.

## Déclaration de préparation au changement
Sur la base des constats, la préparation est moyenne: les fondamentaux existent mais doivent être harmonisés. Priorités: (1) gouvernance unifiée et ownership clairs, (2) contrôle de qualité sur les CDEs, (3) intégration inter‑domaines, (4) opérationnalisation homogène de la conformité.

## Prochaines étapes (ciblées)
- Programme d’amélioration focalisé par domaine et par CDE, aligné sur les objectifs EIM de l’entreprise.
- Suivi par métriques: index IMM (1–5) comme repère, scorecards de qualité et respect des SLAs conformité.

## Référence sigles
Glossaire des abréviations: voir `fr/abbrev_1.md`.
