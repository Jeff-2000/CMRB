<!-- DOCUMENT GÉNÉRÉ : ne pas modifier directement. Empreinte des sources : a2e037bc28a3c8b7c0b1ab2c8ef7040780f8aacda22381c8d328c4bb9551a9f3 -->

# CMRB — Dictionnaire de données de la baseline

## 1. Règles de lecture

Les 29 concepts et 76 attributs sont repris du dictionnaire canonique. Les contraintes de publication, d’habilitation et de conservation proviennent des décisions de baseline.

Les exemples sont fictifs. Les noms physiques de colonnes pourront être affinés en conception détaillée sans modifier le sens métier, les relations ni les critères de recette.

Les types, clés, longueurs, métadonnées et décisions d’audit restent dans le [dictionnaire technique](../data/DATA_DICTIONARY.md). Les décisions sont consultables dans le [document des workflows](CMRB_WORKFLOWS_FOR_VALIDATION.md#q-001).

## 2. Concepts et champs

### ENT-001 — Utilisateur

**Définition :** Compte permettant de rattacher une identité aux rôles utilisés pour accéder aux fonctions CMRB.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Habilitations; pas d’attribution de permission implicite

**Sources :** §6.1; EF-SEC-001

**Workflows :** WF-032, WF-033

**Décisions de baseline :** Q-002, Q-024, Q-025, Q-026, Q-031

#### ENT-001-A01 — Rôle attribué

| Élément de baseline | Définition |
| --- | --- |
| Définition | Une ou plusieurs références de rôle actives, uniques par compte, parmi ACCUEIL, MEDECIN, PARAMEDICAL, COMPTABILITE, RH, STOCK, DIRECTION, ADMIN_HABILITATIONS et PATIENT |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Une ou plusieurs références de rôle actives, uniques par compte, parmi ACCUEIL, MEDECIN, PARAMEDICAL, COMPTABILITE, RH, STOCK, DIRECTION, ADMIN_HABILITATIONS et PATIENT |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-024, Q-025, Q-026, Q-031; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-SEC-001 |
| Utilisation | WF-032, WF-033 |

### ENT-002 — Rôle

**Définition :** Ensemble de droits associé à une catégorie d’utilisateurs ; la liste et le cumul restent arrêté pour la baseline.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Habilitations; pas d’attribution de permission implicite

**Sources :** §6.1; EF-SEC-003

**Workflows :** WF-032, WF-033

**Décisions de baseline :** Q-002, Q-024, Q-025, Q-026, Q-031

#### ENT-002-A01 — Nom du rôle

| Élément de baseline | Définition |
| --- | --- |
| Définition | Code unique parmi ACCUEIL, MEDECIN, PARAMEDICAL, COMPTABILITE, RH, STOCK, DIRECTION, ADMIN_HABILITATIONS et PATIENT |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Code unique parmi ACCUEIL, MEDECIN, PARAMEDICAL, COMPTABILITE, RH, STOCK, DIRECTION, ADMIN_HABILITATIONS et PATIENT |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-024, Q-025, Q-026, Q-031; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-SEC-003 |
| Utilisation | WF-032, WF-033 |

### ENT-003 — Employé

**Définition :** Personne appartenant au personnel du centre, dont les informations servent notamment à la paie.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** RH; pas d’attribution de permission implicite

**Sources :** §6.1; EF-RH-001

**Workflows :** WF-027, WF-028

**Décisions de baseline :** Q-014, Q-022, Q-025, Q-026, Q-034

#### ENT-003-A01 — Identification du salarié

| Élément de baseline | Définition |
| --- | --- |
| Définition | Matricule unique, nom, prénoms, fonction, contact professionnel, date de début et statut ACTIF/INACTIF |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Matricule unique, nom, prénoms, fonction, contact professionnel, date de début et statut ACTIF/INACTIF |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-022, Q-025, Q-026, Q-034; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-RH-001 |
| Utilisation | WF-027, WF-028 |

### ENT-004 — Patient

**Définition :** Personne bénéficiaire des prestations du centre, identifiée pour ses dossiers et son parcours.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Accueil; pas d’attribution de permission implicite

**Sources :** §6.1; EF-PAT-007

**Workflows :** WF-001, WF-002, WF-003, WF-004, WF-005, WF-009, WF-010, WF-011, WF-012, WF-013, WF-014, WF-015, WF-016, WF-017, WF-018, WF-023, WF-024, WF-025, WF-032

**Décisions de baseline :** Q-002, Q-003, Q-004, Q-005, Q-006, Q-007, Q-008, Q-009, Q-011, Q-012, Q-013, Q-015, Q-016, Q-017, Q-018, Q-020, Q-023, Q-024, Q-025, Q-026, Q-027, Q-028, Q-029, Q-035

#### ENT-004-A01 — Identification du patient

| Élément de baseline | Définition |
| --- | --- |
| Définition | Nom, prénoms, date de naissance, sexe administratif, téléphone ou e-mail et canal de contact; identifiant interne UUID v7 unique selon Q-011 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Nom, prénoms, date de naissance, sexe administratif, téléphone ou e-mail et canal de contact; identifiant interne UUID v7 unique selon Q-011 |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-004, Q-005, Q-006, Q-007, Q-008, Q-009, Q-011, Q-012, Q-013, Q-015, Q-016, Q-017, Q-018, Q-020, Q-023, Q-024, Q-025, Q-026, Q-027, Q-028, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-PAT-007 |
| Utilisation | WF-001, WF-002, WF-003, WF-004, WF-005, WF-009, WF-010, WF-011, WF-012, WF-013, WF-014, WF-015, WF-016, WF-017, WF-018, WF-023, WF-024, WF-025, WF-032 |

### ENT-005 — Dossier administratif

**Définition :** Informations administratives associées au patient, distinctes du contenu clinique.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Accueil; pas d’attribution de permission implicite

**Sources :** §1.3; §6.1; EF-PAT-005

**Workflows :** WF-001, WF-002, WF-003, WF-004, WF-023

**Décisions de baseline :** Q-003, Q-005, Q-006, Q-011, Q-012, Q-024, Q-025, Q-028

#### ENT-005-A01 — Patient concerné

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire et unique vers le patient; un seul dossier administratif actif par patient |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire et unique vers le patient; un seul dossier administratif actif par patient |
| Règles et décisions applicables | Règles citées et décisions Q-003, Q-005, Q-006, Q-011, Q-012, Q-024, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §1.3; §6.1; EF-PAT-005 |
| Utilisation | WF-001, WF-002, WF-003, WF-004, WF-023 |

### ENT-006 — Dossier médical

**Définition :** Informations médicales du patient, dont motif, diagnostic et observations, soumises à des accès spécifiques.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Médical; pas d’attribution de permission implicite

**Sources :** §1.3; §6.1; EF-DM-004

**Workflows :** WF-004, WF-009, WF-010, WF-011, WF-023

**Décisions de baseline :** Q-002, Q-003, Q-005, Q-006, Q-011, Q-012, Q-016, Q-025, Q-028

#### ENT-006-A01 — Patient concerné

| Élément de baseline | Définition |
| --- | --- |
| Définition | §6.2 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | §6.2 |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-005, Q-006, Q-011, Q-012, Q-016, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §1.3; §6.1; EF-DM-004 |
| Utilisation | WF-004, WF-009, WF-010, WF-011, WF-023 |

#### ENT-006-A02 — Motif médical

| Élément de baseline | Définition |
| --- | --- |
| Définition | Motif clinique en texte UTF-8, 2 000 caractères maximum, obligatoire avant validation de la consultation |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Motif clinique en texte UTF-8, 2 000 caractères maximum, obligatoire avant validation de la consultation |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-005, Q-006, Q-011, Q-012, Q-016, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §1.3; §6.1; EF-DM-004 |
| Utilisation | WF-004, WF-009, WF-010, WF-011, WF-023 |

#### ENT-006-A03 — Diagnostic

| Élément de baseline | Définition |
| --- | --- |
| Définition | Diagnostic saisi uniquement par le médecin, texte UTF-8 de 4 000 caractères maximum; code de nomenclature facultatif et versionné |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Diagnostic saisi uniquement par le médecin, texte UTF-8 de 4 000 caractères maximum; code de nomenclature facultatif et versionné |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-005, Q-006, Q-011, Q-012, Q-016, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §1.3; §6.1; EF-DM-004 |
| Utilisation | WF-004, WF-009, WF-010, WF-011, WF-023 |

#### ENT-006-A04 — Observations cliniques

| Élément de baseline | Définition |
| --- | --- |
| Définition | Observations de soins par le paramédical; diagnostic, prescription et conclusion réservés au médecin selon Q-002 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Observations de soins par le paramédical; diagnostic, prescription et conclusion réservés au médecin selon Q-002 |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-005, Q-006, Q-011, Q-012, Q-016, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §1.3; §6.1; EF-DM-004 |
| Utilisation | WF-004, WF-009, WF-010, WF-011, WF-023 |

### ENT-007 — Rendez-vous

**Définition :** Réservation d’un créneau pour un patient, avec confirmation et annulation selon règles Q-009, Q-020, Q-024 et Q-035.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Accueil; pas d’attribution de permission implicite

**Sources :** §6.1; EF-RDV-001

**Workflows :** WF-005, WF-006, WF-007, WF-008

**Décisions de baseline :** Q-013, Q-014, Q-015, Q-025, Q-026, Q-027

#### ENT-007-A01 — Patient concerné

| Élément de baseline | Définition |
| --- | --- |
| Définition | §6.2 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | §6.2 |
| Règles et décisions applicables | Règles citées et décisions Q-013, Q-014, Q-015, Q-025, Q-026, Q-027; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-RDV-001 |
| Utilisation | WF-005, WF-006, WF-007, WF-008 |

#### ENT-007-A02 — Date et heure prévues

| Élément de baseline | Définition |
| --- | --- |
| Définition | Horodatage ISO 8601 en Africa/Abidjan; borne d'annulation autonome incluse jusqu'à début moins 24 heures selon Q-013 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Horodatage ISO 8601 en Africa/Abidjan; borne d'annulation autonome incluse jusqu'à début moins 24 heures selon Q-013 |
| Règles et décisions applicables | Règles citées et décisions Q-013, Q-014, Q-015, Q-025, Q-026, Q-027; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-RDV-001 |
| Utilisation | WF-005, WF-006, WF-007, WF-008 |

#### ENT-007-A03 — Situation du rendez-vous

| Élément de baseline | Définition |
| --- | --- |
| Définition | DEMANDE, À_CONFIRMER, CONFIRMÉ, ARRIVÉ, EN_COURS, TERMINÉ, ANNULÉ_PATIENT, ANNULÉ_CMRB, ABSENT ou REPORTÉ selon Q-015 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | DEMANDE, À_CONFIRMER, CONFIRMÉ, ARRIVÉ, EN_COURS, TERMINÉ, ANNULÉ_PATIENT, ANNULÉ_CMRB, ABSENT ou REPORTÉ selon Q-015 |
| Règles et décisions applicables | Règles citées et décisions Q-013, Q-014, Q-015, Q-025, Q-026, Q-027; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-RDV-001 |
| Utilisation | WF-005, WF-006, WF-007, WF-008 |

### ENT-008 — Prestation

**Définition :** Acte ou service réalisé pour un patient et pouvant alimenter son dossier et sa facturation.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Médical / facturation; pas d’attribution de permission implicite

**Sources :** §6.1; EF-SRV-TRA-001

**Workflows :** WF-009, WF-010, WF-011, WF-012, WF-013, WF-014, WF-015, WF-016, WF-018, WF-026

**Décisions de baseline :** Q-002, Q-003, Q-007, Q-008, Q-009, Q-011, Q-016, Q-017, Q-018, Q-020, Q-021, Q-023, Q-024, Q-025, Q-027, Q-028, Q-029, Q-035

#### ENT-008-A01 — Bénéficiaire

| Élément de baseline | Définition |
| --- | --- |
| Définition | §6.2 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | §6.2 |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-007, Q-008, Q-009, Q-011, Q-016, Q-017, Q-018, Q-020, Q-021, Q-023, Q-024, Q-025, Q-027, Q-028, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-SRV-TRA-001 |
| Utilisation | WF-009, WF-010, WF-011, WF-012, WF-013, WF-014, WF-015, WF-016, WF-018, WF-026 |

#### ENT-008-A02 — Nature de prestation

| Élément de baseline | Définition |
| --- | --- |
| Définition | CONSULTATION, HOSPITALISATION, OBSERVATION, IMAGERIE, LABORATOIRE ou PHARMACIE; ajout par référentiel versionné |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | CONSULTATION, HOSPITALISATION, OBSERVATION, IMAGERIE, LABORATOIRE ou PHARMACIE; ajout par référentiel versionné |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-007, Q-008, Q-009, Q-011, Q-016, Q-017, Q-018, Q-020, Q-021, Q-023, Q-024, Q-025, Q-027, Q-028, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-SRV-TRA-001 |
| Utilisation | WF-009, WF-010, WF-011, WF-012, WF-013, WF-014, WF-015, WF-016, WF-018, WF-026 |

### ENT-009 — Facture

**Définition :** Document regroupant les éléments facturés à un payeur ; montant et archivage sont distincts du paiement.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Comptabilité; pas d’attribution de permission implicite

**Sources :** §6.1; EF-FAC-001

**Workflows :** WF-016, WF-017, WF-018, WF-019, WF-020, WF-021, WF-022, WF-026

**Décisions de baseline :** Q-007, Q-008, Q-009, Q-010, Q-016, Q-019, Q-020, Q-021, Q-024, Q-027, Q-029, Q-035

#### ENT-009-A01 — Payeur de facture

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers un patient ou un organisme payeur, avec type de payeur explicite et intégrité contrôlée |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers un patient ou un organisme payeur, avec type de payeur explicite et intégrité contrôlée |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-010, Q-016, Q-019, Q-020, Q-021, Q-024, Q-027, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-FAC-001 |
| Utilisation | WF-016, WF-017, WF-018, WF-019, WF-020, WF-021, WF-022, WF-026 |

#### ENT-009-A02 — Total facturé

| Élément de baseline | Définition |
| --- | --- |
| Définition | Montant entier XOF égal à la somme des lignes, après remises et taxes configurées; arrondi demi-supérieur selon Q-009/Q-035 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Montant entier XOF égal à la somme des lignes, après remises et taxes configurées; arrondi demi-supérieur selon Q-009/Q-035 |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-010, Q-016, Q-019, Q-020, Q-021, Q-024, Q-027, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-FAC-001 |
| Utilisation | WF-016, WF-017, WF-018, WF-019, WF-020, WF-021, WF-022, WF-026 |

#### ENT-009-A03 — Situation d’archivage

| Élément de baseline | Définition |
| --- | --- |
| Définition | État ARCHIVÉ en lecture seule après paiement complet; solde conservé séparément selon Q-020 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | État ARCHIVÉ en lecture seule après paiement complet; solde conservé séparément selon Q-020 |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-010, Q-016, Q-019, Q-020, Q-021, Q-024, Q-027, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-FAC-001 |
| Utilisation | WF-016, WF-017, WF-018, WF-019, WF-020, WF-021, WF-022, WF-026 |

#### ENT-009-A04 — Devise du montant facturé

| Élément de baseline | Définition |
| --- | --- |
| Définition | Devise obligatoire XOF, zéro décimale, selon Q-035 |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Devise obligatoire XOF, zéro décimale, selon Q-035 |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-010, Q-016, Q-019, Q-020, Q-021, Q-024, Q-027, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-FAC-001 |
| Utilisation | WF-016, WF-017, WF-018, WF-019, WF-020, WF-021, WF-022, WF-026 |

### ENT-010 — Paiement

**Définition :** Règlement reçu à enregistrer et à rattacher aux dettes concernées selon règles défini par la baseline.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Comptabilité; pas d’attribution de permission implicite

**Sources :** §6.1; EF-PAI-003

**Workflows :** WF-019, WF-020, WF-021, WF-026

**Décisions de baseline :** Q-008, Q-009, Q-019, Q-020, Q-021, Q-024, Q-029, Q-035

#### ENT-010-A01 — Montant reçu

| Élément de baseline | Définition |
| --- | --- |
| Définition | Entier XOF strictement positif; un trop-perçu devient crédit ou remboursement tracé |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Entier XOF strictement positif; un trop-perçu devient crédit ou remboursement tracé |
| Règles et décisions applicables | Règles citées et décisions Q-008, Q-009, Q-019, Q-020, Q-021, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-PAI-003 |
| Utilisation | WF-019, WF-020, WF-021, WF-026 |

#### ENT-010-A02 — Moyen de règlement

| Élément de baseline | Définition |
| --- | --- |
| Définition | ESPECES, VIREMENT ou MOBILE_MONEY en V1 selon Q-019 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | ESPECES, VIREMENT ou MOBILE_MONEY en V1 selon Q-019 |
| Règles et décisions applicables | Règles citées et décisions Q-008, Q-009, Q-019, Q-020, Q-021, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-PAI-003 |
| Utilisation | WF-019, WF-020, WF-021, WF-026 |

#### ENT-010-A03 — Auteur du règlement

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers le patient ou l'organisme qui effectue le règlement |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers le patient ou l'organisme qui effectue le règlement |
| Règles et décisions applicables | Règles citées et décisions Q-008, Q-009, Q-019, Q-020, Q-021, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-PAI-003 |
| Utilisation | WF-019, WF-020, WF-021, WF-026 |

#### ENT-010-A04 — Devise du montant reçu

| Élément de baseline | Définition |
| --- | --- |
| Définition | XOF obligatoire; toutes les imputations d'un paiement utilisent la même devise |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | XOF obligatoire; toutes les imputations d'un paiement utilisent la même devise |
| Règles et décisions applicables | Règles citées et décisions Q-008, Q-009, Q-019, Q-020, Q-021, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-PAI-003 |
| Utilisation | WF-019, WF-020, WF-021, WF-026 |

### ENT-011 — Organisme payeur

**Définition :** Assureur ou mutuelle intervenant dans la couverture et le règlement des prestations.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Comptabilité; pas d’attribution de permission implicite

**Sources :** §6.1; EF-FAC-006

**Workflows :** WF-018, WF-019, WF-020, WF-026

**Décisions de baseline :** Q-007, Q-008, Q-009, Q-019, Q-021, Q-024, Q-029, Q-035

#### ENT-011-A01 — Organisme concerné

| Élément de baseline | Définition |
| --- | --- |
| Définition | Raison ou nom d'organisme obligatoire et unique dans sa catégorie après normalisation |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Raison ou nom d'organisme obligatoire et unique dans sa catégorie après normalisation |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-019, Q-021, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-FAC-006 |
| Utilisation | WF-018, WF-019, WF-020, WF-026 |

#### ENT-011-A02 — Assurance ou mutuelle

| Élément de baseline | Définition |
| --- | --- |
| Définition | ASSURANCE, MUTUELLE ou AUTRE selon Q-008 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | ASSURANCE, MUTUELLE ou AUTRE selon Q-008 |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-019, Q-021, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-FAC-006 |
| Utilisation | WF-018, WF-019, WF-020, WF-026 |

### ENT-012 — Produit de stock

**Définition :** Article de pharmacie ou de bureautique suivi dans le stock du centre.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Stock; pas d’attribution de permission implicite

**Sources :** §6.1; EF-STK-001

**Workflows :** WF-015, WF-029, WF-030, WF-031

**Décisions de baseline :** Q-018, Q-023

#### ENT-012-A01 — Produit concerné

| Élément de baseline | Définition |
| --- | --- |
| Définition | Désignation obligatoire, unique par catégorie et unité après normalisation |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Désignation obligatoire, unique par catégorie et unité après normalisation |
| Règles et décisions applicables | Règles citées et décisions Q-018, Q-023; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-STK-001 |
| Utilisation | WF-015, WF-029, WF-030, WF-031 |

#### ENT-012-A02 — Famille de stock

| Élément de baseline | Définition |
| --- | --- |
| Définition | Pharmacie ou bureautique |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Pharmacie ou bureautique |
| Règles et décisions applicables | Règles citées et décisions Q-018, Q-023; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-STK-001 |
| Utilisation | WF-015, WF-029, WF-030, WF-031 |

#### ENT-012-A03 — Seuil renseigné

| Élément de baseline | Définition |
| --- | --- |
| Définition | Valeur non négative dans l'unité du produit et définie par emplacement; alerte lorsque disponible ≤ seuil |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Valeur non négative dans l'unité du produit et définie par emplacement; alerte lorsque disponible ≤ seuil |
| Règles et décisions applicables | Règles citées et décisions Q-018, Q-023; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-STK-001 |
| Utilisation | WF-015, WF-029, WF-030, WF-031 |

#### ENT-012-A04 — Quantité disponible

| Élément de baseline | Définition |
| --- | --- |
| Définition | Quantité disponible calculée comme somme des mouvements validés; lecture seule et jamais négative |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Quantité disponible calculée comme somme des mouvements validés; lecture seule et jamais négative |
| Règles et décisions applicables | Règles citées et décisions Q-018, Q-023; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-STK-001 |
| Utilisation | WF-015, WF-029, WF-030, WF-031 |

### ENT-013 — Mouvement de stock

**Définition :** Entrée ou sortie d’une quantité de produit, utilisée pour suivre le stock disponible.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Stock; pas d’attribution de permission implicite

**Sources :** §6.1; EF-STK-003

**Workflows :** WF-015, WF-030, WF-031

**Décisions de baseline :** Q-018, Q-023

#### ENT-013-A01 — Produit déplacé

| Élément de baseline | Définition |
| --- | --- |
| Définition | §6.2 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | §6.2 |
| Règles et décisions applicables | Règles citées et décisions Q-018, Q-023; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-STK-003 |
| Utilisation | WF-015, WF-030, WF-031 |

#### ENT-013-A02 — Entrée ou sortie

| Élément de baseline | Définition |
| --- | --- |
| Définition | ENTREE, SORTIE, RETOUR ou AJUSTEMENT; une correction crée un mouvement inverse, jamais une suppression |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | ENTREE, SORTIE, RETOUR ou AJUSTEMENT; une correction crée un mouvement inverse, jamais une suppression |
| Règles et décisions applicables | Règles citées et décisions Q-018, Q-023; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-STK-003 |
| Utilisation | WF-015, WF-030, WF-031 |

#### ENT-013-A03 — Quantité déplacée

| Élément de baseline | Définition |
| --- | --- |
| Définition | Quantité strictement positive dans l'unité du produit; le sens porte le signe comptable |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Quantité strictement positive dans l'unité du produit; le sens porte le signe comptable |
| Règles et décisions applicables | Règles citées et décisions Q-018, Q-023; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-STK-003 |
| Utilisation | WF-015, WF-030, WF-031 |

### ENT-014 — Bulletin de paie

**Définition :** Document de paie d’un employé pour une période ; contenu et calculs restent défini par la baseline.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** RH; pas d’attribution de permission implicite

**Sources :** §6.1; EF-RH-003

**Workflows :** WF-028

**Décisions de baseline :** Q-014, Q-022, Q-026, Q-034

#### ENT-014-A01 — Salarié bénéficiaire

| Élément de baseline | Définition |
| --- | --- |
| Définition | Un bulletin par salarié et par mois civil |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Un bulletin par salarié et par mois civil |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-022, Q-026, Q-034; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-RH-003 |
| Utilisation | WF-028 |

#### ENT-014-A02 — Période de paie

| Élément de baseline | Définition |
| --- | --- |
| Définition | Mois civil au format YYYY-MM; une seule version validée par employé et période |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Mois civil au format YYYY-MM; une seule version validée par employé et période |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-022, Q-026, Q-034; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-RH-003 |
| Utilisation | WF-028 |

#### ENT-014-A03 — Éléments du bulletin

| Élément de baseline | Définition |
| --- | --- |
| Définition | Montant XOF saisi par RH, contrôlé par la comptabilité et approuvé par la direction selon Q-022; aucun calcul légal automatique |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Montant XOF saisi par RH, contrôlé par la comptabilité et approuvé par la direction selon Q-022; aucun calcul légal automatique |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-022, Q-026, Q-034; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.1; EF-RH-003 |
| Utilisation | WF-028 |

### ENT-015 — Constantes

**Définition :** Mesures cliniques citées avant consultation : tension, température et glycémie ; unités et validations défini par la baseline.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Médical / paramédical; pas d’attribution de permission implicite

**Sources :** ADD-001; EF-DM-004

**Workflows :** WF-009, WF-010

**Décisions de baseline :** Q-002, Q-011, Q-016, Q-028

#### ENT-015-A01 — Tension relevée

| Élément de baseline | Définition |
| --- | --- |
| Définition | Systolique et diastolique entières en mmHg; plages techniques 30–300 et 20–200, systolique > diastolique; valeur hors plage arrêté pour la baseline sans bloquer l'urgence |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Systolique et diastolique entières en mmHg; plages techniques 30–300 et 20–200, systolique > diastolique; valeur hors plage arrêté pour la baseline sans bloquer l'urgence |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-011, Q-016, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-001; EF-DM-004 |
| Utilisation | WF-009, WF-010 |

#### ENT-015-A02 — Température relevée

| Élément de baseline | Définition |
| --- | --- |
| Définition | Température décimale en °C, plage technique 25,0–45,0; valeur hors plage arrêté pour la baseline sans diagnostic automatique |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Température décimale en °C, plage technique 25,0–45,0; valeur hors plage arrêté pour la baseline sans diagnostic automatique |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-011, Q-016, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-001; EF-DM-004 |
| Utilisation | WF-009, WF-010 |

#### ENT-015-A03 — Glycémie relevée

| Élément de baseline | Définition |
| --- | --- |
| Définition | Glycémie décimale en mg/dL, plage technique 10–1 000 et contexte A_JEUN, POSTPRANDIAL ou ALEATOIRE |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Glycémie décimale en mg/dL, plage technique 10–1 000 et contexte A_JEUN, POSTPRANDIAL ou ALEATOIRE |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-011, Q-016, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-001; EF-DM-004 |
| Utilisation | WF-009, WF-010 |

#### ENT-015-A04 — Prestation clinique portant la mesure

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers l'épisode ou la prestation et vers le patient; auteur et horodatage serveur obligatoires |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers l'épisode ou la prestation et vers le patient; auteur et horodatage serveur obligatoires |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-011, Q-016, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-001; EF-DM-004 |
| Utilisation | WF-009, WF-010 |

### ENT-016 — Séjour / observation

**Définition :** Hospitalisation ou observation d’un patient, reliée aux prestations et à la facturation du séjour.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Médical; pas d’attribution de permission implicite

**Sources :** EF-SRV-CONS-003; ADD-008

**Workflows :** WF-012, WF-017

**Décisions de baseline :** Q-002, Q-009, Q-016, Q-020, Q-024, Q-035

#### ENT-016-A01 — Patient admis

| Élément de baseline | Définition |
| --- | --- |
| Définition | Bénéficiaire du séjour |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Bénéficiaire du séjour |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-009, Q-016, Q-020, Q-024, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-SRV-CONS-003; ADD-008 |
| Utilisation | WF-012, WF-017 |

#### ENT-016-A02 — Hospitalisation ou observation

| Élément de baseline | Définition |
| --- | --- |
| Définition | OBSERVATION ou HOSPITALISATION; seule l'hospitalisation exige une affectation de lit |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | OBSERVATION ou HOSPITALISATION; seule l'hospitalisation exige une affectation de lit |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-009, Q-016, Q-020, Q-024, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-SRV-CONS-003; ADD-008 |
| Utilisation | WF-012, WF-017 |

#### ENT-016-A03 — Durée facturable

| Élément de baseline | Définition |
| --- | --- |
| Définition | Hospitalisation facturée par nuit civile en Africa/Abidjan : max(1, date_sortie − date_admission); observation suivie en durée horaire sans lit permanent |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Hospitalisation facturée par nuit civile en Africa/Abidjan : max(1, date_sortie − date_admission); observation suivie en durée horaire sans lit permanent |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-009, Q-016, Q-020, Q-024, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-SRV-CONS-003; ADD-008 |
| Utilisation | WF-012, WF-017 |

#### ENT-016-A04 — Chambre du séjour

| Élément de baseline | Définition |
| --- | --- |
| Définition | Affectation obligatoire pour hospitalisation; chaque transfert clôt l'affectation précédente et en crée une nouvelle sans chevauchement |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Affectation obligatoire pour hospitalisation; chaque transfert clôt l'affectation précédente et en crée une nouvelle sans chevauchement |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-009, Q-016, Q-020, Q-024, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-SRV-CONS-003; ADD-008 |
| Utilisation | WF-012, WF-017 |

### ENT-017 — Chambre

**Définition :** Chambre individuelle ou double mentionnée pour un séjour ; aucun modèle de lits n’est déduit.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Séjour; pas d’attribution de permission implicite

**Sources :** ADD-008

**Workflows :** WF-012, WF-017

**Décisions de baseline :** Q-002, Q-009, Q-016, Q-020, Q-024, Q-035

#### ENT-017-A01 — Individuelle ou double

| Élément de baseline | Définition |
| --- | --- |
| Définition | INDIVIDUELLE ou DOUBLE; lit identifié de manière unique dans la chambre et non affectable à deux séjours simultanés |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | INDIVIDUELLE ou DOUBLE; lit identifié de manière unique dans la chambre et non affectable à deux séjours simultanés |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-009, Q-016, Q-020, Q-024, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-008 |
| Utilisation | WF-012, WF-017 |

### ENT-018 — Résultat / compte rendu

**Définition :** Contenu associé à un examen de laboratoire ou d’imagerie ; saisie, validation et diffusion restent distinctes.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Médical; pas d’attribution de permission implicite

**Sources :** EF-SRV-LAB-002 EF-SRV-IMG-002 ADD-013

**Workflows :** WF-011, WF-013, WF-014, WF-023

**Décisions de baseline :** Q-002, Q-003, Q-005, Q-006, Q-017, Q-025, Q-027, Q-028

#### ENT-018-A01 — Examen concerné

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers la prestation prescrite ou demandée et le patient correspondant |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers la prestation prescrite ou demandée et le patient correspondant |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-005, Q-006, Q-017, Q-025, Q-027, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-SRV-LAB-002 EF-SRV-IMG-002 ADD-013 |
| Utilisation | WF-011, WF-013, WF-014, WF-023 |

#### ENT-018-A02 — Résultat ou compte rendu

| Élément de baseline | Définition |
| --- | --- |
| Définition | Contenu texte structuré et pièces jointes; états BROUILLON, VALIDÉ, PUBLIÉ ou CORRIGÉ_PAR_ADDENDUM selon Q-017 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Contenu texte structuré et pièces jointes; états BROUILLON, VALIDÉ, PUBLIÉ ou CORRIGÉ_PAR_ADDENDUM selon Q-017 |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-005, Q-006, Q-017, Q-025, Q-027, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-SRV-LAB-002 EF-SRV-IMG-002 ADD-013 |
| Utilisation | WF-011, WF-013, WF-014, WF-023 |

### ENT-019 — Ordonnance

**Définition :** Prescription consultable dans le parcours patient ; sa visibilité de 15 jours ne fixe pas sa conservation.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Médical; pas d’attribution de permission implicite

**Sources :** ADD-002; EF-DM-004

**Workflows :** WF-010, WF-011, WF-023, WF-024

**Décisions de baseline :** Q-002, Q-003, Q-004, Q-005, Q-006, Q-016, Q-025, Q-028

#### ENT-019-A01 — Prescription consultable

| Élément de baseline | Définition |
| --- | --- |
| Définition | Prescription structurée : médicament, dose, unité, voie, fréquence, durée et instructions; signature du médecin et horodatage obligatoires |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Prescription structurée : médicament, dose, unité, voie, fréquence, durée et instructions; signature du médecin et horodatage obligatoires |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-004, Q-005, Q-006, Q-016, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-002; EF-DM-004 |
| Utilisation | WF-010, WF-011, WF-023, WF-024 |

#### ENT-019-A02 — Point de départ des 15 jours

| Élément de baseline | Définition |
| --- | --- |
| Définition | Horodatage de publication de la prescription signée, en Africa/Abidjan |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Horodatage de publication de la prescription signée, en Africa/Abidjan |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-004, Q-005, Q-006, Q-016, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-002; EF-DM-004 |
| Utilisation | WF-010, WF-011, WF-023, WF-024 |

#### ENT-019-A03 — Fin de visibilité patient

| Élément de baseline | Définition |
| --- | --- |
| Définition | Instant exclusif égal à la publication signée + 15 jours calendaires selon Q-004 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Instant exclusif égal à la publication signée + 15 jours calendaires selon Q-004 |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-004, Q-005, Q-006, Q-016, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-002; EF-DM-004 |
| Utilisation | WF-010, WF-011, WF-023, WF-024 |

#### ENT-019-A04 — Bénéficiaire de l’ordonnance

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers le patient bénéficiaire; contrôle objet côté serveur |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers le patient bénéficiaire; contrôle objet côté serveur |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-004, Q-005, Q-006, Q-016, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-002; EF-DM-004 |
| Utilisation | WF-010, WF-011, WF-023, WF-024 |

### ENT-020 — Pièce jointe

**Définition :** Document joint à un dossier ou élément clinique ; formats et rattachements restent arrêté pour la baseline.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Médical; pas d’attribution de permission implicite

**Sources :** ADD-020

**Workflows :** WF-010, WF-011, WF-013, WF-014, WF-023, WF-025

**Décisions de baseline :** Q-002, Q-003, Q-005, Q-006, Q-016, Q-017, Q-025, Q-027, Q-028

#### ENT-020-A01 — Document joint

| Élément de baseline | Définition |
| --- | --- |
| Définition | PDF, JPEG ou PNG; 10 Mo maximum; contrôle MIME, signature, antivirus et SHA-256 selon Q-028 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | PDF, JPEG ou PNG; 10 Mo maximum; contrôle MIME, signature, antivirus et SHA-256 selon Q-028 |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-005, Q-006, Q-016, Q-017, Q-025, Q-027, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-020 |
| Utilisation | WF-010, WF-011, WF-013, WF-014, WF-023, WF-025 |

#### ENT-020-A02 — Dossier concerné

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers dossier, ordonnance, résultat ou demande de copie; type de ressource explicite |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers dossier, ordonnance, résultat ou demande de copie; type de ressource explicite |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-003, Q-005, Q-006, Q-016, Q-017, Q-025, Q-027, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-020 |
| Utilisation | WF-010, WF-011, WF-013, WF-014, WF-023, WF-025 |

### ENT-021 — Demande de copie

**Définition :** Demande du patient pour obtenir une copie de son dossier, avec périmètre et identité à vérifier.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Service médical pour copie clinique; administration/comptabilité pour copie administrative ou financière selon Q-005

**Sources :** ADD-003

**Workflows :** WF-025

**Décisions de baseline :** Q-005, Q-006, Q-025, Q-028

#### ENT-021-A01 — Patient dont le dossier est demandé

| Élément de baseline | Définition |
| --- | --- |
| Définition | Patient authentifié par date de naissance et code à usage unique sur contact vérifié; revue manuelle en cas d'écart selon Q-025 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Patient authentifié par date de naissance et code à usage unique sur contact vérifié; revue manuelle en cas d'écart selon Q-025 |
| Règles et décisions applicables | Règles citées et décisions Q-005, Q-006, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-003 |
| Utilisation | WF-025 |

#### ENT-021-A02 — Éléments demandés

| Élément de baseline | Définition |
| --- | --- |
| Définition | COMPLET ou PARTIEL; si PARTIEL, liste obligatoire des catégories et de la période demandées |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | COMPLET ou PARTIEL; si PARTIEL, liste obligatoire des catégories et de la période demandées |
| Règles et décisions applicables | Règles citées et décisions Q-005, Q-006, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-003 |
| Utilisation | WF-025 |

#### ENT-021-A03 — Identité du demandeur

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers le compte demandeur et preuve de vérification séparée du contenu clinique |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers le compte demandeur et preuve de vérification séparée du contenu clinique |
| Règles et décisions applicables | Règles citées et décisions Q-005, Q-006, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-003 |
| Utilisation | WF-025 |

### ENT-022 — Ligne de facture

**Définition :** Détail de baseline d’une facture reliant prestation, bénéficiaire et montant, notamment pour le groupement de patients.

**Statut du concept :** Décision de cadrage de la baseline

**Domaine responsable :** Comptabilité; pas d’attribution de permission implicite

**Sources :** §6.2; ADD-004 ADD-008

**Workflows :** WF-015, WF-016, WF-017, WF-018

**Décisions de baseline :** Q-007, Q-008, Q-009, Q-016, Q-018, Q-020, Q-023, Q-024, Q-029, Q-035

#### ENT-022-A01 — Facture porteuse

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers une facture; une facture organisme contient au plus dix patients selon Q-007 |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers une facture; une facture organisme contient au plus dix patients selon Q-007 |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-016, Q-018, Q-020, Q-023, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.2; ADD-004 ADD-008 |
| Utilisation | WF-015, WF-016, WF-017, WF-018 |

#### ENT-022-A02 — Prestation facturée

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers la prestation et son patient; unicité facture/prestation |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers la prestation et son patient; unicité facture/prestation |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-016, Q-018, Q-020, Q-023, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.2; ADD-004 ADD-008 |
| Utilisation | WF-015, WF-016, WF-017, WF-018 |

#### ENT-022-A03 — Montant de ligne

| Élément de baseline | Définition |
| --- | --- |
| Définition | Montant entier XOF = quantité × tarif versionné après remises/taxes, arrondi demi-supérieur |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Montant entier XOF = quantité × tarif versionné après remises/taxes, arrondi demi-supérieur |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-016, Q-018, Q-020, Q-023, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.2; ADD-004 ADD-008 |
| Utilisation | WF-015, WF-016, WF-017, WF-018 |

### ENT-023 — Prise en charge

**Définition :** Prise en charge financière par un organisme payeur, exprimée notamment par une quote-part ; ne désigne pas un épisode de soins.

**Statut du concept :** Clôturé pour la baseline

**Domaine responsable :** Comptabilité; pas d’attribution de permission implicite

**Sources :** ADD-010; §7.5

**Workflows :** WF-018, WF-020

**Décisions de baseline :** Q-007, Q-008, Q-009, Q-019, Q-029, Q-035

#### ENT-023-A01 — Organisme couvrant

| Élément de baseline | Définition |
| --- | --- |
| Définition | Couverture calculée par ligne de prestation éligible selon Q-009 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Couverture calculée par ligne de prestation éligible selon Q-009 |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-019, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-010; §7.5 |
| Utilisation | WF-018, WF-020 |

#### ENT-023-A02 — Quote-part de prise en charge

| Élément de baseline | Définition |
| --- | --- |
| Définition | Pourcentage entre 0 et 100 inclus; une couverture principale V1; calcul par ligne et arrondi demi-supérieur selon Q-009 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Pourcentage entre 0 et 100 inclus; une couverture principale V1; calcul par ligne et arrondi demi-supérieur selon Q-009 |
| Règles et décisions applicables | Règles citées et décisions Q-007, Q-008, Q-009, Q-019, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-010; §7.5 |
| Utilisation | WF-018, WF-020 |

### ENT-024 — Décision de copie

**Définition :** Représentation technique retenue pour la baseline de la réponse à une demande de copie ; l’acceptation seule est explicitement citée.

**Statut du concept :** Décision de cadrage de la baseline

**Domaine responsable :** Médecin auteur ou directeur médical délégué pour le clinique; responsable administratif pour l'administratif/financier, selon Q-005

**Sources :** ADD-003

**Workflows :** WF-025

**Décisions de baseline :** Q-005, Q-006, Q-025, Q-028

#### ENT-024-A01 — Demande examinée

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire et unique vers la demande de copie |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire et unique vers la demande de copie |
| Règles et décisions applicables | Règles citées et décisions Q-005, Q-006, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-003 |
| Utilisation | WF-025 |

#### ENT-024-A02 — Acceptation ou autre réponse

| Élément de baseline | Définition |
| --- | --- |
| Définition | ACCEPTEE, REFUSEE ou COMPLEMENT_REQUIS; motif et horodatage obligatoires |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | ACCEPTEE, REFUSEE ou COMPLEMENT_REQUIS; motif et horodatage obligatoires |
| Règles et décisions applicables | Règles citées et décisions Q-005, Q-006, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-003 |
| Utilisation | WF-025 |

#### ENT-024-A03 — Auteur de la décision

| Élément de baseline | Définition |
| --- | --- |
| Définition | Médecin auteur/directeur médical délégué pour le clinique; responsable administratif pour l'administratif/financier selon Q-005 |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Médecin auteur/directeur médical délégué pour le clinique; responsable administratif pour l'administratif/financier selon Q-005 |
| Règles et décisions applicables | Règles citées et décisions Q-005, Q-006, Q-025, Q-028; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-003 |
| Utilisation | WF-025 |

### ENT-025 — Autorisation par action

**Définition :** Représentation technique retenue pour la baseline d’un droit associant rôle, action et périmètre de données.

**Statut du concept :** Décision de cadrage de la baseline

**Domaine responsable :** Habilitations; pas d’attribution de permission implicite

**Sources :** EF-SEC-003

**Workflows :** WF-033

**Décisions de baseline :** Q-002, Q-024, Q-025, Q-031

#### ENT-025-A01 — Rôle concerné

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers un rôle actif de la matrice définitive |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers un rôle actif de la matrice définitive |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-024, Q-025, Q-031; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-SEC-003 |
| Utilisation | WF-033 |

#### ENT-025-A02 — Action contrôlée

| Élément de baseline | Définition |
| --- | --- |
| Définition | CREER, LIRE, MODIFIER, VALIDER, PUBLIER, ANNULER, REMBOURSER, EXPORTER ou ADMINISTRER selon Q-031 |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | CREER, LIRE, MODIFIER, VALIDER, PUBLIER, ANNULER, REMBOURSER, EXPORTER ou ADMINISTRER selon Q-031 |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-024, Q-025, Q-031; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-SEC-003 |
| Utilisation | WF-033 |

#### ENT-025-A03 — Périmètre de donnée

| Élément de baseline | Définition |
| --- | --- |
| Définition | Type de ressource et portée PROPRE, EPISODE, SERVICE ou GLOBAL; GLOBAL réservé à la direction ou administration déléguée |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Type de ressource et portée PROPRE, EPISODE, SERVICE ou GLOBAL; GLOBAL réservé à la direction ou administration déléguée |
| Règles et décisions applicables | Règles citées et décisions Q-002, Q-024, Q-025, Q-031; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-SEC-003 |
| Utilisation | WF-033 |

### ENT-026 — Notification

**Définition :** Représentation technique retenue pour la baseline d’un rappel de rendez-vous ou d’un message de paie, avec résultat de transmission.

**Statut du concept :** Décision de cadrage de la baseline

**Domaine responsable :** Accueil / RH; pas d’attribution de permission implicite

**Sources :** ADD-006 ADD-007

**Workflows :** WF-007, WF-028

**Décisions de baseline :** Q-014, Q-022, Q-026, Q-027, Q-034

#### ENT-026-A01 — Patient ou employé

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers un utilisateur, patient ou employé; adresse résolue depuis une préférence vérifiée |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers un utilisateur, patient ou employé; adresse résolue depuis une préférence vérifiée |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-022, Q-026, Q-027, Q-034; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-006 ADD-007 |
| Utilisation | WF-007, WF-028 |

#### ENT-026-A02 — Rappel RDV ou paie

| Élément de baseline | Définition |
| --- | --- |
| Définition | RENDEZ_VOUS, PUBLICATION_DOCUMENT, PAIEMENT, PAIE ou SECURITE; aucun contenu clinique dans le message |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | RENDEZ_VOUS, PUBLICATION_DOCUMENT, PAIEMENT, PAIE ou SECURITE; aucun contenu clinique dans le message |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-022, Q-026, Q-027, Q-034; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-006 ADD-007 |
| Utilisation | WF-007, WF-028 |

#### ENT-026-A03 — Résultat de transmission

| Élément de baseline | Définition |
| --- | --- |
| Définition | PLANIFIEE, ENVOYEE, LIVREE, ECHEC ou ANNULEE; aucune lecture déduite sans accusé explicite |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | PLANIFIEE, ENVOYEE, LIVREE, ECHEC ou ANNULEE; aucune lecture déduite sans accusé explicite |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-022, Q-026, Q-027, Q-034; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-006 ADD-007 |
| Utilisation | WF-007, WF-028 |

### ENT-027 — Préférence de canal

**Définition :** Choix du canal de rappel par le patient et coordonnées permettant son utilisation.

**Statut du concept :** Besoin sourcé dans le SRS

**Domaine responsable :** Patient / accueil; pas d’attribution de permission implicite

**Sources :** ADD-006

**Workflows :** WF-007

**Décisions de baseline :** Q-014, Q-026, Q-027

#### ENT-027-A01 — Patient choisissant

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire et unique par patient/canal actif |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire et unique par patient/canal actif |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-026, Q-027; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-006 |
| Utilisation | WF-007 |

#### ENT-027-A02 — Canal choisi

| Élément de baseline | Définition |
| --- | --- |
| Définition | SMS, EMAIL ou WHATSAPP; canal actif seulement après vérification |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | SMS, EMAIL ou WHATSAPP; canal actif seulement après vérification |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-026, Q-027; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-006 |
| Utilisation | WF-007 |

#### ENT-027-A03 — Destination du rappel

| Élément de baseline | Définition |
| --- | --- |
| Définition | Adresse normalisée et vérifiée par code à usage unique avant activation |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Adresse normalisée et vérifiée par code à usage unique avant activation |
| Règles et décisions applicables | Règles citées et décisions Q-014, Q-026, Q-027; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | ADD-006 |
| Utilisation | WF-007 |

### ENT-028 — Affectation de paiement

**Définition :** Représentation de baseline de la part d’un paiement attribuée à une dette ; ventilation arbitré par la baseline.

**Statut du concept :** Décision de cadrage de la baseline

**Domaine responsable :** Comptabilité; pas d’attribution de permission implicite

**Sources :** §6.2; EF-PAI-005

**Workflows :** WF-019, WF-020, WF-021

**Décisions de baseline :** Q-009, Q-019, Q-020, Q-024, Q-029, Q-035

#### ENT-028-A01 — Règlement ventilé

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers le paiement confirmé ou placé en attente comptable |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers le paiement confirmé ou placé en attente comptable |
| Règles et décisions applicables | Règles citées et décisions Q-009, Q-019, Q-020, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.2; EF-PAI-005 |
| Utilisation | WF-019, WF-020, WF-021 |

#### ENT-028-A02 — Dette cible

| Élément de baseline | Définition |
| --- | --- |
| Définition | Référence obligatoire vers la facture et, si nécessaire, sa ligne; aucune imputation vers une facture annulée |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Référence obligatoire vers la facture et, si nécessaire, sa ligne; aucune imputation vers une facture annulée |
| Règles et décisions applicables | Règles citées et décisions Q-009, Q-019, Q-020, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.2; EF-PAI-005 |
| Utilisation | WF-019, WF-020, WF-021 |

#### ENT-028-A03 — Part affectée

| Élément de baseline | Définition |
| --- | --- |
| Définition | Montant entier XOF strictement positif; somme des imputations ≤ paiement, dépassement interdit |
| Niveau de validation | Décision de cadrage de la baseline |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Montant entier XOF strictement positif; somme des imputations ≤ paiement, dépassement interdit |
| Règles et décisions applicables | Règles citées et décisions Q-009, Q-019, Q-020, Q-024, Q-029, Q-035; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | §6.2; EF-PAI-005 |
| Utilisation | WF-019, WF-020, WF-021 |

### ENT-029 — Dépense

**Définition :** Concept de baseline nécessaire à la compréhension des rapports de dépenses ; provenance et imputation sont précisés par les décisions de baseline associées.

**Statut du concept :** Clôturé pour la baseline

**Domaine responsable :** Comptabilité; pas d’attribution de permission implicite

**Sources :** EF-REP-002

**Workflows :** WF-026

**Décisions de baseline :** Q-008, Q-021

#### ENT-029-A01 — Dépense à agréger

| Élément de baseline | Définition |
| --- | --- |
| Définition | Saisie comptable manuelle ou import CSV contrôlé, avec référence, justificatif, date et auteur |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Saisie comptable manuelle ou import CSV contrôlé, avec référence, justificatif, date et auteur |
| Règles et décisions applicables | Règles citées et décisions Q-008, Q-021; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-REP-002 |
| Utilisation | WF-026 |

#### ENT-029-A02 — Période d’imputation

| Élément de baseline | Définition |
| --- | --- |
| Définition | Date de comptabilisation pour l'engagement et date de paiement pour le décaissement, exposées séparément selon Q-021 |
| Niveau de validation | Clôturé pour la baseline : concept sourcé, représentation retenue dans ce dictionnaire |
| Obligatoire ou facultatif | Obligatoire avant validation ou publication si nécessaire au résultat métier; facultatif au brouillon |
| Valeurs autorisées | Date de comptabilisation pour l'engagement et date de paiement pour le décaissement, exposées séparément selon Q-021 |
| Règles et décisions applicables | Règles citées et décisions Q-008, Q-021; appliquer les domaines et bornes de la décision Q associée |
| Exemple | Aucun exemple normatif; utiliser des données fictives en recette |
| Origine | EF-REP-002 |
| Utilisation | WF-026 |

## 3. Gouvernance des changements

Toute correction postérieure cite l’identifiant ENT et, si applicable, l’identifiant du champ, puis suit la procédure de changement. La couverture financière « Prise en charge » reste distincte du contexte clinique.
