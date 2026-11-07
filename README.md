# DIKAIA per Claude / DIKAIA for Claude

## Italiano

Questo repository è il marketplace dei plugin di **DIKAIA** per Claude. Contiene un solo plugin, `dikaia`, che collega
Claude alla piattaforma di ricerca giuridica italiana DIKAIA: norme, sentenze, contratti collettivi, termini e
scadenze, pratiche dello studio, sempre con le fonti citate. Il plugin porta il connettore DIKAIA e una skill; tutto
il resto vive sul server DIKAIA.

### Installazione

- **claude.ai e Cowork:** *Personalizza > Plugin > Aggiungi > Aggiungi marketplace* e inserisci
  `wedomagicai/dikaia-claude`, poi installa il plugin **DIKAIA**.
- **Claude Code:**

  ```
  /plugin marketplace add wedomagicai/dikaia-claude
  /plugin install dikaia@dikaia
  ```

Poi apri la scheda **Connettori** del plugin e collega DIKAIA con il tuo account DIKAIA. Sui piani Team ed Enterprise
il proprietario dell'organizzazione aggiunge il connettore per l'organizzazione e ogni membro si collega con il
proprio account.

Usa `/dikaia` seguito dalla richiesta, oppure fai una domanda di diritto italiano.

## English

This repository is the **DIKAIA** plugin marketplace for Claude. It lists one plugin, `dikaia`, which connects Claude
to the DIKAIA Italian legal research platform: statutes, case law, collective agreements, deadlines and the firm's
matters, always with cited sources. The plugin carries the DIKAIA connector and one skill; everything else lives on
the DIKAIA server.

### Install

- **claude.ai and Cowork:** *Customize > Plugins > Add > Add marketplace*, enter `wedomagicai/dikaia-claude`, then
  install the **DIKAIA** plugin.
- **Claude Code:**

  ```
  /plugin marketplace add wedomagicai/dikaia-claude
  /plugin install dikaia@dikaia
  ```

Then open the plugin's **Connectors** tab and connect DIKAIA with your DIKAIA account. On Team and Enterprise plans an
organization Owner adds the connector for the organization and each member connects with their own account.

Type `/dikaia` followed by your request, or ask an Italian legal question.

## Repository layout

- `.claude-plugin/marketplace.json` — the public marketplace `dikaia`.
- `plugins/dikaia/` — the plugin, the single source for every variant.
- `internal/` — the `dikaia-internal` marketplace with the `dikaia-stage` and `dikaia-next` test plugins, generated
  from `plugins/dikaia` by `python tools/build_variants.py` (`--check` fails when they drift). Not part of the public
  marketplace; add it from a local clone with `claude plugin marketplace add ./internal`.

## License

MIT, see `LICENSE`.
