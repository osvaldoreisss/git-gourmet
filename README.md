# git-gourmet

🇧🇷 Receitas com controle de versão. Cada ajuste testado na cozinha vira um commit.
🇬🇧 Version-controlled recipes. Every tweak tested in the kitchen becomes a commit.

## Receitas / Recipes

| Receita | Recipe | Status |
|---|---|---|
| [Pastel de feira](recipes/pastel-de-feira/pt-BR.md) | [Brazilian street-market pastel](recipes/pastel-de-feira/en.md) | 🧪 a testar / to test |
| [Coxinha e bolinha de queijo (massa de batata)](recipes/coxinha-e-bolinha-de-queijo/pt-BR.md) | [Coxinha & cheese balls (potato dough)](recipes/coxinha-e-bolinha-de-queijo/en.md) | 🧪 a testar / to test |
| [Empadinha de frango](recipes/empadinha-de-frango/pt-BR.md) | [Chicken empadinha](recipes/empadinha-de-frango/en.md) | 🧪 a testar / to test |
| [Pão de queijo mineiro](recipes/pao-de-queijo/pt-BR.md) | [Brazilian cheese bread](recipes/pao-de-queijo/en.md) | 🧪 a testar / to test |

Listas de compras / Shopping lists: [`shopping/`](shopping/)

## Experimentos / Experiments

| Experimento | Experiment | Status |
|---|---|---|
| [Proporção polvilho azedo × doce](experiments/pao-de-queijo-proporcao-polvilho/pt-BR.md) | [Sour × sweet starch ratio](experiments/pao-de-queijo-proporcao-polvilho/en.md) | 📋 planejado / planned |

## Estrutura / Layout

```
recipes/<receita>/pt-BR.md   # versão em português
recipes/<receita>/en.md      # English version
experiments/<teste>/{pt-BR,en}.md   # testes controlados de uma variável / one-variable tests
shopping/<data>-<evento>.<lang>.md
```

Cada receita começa com um bloco YAML (`yield`, `status`, `tags`, `sources`).
Each recipe starts with a YAML block (`yield`, `status`, `tags`, `sources`).

## Convenções / Conventions

- Medidas em gramas e ml sempre que possível; colheres: `cs` = colher de sopa (15 ml), `cc` = colher de chá (5 ml).
- Weights in grams/ml where possible; `tbsp` = 15 ml, `tsp` = 5 ml.
- Ingredientes adaptados a supermercados alemães, com o nome em alemão entre parênteses.
- Ingredients adapted to German supermarkets, with the German name in parentheses.
- Depois de testar: atualize `status`, registre o que mudou na seção **Notas de teste** e faça commit com uma mensagem clara (ex.: `pastel: +1 cs de água, massa estava seca`).
- After testing: update `status`, log changes under **Test notes**, and commit with a clear message (e.g. `pastel: +1 tbsp water, dough was dry`).
