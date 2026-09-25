# Dashboard Porsche

Dashboard interativo de vendas da Porsche, construído com HTML, CSS, JavaScript e [Plotly.js](https://plotly.com/javascript/).

## Executar localmente

A aplicação é estática e pode ser executada com qualquer servidor HTTP:

```bash
python3 -m http.server 8000
```

Depois acesse <http://localhost:8000> e abra `index.html`. Usar um servidor HTTP evita limitações do navegador ao carregar arquivos locais.

## Estrutura atual

- `index.html` — aplicação web principal e ponto de entrada do projeto.
- `Dashboard_Porsch.ipynb` — notebook de limpeza e preparação dos dados no Colab.
- `Base de Dados` — arquivo Excel original; mantenha-o como fonte de dados brutos.
- `README.md` — documentação do projeto.
- `.gitignore` — arquivos locais e saídas geradas que não devem ser versionados.
- `docs/` — notas de organização e decisões de manutenção.

Arquivos legados e exportações de experimentos permanecem no histórico para preservar rastreabilidade. Novas alterações do dashboard devem ser feitas em `index.html`; não crie uma nova cópia HTML para cada teste.

## Funcionalidades

- KPIs de vendas, receita, ticket médio, cidades e modelos.
- Filtros por modelo, ano, cidade, forma de pagamento e status de entrega.
- Gráficos interativos com Plotly.js.
- Tabela das transações filtradas.
- Layout responsivo para desktop e telas menores.

## Desenvolvimento

Antes de publicar uma alteração:

1. Execute o dashboard com `python3 -m http.server 8000`.
2. Teste todos os filtros, inclusive a combinação que não retorna registros.
3. Confirme no console do navegador que não existem erros JavaScript.
4. Verifique o layout em uma janela estreita.
5. Faça um commit pequeno e descritivo.

## Publicação

O dashboard pode ser publicado pelo GitHub Pages usando a branch `main` e a pasta raiz. O arquivo `index.html` deve permanecer na raiz para ser reconhecido como página inicial.
