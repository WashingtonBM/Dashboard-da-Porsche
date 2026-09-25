# Organização do projeto

## Decisões

- `index.html` é a única entrada web oficial.
- O notebook é mantido como ferramenta de preparação/limpeza, não como runtime do dashboard.
- `Base de Dados` é um arquivo binário Excel. Ele não deve ser editado como texto nem duplicado com nomes alternativos.
- Os arquivos sem extensão e as exportações de ferramentas diferentes são artefatos legados. Não devem receber novas funcionalidades.

## Próxima limpeza manual

A API de edição usada nesta sessão permite criar e atualizar arquivos, mas não excluir ou mover arquivos. Por isso, os arquivos legados ainda estão no repositório e devem ser removidos pelo GitHub Desktop, Codespaces ou terminal após validar que não são necessários:

```bash
git rm "Dashboard Porsch" "Dashboard Porsch.html" "Dashboard no Chat Gpt" "Dashboard no Colab" "Dashboard no Github Dev" "Dashbord in VS Code local" "Imagem VS Code local"
git commit -m "chore: remove dashboard artifacts"
```

Não remova `Dashboard_Porsch.ipynb`, `Base de Dados` ou `index.html` sem confirmar que não serão mais usados.

## Melhorias aplicadas nesta etapa

- `.gitignore` ampliado para ambientes Python, checkpoints do Jupyter, caches, logs e arquivos gerados.
- README reescrito com instruções de execução e uma fonte oficial do dashboard.
- Documentação criada para evitar novas cópias e orientar a remoção segura dos artefatos.

## Revisão recomendada do JavaScript

Ao alterar `index.html`, preserve estas garantias:

- gráficos sem dados devem exibir um estado vazio em vez de falhar;
- valores monetários inválidos devem ser tratados como zero apenas para cálculo;
- conteúdo da tabela deve ser inserido com `textContent` ou escapado antes de usar HTML;
- filtros devem ter uma opção clara de restauração (`Todos`);
- status exibidos em português devem ser usados também na regra de cores.
