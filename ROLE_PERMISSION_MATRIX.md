# Matrice définitive des rôles et actions

**C** créer, **L** lire, **M** modifier, **V** valider, **P** publier, **A** annuler, **R** rembourser, **E** exporter, **G** administrer, **N** interdit. Toute action est contrôlée côté serveur sur la ressource et journalisée. L'absence d'une lettre vaut refus.

| Action | Accueil ACT-001 | Médecin ACT-002 | Paramédical ACT-003 | Compta ACT-004 | Patient ACT-005 | RH ACT-007 | Stock ACT-008 | Direction ACT-009 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Dossier administratif | C/L/M | L | L épisode actif | L identité facturation | C/L propre | L identité emploi | N | L/E |
| Rendez-vous | C/L/M/A | L/M disponibilités | L/M arrivée | L | C/L/M/A propre | N | N | L/E |
| Constantes et soins | N | C/L/M/V | C/L/M avant validation | N | L publié seulement | N | N | L audit |
| Diagnostic, prescription, conclusion | N | C/L/M/V/P | L prescriptions actives | N | L publié selon portail | N | N | L audit médical délégué |
| Résultats laboratoire/imagerie | N | L/V/P | C/L/M brouillon | N | L publié | N | N | L audit médical délégué |
| Factures patient brouillon | C/L/M | L | N | C/L/M/V/P/A/E | L propre émise | N | N | L/E |
| Paiements patient | C/L | L | N | C/L/M/V/R/E | L propre | N | N | L/E |
| Factures organismes et rapprochement | L | L | N | C/L/M/V/P/A/R/E | N | N | N | L/E |
| Tarifs, taxes et conventions | N | L | N | C/L/M/V | N | N | N | L/V/E |
| Produits et stock | L disponibilité | L disponibilité | L disponibilité | L valorisation | N | N | C/L/M/V/E | L/E |
| Personnel et paie | N | N | N | L/V montants | N | C/L/M/V/P/E | N | L/V/E |
| Rapports financiers | N | L agrégé autorisé | N | L/E | N | N | L stock | L/E |
| Copie administrative/financière | C remise | N | N | C/V/P | C/L propre | N | N | L/E |
| Copie clinique | N | V/P | N | N | C/L propre | N | N | V/P directeur médical délégué |
| Comptes et habilitations | N | N | N | N | N | N | N | G via administrateur désigné |
| Suppression physique clinique | N | N | N | N | N | N | N | N |

## Règles de cumul et contrôle

- Les rôles sont cumulatifs uniquement après approbation; un refus explicite de sécurité prévaut sur une autorisation de module.
- L'accueil encaisse mais ne rembourse pas; la comptabilité rapproche et rembourse; la direction approuve les conventions et les exceptions.
- L'accès d'urgence clinique est réservé à un médecin, exige un motif et déclenche une alerte au directeur médical.
- Le patient n'accède qu'aux ressources rattachées à son identité vérifiée et publiées.
- Les organismes payeurs ne disposent d'aucun compte direct en V1; les échanges passent par la comptabilité.

Statut : `CLOSED_FOR_BASELINE`. Décisions : Q-002, Q-003, Q-005, Q-017, Q-024, Q-025 et Q-031.
