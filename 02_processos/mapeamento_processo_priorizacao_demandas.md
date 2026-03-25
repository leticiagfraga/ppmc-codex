# Mapeamento do Processo de Priorização de Demandas

## Metadados
- Contexto: ausência de documentação consolidada do processo de priorização de demandas no repositório.
- Objetivo: estabelecer uma versão inicial utilizável do processo, com As Is, To Be, lacunas, riscos, indicadores e plano de transição.
- Escopo: fluxo de priorização de demandas desde o recebimento até a publicação da ordem de execução.
- Responsável(is): [dono(a) do processo], [responsável pelo documento].
- Data de criação: 2026-03-25.
- Data da última atualização: 2026-03-25.
- Status: em revisão.
- Referências relacionadas: `AGENTS.md`, `00_governanca/padroes_documentais.md`, `00_governanca/criterios_qualidade.md`, `04_templates/ficha_processo_modelo.md`.
- Próximo passo: validar o As Is com as áreas envolvidas e aprovar a versão inicial do To Be.
- Prazo: [AAAA-MM-DD].
- Riscos ou bloqueios: falta de dados consolidados sobre critérios atuais, papéis e desempenho do processo.
- Decisões pendentes: definir dono formal do processo, rito de priorização e alçada de decisão.

## Resumo executivo
- Este documento inaugura o registro operacional do processo de priorização de demandas na pasta `02_processos`.
- O As Is foi estruturado como base de levantamento, com placeholders nos pontos ainda não documentados.
- O To Be propõe um fluxo padronizado para priorização rastreável, com critérios explícitos e governança mínima.
- O principal risco de curto prazo é manter decisões de prioridade sem dados comparáveis e sem rito definido.
- Encaminhamento imediato: preencher lacunas críticas, validar indicadores e executar ciclo piloto de priorização.

## 1. Identificação do processo
- Nome do processo: priorização de demandas.
- Área(s) envolvida(s): [áreas demandantes], [área de projetos/processos], [área executora], [liderança].
- Dono(a) do processo: [nome].
- Gatilho principal: recebimento de nova demanda por [canal oficial].
- Periodicidade: [semanal/quinzenal/mensal].

## 2. Processo atual (As Is)
### 2.1 Entradas
- Demanda recebida por [canal(is) atual(is)].
- Descrição da demanda com [campos atualmente exigidos].
- Contexto de urgência/impacto informado por [papel responsável].
- Capacidade disponível da equipe em [fonte de informação].

### 2.2 Etapas macro
1. Recebimento da demanda por [canal atual].
2. Triagem inicial por [papel atual], com critérios [não formalizados/documentar].
3. Avaliação de prioridade em [fórum atual] com base em [critérios atuais].
4. Comunicação da decisão para [stakeholders].
5. Encaminhamento para execução e acompanhamento em [sistema/ferramenta].

### 2.3 Saídas
- Lista de demandas priorizadas para execução.
- Registro de demandas não priorizadas/postergadas com justificativa.
- Comunicação de encaminhamento para áreas solicitantes e executoras.

### 2.4 Papéis e responsabilidades
| Papel | Responsabilidade |
|---|---|
| [solicitante] | Submeter demanda com informações mínimas exigidas. |
| [triagem] | Validar completude e enquadramento inicial da demanda. |
| [decisor/fórum] | Deliberar prioridade e registrar justificativa. |
| [execução] | Planejar atendimento conforme ordem priorizada. |

### 2.5 Regras, exceções e controles
- Regras: [regras de priorização atualmente praticadas].
- Exceções: [situações tratadas fora do fluxo padrão].
- Controles: [controles para rastreabilidade de decisão e mudança de prioridade].

### 2.6 Indicadores e sistemas envolvidos
- Indicadores atuais: [indicadores atualmente monitorados, se existentes].
- Sistemas/ferramentas envolvidos: [sistemas utilizados no processo atual].

## 3. Processo futuro (To Be)
### 3.1 Objetivo do desenho futuro
Implementar priorização de demandas com critérios claros, comparáveis e auditáveis, reduzindo subjetividade e retrabalho.

### 3.2 Etapas macro propostas
1. Registrar demanda em canal único com campos obrigatórios padronizados.
2. Realizar triagem de elegibilidade e completude das informações.
3. Classificar demanda por critérios aprovados de impacto, urgência, esforço e risco.
4. Deliberar prioridade em rito formal com decisão registrada.
5. Publicar backlog priorizado e comunicar decisões.
6. Revisar prioridades em ciclo definido e registrar mudanças.

### 3.3 Papéis, regras e controles propostos
- Papéis: solicitante, analista de triagem, fórum de priorização, responsável pela execução e dono do processo [nomes a definir].
- Regras: critérios de priorização e pesos [a definir], critérios de entrada mínima [a definir], SLA de resposta [a definir].
- Controles: registro obrigatório de decisão, trilha de alterações de prioridade e revisão periódica de aderência.

### 3.4 Indicadores e validação
| Indicador | Baseline | Meta | Método de validação | Responsável | Prazo |
|---|---|---|---|---|---|
| Lead time de priorização (recebimento até decisão) | [valor atual] | [meta] | Medição por amostra mensal de demandas. | [nome] | [AAAA-MM-DD] |
| Percentual de demandas com dados completos no cadastro inicial | [valor atual] | [meta] | Auditoria quinzenal dos registros submetidos. | [nome] | [AAAA-MM-DD] |
| Percentual de decisões com justificativa registrada | [valor atual] | [meta] | Revisão mensal das atas/registros de decisão. | [nome] | [AAAA-MM-DD] |
| Taxa de repriorização fora do rito definido | [valor atual] | [meta] | Comparação entre alterações e calendário do rito. | [nome] | [AAAA-MM-DD] |

## 4. Análise de lacunas e oportunidades
### Fatos
- Não havia artefato operacional deste processo na pasta `02_processos` até esta versão.
- Critérios formais de priorização não estão documentados no repositório no momento.
- Papéis, alçadas, exceções e sistemas do processo atual ainda não estão consolidados neste documento.

### Hipóteses
- A priorização atual ocorre com variação de critério entre áreas.
- Parte das decisões pode estar registrada apenas em canais não estruturados.
- Repriorizações podem ocorrer sem histórico formal de justificativa.

### Análises
- Sem critérios explícitos e registro de decisão, o processo tende a baixa previsibilidade e disputa de prioridade.
- A ausência de baseline de indicadores impede avaliação objetiva de melhoria.
- Definir canal único e rito formal é condição mínima para governança do processo.

### Recomendações
- Validar o As Is com representantes de todas as áreas envolvidas em sessão única.
- Aprovar critérios e pesos de priorização antes de iniciar a operação do To Be.
- Iniciar piloto com medição dos indicadores propostos para criação da baseline.

## 5. Plano de transição inicial
| Ação | Responsável | Prazo | Dependências | Status |
|---|---|---|---|---|
| Validar o fluxo As Is com áreas envolvidas e fechar versão 1.0. | [nome] | [AAAA-MM-DD] | Disponibilidade dos participantes-chave. | [aberto/em andamento/concluído] |
| Definir dono do processo e fórum de priorização. | [nome] | [AAAA-MM-DD] | Deliberação da liderança. | [aberto/em andamento/concluído] |
| Aprovar critérios de priorização e regra de exceção. | [nome] | [AAAA-MM-DD] | Consenso sobre critérios e pesos. | [aberto/em andamento/concluído] |
| Implantar cadastro padrão de demanda em canal único. | [nome] | [AAAA-MM-DD] | Definição dos campos mínimos obrigatórios. | [aberto/em andamento/concluído] |
| Executar ciclo piloto e capturar baseline dos indicadores. | [nome] | [AAAA-MM-DD] | Processo To Be minimamente implantado. | [aberto/em andamento/concluído] |

## 6. Riscos e bloqueios da transição
| Item | Tipo (risco/bloqueio) | Impacto | Probabilidade | Plano de resposta | Responsável | Prazo |
|---|---|---|---|---|---|---|
| Indefinição de dono do processo e alçada de decisão. | risco | alto | alta | Formalizar governança mínima antes do piloto. | [nome] | [AAAA-MM-DD] |
| Falta de padronização dos dados de entrada das demandas. | risco | alto | alta | Definir campos obrigatórios e validar completude na triagem. | [nome] | [AAAA-MM-DD] |
| Baixa adesão ao rito formal de priorização. | risco | medio | media | Comunicar rito, registrar decisões e monitorar aderência. | [nome] | [AAAA-MM-DD] |
| Ausência de histórico confiável para baseline inicial. | bloqueio | medio | alta | Adotar baseline a partir do primeiro ciclo piloto registrado. | [nome] | [AAAA-MM-DD] |

## 7. Lacunas críticas para preenchimento pela área
- Dono(a) formal do processo e responsáveis por triagem, decisão e execução.
- Canais atuais de entrada e sistema oficial para registro das demandas.
- Critérios atuais e futuros de priorização (incluindo pesos e regras de exceção).
- Rito de priorização (frequência, participantes e alçada de decisão).
- Baseline e metas dos indicadores definidos na seção 3.4.
- Prazos e responsáveis do plano de transição e mitigação de riscos.

## 8. Histórico de revisões
| Data | Alteração | Responsável |
|---|---|---|
| 2026-03-25 | Criação da versão inicial do mapeamento do processo de priorização de demandas (As Is, To Be, lacunas, riscos, indicadores e plano de transição). | Codex |
