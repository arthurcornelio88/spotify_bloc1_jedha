# Spotify — Rapport bref : Maturité des données et défis de gouvernance

## Résumé exécutif
- Maturité mixte : cinq dimensions au Niveau 2 (Réactif) et quatre au Niveau 3 (Proactif).
- Plus grands écarts : gouvernance/ownership fragmentés, qualité sur CDEs inégale, intégration inter-domaines et opérations de conformité ; la littératie data est en retard.
- Risques : exposition réglementaire (RGPD/CCPA), perte de confiance, décisions plus lentes/time‑to‑market, plus de retouches et d’incidents.

Définition courte (DG)
- La gouvernance des données est la manière dont l’organisation décide, priorise et contrôle la qualité, l’usage, l’accès et la conformité de ses informations, pour créer de la valeur et réduire les risques.

Elevator speech
- « DG n’est pas un projet IT. C’est une façon commune d’agir pour traiter les données comme un actif: des rôles clairs, des règles simples, des métriques visibles. »

## Instantané de maturité
Modèle utilisé: échelle Gartner EIM/Gouvernance (niveaux 1–5 ; le niveau 0 « Non conscient » n’est pas utilisé ici).
- Niveau 2 (Réactif) : Gouvernance des données, Qualité des données, Conformité, Intégration des données, Littératie data
- Niveau 3 (Proactif) : Architecture des données, Usage & Accessibilité, Sécurité des données, Analytics & BI

Faits saillants du business case :
- Empreinte globale (180+ pays, 450M+ MAU) et diversité des données (écoutes, métadonnées de contenu, abonnements/facturation, engagement marketing) augmentent les enjeux de privacy, qualité et intégration.
- La personnalisation et la croissance dépendent de données exactes, fraîches et jointes, gouvernées de manière cohérente.

Portée et couches de gouvernance
- Portée: données clients, contenus, événements produits, finance, marketing; intensité variable selon couches (central/ régional/ local) avec standards communs.

## Défis de gouvernance et causes racines
1) Décisions/ownership fragmentés (Gouvernance — N2)
- Pas de comité unifié, RACI ou playbook ; départements en silos.
- Effet : standards incohérents, résolution lente, responsabilité floue.

2) Lacunes de qualité sur les CDEs (Qualité — N2)
- Métadonnées obsolètes, événements incomplets, peu de contrôles/SLAs automatisés.
- Linéage limité ; incidents détectés tard et corrigés ad hoc.
- Impact : recommandations moins fiables et analytics incertaines.

3) Freins à l’intégration inter-domaines (Intégration — N2)
- Silos Produit/Contenu/Ingénierie/Marketing ; identifiants incohérents.
- Peu de contrats de données standardisés et de règles de promotion (brut → curé → analytique).
- Impact : analytics de features retardées, activation marketing plus lente, rework.

4) Opérationnalisation de la conformité inégale (Conformité — N2)
- Journalisation du consentement, outillage DSR/SLA, workflows DPIA, exercices de brèche 72h, et ROPA non homogènes selon les régions.
- Impact : risque réglementaire accru ; posture réactive.

5) Self‑service limité et privacy‑by‑design perfectible (Usage/Sécurité — N3)
- Jeux de données curés et couche sémantique pas universels ; RBAC/ABAC et revues périodiques incomplètes.
- PETs (pseudonymisation/anonymisation) et minimisation pas par défaut.
- Impact : time‑to‑insight plus long et risques de surexposition.

6) Littératie data et langage partagé (Littératie — N2)
- Glossaire/documentation inégaux ; conscience des politiques variable.
- Impact : divergences de KPIs/définitions, collaboration inefficiente.

## Impacts business (pourquoi maintenant)
- Conformité : amendes (RGPD : jusqu’à 20 M€ ou 4% du CA mondial) + réputation.
- Produit : la personnalisation et les nouvelles features requièrent des données complètes, fraîches et jointes.
- Opérations : cycles analytics plus longs ; plus d’incidents et de rework ; difficulté d’échelle globale.

## Principaux risques
- Résistance au changement.
- Exigences/pratiques régionales divergentes.
- Tension vitesse vs contrôle.

## Handoff
- Ce rapport résume l’état et les défis.
- La Politique de Gouvernance définit principes, rôles et contrôles.
- Le Plan de Mise en Œuvre détaille le déploiement, le pilote et les KPIs.

## Conclusion
Base de référence pour la conception et l’exécution de la gouvernance. Voir la politique pour le « quoi » et le plan pour le « comment ».

Éléments clés du programme (aperçu)
- Organisation: comité de gouvernance + Owners/Stewards par domaine.
- Principes: transparence, qualité CDEs, minimisation, conformité, sécurité (principe du moindre privilège — accès minimal nécessaire), usage éthique.
- Facteurs de succès (CSFs): sponsorship exécutif, priorisation par valeur/CDEs, intégration au delivery (privacy‑by‑design), métriques simples, quick wins.
- Mesure: scorecards de qualité, SLAs DSR, revues d’accès, couverture DPIA, temps d’onboarding datasets.

Attendu de la direction
- Expression d’intérêt, accord de principe pour démarrer, retours sur l’alignement business, et validation des risques/impacts.
