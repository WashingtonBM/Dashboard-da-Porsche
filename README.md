# Dashboard Porsche

Esse repositório contém um dashboard de visualização de vendas da Porsche usando HTML, CSS e JavaScript (Plotly.js). O objetivo é fornecer gráficos, KPIs e tabelas interativas para análise rápida.

## Estrutura do repositório

- `index.html` — Dashboard principal (versão melhorada)
- `Dashboard Porsch.html` — Versão original/cópia
- `Dashboard Porsch` — Arquivo adicional presente no workspace

> Observação: verifique os arquivos no diretório raiz e subpastas antes de alterar.

## Como executar (rápido)

1) Servidor local com Python (recomendado):

```bash
cd /workspaces/Dashboard-da-Porsche
python3 -m http.server 8000
```
Abra: http://localhost:8000/index.html

2) Usando VS Code Live Server
- Instale a extensão "Live Server"
- Clique com o botão direito em `index.html` e escolha "Open with Live Server"

3) Dashboard criado usando Colab
- Abra (https://colab.research.google.com/drive/16ZED05j9sXO3KVLE4Ys5wK-x8Lsr7Otb#scrollTo=9c02d672&fullscreenOutput=true)

## Incluir todos os arquivos no repositório (comandos git)

Se quiser garantir que todos os arquivos do workspace sejam versionados, execute:

```bash
git add .
git commit -m "Adicionar arquivos do dashboard e implementar README"
git push origin main
```

Se o repositório ainda não tiver remoto configurado, adicione com:

```bash
git remote add origin <URL_DO_REPOSITORIO>
git push -u origin main
```

## Principais recursos

- KPIs de vendas e receita
- Gráficos interativos (histórico, distribuição por cidade, top modelos)
- Filtros por modelo, ano, cidade e método de pagamento
- Tabela com últimas transações

## Personalização rápida

- Adicionar/alterar dados: edite a variável `data` nos scripts JavaScript.
- Cores: ajuste variáveis CSS (ex.: `--color-primary`).

## Problemas comuns & solução rápida

- Se gráficos não carregarem: abra o DevTools (F12) e veja a aba Console.
- Se estiver usando `file://` e houver erros, rode um servidor HTTP local.

## Próximos passos sugeridos

1. Verificar os arquivos do workspace e confirmar quais devem ser commitados.
2. Ajustar dados de exemplo para seu conjunto real.
3. Automatizar build/empacotamento se necessário.

---

Se quiser, eu posso:
- adicionar um `.gitignore` básico;
- executar os comandos `git add`/`commit`/`push` aqui (se autorizar);
- listar os arquivos no workspace para confirmar o que será enviado.

Obrigado — quer que eu faça o commit e push agora?

## Arquivos no repositório (raiz)

Lista de arquivos presentes no diretório raiz do workspace (profundidade 2):

- .gitignore
- 8683bed0-cc33-4e06-bca9-04db9c31f9e2.xlsx
- ChatGPT Image 19 de jun. de 2026, 20_15_02.png
- Dashboard Porsch
- Dashboard Porsch.html
- README.md
- index.html
