# Étape 3 — Glossaire & Stack suggérée (Plan de mise en œuvre)

## Sigles (rappel)
- OKR — Objectives and Key Results : cadre d’objectifs trimestriels.
- CoE — Centre d’Excellence : comité central + relais par domaine.
- CDE — Élément de Donnée Critique : focus des contrôles/SLAs.
- RBAC/ABAC — Contrôles d’accès par rôles / par attributs.
- DPIA — Data Protection Impact Assessment : analyse d’impact des traitements.
- DSR — Data Subject Request : gestion des droits (SLA, preuves, propagation).
- SIEM — Security Information and Event Management : supervision sécurité.
- KMS — Key Management Service : clés et séparation des rôles.
- MTTR — Mean Time To Recovery/Resolve : délai moyen de résolution d’incidents.
- BAU — Business As Usual : régime d’exploitation continu.
- ROPA — Record of Processing Activities : registre des traitements.
- PETs — Privacy‑Enhancing Technologies : protections par défaut.
- SLA/SLO — Engagements et objectifs de service.
- GPC — Global Privacy Control : respect de l’opt‑out navigateur.
- KPI — Key Performance Indicator : mesure les résultats (qualité, conformité, délais).

## Stack suggérée (par usage)

### Catalogue & Gouvernance
- Collibra ou Alation — Catalogue d’entreprise, glossaire/domaines, workflows d’accès (RBAC/ABAC), gouvernance des contrats et intégration du linéage; point unique de vérité sur qui possède quoi et comment y accéder.
- Alternatives OSS: Apache Atlas, OpenMetadata — Couverture solide du linéage et des métadonnées, plus d’effort d’intégration/ops.

### Qualité des données
- Ataccama ONE (ou Informatica DQ / Talend DQ) — Profiling, règles (schéma/valeurs), détection d’anomalies, SLAs/scorecards, alerting et hooks de remédiation sur CDEs.
- Alternatives OSS: Great Expectations, Soda — Tests orientés code, intégration CI/ETL, idéal pour un MVP rapide.

### Privacy & Conformité
- OneTrust (ou TrustArc) — CMP/GPC, portail DSR, ROPA, modèles DPIA, journaux de preuves et rapports d’audit; opère les exigences RGPD/CCPA au quotidien.
- MVP interne: Portail DSR + tickets + tableurs ROPA — Point de départ économique pour un pilote, à industrialiser ensuite.

### Sécurité & Monitoring
- SIEM: Splunk (ou Elastic/Chronicle) — Ingestion et corrélation de journaux, détection/alertes, tableaux de bord; supporte drills brèche 72h et audits PCI‑DSS/SSI.
- KMS: Vormetric ou cloud‑native (AWS KMS / GCP KMS / Azure Key Vault) — Chiffrement au repos, rotation des clés, séparation des rôles et preuves d’audit.

### IAM / Accès
- SSO/IAM (Okta, Azure AD, Google Cloud IAM) — Fédération d’identité, MFA et gestion de groupes/claims pour piloter RBAC/ABAC depuis le catalogue.

### Pipelines & BI
- ETL/ELT & Orchestration (dbt, Airflow; cloud: Glue/ADF/Dataflow) — Transformations, promotion brut→curé→analytique et traçabilité.
- BI/Analytics (Looker, Power BI, Tableau) — Couche sémantique et tableaux de bord sur datasets gouvernés.

Notes d’intégration
- Le catalogue reste la « colonne vertébrale »: il relie IAM (accès), Qualité (règles/scorecards), Privacy (ROPA/consent), et BI (définitions/KPIs).
- Les contrôles qualité se branchent aux points de promotion des données; le linéage alimente DSR/DPIA et les post‑mortems.
