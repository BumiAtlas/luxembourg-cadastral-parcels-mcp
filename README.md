# Luxembourg Cadastral Parcels & Lookup MCP

[Français](#français)

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Luxembourg land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- All ~717k cadastral parcels from the ACT's Plan Cadastral Numérisé (October 2026)
- Parcel lookup by parcel id (`054A00242005293`), lieu-dit and number (`Kirchberg 242/5293`), a whole lieu-dit (paged), or coordinates
- Commune, section and the parcel's nature, with its French label and category
- Satellite and street map images of a parcel and its neighbours, labelled by parcel number

Parcels have no owner, right, price or registered area.

## Connect

```
https://bumiatlas.com/mcp/luxembourg
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/luxembourg](https://bumiatlas.com/mcp-docs/luxembourg).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `LU_parcel_search` | Find parcels by id, lieu-dit and number, a whole lieu-dit (paged), or `latitude, longitude`; each result is the whole record, the boundary as GeoJSON on request |
| `LU_parcel_image` | Satellite or street map image of a parcel or point, with every parcel in view outlined and labelled with its number |

## Example prompts

- *"Which parcel is at 49.6116, 6.1319? What is its nature?"*
- *"Look up parcel 054A00242005293 and show it on satellite imagery."*
- *"List the parcels in the lieu-dit Kirchberg."*
- *"Which section is this parcel in?"*

## Data source

Parcels © Administration du cadastre et de la topographie (ACT), Plan Cadastral Numérisé (CC BY 4.0). A copy of public data for research, not a legal land record.

## Français

Connectez votre assistant IA (Claude, ChatGPT ou Cursor) à [BumiAtlas](https://bumiatlas.com) via le Model Context Protocol (MCP) pour vos recherches cadastrales au Luxembourg.

- Les ~717 000 parcelles du Plan Cadastral Numérisé de l'ACT
- Recherche par identifiant, lieu-dit et numéro (`Kirchberg 242/5293`) ou par coordonnées
- Nature de la parcelle, images satellite et plan de la parcelle et de ses voisines

Aucun propriétaire, droit, prix ni superficie enregistrée.

**Connexion :** ajoutez `https://bumiatlas.com/mcp/luxembourg` comme connecteur personnalisé dans votre client MCP et connectez-vous avec Google. Les noms des outils sont en anglais, mais l'assistant peut répondre en français.
