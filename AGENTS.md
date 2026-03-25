# AGENTS.md — Regras operacionais do repositório PPMC

## Missão
Apoiar a área de Projetos, Processos e Melhoria Contínua com artefatos claros, rastreáveis, reutilizáveis e orientados à execução.

## Como atuar neste repositório
- Trabalhe em português do Brasil.
- Preserve a estrutura atual do repositório.
- Use templates existentes antes de criar documentos do zero.
- Prefira mudanças pequenas, claras e fáceis de revisar.
- Não invente sistemas, ferramentas, rituais ou dados inexistentes.
- Quando faltar informação, registre a lacuna com clareza em vez de supor fatos.
- Sempre diferencie claramente: fato, hipótese, análise e recomendação.
- Quando o público for gerencial, comece pelo resumo executivo.
- Sempre que fizer sentido, explicite próximo passo, responsável e prazo.
- Ao concluir alterações, registre resumo objetivo do que foi criado, alterado ou movido.

## Escopo do repositório
- Consolidar documentação de governança.
- Registrar iniciativas de projetos.
- Mapear, revisar e padronizar processos.
- Conduzir e acompanhar ações de melhoria contínua.
- Manter templates reutilizáveis.

## Estrutura oficial
- `00_governanca`: glossário, diretrizes, convenções, critérios de qualidade e padrões da área.
- `01_projetos`: planejamento, acompanhamento, riscos, decisões, entregas e encerramento de iniciativas.
- `02_processos`: mapeamento do processo atual, proposta futura, regras, indicadores e controles.
- `03_melhoria_continua`: oportunidades, priorização, planos de ação, experimentos, execução e resultados.
- `04_templates`: modelos padronizados para documentos recorrentes.
- `.codex`: configuração local do Codex para este repositório.

## Ordem de consulta recomendada
Antes de produzir ou alterar artefatos:
1. Ler este `AGENTS.md`.
2. Consultar `00_governanca` para glossário, padrões e critérios.
3. Verificar se existe template compatível em `04_templates`.
4. Só então criar ou revisar materiais em `01_projetos`, `02_processos` ou `03_melhoria_continua`.

## Regras universais de documentação
Todo novo documento deve conter, no mínimo, quando aplicável:
- contexto
- objetivo
- escopo
- responsável(is)
- data de criação
- data da última atualização
- status
- referências relacionadas
- próximo passo
- prazo
- riscos ou bloqueios
- decisões pendentes

## Regras por frente

### 00_governanca
- Use esta pasta para padrões permanentes ou recorrentes da área.
- Atualize glossário, convenções e critérios sempre que um aprendizado deixar de ser pontual.
- Não use esta pasta para material operacional de um caso isolado.

### 01_projetos
- Trate cada iniciativa como algo que precisa de objetivo, escopo, entregas, riscos, responsáveis e status.
- Em materiais de projeto, destaque dependências, bloqueios, decisões e próximos passos.
- Prefira saídas orientadas à gestão e à execução, não apenas registro passivo.

### 02_processos
- Diferencie claramente processo atual (As Is) e processo futuro (To Be).
- Identifique gatilho, entradas, saídas, papéis, regras, exceções, indicadores, controles e sistemas envolvidos.
- Ao propor melhoria de processo, registre ganho esperado e forma de validação.

### 03_melhoria_continua
- Estruture melhorias como: problema, evidência, hipótese de causa, ação proposta, benefício esperado, responsável, prazo e métrica.
- Priorize ações por impacto, esforço e risco.
- Evite recomendações genéricas; transforme observações em ações verificáveis.

### 04_templates
- Atualize templates quando surgir padrão recorrente.
- Evite duplicar modelos muito parecidos.
- Se criar um novo template, ele deve ser simples, reutilizável e aderente à taxonomia da área.

## Convenções de nomenclatura
- Pastas: `snake_case`, nomes curtos e sem ambiguidade.
- Arquivos: minúsculas, descritivos e separados por `_`.
- Quando fizer sentido, prefixe com data no formato `AAAA-MM-DD`.
- Evite abreviações pouco óbvias.

Exemplos:
- `2026-03-25_plano_implantacao.md`
- `mapeamento_fluxo_aprovacao.md`
- `backlog_melhorias_priorizado.md`

## Versionamento e histórico
- Não apagar conteúdo relevante sem justificativa registrada no próprio arquivo.
- Em revisões significativas, incluir breve histórico com:
  - data
  - alteração realizada
  - responsável
- Materiais obsoletos devem ser marcados como `arquivado`, mantendo rastreabilidade.
- Não sobrescrever material-fonte sem instrução explícita; preferir nova versão, rascunho ou documento derivado.
- Evitar duplicidade; referenciar documentos existentes sempre que possível.

## Critérios de qualidade antes de concluir
Verifique se:
- o material está na pasta correta;
- existe vínculo claro com projeto, processo ou melhoria;
- há responsável e status atual;
- fatos, hipóteses, análises e recomendações estão separados;
- existe resumo executivo quando o público for gerencial;
- há próximo passo definido quando o documento exigir encaminhamento;
- termos críticos estão alinhados ao glossário;
- o documento está compreensível por alguém fora do contexto imediato.

## Saída esperada do agente ao concluir um trabalho
Sempre que concluir uma alteração relevante, informar:
- arquivos criados
- arquivos alterados
- arquivos movidos
- resumo do que mudou
- pendências ou lacunas encontradas