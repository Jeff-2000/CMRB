# Registre des décisions de baseline

Ce registre conserve les 35 questions d'origine et les clôture pour la baseline fonctionnelle du 17 septembre 2026. `SOURCE_EXPLICITE` désigne une règle directement étayée; `DECISION_DE_CADRAGE` désigne un choix expert, réversible ou paramétrable lorsque possible. Une décision de cadrage n'est pas présentée comme une approbation antérieure du client.

La validation demandée au client porte sur le dossier consolidé dans son ensemble. Toute modification ultérieure suit la procédure de demande de changement.

## Q-001 — Quelle priorité accorder aux commentaires, révisions et texte contradictoire ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quelle priorité accorder aux commentaires, révisions et texte contradictoire ? |
| Source | Couverture; §1.5; statuts locaux |
| Exigences | EF-PAT-007 |
| Workflows | Transverse / aucun processus nouveau |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le texte courant du SRS reste la preuve source. Chaque commentaire ou révision est traité individuellement : il ne remplace le texte que lorsqu'une décision de cadrage l'adopte explicitement et en conserve la trace. |
| Type de décision | SOURCE_EXPLICITE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Gouvernance documentaire et traitement des changements. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-001 |

## Q-002 — Quels champs les paramédicaux peuvent-ils saisir, corriger et consulter ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quels champs les paramédicaux peuvent-ils saisir, corriger et consulter ? |
| Source | §2.2; §4.3; §4.10; commentaire 173 |
| Exigences | EF-DM-002 EF-DM-004 EF-SEC-002 |
| Workflows | WF-009, WF-010, WF-011, WF-012, WF-033 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le paramédical lit les données nécessaires à l'épisode actif et saisit les constantes, allergies signalées, observations de soins et administrations de médicaments prescrits. Il ne saisit ni diagnostic, ni prescription, ni compte rendu final. Avant validation médicale il corrige sa saisie; après validation, toute correction est un addendum tracé. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Sépare les actes de soins paramédicaux de la responsabilité diagnostique et prescriptive. |
| Conséquences fonctionnelles et techniques | RBAC, dossier clinique, consultation, audit et tests de modification. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-002 |

## Q-003 — Quelles données et versions sont visibles, pour quels patients et à partir de quel événement ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quelles données et versions sont visibles, pour quels patients et à partir de quel événement ? |
| Source | §2.2; §3.1; §4.11; commentaire 176 |
| Exigences | EF-DM-005 EF-PORT-003 EF-PORT-004 |
| Workflows | WF-011, WF-023, WF-024 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le portail expose au patient authentifié ses données d'identité, rendez-vous, factures, reçus, ordonnances signées encore visibles, résultats publiés et comptes rendus de sortie signés. Les brouillons, notes internes, données de tiers et journaux restent exclus. La visibilité commence à la publication et exige un lien compte-patient vérifié. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Applique minimisation, confidentialité et maîtrise de la publication. |
| Conséquences fonctionnelles et techniques | Portail, publication, identité, documents et sécurité objet. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-003 |

## Q-004 — Les 15 jours commencent-ils à la prescription, validation ou publication; que se passe-t-il à la limite exacte ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Les 15 jours commencent-ils à la prescription, validation ou publication; que se passe-t-il à la limite exacte ? |
| Source | §2.2 acteur Patient |
| Exigences | EF-PORT-003 |
| Workflows | WF-024 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | La fenêtre d'une ordonnance court de sa publication signée jusqu'à l'instant exclu publication + 15 jours calendaires, selon le fuseau Africa/Abidjan. L'expiration masque le document dans le portail sans supprimer le dossier clinique ni empêcher une demande formelle de copie. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Ordonnance, planification temporelle et portail. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-004 |

## Q-005 — Qui accepte/refuse, pour quels motifs, quel format et quel canal de remise ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Qui accepte/refuse, pour quels motifs, quel format et quel canal de remise ? |
| Source | Commentaire 176, §11 |
| Exigences | EF-PORT-003 |
| Workflows | WF-023, WF-025 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le médecin auteur ou le directeur médical délégué décide des copies cliniques; le responsable administratif décide des pièces administratives ou financières. La demande indique identité, périmètre et motif. La remise se fait en PDF protégé à lien unique valable 72 heures ou sous enveloppe scellée, avec preuve de remise. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Demande de copie, approbation, remise et preuve. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-005 |

## Q-006 — L’objectif porte-t-il sur la fonction de téléchargement ou sur toute reproduction ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | L’objectif porte-t-il sur la fonction de téléchargement ou sur toute reproduction ? |
| Source | Commentaire 176 |
| Exigences | EF-PORT-003 |
| Workflows | WF-023, WF-025 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le système contrôle la délivrance côté serveur, les URL temporaires, l'authentification, le filigrane et le journal de téléchargement. Il n'affirme pas empêcher une photographie ou une capture d'écran; cette limite est affichée et couverte par les règles d'usage. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Téléchargement, stockage, journalisation et information utilisateur. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-006 |

## Q-007 — Est-ce exactement 10, un maximum de 10, ou un exemple; par organisme et par période ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Est-ce exactement 10, un maximum de 10, ou un exemple; par organisme et par période ? |
| Source | §3.1 Facturation |
| Exigences | EF-FAC-002 EF-FAC-003 |
| Workflows | WF-018 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Une facture destinée à un organisme regroupe au maximum dix patients pour un même organisme et une même période de facturation. Un lot incomplet est autorisé. Chaque patient, prestation et montant reste identifiable par une ligne distincte. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Agrégation de factures organisme et traçabilité patient. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-007 |

## Q-008 — Un même type d’organisme couvre-t-il assurance et mutuelle, avec ou sans catégorie distincte ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Un même type d’organisme couvre-t-il assurance et mutuelle, avec ou sans catégorie distincte ? |
| Source | §1.3; §4.5 |
| Exigences | EF-FAC-003 EF-FAC-006 |
| Workflows | WF-018, WF-026 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Assurance et mutuelle partagent l'entité Organisme payeur, avec une catégorie obligatoire ASSURANCE, MUTUELLE ou AUTRE. L'identité, les conventions et les comptes sont communs; les rapports et règles de couverture restent séparables par catégorie. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Modèle de payeur, conventions et reporting. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-008 |

## Q-009 — Sur quelle base calculer les pourcentages, arrondis, plafonds, exceptions et reste patient ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Sur quelle base calculer les pourcentages, arrondis, plafonds, exceptions et reste patient ? |
| Source | Commentaire 167; §7.5; §12 |
| Exigences | EF-PAI-005 EF-FAC-006 |
| Workflows | WF-016, WF-017, WF-018, WF-020 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | La couverture est calculée par ligne éligible : montant couvert = minimum(base éligible après remises × taux, plafond restant), puis exclusions. Les montants sont arrondis au franc CFA le plus proche, méthode demi-supérieure. Le patient supporte le reste. Une seule couverture principale est gérée en V1; les cumuls relèvent d'un changement ultérieur. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Lignes de facture, couverture et reste patient. |
| Risque résiduel | Modéré; revue juridique, fiscale ou métier ciblée avant mise en production, sans bloquer la conception ni le développement. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-009 |

## Q-010 — Le bouton ouvre-t-il seulement la plateforme ou transmet-il aussi des informations ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Le bouton ouvre-t-il seulement la plateforme ou transmet-il aussi des informations ? |
| Source | §1.3; §4.5; §8; §11 |
| Exigences | EF-FAC-004 |
| Workflows | WF-022 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | La V1 ouvre la plateforme FNE de la DGI dans un nouvel onglet et conserve dans CMRB le numéro FNE, le QR ou justificatif et l'état de rapprochement saisis par un utilisateur habilité. Aucune donnée n'est transmise automatiquement. L'API FNE est un lot ultérieur soumis au guide DGI et à l'agrément applicable. |
| Type de décision | SOURCE_EXPLICITE |
| Justification | Respecte le besoin source d'un lien tout en évitant de simuler une certification fiscale. |
| Conséquences fonctionnelles et techniques | Workflow FNE, preuve fiscale et intégrations. |
| Risque résiduel | Modéré; revue juridique, fiscale ou métier ciblée avant mise en production, sans bloquer la conception ni le développement. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-010 |

## Q-011 — Quels champs, justificatifs, règles d’unicité et traitement des homonymes sont requis par canal ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quels champs, justificatifs, règles d’unicité et traitement des homonymes sont requis par canal ? |
| Source | §4.1; §11 |
| Exigences | EF-PAT-007 |
| Workflows | WF-001, WF-002, WF-003, WF-009 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | La création exige nom, prénoms, date de naissance, sexe administratif, au moins un téléphone ou e-mail et le canal de contact. Adresse, pièce d'identité et contact d'urgence sont facultatifs sauf exigence opérationnelle. Le système attribue un identifiant interne immuable, signale les doublons sur identité normalisée, naissance et contact, et interdit toute fusion automatique. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Formulaires patient, doublons et dictionnaire. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-011 |

## Q-012 — Quelles durées par donnée, quel déclencheur, gel, archivage et destruction autorisée ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quelles durées par donnée, quel déclencheur, gel, archivage et destruction autorisée ? |
| Source | §4.1; commentaire 169 |
| Exigences | EF-PAT-006 ENF-002 |
| Workflows | WF-004 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Aucune suppression physique automatique n'est autorisée. Les dossiers cliniques sont conservés 25 ans après le dernier épisode; les dossiers de mineurs au moins jusqu'au 28e anniversaire et jamais moins de 25 ans après le dernier épisode. Les pièces financières sont conservées 10 ans, les données RH 10 ans après départ, les journaux de sécurité 12 mois et les traces d'accès clinique 10 ans. Un gel juridique suspend toute échéance. À terme, anonymisation irréversible après autorisation du responsable désigné. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Privilégie la conservation clinique et interdit une destruction automatisée juridiquement risquée. |
| Conséquences fonctionnelles et techniques | Archivage, anonymisation, gel et politiques de rétention. |
| Risque résiduel | Modéré; revue juridique, fiscale ou métier ciblée avant mise en production, sans bloquer la conception ni le développement. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-012 |

## Q-013 — Confirmez-vous l’unité heure, la limite inclusive, les acteurs, exceptions et effet d’un report ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Confirmez-vous l’unité heure, la limite inclusive, les acteurs, exceptions et effet d’un report ? |
| Source | Commentaire 171; §4.2 |
| Exigences | EF-RDV-007 |
| Workflows | WF-005, WF-008 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | L'annulation autonome du patient est permise jusqu'à 24 heures incluses avant le début prévu. À moins de 24 heures, l'accueil traite la demande et consigne le motif. Le report annule l'ancien créneau et crée un nouveau rendez-vous lié. La réservation est transactionnelle et interdit le double-booking, sauf dérogation nominative tracée par un responsable. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Agenda, annulation, report et concurrence. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-013 |

## Q-014 — Combien de rappels, à quel moment, avec quel contenu et quel repli en cas d’échec ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Combien de rappels, à quel moment, avec quel contenu et quel repli en cas d’échec ? |
| Source | §4.2; commentaire 170 |
| Exigences | EF-RDV-003 EF-RDV-005 |
| Workflows | WF-006, WF-007, WF-028 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Deux rappels sont planifiés à 48 heures puis 24 heures avant le rendez-vous, par canal vérifié choisi entre SMS, e-mail et WhatsApp. En cas d'échec, deux nouvelles tentatives sont effectuées puis un repli SMS, ou e-mail si aucun mobile n'est vérifié. Aucun contenu clinique n'est envoyé et les rappels cessent après annulation ou arrivée. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Notifications, consentement de canal et reprise. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-014 |

## Q-015 — Quels agendas, ressources, durées, doublons, absences et statuts sont nécessaires ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quels agendas, ressources, durées, doublons, absences et statuts sont nécessaires ? |
| Source | §4.2 |
| Exigences | EF-RDV-001 EF-RDV-006 |
| Workflows | WF-005, WF-006, WF-008 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | L'agenda est géré par praticien et ressource obligatoire éventuelle. La durée provient du type de rendez-vous et reste paramétrable. Les états sont DEMANDE, À_CONFIRMER, CONFIRMÉ, ARRIVÉ, EN_COURS, TERMINÉ, ANNULÉ_PATIENT, ANNULÉ_CMRB, ABSENT et REPORTÉ. Les absences, congés, conflits et surbooking exceptionnel sont tracés. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Agenda, ressources, états et disponibilité. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-015 |

## Q-016 — Quelles admissions, chambres, durées, transferts, sorties et différences observation/hospitalisation ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quelles admissions, chambres, durées, transferts, sorties et différences observation/hospitalisation ? |
| Source | §3.2; §4.4.2; §7.3 |
| Exigences | EF-SRV-HOSP-002 |
| Workflows | WF-010, WF-012, WF-017 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le médecin décide observation ou hospitalisation. Le séjour comprend admission, affectation chambre/lit, transferts historisés, épisodes de soins, sortie signée et clôture administrative. L'observation peut rester sans lit permanent. La facture détaille chambre par nuit, visites, soins infirmiers, pharmacie, laboratoire, imagerie et autres prestations réellement enregistrées. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Séjour, chambre, soins, sortie et facturation. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-016 |

## Q-017 — Qui saisit, valide, corrige et publie les résultats et comptes rendus ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Qui saisit, valide, corrige et publie les résultats et comptes rendus ? |
| Source | §4.4.3; §4.4.4 |
| Exigences | EF-SRV-LAB-002 EF-SRV-IMG-002 |
| Workflows | WF-013, WF-014 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le technicien ou l'assistante habilitée saisit un brouillon de résultat; le responsable du service ou médecin habilité le valide; le médecin prescripteur ou le valideur autorisé le publie. Après validation, aucune modification destructive : une correction crée une nouvelle version et un addendum motivé. Seule la version publiée est visible au patient. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Laboratoire, imagerie, versions et publication. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-017 |

## Q-018 — Quand une dispensation décrémente-t-elle le stock et devient-elle facturable; comment gérer retour ou annulation ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quand une dispensation décrémente-t-elle le stock et devient-elle facturable; comment gérer retour ou annulation ? |
| Source | §4.4.5; §3.2 |
| Exigences | EF-SRV-PHA-002 |
| Workflows | WF-015, WF-030 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le stock est décrémenté et la ligne devient facturable lors de la confirmation de dispensation. Une réservation ne décrémente pas le stock. Un retour admissible crée un mouvement inverse et un avoir; un médicament délivré non réintégrable reste sorti. Toute annulation après dispensation passe par une opération de contrepassation, jamais par suppression. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Dispensation, mouvements, facturation et avoirs. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-018 |

## Q-019 — Quels moyens au lancement; saisie manuelle ou intégration; quelle preuve et quel traitement des rejets ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quels moyens au lancement; saisie manuelle ou intégration; quelle preuve et quel traitement des rejets ? |
| Source | §4.6; commentaire 168 |
| Exigences | EF-PAI-004 EF-PAI-005 |
| Workflows | WF-019, WF-020 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | La V1 accepte espèces, virement bancaire et mobile money enregistrés manuellement. Chaque paiement porte montant, date, payeur, mode, référence et justificatif éventuel. Les statuts sont EN_ATTENTE, CONFIRMÉ, REJETÉ, ANNULÉ et REMBOURSÉ. Cartes, PayPal, Stripe et confirmation automatique sont hors V1. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Caisse, justificatifs, états et rapprochement. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-019 |

## Q-020 — Payée signifie-t-il solde nul toutes parts comprises; que permet l’archivage, puis un remboursement ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Payée signifie-t-il solde nul toutes parts comprises; que permet l’archivage, puis un remboursement ? |
| Source | §7.4; §4.5 |
| Exigences | EF-FAC-005 |
| Workflows | WF-016, WF-017, WF-021 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Une facture est PAYÉE lorsque les paiements confirmés et avoirs imputés couvrent toutes les parts dues. Un trop-perçu crée un crédit ou un remboursement tracé. L'archivage rend la facture non modifiable mais consultable. Un remboursement ou avoir postérieur conserve l'original, crée une écriture inverse et recalcule le solde. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Cycle facture, archive, crédits et remboursements. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-020 |

## Q-021 — Quelle base CA, consommation et dépenses; date de service, facture ou paiement; formats attendus ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quelle base CA, consommation et dépenses; date de service, facture ou paiement; formats attendus ? |
| Source | §4.7; commentaire 174 |
| Exigences | EF-REP-001 EF-REP-002 EF-REP-003 EF-REP-004 EF-REP-005 |
| Workflows | WF-026 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Les rapports distinguent comptabilité d'engagement par date de prestation/facture et trésorerie par date de paiement. La période mensuelle est proposée par défaut, avec plage libre. Les filtres couvrent payeur, catégorie, service, prestation, praticien et statut. Les exports autorisés sont PDF et CSV; les dépenses suivent leur date de comptabilisation. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Indicateurs, périodes, filtres et exports. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-021 |

## Q-022 — Quel lot pour RH/paie, formule, période, validations, confidentialité et date déclenchant la notification ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quel lot pour RH/paie, formule, période, validations, confidentialité et date déclenchant la notification ? |
| Source | §3.1; §4.8; commentaires 115 et 175 |
| Exigences | EF-RH-001 EF-RH-002 EF-RH-003 EF-RH-004 |
| Workflows | WF-027, WF-028 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | La V1 RH couvre registre du personnel, contrat, période, montants de base, primes, retenues, brut, net et bulletin. Elle ne calcule pas automatiquement des règles sociales ou fiscales non fournies. Le RH prépare, la comptabilité contrôle, la direction approuve; le bulletin est verrouillé puis l'employé est notifié à la date de paiement enregistrée. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Évite d'inventer les calculs sociaux et fiscaux tout en livrant le processus documentaire demandé. |
| Conséquences fonctionnelles et techniques | RH, paie, approbation, confidentialité et notification. |
| Risque résiduel | Modéré; revue juridique, fiscale ou métier ciblée avant mise en production, sans bloquer la conception ni le développement. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-022 |

## Q-023 — Quels achats, fournisseurs, unités, inventaires, seuils, lots, péremption et alertes sont requis ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quels achats, fournisseurs, unités, inventaires, seuils, lots, péremption et alertes sont requis ? |
| Source | §3.2; §4.9 |
| Exigences | EF-STK-003 EF-STK-005 |
| Workflows | WF-015, WF-029, WF-030, WF-031 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le stock gère produits, catégories, unités, fournisseurs, réceptions, sorties, retours, ajustements et inventaires. Lot et péremption sont obligatoires pour les médicaments et facultatifs pour la bureautique. La sortie applique FEFO, les seuils sont définis par produit et emplacement, et la valorisation V1 utilise le coût moyen pondéré. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Lots, péremption, inventaire, seuils et valorisation. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-023 |

## Q-024 — Quelles actions de facture et paiement sont autorisées à l’accueil ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quelles actions de facture et paiement sont autorisées à l’accueil ? |
| Source | UC-07 UC-08; §4.10 |
| Exigences | EF-SEC-004 EF-FAC-001 EF-PAI-001 |
| Workflows | WF-002, WF-016, WF-017, WF-019, WF-033 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | L'accueil peut créer une facture brouillon à partir des prestations enregistrées, encaisser une part patient par mode autorisé et imprimer un reçu. Il ne modifie ni tarifs ni couverture, ne valide pas les bordereaux organisme, ne rembourse pas et n'annule pas une facture émise. La comptabilité émet, rapproche, crée les avoirs et traite remboursements et rejets. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Séparation des tâches accueil/comptabilité. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-024 |

## Q-025 — Comment créer, vérifier, attribuer et retirer un accès; prouver le lien compte-patient; gérer les sessions ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Comment créer, vérifier, attribuer et retirer un accès; prouver le lien compte-patient; gérer les sessions ? |
| Source | §5.2; §4.10; §6.1 |
| Exigences | EF-SEC-001 ENF-002 |
| Workflows | WF-001, WF-002, WF-003, WF-004, WF-005, WF-011, WF-023, WF-024, WF-025, WF-027, WF-032, WF-033 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Chaque personne possède un compte nominatif et des rôles cumulables approuvés par un administrateur désigné par la direction. Le premier lien patient exige date de naissance, code à usage unique sur contact vérifié et validation manuelle en cas d'écart. MFA est obligatoire pour comptes internes sensibles; inactivité 15 minutes, durée maximale 12 heures, révocation immédiate. Un accès d'urgence médical exige motif et alerte au directeur médical. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Comptes, sessions, MFA, liaison patient et accès d'urgence. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-025 |

## Q-026 — Quels volumes, p95, disponibilité, RPO/RTO, rétention logs, restauration, navigateurs et SLA ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quels volumes, p95, disponibilité, RPO/RTO, rétention logs, restauration, navigateurs et SLA ? |
| Source | §5.2; commentaire 114 |
| Exigences | ENF-001 ENF-002 ENF-005 ENF-006 |
| Workflows | WF-007, WF-028, WF-032 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Cibles V1 : p95 ≤ 2 s pour les actions courantes et ≤ 10 s pour les rapports; disponibilité mensuelle 99,5 % hors maintenance annoncée limitée à 4 h/mois; RPO 15 min et RTO 4 h; sauvegardes chiffrées quotidiennes 35 jours et mensuelles 12 mois; 200 utilisateurs simultanés, 100 000 patients et 20 % de croissance annuelle; navigateurs majeurs sur leurs deux dernières versions; SLA P1 prise en charge 30 min et contournement 4 h. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Fournit des seuils V1 mesurables, proportionnés à un centre médical unique. |
| Conséquences fonctionnelles et techniques | Architecture, exploitation, tests de charge, reprise et support. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-026 |

## Q-027 — Aucun logiciel métier tiers, ou aucune dépendance même pour SMS et paiement ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Aucun logiciel métier tiers, ou aucune dépendance même pour SMS et paiement ? |
| Source | §8; commentaire 177 |
| Exigences | ENF-004 |
| Workflows | WF-007, WF-013, WF-022 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Les modules métier cœur sont réunis dans CMRB. Les services externes nécessaires restent autorisés derrière des adaptateurs : FNE, SMS/e-mail/WhatsApp, mobile money, hébergement, antivirus et identité. Leur indisponibilité ne doit pas corrompre une transaction; les échanges sont mis en attente, réessayés et rapprochés. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Architecture d'intégration et résilience. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-027 |

## Q-028 — Quels fichiers, taille, version, validation de contenu et règles de téléchargement ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quels fichiers, taille, version, validation de contenu et règles de téléchargement ? |
| Source | §4.3; commentaire 172 |
| Exigences | EF-DM-004 |
| Workflows | WF-003, WF-010, WF-011, WF-013, WF-014, WF-025 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Les pièces jointes V1 acceptent PDF, JPEG et PNG, 10 Mo maximum par fichier. Le système vérifie extension, type MIME, signature, taille et antivirus, calcule SHA-256, chiffre le stockage et interdit l'exécution. Les versions sont immuables; validation, publication, remplacement par nouvelle version et téléchargement sont autorisés selon rôle et ressource. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Documents, sécurité, versions et droits. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-028 |

## Q-029 — Quel niveau d’affectation d’un règlement et d’identification de chaque ligne ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quel niveau d’affectation d’un règlement et d’identification de chaque ligne ? |
| Source | §6.2; §3.1; §4.6 |
| Exigences | EF-FAC-002 EF-PAI-003 |
| Workflows | WF-018, WF-019, WF-020, WF-021 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Chaque règlement est imputé explicitement à une ou plusieurs factures et, si nécessaire, à leurs lignes. Une zone d'attente comptable temporaire est permise mais doit être apurée. L'enregistrement exige payeur, montant, devise XOF, date, mode, référence unique et clé d'idempotence. La ventilation ne détruit jamais l'écriture d'origine. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Paiements, imputations, unicité et rapprochement. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-029 |

## Q-030 — Valider le glossaire harmonisé sans modifier les citations sources.

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Valider le glossaire harmonisé sans modifier les citations sources. |
| Source | Glossaire; acteurs; statuts |
| Exigences | EF-FAC-006 |
| Workflows | Transverse / aucun processus nouveau |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le glossaire harmonisé est adopté : Patient, Dossier administratif, Dossier médical, Épisode, Prestation, Facture, Ligne de facture, Paiement, Imputation, Organisme payeur et Document sont des concepts distincts. Les citations sources restent inchangées. |
| Type de décision | SOURCE_EXPLICITE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Terminologie, données et API. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-030 |

## Q-031 — Confirmer la décomposition technique des capacités pour appliquer les droits existants.

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Confirmer la décomposition technique des capacités pour appliquer les droits existants. |
| Source | §4.10; §5.1 |
| Exigences | EF-SEC-001 ENF-003 |
| Workflows | WF-033 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Les permissions sont décomposées par action créer, lire, modifier, valider, publier, annuler, rembourser, exporter et administrer, puis contrôlées côté serveur sur l'action et la ressource. Le droit au module n'accorde aucun droit implicite sur toutes ses données. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | RBAC fin et contrôles serveur. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-031 |

## Q-032 — Souhaitez-vous ouvrir des demandes de changement distinctes pour ces capacités ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Souhaitez-vous ouvrir des demandes de changement distinctes pour ces capacités ? |
| Source | §3.2 |
| Exigences | EF-REP-006 |
| Workflows | Transverse / aucun processus nouveau |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Les fonctions non retenues en V1 deviennent des demandes de changement distinctes : API FNE, paiement en ligne automatisé, interopérabilité HL7/FHIR/DICOM, télémédecine, application mobile native, moteur complet de paie, multi-site et rapports médicaux avancés. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Périmètre V1 et backlog contractuel. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-032 |

## Q-033 — Quel cadre applicable, lieu d’hébergement, données à reprendre, validation et procédure de bascule ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quel cadre applicable, lieu d’hébergement, données à reprendre, validation et procédure de bascule ? |
| Source | §9.2; §11 |
| Exigences | ENF-002 |
| Workflows | Transverse / aucun processus nouveau |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | La production et les sauvegardes sont hébergées dans une zone approuvée contractuellement, avec préférence Côte d'Ivoire; tout transfert hors territoire exige l'analyse et les formalités applicables. La reprise V1 utilise des modèles CSV contrôlés, rapprochement des totaux et procès-verbal. La bascule suit répétition, gel, sauvegarde, migration, contrôle, décision go/no-go et retour arrière. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Rend la migration et le transfert de données contrôlables sans présumer d'un hébergeur. |
| Conséquences fonctionnelles et techniques | Hébergement, migration, bascule et retour arrière. |
| Risque résiduel | Modéré; revue juridique, fiscale ou métier ciblée avant mise en production, sans bloquer la conception ni le développement. |
| Priorité historique | P1 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-033 |

## Q-034 — Quels lots, échéances, responsables de validation et conditions de passage en développement ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quels lots, échéances, responsables de validation et conditions de passage en développement ? |
| Source | §11; périmètre §3 |
| Exigences | EF-RH-004 |
| Workflows | WF-027, WF-028 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Le plan de référence dure 24 semaines : cadrage 2, conception 4, construction 10, intégration/QA 4, recette-déploiement 2 et hypercare 2. Chaque jalon possède critères d'entrée/sortie; le client répond sous 5 jours ouvrés. Un retard de dépendance client décale le jalon sans modifier silencieusement le périmètre. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Lots, jalons, dépendances et recette. |
| Risque résiduel | Faible; revue client globale et recette couvrent les écarts. |
| Priorité historique | P2 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-034 |

## Q-035 — Quels tarifs et dates d’effet, devise, arrondis, taxes, numéros, annulations, avoirs et corrections après émission ?

| Champ | Valeur |
| --- | --- |
| Type | DECISION_RECORD |
| Question d'origine | Quels tarifs et dates d’effet, devise, arrondis, taxes, numéros, annulations, avoirs et corrections après émission ? |
| Source | §4.5; §7.4 |
| Exigences | EF-FAC-001 EF-FAC-005 |
| Workflows | WF-016, WF-017, WF-018, WF-021 |
| Enjeu historique | Ambiguïté recensée pendant la revue |
| Décision retenue | Les tarifs sont versionnés avec date d'effet et devise XOF sans décimales. Les taxes et exonérations sont des codes configurables. Une facture émise est immuable; correction par avoir puis nouvelle facture. La séquence interne et le numéro officiel FNE sont distincts, uniques et conservés. Remises, annulations et remboursements exigent motif, habilitation et piste d'audit. |
| Type de décision | DECISION_DE_CADRAGE |
| Justification | Choix V1 sûr, testable, paramétrable lorsque pertinent et limitant le risque de reprise. |
| Conséquences fonctionnelles et techniques | Tarification, taxes, numérotation et corrections. |
| Risque résiduel | Modéré; revue juridique, fiscale ou métier ciblée avant mise en production, sans bloquer la conception ni le développement. |
| Priorité historique | P0 |
| Statut | CLOSED_FOR_BASELINE |
| Décision / date / preuve | 17 septembre 2026; baseline experte CMRB; dossier global et présent registre |
| Revue | REV-035 |

