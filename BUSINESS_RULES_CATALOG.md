# Règles métier de la baseline

Les règles ci-dessous sont actives pour la V1. Les formulations sources restent dans le catalogue des exigences; les ajouts sont des `DECISION_DE_CADRAGE` reliées au registre Q-001 à Q-035.

## BR-001 — Séparer données administratives et cliniques

Les dossiers administratif et médical utilisent des permissions et des données distinctes; aucun droit administratif n'accorde un accès clinique.

Source : EF-PAT-005 EF-DM-003. Statut : CLOSED_FOR_BASELINE. Workflows : WF-002, WF-003, WF-011.

## BR-002 — Encadrer l'écriture clinique

Les médecins rédigent diagnostic, prescription et conclusion. Les paramédicaux saisissent constantes, observations de soins et administrations prescrites selon Q-002.

Source : EF-DM-002 EF-SEC-002 ADD-001 ADD-015. Statut : CLOSED_FOR_BASELINE. Workflows : WF-009, WF-010, WF-033.

## BR-003 — Interdire la suppression destructive

Aucun dossier clinique n'est supprimé physiquement; archivage, gel et anonymisation suivent Q-012.

Source : EF-PAT-006 ADD-012. Statut : CLOSED_FOR_BASELINE. Workflows : WF-004.

## BR-004 — Appliquer le délai d'annulation

L'annulation autonome est permise jusqu'à 24 heures incluses avant le rendez-vous; ensuite l'accueil intervient et motive l'opération.

Source : ADD-005. Statut : CLOSED_FOR_BASELINE. Workflows : WF-008.

## BR-005 — Limiter la visibilité d'une ordonnance

Une ordonnance publiée est visible pendant 15 jours calendaires selon Q-004 sans suppression de la preuve clinique.

Source : ADD-002. Statut : CLOSED_FOR_BASELINE. Workflows : WF-024.

## BR-006 — Remettre une copie après décision habilitée

La copie est délivrée après contrôle d'identité et décision selon Q-005, par lien temporaire ou remise scellée.

Source : ADD-003. Statut : CLOSED_FOR_BASELINE. Workflows : WF-023, WF-025.

## BR-007 — Limiter le groupement organisme

Une facture organisme regroupe au maximum dix patients d'un même organisme et d'une même période, avec détail par patient.

Source : ADD-004. Statut : CLOSED_FOR_BASELINE. Workflows : WF-018.

## BR-008 — Calculer la couverture par ligne

La quote-part suit la formule, les plafonds, exclusions et arrondis définis dans Q-009.

Source : ADD-010. Statut : CLOSED_FOR_BASELINE. Workflows : WF-018, WF-020.

## BR-009 — Archiver une facture soldée

Une facture soldée est verrouillée et archivée; les corrections passent par avoir, remboursement ou nouvelle facture.

Source : ADD-009. Statut : CLOSED_FOR_BASELINE. Workflows : WF-021.

## BR-010 — Respecter le canal de rappel

Le patient choisit un canal vérifié; le calendrier, les tentatives et le repli suivent Q-014.

Source : ADD-006. Statut : CLOSED_FOR_BASELINE. Workflows : WF-007.

## BR-011 — Notifier la paie approuvée

L'employé est notifié à la date de paiement d'un bulletin approuvé et verrouillé.

Source : ADD-007. Statut : CLOSED_FOR_BASELINE. Workflows : WF-028.

## BR-012 — Facturer individuellement l'ambulatoire

Chaque patient ambulatoire reçoit une facture individuelle; le groupement concerne les bordereaux organisme.

Source : EF-FAC-001. Statut : CLOSED_FOR_BASELINE. Workflows : WF-016, WF-017.

## BR-013 — Conserver les catégories de prestations

Consultation, hospitalisation, imagerie, laboratoire et pharmacie utilisent un socle commun de prestation et des détails spécialisés.

Source : EF-SRV-TRA-001. Statut : CLOSED_FOR_BASELINE. Workflows : WF-016.

## BR-014 — Conserver l'historique des paiements

Toute opération de paiement, rejet, imputation, remboursement et contrepassation reste consultable et non destructive.

Source : EF-PAI-003. Statut : CLOSED_FOR_BASELINE. Workflows : WF-019.

## BR-015 — Appliquer la politique de conservation

Les durées, gels et anonymisations sont celles de Q-012 et restent configurables sans autoriser une destruction silencieuse.

Source : ADD-012. Statut : CLOSED_FOR_BASELINE. Workflows : Transverse.

## BR-016 — Contrôler chaque action et ressource

Les droits sont décomposés par action et vérifiés côté serveur selon Q-031.

Source : EF-SEC-001 ENF-003. Statut : CLOSED_FOR_BASELINE. Workflows : WF-032, WF-033.

## BR-017 — Alerter sur les seuils de stock

Chaque produit et emplacement possède un seuil; l'alerte ne modifie jamais automatiquement le stock.

Source : ADD-017. Statut : CLOSED_FOR_BASELINE. Workflows : WF-031.

## BR-018 — Distinguer engagement et trésorerie

Les rapports appliquent les dates, filtres et formats définis par Q-021.

Source : ADD-011. Statut : CLOSED_FOR_BASELINE. Workflows : WF-026.

