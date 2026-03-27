# Regras de Derivacao de KPIs e Campos Executivos

## Resumo executivo
Este documento define as regras oficiais para derivar campos executivos da base de projetos e consolidar KPIs da area PPMC no modelo hibrido.

Ordem obrigatoria de operacao:
1. Atualizacao documental da iniciativa.
2. Atualizacao das bases CSV.
3. Consolidacao mensal dos KPIs.
4. Leitura executiva e proposta de atualizacao da planilha `.xlsx`.

## Metadados
- Contexto: implantacao do modelo operacional hibrido da area PPMC.
- Objetivo: padronizar derivacoes, reduzir subjetividade e manter rastreabilidade.
- Escopo: `01_projetos/*` e `05_bases/kpis/*.csv`.
- Responsavel(is): Leticia Fraga (dona funcional); Codex (apoio operacional).
- Data de criacao: 2026-03-26.
- Data da ultima atualizacao: 2026-03-27.
- Status: ativo.
- Referencias relacionadas: `05_bases/kpis/README.md`, `00_governanca/rotina_operacional_codex_ppmc.md`, `01_projetos/*/02_status_report.md`, `01_projetos/*/03_riscos_impedimentos.md`.
- Proximo passo: aplicar a derivacao no proximo fechamento mensal.
- Prazo: [definir].
- Riscos ou bloqueios: preenchimento incompleto dos dossies reduz confiabilidade da derivacao.
- Decisoes pendentes: confirmar periodicidade oficial de apuracao (mensal recomendado).

## 1. Definicoes de apuracao
- Periodo de apuracao: recorte `ano` e `mes` usado nas bases CSV (ex.: `2026` e `3`).
- Iniciativa ativa no periodo: iniciativa registrada em `base_projetos_ativos.csv` para o mes de referencia.
- Documento minimamente preenchido:
  - metadados obrigatorios preenchidos;
  - secao operacional principal com pelo menos um registro valido ou `N_A` justificado quando cabivel;
  - historico de revisoes atualizado.

## 2. Regra oficial - `governanca_em_dia`
### Resultado permitido
- `Sim`
- `Nao`

### `governanca_em_dia = Sim`
Quando TODOS os itens obrigatorios abaixo estao atendidos para a iniciativa no periodo:
1. `01_charter_kickoff.md` existe e esta minimamente preenchido.
2. Escopo aprovado/documentado no charter (`## 3. Escopo aprovado`) com aprovacao inicial registrada.
3. Baseline de cronograma ou marcos principais documentados em `05_entregas_marcos.md`.
4. `02_status_report.md` atualizado no periodo de apuracao.
5. `03_riscos_impedimentos.md` atualizado com registro ativo.
6. `04_decisoes_atas.md` atualizado quando aplicavel, ou `N_A` justificado.

### `governanca_em_dia = Nao`
Quando QUALQUER item obrigatorio estiver:
- ausente;
- vazio;
- desatualizado para o periodo;
- marcado como `N_A` sem justificativa objetiva.

## 3. Regra oficial - `ultimo_status_report`
### Fonte primaria
- `01_projetos/<slug>/02_status_report.md`.

### Regra de derivacao
1. Priorizar o campo `Ultimo_Status_Report (derivacao): AAAA-MM-DD`.
2. Se ausente, usar `Data da ultima atualizacao` do mesmo arquivo.
3. Escrever em `base_projetos_ativos.csv` na coluna `ultimo_status_report`.

### Validacao temporal
- Para o mes apurado, a data deve estar no mesmo `ano`/`mes`.
- Se fora do periodo, `governanca_em_dia` deve ser `Nao`.

## 4. Regra oficial - `risco_critico_aberto`
### Resultado permitido
- `Sim`
- `Nao`
- `N_A` (apenas para dado insuficiente, com justificativa em `observacoes`)

### Fonte primaria
- `01_projetos/<slug>/03_riscos_impedimentos.md`.

### Regra de derivacao
- `risco_critico_aberto = Sim` quando existir ao menos uma linha com:
  - `Tipo = risco`;
  - `Criticidade = alta`;
  - `Status = aberto` ou `em tratamento`.
- `risco_critico_aberto = Nao` quando o registro estiver atualizado e nenhum risco atender o criterio acima.
- `risco_critico_aberto = N_A` quando nao houver dado minimo para classificar criticidade/status (ex.: campos essenciais como `[definir]`).

### Relacao com governanca
- Se `risco_critico_aberto = N_A` por dado insuficiente, classificar `governanca_em_dia = Nao`.

## 5. Campos que o Codex deve atualizar automaticamente

| Base | Campo | Origem principal | Regra |
|---|---|---|---|
| `base_projetos_ativos.csv` | `status_projeto` | `02_status_report.md` | Copiar status geral vigente. |
| `base_projetos_ativos.csv` | `governanca_em_dia` | dossie da iniciativa | Aplicar secao 2. |
| `base_projetos_ativos.csv` | `ultimo_status_report` | `02_status_report.md` | Aplicar secao 3. |
| `base_projetos_ativos.csv` | `risco_critico_aberto` | `03_riscos_impedimentos.md` | Aplicar secao 4. |
| `base_projetos_ativos.csv` | `observacoes` | analise do ciclo | Registrar lacunas, alertas e justificativas de `N_A`. |
| `base_entregas.csv` | colunas de prazo/replanejamento | `05_entregas_marcos.md` | Espelhar entregas e status do periodo. |
| `base_mudancas_escopo.csv` | colunas de mudanca/aprovacao | `07_change_requests.md` | Espelhar mudancas identificadas e decisoes. |

## 6. Regra de uso de `N_A`
Usar `N_A` somente quando o item nao for aplicavel por natureza do periodo/iniciativa, com justificativa objetiva contendo:
- motivo;
- responsavel pela justificativa;
- data.

Nao usar `N_A` para esconder dado faltante de item obrigatorio. Nesse caso:
- usar `[definir]` no documento fonte;
- registrar pendencia em `observacoes`;
- classificar `governanca_em_dia = Nao`.

## 7. Ordem operacional obrigatoria
1. Atualizar `01_projetos/<slug>/*.md`.
2. Refletir derivacoes nas bases CSV (`05_bases/kpis/*.csv`).
3. Consolidar `entrada_mensal_kpis.csv` e revisar `status_kpis.csv`.
4. Propor atualizacao do `PPC_KPIs_e_Metas_2026.xlsx`.

Se o `.xlsx` nao estiver no repositorio, registrar lacuna explicitamente no fechamento e manter consolidacao nos CSVs.

## 8. Historico de revisoes
| Data | Alteracao | Responsavel |
|---|---|---|
| 2026-03-27 | Refinamento das regras de derivacao, incluindo tratamento de dado insuficiente e tabela de campos automaticos. | Codex |
| 2026-03-26 | Criacao das regras oficiais de derivacao de campos executivos e KPIs. | Codex |
