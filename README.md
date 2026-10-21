# lg-systems-mods

Marketplace de plugins da LG-Systems para o Claude Code.

## Instalar

```bash
claude plugin marketplace add luismiggarcia/lg-systems-mods
claude plugin install usage-bars@lg-systems-mods
```

Para receber plugins novos: `claude plugin marketplace update lg-systems-mods`.

## Plugins

| Plugin | Repositório |
|---|---|
| usage-bars | [luismiggarcia/claude-usage-bars](https://github.com/luismiggarcia/claude-usage-bars) |

## Adicionar um plugin

1. Criar o plugin numa subpasta (`<nome>/`) com o seu próprio repositório git.
2. Acrescentar uma entrada em `.claude-plugin/marketplace.json` com `"source": { "source": "github", "repo": "luismiggarcia/<repo>" }`.
3. Commit e push deste repositório.
