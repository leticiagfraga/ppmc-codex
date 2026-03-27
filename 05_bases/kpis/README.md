# Bases de KPIs PPMC (Fonte Operacional)

## Resumo executivo
A pasta `05_bases/kpis` e a fonte operacional editavel pelo Codex para KPIs e metas. O arquivo `PPC_KPIs_e_Metas_2026.xlsx` permanece como artefato executivo de consolidacao.

## Metadados
- Contexto: migracao para modelo hibrido de operacao PPMC.
- Objetivo: garantir base estruturada, versionavel e confiavel para leitura e edicao recorrente.
- Escopo: todos os CSVs desta pasta e sua sincronizacao com os dossies das iniciativas.
- Responsavel(is): Leticia Fraga (dona funcional); Codex (apoio operacional).
- Data de criacao: 2026-03-26.
- Data da ultima atualizacao: 2026-03-27.
- Status: ativo.
- Referencias relacionadas: `00_governanca/regras_derivacao_kpis.md`, `00_governanca/rotina_operacional_codex_ppmc.md`, `01_projetos/*`.
- Proximo passo: executar fechamento mensal usando a ordem oficial de sincronizacao.
- Prazo: [definir].
- Riscos ou bloqueios: atualizar CSV sem atualizar documento fonte gera divergencia de governanca.
- Decisoes pendentes: confirmar cadencia formal de publicacao da leitura executiva da planilha `.xlsx`.

## 1. Estrutura da pasta
- `dicionario_kpis.csv`: catalogo oficial de indicadores, formula, fonte e responsavel.
- `base_processos_criticos.csv`: base mensal da governanca de processos criticos.
- `base_projetos_ativos.csv`: base mensal de iniciativas ativas e campos derivados.
- `base_entregas.csv`: base mensal no nivel de entrega.
- `base_pesquisa.csv`: respostas de satisfacao/adocao pos-implantacao.
- `base_mudancas_escopo.csv`: trilha de mudancas de escopo e lead time de aprovacao.
- `entrada_mensal_kpis.csv`: consolidado mensal por KPI (jan-dez).
- `status_kpis.csv`: leitura executiva do periodo vigente.
- `plano_acoes_kpis.csv`: plano de acao para desvios de meta.

## 2. Regra operacional de sincronizacao
### Ordem obrigatoria
1. Atualizacao documental primeiro.
2. Atualizacao das bases CSV depois.
3. Consolidacao mensal em seguida.
4. Leitura executiva por ultimo.

### 2.1 Quando atualizar documentos da iniciativa
Atualizar os arquivos do dossie (`01_projetos/<slug>`) sempre que houver:
- mudanca de status;
- novo risco/impedimento;
- nova entrega/marco;
- decisao relevante;
- mudanca de escopo.

### 2.2 Quando refletir em `base_projetos_ativos.csv`
Atualizar imediatamente apos revisar:
- `02_status_report.md`
- `03_riscos_impedimentos.md`
- `04_decisoes_atas.md`
- `05_entregas_marcos.md`

Campos derivados obrigatorios:
- `governanca_em_dia`
- `ultimo_status_report`
- `risco_critico_aberto`

### 2.3 Quando recalcular `entrada_mensal_kpis.csv`
- No fechamento mensal, apos atualizar todas as bases do `ano`/`mes`.
- Sempre que houver correcao retroativa em base fonte.

### 2.4 Quando revisar `status_kpis.csv`
- Apos recalculo de `entrada_mensal_kpis.csv`.
- Quando houver mudanca de meta, formula, regra de status ou comentario executivo.

### 2.5 Quando propor atualizacao do `PPC_KPIs_e_Metas_2026.xlsx`
- No fechamento mensal (recomendado).
- Obrigatoriamente no fechamento quadrimestral.
- Somente apos validacao de consistencia entre dossies e CSVs.

Se o `.xlsx` nao estiver disponivel no repositorio, registrar a lacuna no fechamento e manter os CSVs como consolidado oficial.

## 3. Regras de preenchimento
- Nao inventar dados reais; usar placeholders explicitos (`[definir]`) quando faltar informacao.
- Datas no padrao `AAAA-MM-DD`.
- Campos booleanos em `Sim` ou `Nao`.
- Usar `N_A` apenas quando nao aplicavel e com justificativa em `observacoes`.

## 4. Mapa de derivacao rapida
| Campo alvo | Origem | Regra resumida |
|---|---|---|
| `governanca_em_dia` | dossie da iniciativa | `Sim` somente com todos os obrigatorios em dia; senao `Nao`. |
| `ultimo_status_report` | `02_status_report.md` | Data do campo derivado; fallback para ultima atualizacao. |
| `risco_critico_aberto` | `03_riscos_impedimentos.md` | `Sim` se houver risco alto aberto/em tratamento; `Nao` se nao houver; `N_A` se dado insuficiente. |

## 5. Fluxo operacional do dia a dia
1. Atualizar dossie da iniciativa.
2. Aplicar derivacao em `base_projetos_ativos.csv`.
3. Atualizar bases complementares (`entregas`, `mudancas`, `pesquisa`, `processos`) conforme eventos.
4. No fechamento mensal, consolidar `entrada_mensal_kpis.csv` e revisar `status_kpis.csv`.
5. Abrir ou atualizar `plano_acoes_kpis.csv` para KPI fora da meta.

## 6. Historico de revisoes
| Data | Alteracao | Responsavel |
|---|---|---|
| 2026-03-27 | Refinamento da regra de sincronizacao e do mapa de derivacao operacional. | Codex |
| 2026-03-26 | Criacao da base operacional de KPIs em CSV e regras de sincronizacao. | Codex |
