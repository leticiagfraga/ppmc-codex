# Repositorio da Area de Projetos, Processos e Melhoria Continua (PPMC)

## Objetivo
Organizar os artefatos da area PPMC de forma simples, rastreavel, reutilizavel e orientada a execucao.

## Modelo operacional atual (hibrido)
- Fonte de verdade operacional: dossies das iniciativas em `01_projetos` + bases estruturadas em `05_bases/kpis`.
- Artefato executivo consolidado: `PPC_KPIs_e_Metas_2026.xlsx`.
- Regra de operacao: atualizar primeiro os documentos da iniciativa, depois os CSVs, depois a consolidacao mensal e por ultimo a leitura executiva.

## Estrutura da raiz
```text
.
├── .codex/
├── 00_governanca/
├── 01_projetos/
├── 02_processos/
├── 03_melhoria_continua/
├── 04_templates/
├── 05_bases/
├── AGENTS.md
└── README.md
```

## Dossie padrao por iniciativa
Cada iniciativa em `01_projetos/<slug_da_iniciativa>/` deve conter:
- `00_contexto_iniciativa.md`
- `01_charter_kickoff.md`
- `02_status_report.md`
- `03_riscos_impedimentos.md`
- `04_decisoes_atas.md`
- `05_entregas_marcos.md`
- `06_evidencias_referencias.md`
- `07_change_requests.md`

Iniciativas estruturadas:
- `01_projetos/jornada_do_cliente`
- `01_projetos/olympus`
- `01_projetos/metas_indicadores_area_ppmc`

## Bases estruturadas de KPI
Pasta: `05_bases/kpis`
- `README.md`: regra operacional de sincronizacao.
- `dicionario_kpis.csv`: definicao oficial dos indicadores.
- Bases operacionais: `base_processos_criticos.csv`, `base_projetos_ativos.csv`, `base_entregas.csv`, `base_pesquisa.csv`, `base_mudancas_escopo.csv`.
- Consolidacao e leitura: `entrada_mensal_kpis.csv`, `status_kpis.csv`, `plano_acoes_kpis.csv`.

## Governanca de derivacao
Regras oficiais em:
- `00_governanca/regras_derivacao_kpis.md`

Campos executivos derivados por regra:
- `governanca_em_dia`
- `ultimo_status_report`
- `risco_critico_aberto`

## Operacao no dia a dia
1. Atualize o dossie da iniciativa em `01_projetos/<slug>`.
2. Reflita a derivacao em `05_bases/kpis/base_projetos_ativos.csv`.
3. Atualize bases complementares (`entregas`, `mudancas`, `pesquisa`, `processos`) quando houver evento novo.
4. No fechamento mensal, consolide `entrada_mensal_kpis.csv` e revise `status_kpis.csv`.
5. No fechamento quadrimestral, gere leitura executiva e proponha atualizacao da planilha `.xlsx`.

Guia detalhado:
- `00_governanca/rotina_operacional_codex_ppmc.md`

## Lacuna registrada
- Em 2026-03-27 nao foi encontrado no workspace o arquivo `PPC_KPIs_e_Metas_2026.xlsx`.
- Acao recomendada: incluir a planilha no repositorio para manter a trilha completa do modelo hibrido.

## Regras importantes
- Trabalhar em portugues do Brasil.
- Nao inventar dados reais da empresa.
- Registrar lacunas com placeholders explicitos (ex.: `[definir]`).
- Preservar historico de revisoes em documentos markdown.
- Preferir templates existentes em `04_templates`.
