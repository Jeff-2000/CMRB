# Catalogue normalisé des exigences

Les identifiants EF et ENF sont conservés. ADD désigne un complément présent dans le SRS ou ses commentaires, et non une nouvelle exigence approuvée. NFR identifie les 11 rubriques non numérotées de §5.2, sans leur attribuer de cible chiffrée. Une ligne dont le texte demande une décision reste une contrainte de préparation, même si son statut source dit « Confirmé ».

Les champs « Description source » et « Statut source exact » sont des preuves historiques; les références Q renvoient désormais à des décisions `CLOSED_FOR_BASELINE`.

Source intégrale : [texte courant](source/SRS_CURRENT_TEXT.md), [commentaires](source/SRS_COMMENTS.md), [révisions](source/SRS_REVISIONS.md).

## EF-PAT-001 — Le système doit permettre à un utilisateur interne autorisé de créer un dossier patient administratif

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre à un utilisateur interne autorisé de créer un dossier patient administratif. |
| Source | 4.1 Gestion des patients; P0229 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-001: Demande d’inscription au centre ou en ligne |
| Workflows | WF-001 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-005 |
| Résultat attendu | Inscription enregistrée; statut et numéro patient non spécifiés |
| Critères existants associés | AC-01 AC-02 |
| Décisions de baseline | Q-011, Q-025 |

## EF-PAT-002 — Le système doit permettre à un utilisateur interne autorisé de modifier un dossier patient administratif

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre à un utilisateur interne autorisé de modifier un dossier patient administratif. |
| Source | 4.1 Gestion des patients; P0229 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-012 |
| Préconditions | WF-003: Correction d’une donnée administrative |
| Workflows | WF-003 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-005 |
| Résultat attendu | Dossier administratif modifié; traçabilité de correction à définir |
| Critères existants associés | AC-01 AC-02 |
| Décisions de baseline | Q-011, Q-025, Q-028 |

## EF-PAT-003 — Le système doit permettre la consultation d'un dossier patient administratif par les rôles autorisés

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la consultation d'un dossier patient administratif par les rôles autorisés. |
| Source | 4.1 Gestion des patients; P0229 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-012 |
| Préconditions | WF-002: Besoin d’identifier le patient à prendre en charge |
| Workflows | WF-002 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-005 |
| Résultat attendu | Dossier administratif consulté sans modification |
| Critères existants associés | AC-01 AC-02 |
| Décisions de baseline | Q-011, Q-024, Q-025 |

## EF-PAT-004 — Le système doit exposer un formulaire d'inscription patient accessible en ligne et une interface interne d'inscription au centre

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit exposer un formulaire d'inscription patient accessible en ligne et une interface interne d'inscription au centre. |
| Source | 4.1 Gestion des patients; P0229 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-001: Demande d’inscription au centre ou en ligne |
| Workflows | WF-001 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-005 |
| Résultat attendu | Inscription enregistrée; statut et numéro patient non spécifiés |
| Critères existants associés | AC-01 AC-02 |
| Décisions de baseline | Q-011, Q-025 |

## EF-PAT-005 — Le système doit distinguer techniquement le dossier patient administratif du dossier médical confidentiel

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit distinguer techniquement le dossier patient administratif du dossier médical confidentiel. |
| Source | 4.1 Gestion des patients; P0229 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-012 |
| Préconditions | WF-002: Besoin d’identifier le patient à prendre en charge; WF-003: Correction d’une donnée administrative |
| Workflows | WF-002, WF-003 |
| Règles | BR-001 |
| Données | ENT-004, ENT-005 |
| Résultat attendu | Dossier administratif consulté sans modification; Dossier administratif modifié; traçabilité de correction à définir |
| Critères existants associés | AC-01 AC-02 |
| Décisions de baseline | Q-011, Q-024, Q-025, Q-028 |

## EF-PAT-006 — Le système ne doit pas autoriser de suppression physique de dossier patient tant que le mode cible de suppression n'a pas été formellement arbitré

| Champ | Valeur |
| --- | --- |
| Description source | Le système ne doit pas autoriser de suppression physique de dossier patient tant que le mode cible de suppression n'a pas été formellement arbitré. |
| Source | 4.1 Gestion des patients; P0229 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-012 |
| Préconditions | WF-004: Demande de suppression d’un dossier |
| Workflows | WF-004 |
| Règles | BR-003 |
| Données | ENT-004, ENT-005, ENT-006 |
| Résultat attendu | Demande non exécutée tant que la politique est absente |
| Critères existants associés | AC-01 AC-02 |
| Décisions de baseline | Q-012, Q-025 |

## EF-PAT-007 — Le système doit appliquer une politique de validation des données obligatoires de création de patient dès que cette liste est validée dans le dictionnaire de données

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit appliquer une politique de validation des données obligatoires de création de patient dès que cette liste est validée dans le dictionnaire de données. |
| Source | 4.1 Gestion des patients; P0229 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-001: Demande d’inscription au centre ou en ligne; WF-003: Correction d’une donnée administrative |
| Workflows | WF-001, WF-003 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-005 |
| Résultat attendu | Inscription enregistrée; statut et numéro patient non spécifiés; Dossier administratif modifié; traçabilité de correction à définir |
| Critères existants associés | AC-01 AC-02 |
| Décisions de baseline | Q-011, Q-025, Q-028 |

## EF-RDV-001 — Le système doit permettre la planification d'un rendez-vous

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la planification d'un rendez-vous. |
| Source | 4.2 Gestion des rendez-vous; P0263 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-005: Demande de rendez-vous par patient ou accueil |
| Workflows | WF-005 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-007 |
| Résultat attendu | Rendez-vous planifié; statut exact non arrêté |
| Critères existants associés | AC-03 |
| Décisions de baseline | Q-013, Q-015, Q-025 |

## EF-RDV-002 — Le système doit permettre la confirmation d'un rendez-vous

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la confirmation d'un rendez-vous. |
| Source | 4.2 Gestion des rendez-vous; P0263 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-012 |
| Préconditions | WF-006: Rendez-vous à confirmer |
| Workflows | WF-006 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-007 |
| Résultat attendu | Confirmation enregistrée; transition partielle documentée |
| Critères existants associés | AC-03 |
| Décisions de baseline | Q-014, Q-015 |

## EF-RDV-003 — Le système doit permettre l'envoi d'un rappel de rendez-vous

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'envoi d'un rappel de rendez-vous. |
| Source | 4.2 Gestion des rendez-vous; P0263 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012, ACT-014 |
| Préconditions | WF-007: Échéance de rappel à fixer |
| Workflows | WF-007 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-007, ENT-026, ENT-027 |
| Résultat attendu | Rappel transmis ou échec identifié; livraison effective non assimilée à acceptation technique |
| Critères existants associés | AC-03 |
| Décisions de baseline | Q-014, Q-026, Q-027 |

## EF-RDV-004 — Le système doit permettre la prise de rendez-vous via une interface en ligne destinée au patient

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la prise de rendez-vous via une interface en ligne destinée au patient. |
| Source | 4.2 Gestion des rendez-vous; P0263 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-005: Demande de rendez-vous par patient ou accueil |
| Workflows | WF-005 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-007 |
| Résultat attendu | Rendez-vous planifié; statut exact non arrêté |
| Critères existants associés | AC-03 |
| Décisions de baseline | Q-013, Q-015, Q-025 |

## EF-RDV-005 — Le système doit empêcher de figer un canal unique de rappel tant que les canaux autorisés (SMS, e-mail, appel, autre…) ne sont pas validé

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit empêcher de figer un canal unique de rappel tant que les canaux autorisés (SMS, e-mail, appel, autre…) ne sont pas validé |
| Source | 4.2 Gestion des rendez-vous; P0263 |
| Priorité source | MVP |
| Statut source exact | À valider |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012, ACT-014 |
| Préconditions | WF-007: Échéance de rappel à fixer |
| Workflows | WF-007 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-007, ENT-026, ENT-027 |
| Résultat attendu | Rappel transmis ou échec identifié; livraison effective non assimilée à acceptation technique |
| Critères existants associés | AC-03 |
| Décisions de baseline | Q-014, Q-026, Q-027 |

## EF-RDV-006 — Le système doit être conçu de manière à supporter un statut de rendez-vous ; la liste exacte des statuts reste à valider

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit être conçu de manière à supporter un statut de rendez-vous ; la liste exacte des statuts reste à valider. |
| Source | 4.2 Gestion des rendez-vous; P0263 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-005: Demande de rendez-vous par patient ou accueil; WF-006: Rendez-vous à confirmer |
| Workflows | WF-005, WF-006 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-007 |
| Résultat attendu | Rendez-vous planifié; statut exact non arrêté; Confirmation enregistrée; transition partielle documentée |
| Critères existants associés | AC-03 |
| Décisions de baseline | Q-013, Q-014, Q-015, Q-025 |

## EF-RDV-007 — Les règles d'annulation, de report, d'absence patient et de gestion des créneaux ne doivent pas être implémentées sans validation du workflow cible

| Champ | Valeur |
| --- | --- |
| Description source | Les règles d'annulation, de report, d'absence patient et de gestion des créneaux ne doivent pas être implémentées sans validation du workflow cible. |
| Source | 4.2 Gestion des rendez-vous; P0263 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-008: Demande d’annulation ou nouveau rendez-vous |
| Workflows | WF-008 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-007 |
| Résultat attendu | Annulation enregistrée si autorisée; nouvelle réservation indépendante tant que lien non décidé |
| Critères existants associés | AC-03 |
| Décisions de baseline | Q-013, Q-015 |

## EF-DM-001 — Le système doit permettre la consultation de l'historique médical des patients par les rôles autorisés

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la consultation de l'historique médical des patients par les rôles autorisés. |
| Source | 4.3 Dossier médical; P0296 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-012 |
| Préconditions | WF-011: Besoin clinique d’historique |
| Workflows | WF-011 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-006, ENT-008, ENT-018, ENT-019, ENT-020 |
| Résultat attendu | Historique consulté; aucune publication patient induite |
| Critères existants associés | AC-04 AC-05 |
| Décisions de baseline | Q-002, Q-003, Q-025, Q-028 |

## EF-DM-002 — Le système doit autoriser la création et la modification du dossier médical confidentiel uniquement par des médecins

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit autoriser la création et la modification du dossier médical confidentiel uniquement par des médecins. |
| Source | 4.3 Dossier médical; P0296 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-010: Consultation en attente prise par un médecin |
| Workflows | WF-010 |
| Règles | BR-002 |
| Données | ENT-004, ENT-006, ENT-008, ENT-015, ENT-019, ENT-020 |
| Résultat attendu | Consultation enregistrée et disponible pour facturation |
| Critères existants associés | AC-04 AC-05 |
| Décisions de baseline | Q-002, Q-016, Q-028 |

## EF-DM-003 — Le système doit séparer les permissions du dossier médical des permissions du dossier patient administratif

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit séparer les permissions du dossier médical des permissions du dossier patient administratif. |
| Source | 4.3 Dossier médical; P0296 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-012 |
| Préconditions | WF-011: Besoin clinique d’historique |
| Workflows | WF-011 |
| Règles | BR-001 |
| Données | ENT-004, ENT-006, ENT-008, ENT-018, ENT-019, ENT-020 |
| Résultat attendu | Historique consulté; aucune publication patient induite |
| Critères existants associés | AC-04 AC-05 |
| Décisions de baseline | Q-002, Q-003, Q-025, Q-028 |

## EF-DM-004 — Le contenu métier exact du dossier médical (motif, constantes( paramedicaux peuvent remplir…), diagnostic, actes, pièces jointes, prescriptions, observations) doit être validé avant maquettage et développement

| Champ | Valeur |
| --- | --- |
| Description source | Le contenu métier exact du dossier médical (motif, constantes( paramedicaux peuvent remplir…), diagnostic, actes, pièces jointes, prescriptions, observations) doit être validé avant maquettage et développement. |
| Source | 4.3 Dossier médical; P0296 |
| Priorité source | MVP |
| Statut source exact | Bloquant |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-009: Arrivée du patient pour consultation; WF-010: Consultation en attente prise par un médecin |
| Workflows | WF-009, WF-010 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-006, ENT-008, ENT-015, ENT-019, ENT-020 |
| Résultat attendu | Constantes associées au contexte clinique, sous réserve de résolution du conflit; Consultation enregistrée et disponible pour facturation |
| Critères existants associés | AC-04 AC-05 |
| Décisions de baseline | Q-002, Q-011, Q-016, Q-028 |

## EF-DM-005 — Toute capacité d'accès du patient à son dossier médical doit rester hors MVP tant qu'elle n'est pas explicitement autorisée

| Champ | Valeur |
| --- | --- |
| Description source | Toute capacité d'accès du patient à son dossier médical doit rester hors MVP tant qu'elle n'est pas explicitement autorisée. |
| Source | 4.3 Dossier médical; P0296 |
| Priorité source | Hors MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-005, ACT-012 |
| Préconditions | WF-023: Patient ouvre son espace personnel |
| Workflows | WF-023 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-005, ENT-006, ENT-018, ENT-019, ENT-020 |
| Résultat attendu | Contenu consulté dans les limites décidées |
| Critères existants associés | AC-04 AC-05 |
| Décisions de baseline | Q-003, Q-005, Q-006, Q-025 |

## EF-SRV-CONS-001 — Le système doit permettre l'enregistrement d'une consultation comme prestation

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'enregistrement d'une consultation comme prestation. |
| Source | 4.4.1 Consultation; P0323 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-010: Consultation en attente prise par un médecin |
| Workflows | WF-010 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-006, ENT-008, ENT-015, ENT-019, ENT-020 |
| Résultat attendu | Consultation enregistrée et disponible pour facturation |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-002, Q-016, Q-028 |

## EF-SRV-CONS-002 — Une consultation doit pouvoir être rattachée au patient concerné

| Champ | Valeur |
| --- | --- |
| Description source | Une consultation doit pouvoir être rattachée au patient concerné. |
| Source | 4.4.1 Consultation; P0323 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-010: Consultation en attente prise par un médecin |
| Workflows | WF-010 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-006, ENT-008, ENT-015, ENT-019, ENT-020 |
| Résultat attendu | Consultation enregistrée et disponible pour facturation |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-002, Q-016, Q-028 |

## EF-SRV-CONS-003 — La consultation doit pouvoir alimenter le dossier médical si le rôle connecté est médecin

| Champ | Valeur |
| --- | --- |
| Description source | La consultation doit pouvoir alimenter le dossier médical si le rôle connecté est médecin.La consultation peut aboutir a une hspitalisation ou une mise en observation. |
| Source | 4.4.1 Consultation; P0323 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-010: Consultation en attente prise par un médecin; WF-012: Orientation médicale vers un séjour |
| Workflows | WF-010, WF-012 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-006, ENT-008, ENT-015, ENT-016, ENT-017, ENT-019, ENT-020 |
| Résultat attendu | Consultation enregistrée et disponible pour facturation; Séjour et prestations identifiés; admission/sortie détaillées non prêtes |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-002, Q-016, Q-028 |

## EF-SRV-HOSP-001 — Le système doit permettre l'enregistrement d'une hospitalisation comme prestation

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'enregistrement d'une hospitalisation comme prestation. |
| Source | 4.4.2 Hospitalisation; P0342 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-012: Orientation médicale vers un séjour |
| Workflows | WF-012 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-016, ENT-017 |
| Résultat attendu | Séjour et prestations identifiés; admission/sortie détaillées non prêtes |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-002, Q-016 |

## EF-SRV-HOSP-002 — Le workflow complet d'hospitalisation (admission, chambre/lit, transfert, sortie, facturation détaillée) est suspendu tant qu'il n'est pas validé

| Champ | Valeur |
| --- | --- |
| Description source | Le workflow complet d'hospitalisation (admission, chambre/lit, transfert, sortie, facturation détaillée) est suspendu tant qu'il n'est pas validé. |
| Source | 4.4.2 Hospitalisation; P0342 |
| Priorité source | MVP |
| Statut source exact | Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-003, ACT-004, ACT-012 |
| Préconditions | WF-012: Orientation médicale vers un séjour; WF-017: Facturation d’une hospitalisation |
| Workflows | WF-012, WF-017 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-009, ENT-016, ENT-017, ENT-022 |
| Résultat attendu | Séjour et prestations identifiés; admission/sortie détaillées non prêtes; Facture du séjour détaillée; montant non calculable contractuellement avant arbitrage |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-002, Q-009, Q-016, Q-020, Q-024, Q-035 |

## EF-SRV-LAB-001 — Le système doit permettre l'enregistrement d'une prestation de laboratoire

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'enregistrement d'une prestation de laboratoire. |
| Source | 4.4.3 Laboratoire; P0355 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-010, ACT-012 |
| Préconditions | WF-013: Prestation de laboratoire à enregistrer |
| Workflows | WF-013 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-018, ENT-020 |
| Résultat attendu | Prestation enregistrée; résultat non automatiquement publié au portail |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-017, Q-027, Q-028 |

## EF-SRV-LAB-002 — Le détail du processus laboratoire (demande, prélèvement, résultat(assistante peut rentrer les results…), validation, intégration automate) reste à valider

| Champ | Valeur |
| --- | --- |
| Description source | Le détail du processus laboratoire (demande, prélèvement, résultat(assistante peut rentrer les results…), validation, intégration automate) reste à valider. |
| Source | 4.4.3 Laboratoire; P0355 |
| Priorité source | MVP |
| Statut source exact | Bloquant/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-010, ACT-012 |
| Préconditions | WF-013: Prestation de laboratoire à enregistrer |
| Workflows | WF-013 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-018, ENT-020 |
| Résultat attendu | Prestation enregistrée; résultat non automatiquement publié au portail |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-017, Q-027, Q-028 |

## EF-SRV-IMG-001 — Le système doit permettre l'enregistrement d'une prestation d'échographie / imagerie mentionnée au cahier initial

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'enregistrement d'une prestation d'échographie / imagerie mentionnée au cahier initial. |
| Source | 4.4.4 Imagerie / échographie; P0368 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-012 |
| Préconditions | WF-014: Échographie ou autre imagerie réalisée |
| Workflows | WF-014 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-018, ENT-020 |
| Résultat attendu | Prestation d’imagerie enregistrée; diffusion conditionnée aux décisions |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-017, Q-028 |

## EF-SRV-IMG-002 — Le détail du workflow imagerie (demande, acquisition, compte rendu, pièces jointes) reste à valider

| Champ | Valeur |
| --- | --- |
| Description source | Le détail du workflow imagerie (demande, acquisition, compte rendu, pièces jointes) reste à valider. |
| Source | 4.4.4 Imagerie / échographie; P0368 |
| Priorité source | MVP |
| Statut source exact | Bloquant/confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-012 |
| Préconditions | WF-014: Échographie ou autre imagerie réalisée |
| Workflows | WF-014 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-018, ENT-020 |
| Résultat attendu | Prestation d’imagerie enregistrée; diffusion conditionnée aux décisions |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-017, Q-028 |

## EF-SRV-PHA-001 — Le système doit permettre l'enregistrement d'une prestation liée à la pharmacie

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'enregistrement d'une prestation liée à la pharmacie. |
| Source | 4.4.5 Pharmacie; P0381 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-008, ACT-012 |
| Préconditions | WF-015: Prestation pharmacie, notamment pendant un séjour |
| Workflows | WF-015 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-012, ENT-013, ENT-022 |
| Résultat attendu | Prestation pharmacie enregistrée; cohérence stock/facture à spécifier |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-018, Q-023 |

## EF-SRV-PHA-002 — Le lien entre dispensation pharmacie, stock et facturation doit être défini avant développement détaillé

| Champ | Valeur |
| --- | --- |
| Description source | Le lien entre dispensation pharmacie, stock et facturation doit être défini avant développement détaillé. (On suppose Malade hospitalisé: la pharmacie est impliquée dans la facturation) |
| Source | 4.4.5 Pharmacie; P0381 |
| Priorité source | MVP |
| Statut source exact | Bloquant/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-008, ACT-012 |
| Préconditions | WF-015: Prestation pharmacie, notamment pendant un séjour |
| Workflows | WF-015 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-012, ENT-013, ENT-022 |
| Résultat attendu | Prestation pharmacie enregistrée; cohérence stock/facture à spécifier |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-018, Q-023 |

## EF-SRV-TRA-001 — Le système doit enregistrer les prestations suivantes: consultation, hospitalisation, Imagerie(échographie…), laboratoire, pharmacie

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit enregistrer les prestations suivantes: consultation, hospitalisation, Imagerie(échographie…), laboratoire, pharmacie. |
| Source | 4.4.6 Règles transverses de prestation; P0394 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-012 |
| Préconditions | WF-016: Prestations ambulatoires à facturer |
| Workflows | WF-016 |
| Règles | BR-013 |
| Données | ENT-004, ENT-008, ENT-009, ENT-022 |
| Résultat attendu | Facture individuelle émise selon règles encore à compléter |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-009, Q-020, Q-024, Q-035 |

## EF-SRV-TRA-002 — Le système doit permettre le suivi des paiements effectués en lien avec les prestations enregistrées

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre le suivi des paiements effectués en lien avec les prestations enregistrées. |
| Source | 4.4.6 Règles transverses de prestation; P0394 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-005, ACT-006, ACT-012, ACT-015 |
| Préconditions | WF-019: Règlement patient ou organisme reçu |
| Workflows | WF-019 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-009, ENT-010, ENT-011, ENT-028 |
| Résultat attendu | Paiement enregistré; règlement effectif distingué de simple initiation |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-019, Q-024, Q-029 |

## EF-SRV-TRA-003 — Le modèle de detail (pour la phamacie et les examens de laboratoire) par prestation, ses statuts et son rattachement exact à la facturation doivent être validés avant développement

| Champ | Valeur |
| --- | --- |
| Description source | Le modèle de detail (pour la phamacie et les examens de laboratoire) par prestation, ses statuts et son rattachement exact à la facturation doivent être validés avant développement. |
| Source | 4.4.6 Règles transverses de prestation; P0394 |
| Priorité source | MVP |
| Statut source exact | Bloquant/confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-004, ACT-008, ACT-012 |
| Préconditions | WF-015: Prestation pharmacie, notamment pendant un séjour; WF-016: Prestations ambulatoires à facturer |
| Workflows | WF-015, WF-016 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-009, ENT-012, ENT-013, ENT-022 |
| Résultat attendu | Prestation pharmacie enregistrée; cohérence stock/facture à spécifier; Facture individuelle émise selon règles encore à compléter |
| Critères existants associés | AC-06 |
| Décisions de baseline | Q-009, Q-018, Q-020, Q-023, Q-024, Q-035 |

## EF-FAC-001 — Le système doit permettre l'émission d'une facture pour un patient particulier

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'émission d'une facture pour un patient particulier.( Pour les actees mabulatoires, sauf les hospitalization, la facture est individuelle) |
| Source | 4.5 Facturation; P0411 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-012 |
| Préconditions | WF-016: Prestations ambulatoires à facturer; WF-017: Facturation d’une hospitalisation |
| Workflows | WF-016, WF-017 |
| Règles | BR-012 |
| Données | ENT-004, ENT-008, ENT-009, ENT-016, ENT-017, ENT-022 |
| Résultat attendu | Facture individuelle émise selon règles encore à compléter; Facture du séjour détaillée; montant non calculable contractuellement avant arbitrage |
| Critères existants associés | AC-07 |
| Décisions de baseline | Q-009, Q-016, Q-020, Q-024, Q-035 |

## EF-FAC-002 — Le système doit permettre l'émission d'une facture pour une assurance

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'émission d'une facture pour une assurance. |
| Source | 4.5 Facturation; P0411 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-006, ACT-012 |
| Préconditions | WF-018: Constitution d’une facture organisme payeur |
| Workflows | WF-018 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-009, ENT-011, ENT-022, ENT-023 |
| Résultat attendu | Facture organisme et parts à recouvrer identifiées |
| Critères existants associés | AC-07 |
| Décisions de baseline | Q-007, Q-008, Q-009, Q-029, Q-035 |

## EF-FAC-003 — Le système doit permettre l'émission d'une facture pour une mutuelle de santé

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'émission d'une facture pour une mutuelle de santé. |
| Source | 4.5 Facturation; P0411 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-006, ACT-012 |
| Préconditions | WF-018: Constitution d’une facture organisme payeur |
| Workflows | WF-018 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-009, ENT-011, ENT-022, ENT-023 |
| Résultat attendu | Facture organisme et parts à recouvrer identifiées |
| Critères existants associés | AC-07 |
| Décisions de baseline | Q-007, Q-008, Q-009, Q-029, Q-035 |

## EF-FAC-004 — Le système doit intégrer la notion de FNE, mais sa définition métier, fiscale et technique doit être validée avant conception détaillée

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit intégrer la notion de FNE, mais sa définition métier, fiscale et technique doit être validée avant conception détaillée.(Juste un bouton pour aller a la plateforme FNE) |
| Source | 4.5 Facturation; P0411 |
| Priorité source | MVP |
| Statut source exact | Bloquant/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-012, ACT-013 |
| Préconditions | WF-022: Utilisateur active le bouton FNE |
| Workflows | WF-022 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-009 |
| Résultat attendu | Plateforme externe ouverte, sans preuve automatique d’émission fiscale |
| Critères existants associés | AC-07 |
| Décisions de baseline | Q-010, Q-027 |

## EF-FAC-005 — Le cycle de vie d'une facture ne doit pas être implémenté tant que les états, transitions et règles d'annulation n'ont pas été validés

| Champ | Valeur |
| --- | --- |
| Description source | Le cycle de vie d'une facture ne doit pas être implémenté tant que les états, transitions et règles d'annulation n'ont pas été validés. |
| Source | 4.5 Facturation; P0411 |
| Priorité source | MVP |
| Statut source exact | Bloquant/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-012 |
| Préconditions | WF-021: Facture considérée comme payée |
| Workflows | WF-021 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-009, ENT-010, ENT-028 |
| Résultat attendu | Facture archivée si condition de paiement satisfaite |
| Critères existants associés | AC-07 |
| Décisions de baseline | Q-020, Q-029, Q-035 |

## EF-FAC-006 — Le système doit être conçu pour distinguer les facturations cash, assurance et mutuelle

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit être conçu pour distinguer les facturations cash, assurance et mutuelle. |
| Source | 4.5 Facturation; P0411 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-006, ACT-012 |
| Préconditions | WF-016: Prestations ambulatoires à facturer; WF-018: Constitution d’une facture organisme payeur |
| Workflows | WF-016, WF-018 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-009, ENT-011, ENT-022, ENT-023 |
| Résultat attendu | Facture individuelle émise selon règles encore à compléter; Facture organisme et parts à recouvrer identifiées |
| Critères existants associés | AC-07 |
| Décisions de baseline | Q-007, Q-008, Q-009, Q-020, Q-024, Q-029, Q-035 |

## EF-PAI-001 — Le système doit permettre le suivi des paiements effectués par les patients

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre le suivi des paiements effectués par les patients. |
| Source | 4.6 Paiements; P0440 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-005, ACT-006, ACT-012, ACT-015 |
| Préconditions | WF-019: Règlement patient ou organisme reçu |
| Workflows | WF-019 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-009, ENT-010, ENT-011, ENT-028 |
| Résultat attendu | Paiement enregistré; règlement effectif distingué de simple initiation |
| Critères existants associés | AC-08 |
| Décisions de baseline | Q-019, Q-024, Q-029 |

## EF-PAI-002 — Le système doit permettre le suivi des paiements effectués par les assurances

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre le suivi des paiements effectués par les assurances. |
| Source | 4.6 Paiements; P0440 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-005, ACT-006, ACT-012, ACT-015 |
| Préconditions | WF-019: Règlement patient ou organisme reçu |
| Workflows | WF-019 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-009, ENT-010, ENT-011, ENT-028 |
| Résultat attendu | Paiement enregistré; règlement effectif distingué de simple initiation |
| Critères existants associés | AC-08 |
| Décisions de baseline | Q-019, Q-024, Q-029 |

## EF-PAI-003 — Le système doit conserver un historique consultable des paiements enregistrés

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit conserver un historique consultable des paiements enregistrés. |
| Source | 4.6 Paiements; P0440 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-005, ACT-006, ACT-012, ACT-015 |
| Préconditions | WF-019: Règlement patient ou organisme reçu |
| Workflows | WF-019 |
| Règles | BR-014 |
| Données | ENT-009, ENT-010, ENT-011, ENT-028 |
| Résultat attendu | Paiement enregistré; règlement effectif distingué de simple initiation |
| Critères existants associés | AC-08 |
| Décisions de baseline | Q-019, Q-024, Q-029 |

## EF-PAI-004 — Les modes de paiement autorisés doivent être validés avant implémentation

| Champ | Valeur |
| --- | --- |
| Description source | Les modes de paiement autorisés doivent être validés avant implémentation.(En ligne, Cash, Paypal, Stripe, Mobile Money…) |
| Source | 4.6 Paiements; P0440 |
| Priorité source | MVP |
| Statut source exact | Bloquant/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-005, ACT-006, ACT-012, ACT-015 |
| Préconditions | WF-019: Règlement patient ou organisme reçu |
| Workflows | WF-019 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-009, ENT-010, ENT-011, ENT-028 |
| Résultat attendu | Paiement enregistré; règlement effectif distingué de simple initiation |
| Critères existants associés | AC-08 |
| Décisions de baseline | Q-019, Q-024, Q-029 |

## EF-PAI-005 — La gestion des paiements partiels, rejets, remboursements, écarts et rapprochements est suspendue tant que les règles métier ne sont pas validées

| Champ | Valeur |
| --- | --- |
| Description source | La gestion des paiements partiels, rejets, remboursements, écarts et rapprochements est suspendue tant que les règles métier ne sont pas validées. (Paiement differé par l’assurreur ou la Mutuelle) |
| Source | 4.6 Paiements; P0440 |
| Priorité source | MVP |
| Statut source exact | Bloquant/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-006, ACT-012 |
| Préconditions | WF-020: Échéance ou règlement d’un organisme à rapprocher |
| Workflows | WF-020 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-009, ENT-010, ENT-011, ENT-023, ENT-028 |
| Résultat attendu | Encours et écart identifiés; résolution suspendue aux règles financières |
| Critères existants associés | AC-08 |
| Décisions de baseline | Q-009, Q-019, Q-029 |

## EF-REP-001 — Le système doit générer un rapport de chiffre d'affaires

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit générer un rapport de chiffre d'affaires. |
| Source | 4.7 Reporting; P0465 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-009, ACT-012 |
| Préconditions | WF-026: Rapport demandé pour une période |
| Workflows | WF-026 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-008, ENT-009, ENT-010, ENT-011, ENT-029 |
| Résultat attendu | Rapport disponible avec périmètre et base de calcul explicites |
| Critères existants associés | AC-09 |
| Décisions de baseline | Q-008, Q-021 |

## EF-REP-002 — Le système doit générer un rapport de dépenses

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit générer un rapport de dépenses. |
| Source | 4.7 Reporting; P0465 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-009, ACT-012 |
| Préconditions | WF-026: Rapport demandé pour une période |
| Workflows | WF-026 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-008, ENT-009, ENT-010, ENT-011, ENT-029 |
| Résultat attendu | Rapport disponible avec périmètre et base de calcul explicites |
| Critères existants associés | AC-09 |
| Décisions de baseline | Q-008, Q-021 |

## EF-REP-003 — Le système doit générer un rapport de consommation par assurance

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit générer un rapport de consommation par assurance. |
| Source | 4.7 Reporting; P0465 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-009, ACT-012 |
| Préconditions | WF-026: Rapport demandé pour une période |
| Workflows | WF-026 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-008, ENT-009, ENT-010, ENT-011, ENT-029 |
| Résultat attendu | Rapport disponible avec périmètre et base de calcul explicites |
| Critères existants associés | AC-09 |
| Décisions de baseline | Q-008, Q-021 |

## EF-REP-004 — Le système doit générer un rapport de consommation cash

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit générer un rapport de consommation cash. |
| Source | 4.7 Reporting; P0465 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-009, ACT-012 |
| Préconditions | WF-026: Rapport demandé pour une période |
| Workflows | WF-026 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-008, ENT-009, ENT-010, ENT-011, ENT-029 |
| Résultat attendu | Rapport disponible avec périmètre et base de calcul explicites |
| Critères existants associés | AC-09 |
| Décisions de baseline | Q-008, Q-021 |

## EF-REP-005 — La fréquence(mensuelle, à la demande selon la plage choisie par l’utilisateur…), le format d'export et le niveau de détail des rapports doivent être validés avant développement

| Champ | Valeur |
| --- | --- |
| Description source | La fréquence(mensuelle, à la demande selon la plage choisie par l’utilisateur…), le format d'export et le niveau de détail des rapports doivent être validés avant développement. |
| Source | 4.7 Reporting; P0465 |
| Priorité source | MVP |
| Statut source exact | Bloquant/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-009, ACT-012 |
| Préconditions | WF-026: Rapport demandé pour une période |
| Workflows | WF-026 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-008, ENT-009, ENT-010, ENT-011, ENT-029 |
| Résultat attendu | Rapport disponible avec périmètre et base de calcul explicites |
| Critères existants associés | AC-09 |
| Décisions de baseline | Q-008, Q-021 |

## EF-REP-006 — Aucun rapport médical de synthèse n'est confirmé par le cahier initial ; toute demande de reporting médical détaillé doit être arbitrée

| Champ | Valeur |
| --- | --- |
| Description source | Aucun rapport médical de synthèse n'est confirmé par le cahier initial ; toute demande de reporting médical détaillé doit être arbitrée. |
| Source | 4.7 Reporting; P0465 |
| Priorité source | Hors MVP |
| Statut source exact | À valider/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Hors périmètre détaillé : rapport médical non confirmé. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Hors périmètre détaillé : rapport médical non confirmé. |
| Critères existants associés | AC-09 |
| Décisions de baseline | Q-032 |

## EF-RH-001 — Le système doit permettre la gestion du personnel

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la gestion du personnel. |
| Source | 4.8 Gestion RH / Paie; P0494 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-007, ACT-012 |
| Préconditions | WF-027: Création ou mise à jour d’une fiche employé |
| Workflows | WF-027 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-003 |
| Résultat attendu | Fiche personnel exploitable selon champs validés |
| Critères existants associés | AC-10 |
| Décisions de baseline | Q-022, Q-025, Q-034 |

## EF-RH-002 — Le système doit permettre la gestion de la masse salariale

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la gestion de la masse salariale. |
| Source | 4.8 Gestion RH / Paie; P0494 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-007, ACT-011, ACT-012, ACT-014 |
| Préconditions | WF-028: Période de paie à traiter |
| Workflows | WF-028 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-003, ENT-014, ENT-026 |
| Résultat attendu | Bulletin produit et notification de paie selon calendrier retenu |
| Critères existants associés | AC-10 |
| Décisions de baseline | Q-014, Q-022, Q-026, Q-034 |

## EF-RH-003 — Le système doit permettre la génération d'une fiche de paie par salarié

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la génération d'une fiche de paie par salarié. |
| Source | 4.8 Gestion RH / Paie; P0494 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-007, ACT-011, ACT-012, ACT-014 |
| Préconditions | WF-028: Période de paie à traiter |
| Workflows | WF-028 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-003, ENT-014, ENT-026 |
| Résultat attendu | Bulletin produit et notification de paie selon calendrier retenu |
| Critères existants associés | AC-10 |
| Décisions de baseline | Q-014, Q-022, Q-026, Q-034 |

## EF-RH-004 — Le détail des données RH (contrat, présence, primes, retenues, charges, validations) doit être défini avant conception détaillée

| Champ | Valeur |
| --- | --- |
| Description source | Le détail des données RH (contrat, présence, primes, retenues, charges, validations) doit être défini avant conception détaillée. |
| Source | 4.8 Gestion RH / Paie; P0494 |
| Priorité source | MVP |
| Statut source exact | Bloquant/À determiner |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-007, ACT-011, ACT-012, ACT-014 |
| Préconditions | WF-027: Création ou mise à jour d’une fiche employé; WF-028: Période de paie à traiter |
| Workflows | WF-027, WF-028 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-003, ENT-014, ENT-026 |
| Résultat attendu | Fiche personnel exploitable selon champs validés; Bulletin produit et notification de paie selon calendrier retenu |
| Critères existants associés | AC-10 |
| Décisions de baseline | Q-014, Q-022, Q-025, Q-026, Q-034 |

## EF-STK-001 — Le système doit permettre la gestion des produits de pharmacie

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la gestion des produits de pharmacie. |
| Source | 4.9 Gestion de stock; P0515 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-008, ACT-012 |
| Préconditions | WF-029: Produit pharmacie ou bureautique à référencer |
| Workflows | WF-029 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-012 |
| Résultat attendu | Produit référencé |
| Critères existants associés | AC-11 |
| Décisions de baseline | Q-023 |

## EF-STK-002 — Le système doit permettre la gestion des produits de bureautique

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre la gestion des produits de bureautique. |
| Source | 4.9 Gestion de stock; P0515 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-008, ACT-012 |
| Préconditions | WF-029: Produit pharmacie ou bureautique à référencer |
| Workflows | WF-029 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-012 |
| Résultat attendu | Produit référencé |
| Critères existants associés | AC-11 |
| Décisions de baseline | Q-023 |

## EF-STK-003 — Le système doit permettre l'enregistrement des mouvements d'entrée et de sortie de stock dès validation du modèle métier

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre l'enregistrement des mouvements d'entrée et de sortie de stock dès validation du modèle métier. |
| Source | 4.9 Gestion de stock; P0515 |
| Priorité source | MVP |
| Statut source exact | Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-008, ACT-012 |
| Préconditions | WF-030: Approvisionnement, sortie ou consultation de disponibilité |
| Workflows | WF-030 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-012, ENT-013 |
| Résultat attendu | Mouvement enregistré et stock cohérent selon règle future |
| Critères existants associés | AC-11 |
| Décisions de baseline | Q-018, Q-023 |

## EF-STK-004 — Le système doit permettre le suivi du stock courant par produit

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre le suivi du stock courant par produit. |
| Source | 4.9 Gestion de stock; P0515 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-008, ACT-012 |
| Préconditions | WF-030: Approvisionnement, sortie ou consultation de disponibilité |
| Workflows | WF-030 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-012, ENT-013 |
| Résultat attendu | Mouvement enregistré et stock cohérent selon règle future |
| Critères existants associés | AC-11 |
| Décisions de baseline | Q-018, Q-023 |

## EF-STK-005 — Le besoin d'alertes de seuil, d'inventaires, de lots, de dates d'expiration et de valorisation doit être arbitré avant développement

| Champ | Valeur |
| --- | --- |
| Description source | Le besoin d'alertes de seuil, d'inventaires, de lots, de dates d'expiration et de valorisation doit être arbitré avant développement.(Permettre de rentrer les seuils de security) |
| Source | 4.9 Gestion de stock; P0515 |
| Priorité source | MVP |
| Statut source exact | Bloquant/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-008, ACT-012 |
| Préconditions | WF-031: Définition ou modification d’un seuil produit |
| Workflows | WF-031 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-012, ENT-013 |
| Résultat attendu | Seuil enregistré; mécanisme d’alerte reste ouvert |
| Critères existants associés | AC-11 |
| Décisions de baseline | Q-023 |

## EF-SEC-001 — Le système doit gérer les droits d'accès en fonction des rôles utilisateurs

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit gérer les droits d'accès en fonction des rôles utilisateurs. |
| Source | 4.10 Gestion des accès (RBAC); P0540 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-003, ACT-004, ACT-005, ACT-007, ACT-008, ACT-012 |
| Préconditions | WF-032: Accès à une fonction protégée; WF-033: Besoin de définir ou modifier des droits |
| Workflows | WF-032, WF-033 |
| Règles | BR-016 |
| Données | ENT-001, ENT-002, ENT-004, ENT-025 |
| Résultat attendu | Contexte d’accès établi; authentification détaillée classée TECHNICAL_PROPOSAL; Habilitations définies uniquement après arbitrage métier |
| Critères existants associés | AC-12 |
| Décisions de baseline | Q-002, Q-024, Q-025, Q-026, Q-031 |

## EF-SEC-002 — Le système doit empêcher tout utilisateur non médecin de renseigner le dossier médical confidentiel

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit empêcher tout utilisateur non médecin de renseigner le dossier médical confidentiel. |
| Source | 4.10 Gestion des accès (RBAC); P0540 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-009: Arrivée du patient pour consultation; WF-033: Besoin de définir ou modifier des droits |
| Workflows | WF-009, WF-033 |
| Règles | BR-002 |
| Données | ENT-001, ENT-002, ENT-004, ENT-006, ENT-008, ENT-015, ENT-025 |
| Résultat attendu | Constantes associées au contexte clinique, sous réserve de résolution du conflit; Habilitations définies uniquement après arbitrage métier |
| Critères existants associés | AC-12 |
| Décisions de baseline | Q-002, Q-011, Q-024, Q-025, Q-031 |

## EF-SEC-003 — Le système doit permettre une matrice de droits distincte par module

| Champ | Valeur |
| --- | --- |
| Description source | Le système doit permettre une matrice de droits distincte par module. |
| Source | 4.10 Gestion des accès (RBAC); P0540 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-012 |
| Préconditions | WF-033: Besoin de définir ou modifier des droits |
| Workflows | WF-033 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-001, ENT-002, ENT-025 |
| Résultat attendu | Habilitations définies uniquement après arbitrage métier |
| Critères existants associés | AC-12 |
| Décisions de baseline | Q-002, Q-024, Q-025, Q-031 |

## EF-SEC-004 — La liste finale des rôles, sous-rôles et permissions fines doit être validée avant développement

| Champ | Valeur |
| --- | --- |
| Description source | La liste finale des rôles, sous-rôles et permissions fines doit être validée avant développement.( Matrice RBAC à envoyer) |
| Source | 4.10 Gestion des accès (RBAC); P0540 |
| Priorité source | MVP |
| Statut source exact | Bloquant/À envoyer |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-012 |
| Préconditions | WF-033: Besoin de définir ou modifier des droits |
| Workflows | WF-033 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-001, ENT-002, ENT-025 |
| Résultat attendu | Habilitations définies uniquement après arbitrage métier |
| Critères existants associés | AC-12 |
| Décisions de baseline | Q-002, Q-024, Q-025, Q-031 |

## EF-PORT-001 — Le portail patient doit permettre l'inscription en ligne

| Champ | Valeur |
| --- | --- |
| Description source | Le portail patient doit permettre l'inscription en ligne. |
| Source | 4.11 Portail patient; P0672 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-001: Demande d’inscription au centre ou en ligne |
| Workflows | WF-001 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-005 |
| Résultat attendu | Inscription enregistrée; statut et numéro patient non spécifiés |
| Critères existants associés | AC-13 |
| Décisions de baseline | Q-011, Q-025 |

## EF-PORT-002 — Le portail patient doit permettre la prise de rendez-vous en ligne

| Champ | Valeur |
| --- | --- |
| Description source | Le portail patient doit permettre la prise de rendez-vous en ligne. |
| Source | 4.11 Portail patient; P0672 |
| Priorité source | MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-005: Demande de rendez-vous par patient ou accueil |
| Workflows | WF-005 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-007 |
| Résultat attendu | Rendez-vous planifié; statut exact non arrêté |
| Critères existants associés | AC-13 |
| Décisions de baseline | Q-013, Q-015, Q-025 |

## EF-PORT-003 — Le périmètre d'accès du patient à ses données administratives, médicales, financières ou documentaires doit être validé avant conception détaillée

| Champ | Valeur |
| --- | --- |
| Description source | Le périmètre d'accès du patient à ses données administratives, médicales, financières ou documentaires doit être validé avant conception détaillée. |
| Source | 4.11 Portail patient; P0672 |
| Priorité source | MVP |
| Statut source exact | Bloquant/Confirmed |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-005, ACT-012 |
| Préconditions | WF-023: Patient ouvre son espace personnel; WF-024: Patient demande une ordonnance; WF-025: Patient demande à obtenir son dossier |
| Workflows | WF-023, WF-024, WF-025 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-005, ENT-006, ENT-018, ENT-019, ENT-020, ENT-021, ENT-024 |
| Résultat attendu | Contenu consulté dans les limites décidées; Accès accordé ou expiré; ordonnance clinique non supprimée par cette règle; Décision enregistrable après définition; copie remise uniquement si acceptée |
| Critères existants associés | AC-13 |
| Décisions de baseline | Q-003, Q-004, Q-005, Q-006, Q-025, Q-028 |

## EF-PORT-004 — Toute exposition d'informations médicales ou de facturation au patient reste hors MVP tant qu'elle n'est pas explicitement validée

| Champ | Valeur |
| --- | --- |
| Description source | Toute exposition d'informations médicales ou de facturation au patient reste hors MVP tant qu'elle n'est pas explicitement validée. |
| Source | 4.11 Portail patient; P0672 |
| Priorité source | Hors MVP |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-005, ACT-012 |
| Préconditions | WF-023: Patient ouvre son espace personnel |
| Workflows | WF-023 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-005, ENT-006, ENT-018, ENT-019, ENT-020 |
| Résultat attendu | Contenu consulté dans les limites décidées |
| Critères existants associés | AC-13 |
| Décisions de baseline | Q-003, Q-005, Q-006, Q-025 |

## ENF-001 — La solution doit être une plateforme web accessible depuis n'importe quel appareil

| Champ | Valeur |
| --- | --- |
| Description source | La solution doit être une plateforme web accessible depuis n'importe quel appareil. |
| Source | 5.1 Exigences non fonctionnelles confirmées; P0694 |
| Priorité source | Non indiquée |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## ENF-002 — La solution doit protéger les données et la confidentialité des patients

| Champ | Valeur |
| --- | --- |
| Description source | La solution doit protéger les données et la confidentialité des patients. |
| Source | 5.1 Exigences non fonctionnelles confirmées; P0694 |
| Priorité source | Non indiquée |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-003, ACT-004, ACT-005, ACT-007, ACT-008, ACT-012 |
| Préconditions | WF-032: Accès à une fonction protégée |
| Workflows | WF-032 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-001, ENT-002, ENT-004 |
| Résultat attendu | Contexte d’accès établi; authentification détaillée classée TECHNICAL_PROPOSAL |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-025, Q-026, Q-033 |

## ENF-003 — La solution doit gérer les droits d'accès selon les rôles

| Champ | Valeur |
| --- | --- |
| Description source | La solution doit gérer les droits d'accès selon les rôles. |
| Source | 5.1 Exigences non fonctionnelles confirmées; P0694 |
| Priorité source | Non indiquée |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-003, ACT-004, ACT-005, ACT-007, ACT-008, ACT-012 |
| Préconditions | WF-032: Accès à une fonction protégée; WF-033: Besoin de définir ou modifier des droits |
| Workflows | WF-032, WF-033 |
| Règles | BR-016 |
| Données | ENT-001, ENT-002, ENT-004, ENT-025 |
| Résultat attendu | Contexte d’accès établi; authentification détaillée classée TECHNICAL_PROPOSAL; Habilitations définies uniquement après arbitrage métier |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-002, Q-024, Q-025, Q-026, Q-031, Q-033 |

## ENF-004 — La solution doit pouvoir s'intégrer avec d'autres systèmes

| Champ | Valeur |
| --- | --- |
| Description source | La solution doit pouvoir s'intégrer avec d'autres systèmes. |
| Source | 5.1 Exigences non fonctionnelles confirmées; P0694 |
| Priorité source | Non indiquée |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## ENF-005 — Le fournisseur doit assurer un support technique

| Champ | Valeur |
| --- | --- |
| Description source | Le fournisseur doit assurer un support technique. |
| Source | 5.1 Exigences non fonctionnelles confirmées; P0694 |
| Priorité source | Non indiquée |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## ENF-006 — Le fournisseur doit prévoir des mises à jour et améliorations

| Champ | Valeur |
| --- | --- |
| Description source | Le fournisseur doit prévoir des mises à jour et améliorations. |
| Source | 5.1 Exigences non fonctionnelles confirmées; P0694 |
| Priorité source | Non indiquée |
| Statut source exact | Confirmé |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-001 — Performance

| Champ | Valeur |
| --- | --- |
| Description source | Objectifs chiffrés de temps de réponse par parcours critique. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour architecture et tests de charge |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-002 — Disponibilité

| Champ | Valeur |
| --- | --- |
| Description source | Taux de disponibilité cible, plages de maintenance, fenêtres de service. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour hébergement et SLA |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-003 — Sécurité - authentification

| Champ | Valeur |
| --- | --- |
| Description source | Mode d'authentification, politique de mot de passe, MFA éventuel. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour conception sécurité |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-004 — Sécurité - chiffrement

| Champ | Valeur |
| --- | --- |
| Description source | Chiffrement au repos, en transit, gestion des clés. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour architecture sécurité |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-005 — Audit et traçabilité

| Champ | Valeur |
| --- | --- |
| Description source | Journal des accès, des consultations et des modifications sensibles. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour conformité et forensic |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-006 — Sauvegarde & reprise

| Champ | Valeur |
| --- | --- |
| Description source | RPO, RTO, fréquence de sauvegarde, tests de restauration. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour continuité d'activité |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-007 — Journalisation

| Champ | Valeur |
| --- | --- |
| Description source | Niveau de logs, rétention, journal applicatif vs sécurité. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour exploitation |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-008 — Scalabilité

| Champ | Valeur |
| --- | --- |
| Description source | Volume d'utilisateurs, patients, rendez-vous, factures, croissance annuelle. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour dimensionnement |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-009 — Compatibilité

| Champ | Valeur |
| --- | --- |
| Description source | Navigateurs supportés, responsive exact, OS minimum, contraintes terminaux. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour QA |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-010 — Maintenabilité

| Champ | Valeur |
| --- | --- |
| Description source | Normes de code, environnements, CI/CD, politique de versioning. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant pour industrialisation |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## NFR-011 — Support / SLA

| Champ | Valeur |
| --- | --- |
| Description source | Temps de prise en charge, temps de résolution, niveaux de criticité. |
| Source | 5.2 Exigences non fonctionnelles à définir avant développement; P0716 |
| Priorité source | Non indiquée |
| Statut source exact | Non spécifié. Impact source : Bloquant contractuel |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-026, Q-033 |

## ADD-001 — Constantes avant médecin

| Champ | Valeur |
| --- | --- |
| Description source | Le personnel paramédical prend les constantes avant la consultation médicale; consultation en attente visible au médecin. |
| Source | §2.2; §7.1; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-009: Arrivée du patient pour consultation |
| Workflows | WF-009 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-006, ENT-008, ENT-015 |
| Résultat attendu | Constantes associées au contexte clinique, sous réserve de résolution du conflit |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-002, Q-011 |

## ADD-002 — Accès ordonnance limité

| Champ | Valeur |
| --- | --- |
| Description source | L’accès du patient à l’ordonnance est limité à 15 jours; origine et borne non définies. |
| Source | §2.2 Patient; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-005, ACT-012 |
| Préconditions | WF-024: Patient demande une ordonnance |
| Workflows | WF-024 |
| Règles | BR-005 |
| Données | ENT-004, ENT-019 |
| Résultat attendu | Accès accordé ou expiré; ordonnance clinique non supprimée par cette règle |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-003, Q-004, Q-025 |

## ADD-003 — Copie sur demande acceptée

| Champ | Valeur |
| --- | --- |
| Description source | Le patient consulte son dossier; une copie nécessite une demande acceptée; le décideur est absent. |
| Source | commentaire 176, §11; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-005, ACT-012 |
| Préconditions | WF-023: Patient ouvre son espace personnel; WF-025: Patient demande à obtenir son dossier |
| Workflows | WF-023, WF-025 |
| Règles | BR-006 |
| Données | ENT-004, ENT-005, ENT-006, ENT-018, ENT-019, ENT-020, ENT-021, ENT-024 |
| Résultat attendu | Contenu consulté dans les limites décidées; Décision enregistrable après définition; copie remise uniquement si acceptée |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-003, Q-005, Q-006, Q-025, Q-028 |

## ADD-004 — Groupement de patients

| Champ | Valeur |
| --- | --- |
| Description source | La facturation assurance/mutuelle mentionne 10 patients par facture sans préciser plafond ou lot exact. |
| Source | §3.1 Facturation; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-006, ACT-012 |
| Préconditions | WF-018: Constitution d’une facture organisme payeur |
| Workflows | WF-018 |
| Règles | BR-007 |
| Données | ENT-004, ENT-008, ENT-009, ENT-011, ENT-022, ENT-023 |
| Résultat attendu | Facture organisme et parts à recouvrer identifiées |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-007, Q-008, Q-009, Q-029, Q-035 |

## ADD-005 — Annulation anticipée

| Champ | Valeur |
| --- | --- |
| Description source | L’annulation est possible au minimum 24 d’avance, unité absente; le patient peut reprendre rendez-vous. L’unité heure proposée dans le plan reste à confirmer. |
| Source | commentaire 171, §11; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012 |
| Préconditions | WF-008: Demande d’annulation ou nouveau rendez-vous |
| Workflows | WF-008 |
| Règles | BR-004 |
| Données | ENT-007 |
| Résultat attendu | Annulation enregistrée si autorisée; nouvelle réservation indépendante tant que lien non décidé |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-013, Q-015 |

## ADD-006 — Choix de canal

| Champ | Valeur |
| --- | --- |
| Description source | SMS, e-mail et WhatsApp sont mentionnés; le patient choisit le canal. |
| Source | commentaire 170, §11; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-005, ACT-012, ACT-014 |
| Préconditions | WF-007: Échéance de rappel à fixer |
| Workflows | WF-007 |
| Règles | BR-010 |
| Données | ENT-007, ENT-026, ENT-027 |
| Résultat attendu | Rappel transmis ou échec identifié; livraison effective non assimilée à acceptation technique |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-014, Q-026, Q-027 |

## ADD-007 — Notification de paie

| Champ | Valeur |
| --- | --- |
| Description source | L’employé est notifié le jour de paie; contenu et canal non précisés. |
| Source | §3.1 RH; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-007, ACT-011, ACT-012, ACT-014 |
| Préconditions | WF-028: Période de paie à traiter |
| Workflows | WF-028 |
| Règles | BR-011 |
| Données | ENT-003, ENT-014, ENT-026 |
| Résultat attendu | Bulletin produit et notification de paie selon calendrier retenu |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-014, Q-022, Q-026, Q-034 |

## ADD-008 — Rubriques de séjour

| Champ | Valeur |
| --- | --- |
| Description source | Facturation par chambre individuelle/double, visites médicales, soins infirmiers, pharmacie et examens; calcul non défini. |
| Source | §3.2; §7.3; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-002, ACT-003, ACT-004, ACT-012 |
| Préconditions | WF-012: Orientation médicale vers un séjour; WF-017: Facturation d’une hospitalisation |
| Workflows | WF-012, WF-017 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-009, ENT-016, ENT-017, ENT-022 |
| Résultat attendu | Séjour et prestations identifiés; admission/sortie détaillées non prêtes; Facture du séjour détaillée; montant non calculable contractuellement avant arbitrage |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-002, Q-009, Q-016, Q-020, Q-024, Q-035 |

## ADD-009 — Archivage après paiement

| Champ | Valeur |
| --- | --- |
| Description source | Toute facture payée est archivée; la notion de paiement complet reste à préciser. |
| Source | §7.4; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-012 |
| Préconditions | WF-021: Facture considérée comme payée |
| Workflows | WF-021 |
| Règles | BR-009 |
| Données | ENT-009, ENT-010, ENT-028 |
| Résultat attendu | Facture archivée si condition de paiement satisfaite |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-020, Q-029, Q-035 |

## ADD-010 — Pourcentage de prise en charge

| Champ | Valeur |
| --- | --- |
| Description source | Les quotes-parts sont exprimées en pourcentage; base de calcul et arrondis non définis. |
| Source | commentaire 167, §11; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-006, ACT-012 |
| Préconditions | WF-018: Constitution d’une facture organisme payeur; WF-020: Échéance ou règlement d’un organisme à rapprocher |
| Workflows | WF-018, WF-020 |
| Règles | BR-008 |
| Données | ENT-004, ENT-008, ENT-009, ENT-010, ENT-011, ENT-022, ENT-023, ENT-028 |
| Résultat attendu | Facture organisme et parts à recouvrer identifiées; Encours et écart identifiés; résolution suspendue aux règles financières |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-007, Q-008, Q-009, Q-019, Q-029, Q-035 |

## ADD-011 — Périodes des rapports

| Champ | Valeur |
| --- | --- |
| Description source | Rapports journaliers, hebdomadaires, mensuels, annuels et filtre personnalisé, par assurance, mutuelle ou particulier. |
| Source | commentaire 174, §11; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-009, ACT-012 |
| Préconditions | WF-026: Rapport demandé pour une période |
| Workflows | WF-026 |
| Règles | BR-018 |
| Données | ENT-008, ENT-009, ENT-010, ENT-011, ENT-029 |
| Résultat attendu | Rapport disponible avec périmètre et base de calcul explicites |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-008, Q-021 |

## ADD-012 — Conservation annoncée

| Champ | Valeur |
| --- | --- |
| Description source | Plus de 20 ans est indiqué sans préciser catégories de données ni déclencheur; ce n’est pas une vérification juridique. |
| Source | commentaire 169, §11; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | BR-015 |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-012 |

## ADD-013 — Saisie des résultats

| Champ | Valeur |
| --- | --- |
| Description source | Une assistante peut saisir les résultats; responsabilité et autorisation finale à déterminer. |
| Source | §4.4.3; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-010, ACT-012 |
| Préconditions | WF-013: Prestation de laboratoire à enregistrer |
| Workflows | WF-013 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-018, ENT-020 |
| Résultat attendu | Prestation enregistrée; résultat non automatiquement publié au portail |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-017, Q-027, Q-028 |

## ADD-014 — Accès FNE

| Champ | Valeur |
| --- | --- |
| Description source | FNE signifie Facture normalisée électronique de la DGI en Côte d’Ivoire; un bouton vers la plateforme est demandé. |
| Source | §4.5; §11; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-004, ACT-012, ACT-013 |
| Préconditions | WF-022: Utilisateur active le bouton FNE |
| Workflows | WF-022 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-009 |
| Résultat attendu | Plateforme externe ouverte, sans preuve automatique d’émission fiscale |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-010, Q-027 |

## ADD-015 — Paramédical et médicaments

| Champ | Valeur |
| --- | --- |
| Description source | Les constantes et médicaments sont cités pour l’intervention paramédicale, en conflit avec les restrictions générales. |
| Source | commentaire 173, §11; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-009: Arrivée du patient pour consultation |
| Workflows | WF-009 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-006, ENT-008, ENT-015 |
| Résultat attendu | Constantes associées au contexte clinique, sous réserve de résolution du conflit |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-002, Q-011 |

## ADD-016 — Moyens de règlement

| Champ | Valeur |
| --- | --- |
| Description source | Chèques, virements, Mobile Money, carte, espèces et paiement en ligne sont cités; la liste opérationnelle reste à arrêter. |
| Source | commentaire 168; §4.6; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-005, ACT-006, ACT-012, ACT-015 |
| Préconditions | WF-019: Règlement patient ou organisme reçu |
| Workflows | WF-019 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-009, ENT-010, ENT-011, ENT-028 |
| Résultat attendu | Paiement enregistré; règlement effectif distingué de simple initiation |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-019, Q-024, Q-029 |

## ADD-017 — Seuils de stock

| Champ | Valeur |
| --- | --- |
| Description source | Le système permet de renseigner les seuils de sécurité; déclenchement et destinataires des alertes non définis. |
| Source | §4.9; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-008, ACT-012 |
| Préconditions | WF-031: Définition ou modification d’un seuil produit |
| Workflows | WF-031 |
| Règles | BR-017 |
| Données | ENT-012, ENT-013 |
| Résultat attendu | Seuil enregistré; mécanisme d’alerte reste ouvert |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-023 |

## ADD-018 — Périmètre des dépendances

| Champ | Valeur |
| --- | --- |
| Description source | Tout doit être dans le même système et aucun système n’est indiqué; portée vis-à-vis des prestataires à confirmer. |
| Source | §8; commentaire 177; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | Transverse |
| Préconditions | Pas de scénario métier autonome |
| Workflows | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Règles | Règle détaillée non spécifiée |
| Données | Transverse / pas d’entité supplémentaire justifiée |
| Résultat attendu | Contrainte transverse; contrôle de conservation/intégration ou qualité, pas d’action utilisateur autonome. |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-027 |

## ADD-019 — Personnel administratif et finances

| Champ | Valeur |
| --- | --- |
| Description source | Le personnel administratif apparaît comme acteur de facturation et paiement, contrairement à la matrice provisoire. |
| Source | UC-07; UC-08; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-001, ACT-004, ACT-005, ACT-006, ACT-012, ACT-015 |
| Préconditions | WF-016: Prestations ambulatoires à facturer; WF-019: Règlement patient ou organisme reçu |
| Workflows | WF-016, WF-019 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-008, ENT-009, ENT-010, ENT-011, ENT-022, ENT-028 |
| Résultat attendu | Facture individuelle émise selon règles encore à compléter; Paiement enregistré; règlement effectif distingué de simple initiation |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-009, Q-019, Q-020, Q-024, Q-029, Q-035 |

## ADD-020 — Pièces jointes cliniques

| Champ | Valeur |
| --- | --- |
| Description source | Le dossier peut recevoir du texte et des pièces jointes; contraintes et diffusion non définies. |
| Source | commentaire 172; §4.3; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-010: Consultation en attente prise par un médecin |
| Workflows | WF-010 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-006, ENT-008, ENT-015, ENT-019, ENT-020 |
| Résultat attendu | Consultation enregistrée et disponible pour facturation |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-002, Q-016, Q-028 |

## ADD-021 — Spécialités de consultation

| Champ | Valeur |
| --- | --- |
| Description source | Médecine générale, cardiologie, nutrition, gynécologie, urologie et autres sont cités comme exemples de consultation, pas comme liste exhaustive. |
| Source | commentaire 0, §1.3; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-002, ACT-003, ACT-012 |
| Préconditions | WF-010: Consultation en attente prise par un médecin |
| Workflows | WF-010 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-004, ENT-006, ENT-008, ENT-015, ENT-019, ENT-020 |
| Résultat attendu | Consultation enregistrée et disponible pour facturation |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-002, Q-016, Q-028 |

## ADD-022 — Gestion avancée des achats

| Champ | Valeur |
| --- | --- |
| Description source | Achats, fournisseurs, inventaires tournants et valorisation comptable portent une annotation à intégrer dans une liste d’exclusions; portée et lot à arbitrer. |
| Source | §3.2; Voir commentaires ou texte courant |
| Priorité source | Non indiquée |
| Statut source exact | Annotation sourcée; autorité relative non arbitrée |
| Qualification | Exigence ou condition de décision issue du SRS; ne pas confondre acceptation et spécification complète |
| Acteurs | ACT-008, ACT-012 |
| Préconditions | WF-030: Approvisionnement, sortie ou consultation de disponibilité |
| Workflows | WF-030 |
| Règles | Règle détaillée non spécifiée |
| Données | ENT-012, ENT-013 |
| Résultat attendu | Mouvement enregistré et stock cohérent selon règle future |
| Critères existants associés | Aucun critère numéroté directement associé |
| Décisions de baseline | Q-018, Q-023 |

## Cas d’utilisation et critères acceptés

### Cas d’utilisation

| ID | Texte exact | Source |
| --- | --- | --- |
| UC-01 | Inscrire un patient | 2.3 Cas d'utilisation principaux |
| UC-02 | Créer et consulter un dossier patient | 2.3 Cas d'utilisation principaux |
| UC-03 | Planifier un rendez-vous | 2.3 Cas d'utilisation principaux |
| UC-04 | Confirmer et rappeler un rendez-vous | 2.3 Cas d'utilisation principaux |
| UC-05 | Renseigner le dossier médical | 2.3 Cas d'utilisation principaux |
| UC-06 | Enregistrer une prestation | 2.3 Cas d'utilisation principaux |
| UC-07 | Émettre une facture | 2.3 Cas d'utilisation principaux |
| UC-08 | Enregistrer un paiement | 2.3 Cas d'utilisation principaux |
| UC-09 | Générer un rapport financier | 2.3 Cas d'utilisation principaux |
| UC-10 | Gérer un produit de stock | 2.3 Cas d'utilisation principaux |

### Critères de recette

| ID | Texte exact | Source |
| --- | --- | --- |
| AC-01 | Un utilisateur administratif autorisé peut créer, modifier et consulter un dossier patient administratif. | 10. Critères d'acceptation |
| AC-02 | Un patient peut soumettre une inscription via une interface en ligne. | 10. Critères d'acceptation |
| AC-03 | Un rendez-vous peut être planifié, confirmé et marqué comme rappelé selon le canal validé. | 10. Critères d'acceptation |
| AC-04 | Un médecin peut consulter l'historique médical et renseigner le dossier médical confidentiel. | 10. Critères d'acceptation |
| AC-05 | Un utilisateur non médecin ne peut pas créer ou modifier le dossier médical confidentiel. | 10. Critères d'acceptation |
| AC-06 | Le système permet d'enregistrer une prestation de type consultation, hospitalisation, laboratoire, imagerie( échographie,...) ou pharmacie. | 10. Critères d'acceptation |
| AC-07 | Une facture peut être émise pour un patient particulier, une assurance ou une mutuelle. | 10. Critères d'acceptation |
| AC-08 | Le système permet d'enregistrer et de consulter un paiement patient ou assurance. | 10. Critères d'acceptation |
| AC-09 | Le système génère les rapports financiers de chiffre d'affaires, dépenses, consommation assurance et consommation cash. | 10. Critères d'acceptation |
| AC-10 | Le système permet la gestion du personnel, de la masse salariale et la génération d'une fiche de paie par salarié. | 10. Critères d'acceptation |
| AC-11 | Le système permet la gestion des produits de pharmacie et de bureautique, ainsi que le suivi du stock courant. | 10. Critères d'acceptation |
| AC-12 | Les droits d'accès sont appliqués selon la matrice RBAC validée. | 10. Critères d'acceptation |
| AC-13 | Le portail patient permet l'inscription et la prise de rendez-vous en ligne. | 10. Critères d'acceptation |
