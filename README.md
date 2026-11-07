# ogec-connecteurs — marketplace publique

Catalogue de plugins Claude pour les OGEC et les écoles : skills d'usage et de maintenance de connecteurs MCP
génériques. Aucune donnée d'établissement n'y figure.

| Plugin | Dépôt du connecteur | Contenu |
|---|---|---|
| `charlemagne` | [charlemagne-mcp](https://github.com/aghulas/charlemagne-mcp) | Charlemagne (Aplim) : formats d'import, affectation des photos, import des mails et téléphones |
| `ecoledirecte-admin` | [ecoledirecte-admin-mcp](https://github.com/aghulas/ecoledirecte-admin-mcp) | Console d'administration EcoleDirecte : maintenance du connecteur |
| `edumoov` | [edumoov-mcp](https://github.com/aghulas/edumoov-mcp) | Edumoov / Educartable : communication aux familles, contrôle de rentrée |
| `maclasse` | [maclasse-mcp](https://github.com/aghulas/maclasse-mcp) | Photos scolaires maclasse.photo : photos des élèves, suivi des commandes |
| `urssaf-vigilance` | [urssaf-vigilance-mcp](https://github.com/aghulas/urssaf-vigilance-mcp) | Attestations de vigilance Urssaf des fournisseurs |
| `wordpress` | [wordpress-mcp](https://github.com/aghulas/wordpress-mcp) | Site WordPress d'école : consultation, audit, mise à jour confirmée |

## Installation

- **Claude Code** : `claude plugin marketplace add aghulas/ogec-connecteurs-marketplace`, puis par exemple
  `claude plugin install charlemagne@ogec-connecteurs` ; activer l'auto-update dans `/plugin` › Marketplaces.
- **Claude Desktop / Cowork** : réglages des plugins › ajouter une marketplace › `aghulas/ogec-connecteurs-marketplace`.

Les skills décrivent l'usage des connecteurs : installer et configurer le serveur MCP correspondant en suivant
le README de son dépôt.

## Mises à jour

Pas de numéro de version : la version d'un plugin est le SHA du dernier commit de son dépôt. Chaque évolution
d'un connecteur ou de ses skills est une mise à jour, reçue dès que l'auto-update est actif.

## Adapter à son établissement

Les éléments propres à une école (comptes, adresses, interlocuteurs, procédures internes) vont dans un dépôt
**privé** de l'établissement. Si ce dépôt reprend une skill sous le même nom pour y ajouter ces éléments, installer
sa version à la place du plugin public correspondant, pour ne pas charger deux skills concurrentes.

Ce catalogue est généré automatiquement : ne pas éditer `.claude-plugin/marketplace.json` à la main.
