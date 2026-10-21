# lg-systems-mods

Marketplace de plugins da LG-Systems para o Claude Code.

## Plugins

| Plugin | O que faz | Repositório |
|---|---|---|
| usage-bars | Barras de contexto, cache, sessão de 5 horas e limite semanal por cima do prompt | [luismiggarcia/claude-usage-bars](https://github.com/luismiggarcia/claude-usage-bars) |

## Instalar

Abre o **Terminal** e corre:

```bash
claude plugin marketplace add luismiggarcia/lg-systems-mods
claude plugin install usage-bars@lg-systems-mods
```

Depois abre uma **sessão nova** no separador Code da app Claude para desktop.

> Não uses o `/plugin` dentro da app desktop: abre o ecrã de Plugins e ignora os argumentos, por isso não adiciona marketplaces externos.

- Se o primeiro comando falhar por SSH (sem chave do GitHub configurada), usa o URL HTTPS:
  `claude plugin marketplace add https://github.com/luismiggarcia/lg-systems-mods.git`
- Se o `claude plugin list` mostrar "failed to load" no `usage-bars`, podes ignorar: é um aviso do CLI, o plugin carrega normalmente na app.
- Se tiveres instalado o Usage Bars do diretório da Anthropic (`pepperonas/usage-bars`), desinstala-o para não ficares com barras a dobrar.

## Atualizar

```bash
claude plugin marketplace update lg-systems-mods
```

## Desinstalar

```bash
claude plugin uninstall usage-bars@lg-systems-mods
claude plugin marketplace remove lg-systems-mods
```

## Problemas e sugestões

Abre uma issue no repositório do plugin: [claude-usage-bars/issues](https://github.com/luismiggarcia/claude-usage-bars/issues).

## Adicionar um plugin (manutenção)

1. Criar o plugin numa subpasta (`<nome>/`) com o seu próprio repositório git.
2. Acrescentar uma entrada em `.claude-plugin/marketplace.json` com `"source": { "source": "github", "repo": "luismiggarcia/<repo>" }`.
3. Commit e push deste repositório; acrescentar o plugin à tabela acima.

## Autoria

Autor único: Luis Garcia (LG-Systems). Ver [AUTHORS.md](AUTHORS.md) sobre como ler as linhas "Co-Authored-By" do histórico de commits.
