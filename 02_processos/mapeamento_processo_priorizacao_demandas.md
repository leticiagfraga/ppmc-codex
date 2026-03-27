# Mapeamento do Processo de Priorização de Demandas

## Metadados
- Contexto: ausência de documentação consolidada do processo de priorização de demandas no repositório.
- Objetivo: estabelecer uma versão inicial utilizável do processo, com As Is, To Be, lacunas, riscos, indicadores e plano de transição.
- Escopo: fluxo de priorização de demandas desde o recebimento até a publicação da ordem de execução.
- Responsável(is): Letícia Fraga (dona futura do processo), [responsável pelo documento].
- Data de criação: 2026-03-25.
- Data da última atualização: 2026-03-26.
- Status: em revisão.
- Referências relacionadas: `AGENTS.md`, `00_governanca/padroes_documentais.md`, `00_governanca/criterios_qualidade.md`, `04_templates/ficha_processo_modelo.md`.
- Próximo passo: validar o As Is com as áreas envolvidas e aprovar a versão inicial do To Be.
- Prazo: [AAAA-MM-DD].
- Riscos ou bloqueios: pesos dos critérios, SLA e regras detalhadas de repriorização ainda não definidos; baseline e meta de lead time pendentes.
- Decisões pendentes: definir pesos dos critérios, SLA, meta do lead time (em dias) e regras detalhadas de repriorização.

## Resumo executivo
- Este documento inaugura o registro operacional do processo de priorização de demandas na pasta `02_processos`.
- O As Is está documentado com papéis, canais, critérios, exceção e ferramentas atualmente praticadas.
- O To Be define canal único por formulário com planilha central, evolução prevista para `Olympus (R|Tickets)`, rito semanal e decisão conjunta entre Letícia Fraga e diretoria.
- Os KPIs diretos do processo foram delimitados e terão fonte na planilha central; baseline permanece pendente.
- Encaminhamento imediato: definir pesos dos critérios, SLA, meta de lead time e regras detalhadas de repriorização.

## 1. Identificação do processo
- Nome do processo: priorização de demandas.
- Área(s) envolvida(s): áreas demandantes, PPMC, Desenvolver TI e diretoria.
- Dono(a) do processo: Letícia Fraga (definição do To Be).
- Gatilho principal: recebimento de nova demanda por formulário (canal oficial no To Be).
- Periodicidade: sem frequência fixa no As Is; semanal no To Be.

## 2. Processo atual (As Is)
### 2.1 Entradas
- Demanda recebida verbalmente, por mensagens via Teams, mensagens via WhatsApp e formulário.
- Descrição da demanda com nível de detalhe variável (campos mínimos ainda não padronizados).
- Contexto de urgência/impacto informado pelo solicitante e consolidado por Letícia Fraga na triagem.
- Capacidade disponível da equipe em Planner, anotações e planilha de Excel.

### 2.2 Etapas macro
1. Recebimento da demanda por canal verbal, Teams, WhatsApp ou formulário (por Letícia Fraga, Sairon/Desenvolver TI e gestores).
2. Triagem inicial por Letícia Fraga.
3. Avaliação de prioridade por Letícia Fraga com a diretoria, com base em urgência e impacto.
4. Comunicação da decisão para solicitantes e áreas executoras.
5. Encaminhamento para execução e acompanhamento em Planner, anotações e planilha de Excel.

### 2.3 Saídas
- Lista de demandas priorizadas para execução.
- Registro de demandas não priorizadas/postergadas com justificativa.
- Comunicação de encaminhamento para áreas solicitantes e executoras.

### 2.4 Papéis e responsabilidades
| Papel | Responsabilidade |
|---|---|
| Solicitante (gestores e áreas demandantes) | Submeter demanda pelos canais atualmente usados. |
| Letícia Fraga (triagem) | Validar completude possível e enquadramento inicial da demanda. |
| Letícia Fraga + diretoria (decisão) | Deliberar prioridade com base em urgência e impacto. |
| Desenvolver TI e áreas executoras | Planejar atendimento conforme ordem priorizada. |

### 2.5 Regras, exceções e controles
- Regras: priorização por urgência e impacto, sem rito fixo.
- Exceções: demandas urgentes entram fora da fila.
- Controles: registros distribuídos em Planner, anotações e planilha de Excel.

### 2.6 Indicadores e sistemas envolvidos
- Indicadores atuais: não há baseline formal consolidada para indicadores diretos do processo.
- Sistemas/ferramentas envolvidos: Planner, anotações e planilha de Excel.

## 3. Processo futuro (To Be)
### 3.1 Objetivo do desenho futuro
Implementar priorização de demandas com critérios claros, comparáveis e auditáveis, reduzindo subjetividade e retrabalho.

### 3.2 Etapas macro propostas
1. Registrar demanda em canal único com campos obrigatórios padronizados.
2. Realizar triagem de elegibilidade e completude das informações.
3. Classificar demanda por critérios aprovados de ganho tangível, ganho intangível, link com os pilares da organização, impacto, urgência, esforço e risco.
4. Deliberar prioridade em rito formal com decisão registrada.
5. Publicar backlog priorizado e comunicar decisões.
6. Revisar prioridades no ciclo semanal e registrar mudanças (regras detalhadas de repriorização pendentes).

### 3.3 Papéis, regras e controles propostos
- Papéis: solicitante, Letícia Fraga (triagem e dona do processo), Letícia Fraga + diretoria (fórum de priorização) e responsável pela execução.
- Regras: critérios de priorização de ganho tangível, ganho intangível, link com os pilares da organização, impacto, urgência, esforço e risco; pesos [pendente de definição], critérios de entrada mínima [a definir], SLA de resposta [pendente de definição].
- Controles: registro obrigatório de decisão, trilha de alterações de prioridade e revisão periódica de aderência.
- Canal oficial: formulário com planilha central de controle; evolução prevista para feature `R|Tickets` no sistema `Olympus`.
- Exceção no To Be: urgência crítica somente com justificativa e aprovação da diretoria.

### 3.4 Indicadores e validação
| Indicador | Baseline | Meta | Método de validação | Responsável | Prazo |
|---|---|---|---|---|---|
| Lead time de priorização (recebimento até decisão) | não definida | [definir em dias] | Medição semanal dos registros na planilha central. | Letícia Fraga | [AAAA-MM-DD] |
| Percentual de demandas com dados completos no cadastro inicial | não definida | 85% | Auditoria semanal dos registros submetidos na planilha central. | Letícia Fraga | [AAAA-MM-DD] |
| Percentual de decisões com justificativa registrada | não definida | 85% | Revisão semanal dos registros de decisão na planilha central. | Letícia Fraga | [AAAA-MM-DD] |
| Taxa de repriorização fora do rito definido | não definida | [a definir] | Comparação entre alterações e calendário semanal de priorização na planilha central. | Letícia Fraga | [AAAA-MM-DD] |

Contexto gerencial da área (não KPI direto deste processo): `% Processos Críticos com Governança Completa`, `% Projetos Internos com Governança em Dia`, `% Projetos Entregues no Prazo`, `Pesquisa Pós-Implantação (satisfação + adoção)` e `Governança de Escopo (% Mudanças Formalizadas + Tempo de Aprovação)`.

## 4. Análise de lacunas e oportunidades
### Fatos
- Não havia artefato operacional deste processo na pasta `02_processos` até esta versão.
- O processo atual recebe demandas por canal verbal, Teams, WhatsApp e formulário.
- A triagem é feita por Letícia Fraga e a decisão de prioridade por Letícia Fraga com a diretoria.
- O processo atual não possui frequência fixa; usa urgência e impacto como critérios; e trata urgências fora da fila.
- Os controles atuais estão distribuídos entre Planner, anotações e planilha de Excel.
- O To Be prevê canal único por formulário com planilha central e evolução para `Olympus (R|Tickets)`.
- Os indicadores diretos do processo foram definidos, com baseline ainda pendente.

### Hipóteses
- A priorização atual ocorre com variação de registro por causa de múltiplos canais de entrada.
- Parte das decisões pode permanecer sem justificativa padronizada enquanto não houver SLA e regra detalhada de repriorização.
- A definição de pesos tende a reduzir divergência entre prioridade percebida e prioridade deliberada.

### Análises
- Sem critérios explícitos e registro de decisão, o processo tende a baixa previsibilidade e disputa de prioridade.
- A ausência de baseline de indicadores impede avaliação objetiva de melhoria.
- Definir canal único e rito formal semanal é condição mínima para governança do processo.
- A clareza de exceção (urgência crítica com justificativa e aprovação da diretoria) reduz risco de bypass não controlado da fila.

### Recomendações
- Validar o As Is com representantes de todas as áreas envolvidas em sessão única.
- Aprovar pesos dos critérios e SLA antes de iniciar a operação plena do To Be.
- Formalizar regra detalhada de repriorização semanal e governança de exceções críticas.
- Iniciar piloto com medição dos indicadores propostos para criação da baseline e definição da meta de lead time em dias.

## 5. Plano de transição inicial
| Ação | Responsável | Prazo | Dependências | Status |
|---|---|---|---|---|
| Validar o fluxo As Is com áreas envolvidas e fechar versão 1.0. | Letícia Fraga | [AAAA-MM-DD] | Disponibilidade dos participantes-chave. | [aberto/em andamento/concluído] |
| Formalizar rito semanal e alçada de decisão com diretoria. | Letícia Fraga | [AAAA-MM-DD] | Agenda da diretoria. | [aberto/em andamento/concluído] |
| Aprovar pesos dos critérios e regra de exceção crítica. | Letícia Fraga + diretoria | [AAAA-MM-DD] | Consenso sobre pesos e critérios. | [aberto/em andamento/concluído] |
| Implantar cadastro padrão de demanda em canal único (formulário + planilha central). | Letícia Fraga | [AAAA-MM-DD] | Definição dos campos mínimos obrigatórios. | [aberto/em andamento/concluído] |
| Executar ciclo piloto e capturar baseline dos indicadores. | Letícia Fraga | [AAAA-MM-DD] | Processo To Be minimamente implantado; regras de repriorização definidas. | [aberto/em andamento/concluído] |

## 6. Riscos e bloqueios da transição
| Item | Tipo (risco/bloqueio) | Impacto | Probabilidade | Plano de resposta | Responsável | Prazo |
|---|---|---|---|---|---|---|
| Pesos dos critérios de priorização não definidos. | risco | alto | alta | Aprovar pesos em conjunto com a diretoria antes da operação plena. | Letícia Fraga | [AAAA-MM-DD] |
| SLA de priorização não definido. | risco | alto | alta | Definir SLA mínimo e monitorar cumprimento na planilha central. | Letícia Fraga | [AAAA-MM-DD] |
| Regras detalhadas de repriorização ainda não formalizadas. | risco | alto | media | Formalizar critérios de repriorização e trilha obrigatória de justificativa. | Letícia Fraga + diretoria | [AAAA-MM-DD] |
| Ausência de baseline e meta de lead time em dias. | bloqueio | medio | alta | Adotar baseline no piloto e definir meta após primeiro ciclo completo. | Letícia Fraga | [AAAA-MM-DD] |

## 7. Lacunas críticas para preenchimento pela área
- Pesos dos critérios de priorização (ganho tangível, ganho intangível, link com pilares, impacto, urgência, esforço e risco).
- SLA do processo de priorização.
- Meta do lead time de priorização em dias.
- Regras detalhadas de repriorização no ciclo semanal.
- Datas-alvo para execução do plano de transição e mitigação de riscos.

## 8. Histórico de revisões
| Data | Alteração | Responsável |
|---|---|---|
| 2026-03-25 | Criação da versão inicial do mapeamento do processo de priorização de demandas (As Is, To Be, lacunas, riscos, indicadores e plano de transição). | Codex |
| 2026-03-26 | Atualização do As Is e To Be com definições reais de canais, papéis, critérios, frequência, exceções, sistemas e indicadores; inclusão do contexto gerencial da área e explicitação das pendências (pesos, SLA, meta de lead time e repriorização). | Codex |
