# Pagina Executiva Macro - Area PPMC

## Resumo executivo
- Escopo: consolidado da area PPMC com foco em portfolio e operacao recorrente.
- Portfolio: 3 iniciativas ativas (1 verde, 2 amarelas, 0 vermelhas).
- KPIs: consolidacao mensal ainda nao concluida (`status_kpis.csv` com 0 de 6 KPIs com `valor_atual`).
- Principal risco transversal: capacidade operacional (prioridade de outros projetos e mao de obra escassa) e dependencia de sistemas internos.
- Encaminhamento imediato: validar as propostas de governanca e executar o primeiro fechamento mensal recorrente em data fixa.

## Metadados
- Contexto: fechamento da fase de implantacao do modelo operacional PPMC.
- Objetivo: apresentar visao macro executiva para operacao recorrente.
- Escopo: portfolio 2026 + bases de KPI (`status_kpis.csv`, `entrada_mensal_kpis.csv`, `plano_acoes_kpis.csv`).
- Responsavel(is): Leticia Fraga (curadoria funcional - proposta para validacao); Codex (apoio tecnico/documental).
- Data de criacao: 2026-04-02.
- Data da ultima atualizacao: 2026-04-02.
- Status: ativo.
- Referencias relacionadas: `01_projetos/portfolio_iniciativas_2026.md`, `05_bases/kpis/status_kpis.csv`, `05_bases/kpis/entrada_mensal_kpis.csv`, `05_bases/kpis/plano_acoes_kpis.csv`, `00_governanca/rotina_operacional_codex_ppmc.md`.
- Proximo passo: validar as propostas de governanca da secao 5 e executar fechamento mensal completo na ordem oficial.
- Prazo: 2026-05-02.
- Riscos ou bloqueios: capacidade operacional concorrente; dependencia de sistemas usados internamente.
- Decisoes pendentes: validacao formal das definicoes de governanca listadas na secao 5.

## 1. Panorama do portfolio
| Indicador | Valor | Fonte |
|---|---|---|
| Iniciativas ativas | 3 | `01_projetos/portfolio_iniciativas_2026.md` |
| Saude consolidada | 1 verde, 2 amarelas, 0 vermelhas | `01_projetos/portfolio_iniciativas_2026.md` |
| Iniciativas com prioridade alta | 3 de 3 | `01_projetos/portfolio_iniciativas_2026.md` |
| Registros em `base_projetos_ativos.csv` | 3 linhas (mar/2026 e abr/2026) | `05_bases/kpis/base_projetos_ativos.csv` |

## 2. Situacao das bases de KPI
| Base | Situacao atual | Leitura executiva |
|---|---|---|
| `status_kpis.csv` | 6 KPIs com `valor_atual` vazio e `meta` como `[definir]` | Consolidacao mensal pendente |
| `entrada_mensal_kpis.csv` | Sem carga de valores em jan-dez para os 6 KPIs | Serie mensal ainda nao iniciada |
| `plano_acoes_kpis.csv` | Sem registros de acoes | Nao ha plano formalizado para desvios |

## 3. Principais riscos consolidados
| Risco/Bloqueio | Impacto macro | Status atual |
|---|---|---|
| Prioridade de outros projetos e mao de obra escassa (Olympus e Metas/Indicadores) | Reduz capacidade de execucao e previsibilidade do portfolio | Aberto nos dossies |
| Sistemas usados internamente (Jornada do Cliente) | Pode atrasar consolidacao AS-IS/TO-BE e decisoes de desenho | Registrado como bloqueio recorrente |
| Lacunas de sponsor/criticidade em P-2026-002 e P-2026-003 | Limita derivacao confiavel de governanca e risco critico | Pendente de fechamento documental |

## 4. Proximos passos macro
| Acao | Responsavel | Prazo | Status |
|---|---|---|---|
| Concluir D-002 e consolidar E-002 da Jornada do Cliente | Leticia Fraga | 2026-04-02 | em andamento |
| Formalizar sponsor, baseline e classificacao de risco da Olympus | Leticia Fraga | Proposta para validacao: 2026-04-15 | pendente de definicao no dossie |
| Formalizar sponsor, baseline e classificacao de risco da iniciativa Metas e Indicadores | Leticia Fraga | Proposta para validacao: 2026-04-15 | pendente de definicao no dossie |
| Executar fechamento mensal na ordem oficial (documentos > CSV > consolidacao > leitura executiva) | Leticia Fraga + Codex | 2026-05-02 | planejado |

## 5. Parametros de governanca (proposta para validacao)
- Periodicidade oficial de apuracao: mensal.
- Data fixa de fechamento mensal: dia 2 de cada mes.
- Data fixa de fechamento quadrimestral: dia 5 de maio, dia 5 de setembro e dia 5 de janeiro.
- Curadoria formal do portfolio: Leticia Fraga (curadoria funcional) com apoio tecnico do Codex.
- Criterio oficial de saude: verde/amarelo/vermelho por `governanca_em_dia`, `risco_critico_aberto` e atualizacao de status no periodo.
- Cadencia de publicacao da leitura executiva: mensal no dia util seguinte ao fechamento mensal e versao quadrimestral no fechamento quadrimestral.

## 6. Registro analitico
### Fatos
- O portfolio tem 3 iniciativas ativas com IDs formalizados.
- A base de KPI ainda nao foi consolidada no recorte mensal completo.
- Ha risco transversal de capacidade em 2 iniciativas e bloqueio de sistema em 1 iniciativa.

### Hipoteses
- A validacao do calendario fixo de fechamento tende a aumentar previsibilidade e reduzir divergencias de recorte.

### Analises
- A implantacao documental esta funcional, mas a rotina recorrente depende de fechamento das lacunas de governanca nas iniciativas P-2026-002 e P-2026-003.

### Recomendacoes
- Validar o pacote de governanca desta one-page ate 2026-04-05.
- Executar o fechamento mensal completo do mes 2026-04 em 2026-05-02.
- Abrir plano de acao de KPI imediatamente quando houver primeira consolidacao fora da meta.

## 7. Historico de revisoes
| Data | Alteracao | Responsavel |
|---|---|---|
| 2026-04-02 | Criacao da one-page macro da area PPMC para fechamento de implantacao e operacao recorrente. | Codex |
