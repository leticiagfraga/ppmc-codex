# Rotina Operacional Codex - PPMC

## Resumo executivo
Este guia define a operacao recorrente do repositorio PPMC no modelo hibrido:
- dossie documental por iniciativa em `01_projetos`;
- bases estruturadas em CSV em `05_bases/kpis`;
- planilha `.xlsx` como artefato executivo de consolidacao.

## Metadados
- Contexto: padronizar a rotina mensal e quadrimestral da area PPMC.
- Objetivo: garantir consistencia entre documentos, bases estruturadas e leitura executiva.
- Escopo: `01_projetos`, `05_bases/kpis`, `00_governanca` e consolidacao executiva.
- Responsavel(is): Leticia Fraga (dona operacional); Codex (apoio operacional).
- Data de criacao: 2026-03-26.
- Data da ultima atualizacao: 2026-04-02.
- Status: ativo.
- Referencias relacionadas: `00_governanca/regras_derivacao_kpis.md`, `05_bases/kpis/README.md`, `01_projetos/portfolio_iniciativas_2026.md`.
- Proximo passo: validar os parametros oficiais desta rotina e executar o primeiro fechamento mensal em data fixa.
- Prazo: 2026-05-02.
- Riscos ou bloqueios: atualizacao fora da ordem oficial pode gerar divergencia entre fonte documental e base executiva.
- Decisoes pendentes: validar formalmente os parametros da secao 7.

## 1. Como atualizar uma iniciativa
1. Abrir `01_projetos/<slug>/`.
2. Atualizar no minimo:
   - `02_status_report.md`
   - `03_riscos_impedimentos.md`
   - `05_entregas_marcos.md`
   - `04_decisoes_atas.md` (ou `N_A` justificado)
3. Validar metadados obrigatorios e separar fato/hipotese/analise/recomendacao quando aplicavel.
4. Atualizar `Data da ultima atualizacao` e `Historico de revisoes` de cada arquivo alterado.
5. Se faltar dado real, registrar `[definir]` em vez de inferir.

Responsavel primario: gerente da iniciativa.
Prazo recomendado: ate D-2 do fechamento mensal.

## 2. Como gerar um status report
1. Preencher `02_status_report.md` com:
   - resumo executivo;
   - status geral;
   - entregas do periodo;
   - riscos e bloqueios;
   - dependencias;
   - decisoes pendentes;
   - proximos passos.
2. Atualizar `Ultimo_Status_Report (derivacao): AAAA-MM-DD`.
3. Garantir que riscos e dependencias tenham responsavel e prazo de tratativa.

Responsavel primario: gerente da iniciativa.
Prazo recomendado: ate D-1 do fechamento mensal.

## 3. Como refletir isso nas bases
1. Atualizar `base_projetos_ativos.csv` para cada iniciativa ativa no mes.
2. Derivar e preencher:
   - `governanca_em_dia`
   - `ultimo_status_report`
   - `risco_critico_aberto`
3. Atualizar `base_entregas.csv` quando houver movimento em entregas/marcos.
4. Atualizar `base_mudancas_escopo.csv` quando houver mudanca identificada, formalizada ou decidida.
5. Atualizar `observacoes` com lacunas e justificativas relevantes.

Responsavel primario: Codex com validacao da area.
Prazo recomendado: no dia do fechamento mensal.

## 4. Como validar se o KPI mensal refletiu
1. Confirmar que as bases fonte do `ano`/`mes` foram atualizadas.
2. Consolidar `entrada_mensal_kpis.csv`.
3. Revisar `status_kpis.csv` (valor atual, meta, status e comentario executivo).
4. Quando houver desvio de meta, abrir ou atualizar `plano_acoes_kpis.csv`.

Responsavel primario: area PPMC com apoio do Codex.
Prazo recomendado: D+1 do fechamento mensal.

## 5. Como identificar e corrigir inconsistencias
Checklist minimo:
- `governanca_em_dia = Sim` sem status report no periodo -> inconsistente.
- `risco_critico_aberto = Sim` sem risco critico correspondente -> inconsistente.
- `data_real` preenchida em entrega sem `entregue_no_prazo` -> inconsistente.
- mudanca com `aprovada = sim/nao` e `data_decisao` vazia -> inconsistente.

Tratativa padrao:
1. Corrigir primeiro o documento fonte da iniciativa.
2. Reaplicar derivacao no CSV afetado.
3. Registrar ajuste no historico de revisoes do documento fonte.
4. Anotar alerta em `observacoes` quando a regularizacao depender de terceiros.

## 6. Como operar o fechamento quadrimestral
1. Congelar a consolidacao mensal do ultimo mes do quadrimestre.
2. Revisar 100% das iniciativas ativas no periodo.
3. Revalidar os campos derivados em `base_projetos_ativos.csv`.
4. Revisar KPIs em `status_kpis.csv` e priorizar desvios em `plano_acoes_kpis.csv`.
5. Gerar leitura executiva quadrimestral para decisao de gestao.
6. Propor atualizacao do `PPC_KPIs_e_Metas_2026.xlsx`.

Se o `.xlsx` nao estiver no repositorio no momento do fechamento, registrar a lacuna e manter consolidacao oficial nos CSVs.

## 7. Cadencia oficial (proposta para validacao)
- Periodicidade oficial de apuracao: mensal.
- Data fixa de fechamento mensal: dia 2 de cada mes (apuracao do mes anterior).
- Data fixa de fechamento quadrimestral: dia 5 de maio, dia 5 de setembro e dia 5 de janeiro.
- Cadencia de publicacao da leitura executiva: mensal no dia util seguinte ao fechamento mensal e versao quadrimestral no fechamento quadrimestral.
- Curadoria formal do portfolio: Leticia Fraga (curadoria funcional) com apoio tecnico do Codex.
- Criterio oficial de saude das iniciativas:
  - Verde: `governanca_em_dia = Sim`, `risco_critico_aberto = Nao` e `ultimo_status_report` no periodo de apuracao.
  - Amarelo: exatamente um criterio acima nao atendido ou `risco_critico_aberto = N_A` por lacuna documental.
  - Vermelho: dois ou mais criterios nao atendidos ou `risco_critico_aberto = Sim`.

## 8. Historico de revisoes
| Data | Alteracao | Responsavel |
|---|---|---|
| 2026-04-02 | Fechamento das pendencias de calendario, curadoria e criterio de saude como proposta objetiva para validacao. | Codex |
| 2026-03-27 | Refinamento do passo a passo operacional mensal/quadrimestral com responsaveis e prazos recomendados. | Codex |
| 2026-03-26 | Criacao da rotina operacional recorrente do Codex para o modelo hibrido PPMC. | Codex |
