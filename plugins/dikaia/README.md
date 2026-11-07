# DIKAIA per Claude

## Italiano

Questo plugin collega Claude a **DIKAIA**, la piattaforma di ricerca giuridica italiana per avvocati. Claude consulta
norme, sentenze, contratti collettivi e i calcolatori dei termini di DIKAIA, oltre alle pratiche e ai documenti del
tuo studio, e cita ogni fonte con il suo link.

Il plugin contiene il connettore DIKAIA e la skill `dikaia`. I flussi di lavoro (ricerca, scadenze, verifica di un
atto, parere, contestazione, preventivo, fascicolo, conflitti) sono forniti dal server DIKAIA e restano sempre
aggiornati.

**Installazione.** Su claude.ai e Cowork: *Personalizza > Plugin > Aggiungi > Aggiungi marketplace* con
`wedomagicai/dikaia-claude`. In Claude Code:

```
/plugin install dikaia --marketplace wedomagicai/dikaia-claude
```

**Uso.** Scrivi `/dikaia` seguito dalla richiesta, ad esempio `/dikaia termine per l'appello di una sentenza del
tribunale`, oppure fai la domanda in italiano: Claude usa DIKAIA quando la domanda riguarda il diritto italiano.

**Collegamento.** Dopo l'installazione apri la scheda **Connettori** del plugin e collega DIKAIA con il tuo account.
Sui piani Team ed Enterprise il proprietario dell'organizzazione aggiunge prima il connettore per l'organizzazione;
ogni membro poi si collega con il proprio account.

**Dati.** Le richieste e i risultati passano per il server DIKAIA (`https://app.dikaia.ai/mcp`) con l'account con
cui ti sei collegato. Il plugin non contiene credenziali e non conserva dati.

## English

This plugin connects Claude to **DIKAIA**, the Italian legal research platform for lawyers. Claude searches Italian
statutes, case law, collective agreements and DIKAIA's deadline calculators, as well as your firm's matters and
documents, and cites every source with its link.

The plugin bundles the DIKAIA connector and the `dikaia` skill. The workflows themselves (research, deadlines, filing
review, legal opinion, disciplinary notice, fee estimate, matter file, conflict check) are served by the DIKAIA server,
so they stay current.

**Install.** On claude.ai and Cowork: *Customize > Plugins > Add > Add marketplace* with
`wedomagicai/dikaia-claude`. In Claude Code:

```
/plugin install dikaia --marketplace wedomagicai/dikaia-claude
```

**Use.** Type `/dikaia` followed by your request, or simply ask an Italian legal question: Claude uses DIKAIA for it.

**Connect.** After installing, open the plugin's **Connectors** tab and connect DIKAIA with your account. On Team and
Enterprise plans an organization Owner first adds the connector for the organization; each member then connects with
their own account.

**Data.** Requests and results go through the DIKAIA server (`https://app.dikaia.ai/mcp`) under the account you
connected. The plugin ships no credentials and stores nothing itself.
