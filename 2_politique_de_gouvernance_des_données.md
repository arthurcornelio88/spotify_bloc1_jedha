# Politique de Gouvernance des Données de Spotify

## 1. Objet & Périmètre
Établit la gestion des données pour assurer qualité, sécurité, confidentialité et conformité réglementaire sur 180+ pays. S’applique aux employés, prestataires, systèmes et tiers traitant des données Spotify.

## 2. Définitions (sélection)
- Donnée personnelle : information relative à une personne identifiée ou identifiable (RGPD art. 4).
- CDE (Élément de Donnée Critique) : champs de données essentiels aux processus/decisions (métadonnées contenu, abonnements/facturation, engagement marketing, inputs recommandations).
- DSR : Demande d’exercice de droits (accès, suppression, etc.).
- PETs : technologies de protection de la vie privée (anonymisation, pseudonymisation).

## 3. Principes
- Responsabilisation : ownership et stewardship clairs par domaine.
- Transparence : notices sur collecte/usage/partage/rétention.
- Sécurité : mesures techniques/organisationnelles ; principe du moindre privilège par défaut (accès minimal nécessaire).
- Qualité : exactitude, complétude, fraîcheur ; monitoring continu sur les CDEs.
- Conformité : base légale, consentement si requis, DSRs, brèche 72h (RGPD), CCPA.
- Minimisation : ne collecter/conserver que le nécessaire.
- Droits des utilisateurs : accès, rectification, suppression, opposition/opt‑out.
- Amélioration continue : revue périodique.
- Usage éthique : IA/ML responsable ; transparence et suivi des biais.

## 4. Énoncés de politique
### 4.1 Gouvernance & responsabilité
- Comité de gouvernance (DPO, CDO, Head of Engineering, Ingénierie Analytics, InfoSec, Juridique, Produit, Marketing, Contenu) pilote politique, priorités, risques.
- Chaque domaine a un Propriétaire et un Steward documentés dans le catalogue.

### 4.2 Qualité des données
- Identifier les CDEs par domaine (recommandations, métadonnées, abonnements, marketing).
- Contrôles : validation de schéma, complétude/fraîcheur, détection d’anomalies, alertes, SLAs de remédiation.
- Publier SLAs de qualité et linéage dans le catalogue.

### 4.3 Vie privée & conformité
- Opérationnaliser RGPD/CCPA : consentement, ROPA, DSR avec SLA, DPIA, brèche 72h.
- CCPA : opt‑out vente/partage ; non‑discrimination.
- Maintenir un socle global avec des « overlays » régionaux si applicable.

### 4.4 Sécurité
- Principe du moindre privilège, MFA, chiffrement en transit/au repos.
- Segmentation environnements/zones (brut/curé/analytique) ; audits d’accès.
- Données de paiement: alignement PCI‑DSS.

### 4.5 Accès & usage
- RBAC/ABAC via le catalogue ; demandes/approbations traçables.
- Jeux de données gouvernés et « consent‑aware » par défaut pour analytics/activation.

### 4.6 Cartographie de conformité (tableau basé sur la checklist)

| Domaine de conformité | Description de l’exigence | Statut de conformité (Oui/Non) | Notes / Plan d’action |
|---|---|---|---|
| RGPD – Principes de traitement des données | Garantir un traitement des données licite, loyal et transparent. | Non | Publier/mettre à jour les notices de confidentialité; cartographier les finalités et bases légales dans le ROPA; aligner les politiques internes. Responsable: Juridique/DPO. Délai: 60 j. |
| RGPD – Droits des personnes | Les utilisateurs doivent pouvoir accéder à, modifier ou supprimer leurs données sur demande. | Non | Déployer un portail DSR avec SLA (30 j), vérification d’identité et propagation aval (suppression/correction). Journalisation complète. Responsable: DPO/Ingénierie. Délai: 60 j. |
| RGPD – Gestion du consentement | Obtenir un consentement explicite et éclairé avant de traiter des données personnelles. | Non | Mettre en place une CMP; préférences par finalité; journalisation du consentement et preuves; synchronisation avec les outils marketing/produit. Responsable: Marketing/Ingénierie/DPO. Délai: 45 j. |
| RGPD – Notification de brèche | Notifier l’autorité de contrôle des violations de données dans les 72 heures. | Non | Établir un runbook incident; réaliser un drill 72 h trimestriel; modèles de notification régulateur/utilisateurs; registres d’incident. Responsable: InfoSec/DPO. Délai: 30 j. |
| RGPD – Délégué à la protection des données (DPO) | Désigner un Délégué à la Protection des Données (DPO) chargé du suivi de la conformité. | Non | Désigner formellement le DPO; définir mandat/indépendance; publier les coordonnées; processus d’escalade. Responsable: RH/Juridique. Délai: 14 j. |
| CCPA – Opt‑out vente/partage | Fournir un mécanisme clair d’opt‑out pour la vente/partage des données personnelles. | Non | Ajouter des liens « Ne pas vendre ni partager mes données »; respecter GPC; intégrer les préférences dans les systèmes; audit régulier. Responsable: Produit/Marketing/Juridique. Délai: 30 j. |
| CCPA – Accès et suppression | Permettre aux utilisateurs de demander l’accès à ou la suppression de leurs données. | Non | Étendre le workflow DSR aux exigences CCPA (accès/suppression); confirmer les identités; SLA conformes; preuves. Responsable: DPO/Ingénierie. Délai: 45 j. |
| CCPA – Non‑discrimination | Garantir l’absence de discrimination envers les utilisateurs exerçant leurs droits CCPA. | Non | Mettre à jour la politique de confidentialité; former les équipes; contrôles de non‑discrimination dans les offres/prix/services. Responsable: Juridique/RH/Produit. Délai: 30 j. |
| PCI‑DSS – Réseau et systèmes sécurisés | Garantir une infrastructure réseau sécurisée et une protection pare‑feu. | Oui | Maintenir la conformité: revues trimestrielles des règles pare‑feu, durcissement, scans; preuves d’audit conservées. Responsable: InfoSec. Délai: régime nominal (BAU). |
| PCI‑DSS – Protection des données titulaires de carte | Protéger les données de titulaires de carte stockées via chiffrement et stockage sécurisé. | Oui | Revue de la couverture de chiffrement; rotation des clés KMS; tests de restauration; validation des zones. Responsable: InfoSec/Ingénierie. Délai: régime nominal (BAU). |
| PCI‑DSS – Gestion des vulnérabilités | Maintenir des systèmes de protection contre les malwares et vulnérabilités. | Oui | Scans hebdomadaires, correctifs sous SLA; EDR/antimalware gérés; rapports de vulnérabilités suivis en comité. Responsable: InfoSec/IT. Délai: régime nominal (BAU). |
| PCI‑DSS – Contrôle d’accès renforcé | Limiter l’accès aux données de titulaires de carte au seul personnel autorisé. | Oui | Revues d’accès trimestrielles; séparation des tâches; JIT/JEA si possible; journaux d’accès. Responsable: InfoSec. Délai: régime nominal (BAU). |
| PCI‑DSS – Supervision et tests réguliers | Mettre en place des systèmes pour tester régulièrement les mesures et procédures de sécurité. | Oui | SIEM avec alerting; tests d’intrusion semestriels; exercices de réponse; preuves d’audit. Responsable: InfoSec. Délai: régime nominal (BAU). |
| PCI‑DSS – Politique de sécurité de l’information | Maintenir une politique de sécurité de l’information à jour pour tout le personnel. | Non | Mettre à jour la politique SSI; communiquer et former 100% du personnel; attestation annuelle; dépôt contrôlé. Responsable: InfoSec/RH. Délai: 30 j. |

### 4.7 Cycle de vie des données
- Collecte : liée à une finalité, documentée.
- Rétention : durée nécessaire et légale ; calendriers par domaine.
- Suppression : effacement automatisé et lié aux DSR ; propagation aval vérifiée.

### 4.8 Intégration & Catalogue
- Catalogue d’entreprise pour découverte, ownership, linéage, classifications et politiques.
- Standardiser les entités (user, session, contenu, campagne) et les contrats de données.

## 5. Rôles & Modèle de gouvernance (résumé)
- DPO : conformité, DSR, brèches, interlocuteur régulateur.
- CDO : exécution de la politique, qualité, culture data, valeur.
- Ingénierie : plateformes, catalogue/linéage, intégration, qualité, fiabilité.
- Juridique : interprétation, risques, revue.
- Produit : privacy‑by‑design ; DPIA si besoin.
- Propriétaires/Stewards : qualité, accès, rétention, entrées de catalogue.

## 6. Processus & contrôles (socle)
- DSR : journalisés, suivis avec SLAs ; vérif. d’identité ; propagation aval.
- DPIA : requis si risque élevé ; suivi des mitigations.
- Incident/brèche : triage/containment/évaluation ; notification ≤72h ; post‑mortem.
- Gestion de changement : revue/versions de schémas/contrats ; communication.
- Qualité : monitoring des CDEs ; incidents suivis jusqu’à remédiation.

## 7. Indicateurs & revues
- KPIs : conformité DSR, incidents qualité critiques, taux de revue d’accès, taux de DPIA, préparation exercices de brèche.
- Revues : mensuelles (comité), trimestrielles (exécutif) ; mise à jour annuelle ou changement réglementaire.

## 8. Application & exceptions
- Non‑conformité : mesures disciplinaires et impacts contractuels pour les fournisseurs.
- Exceptions : approbation DPO/CDO avec contrôles compensatoires et date d’expiration.

## 9. Contact
Questions: DPO ou Data Governance Office.

## 10. Référence sigles
Glossaire des abréviations: voir `fr/abbrev_2.md`.
