# Convenções de Nomenclatura PPMC

## Metadados
- Contexto: necessidade de consolidar um padrão único para nomeação de pastas e arquivos no repositório.
- Objetivo: padronizar nomenclatura para facilitar organização, busca, rastreabilidade e manutenção dos artefatos.
- Escopo: todas as pastas e arquivos do repositório `ppmc-codex`.
- Responsável(is): área de Projetos, Processos e Melhoria Contínua (PPMC).
- Data de criação: 2026-03-25.
- Data da última atualização: 2026-03-25.
- Status: ativo.
- Referências relacionadas: `AGENTS.md`, `README.md`, `00_governanca/padroes_documentais.md`, `00_governanca/criterios_qualidade.md`.
- Próximo passo: aplicar este padrão nos próximos documentos criados e revisar aderência dos materiais existentes.
- Prazo: 2026-04-15.
- Riscos ou bloqueios: manutenção de nomes legados fora do padrão e ambiguidade na identificação de artefatos.
- Decisões pendentes: definir responsável formal pela revisão periódica da nomenclatura.

## 1. Princípios gerais
- Priorizar nomes curtos, claros e sem ambiguidade.
- Usar padrão consistente em todo o repositório.
- Evitar variações para o mesmo tipo de artefato.
- Favorecer legibilidade para pessoas fora do contexto imediato.

## 2. Padrão oficial para pastas
- Usar `snake_case`.
- Usar apenas letras minúsculas, números e `_`.
- Não usar espaços, acentos ou caracteres especiais.
- Manter nomes descritivos e objetivos.
- Nas pastas de primeiro nível da estrutura oficial, manter prefixo numérico (`00_`, `01_`, `02_`, `03_`, `04_`) conforme padrão vigente.

### Exemplos para pastas
| Situação | Nome recomendado | Nome a evitar |
|---|---|---|
| Pasta temática | `fluxo_aprovacao` | `Fluxo Aprovacao` |
| Pasta de melhoria | `melhoria_cadastro_fornecedor` | `melhoria-cadastro-fornecedor` |
| Pasta de projeto | `implantacao_painel_gestao` | `ImplantacaoPainelGestao` |

## 3. Padrão oficial para arquivos
- Usar letras minúsculas e `_` entre termos.
- Usar nomes descritivos e aderentes ao conteúdo.
- Evitar abreviações pouco óbvias.
- Extensão padrão para documentos textuais: `.md`.
- Quando aplicável, usar prefixo de data no formato `AAAA-MM-DD`.

### Estruturas recomendadas para arquivos
- Sem data: `nome_documento.md`
- Com data: `AAAA-MM-DD_nome_documento.md`
- Template: `nome_documento_modelo.md`

## 4. Uso do prefixo de data (`AAAA-MM-DD`)
Usar prefixo de data quando o documento representar recorte temporal, como:
- planos com data de emissão;
- atas de reunião;
- registros de acompanhamento periódico;
- comunicações que precisem de ordenação cronológica explícita.

Não usar prefixo de data quando o documento for permanente ou de referência estável, como:
- glossário;
- critérios;
- convenções;
- templates reutilizáveis.

## 5. Siglas e abreviações
- Evitar siglas no nome do arquivo quando não forem amplamente conhecidas.
- Quando sigla for necessária, usar em minúsculas e manter consistência em todo o repositório.
- Se houver dúvida de entendimento, preferir termo por extenso.

## 6. Checklist rápido de validação
- O nome está em minúsculas?
- O separador usado é `_`?
- O nome descreve claramente o conteúdo?
- Há necessidade real de prefixo de data?
- Existe arquivo semelhante já disponível para evitar duplicidade?

## 7. Exemplos de nomenclatura recomendada
| Tipo de artefato | Exemplo recomendado |
|---|---|
| Plano de implantação | `2026-03-25_plano_implantacao.md` |
| Mapeamento de processo | `mapeamento_fluxo_aprovacao.md` |
| Backlog de melhorias | `backlog_melhorias_priorizado.md` |
| Template de status | `status_projeto_modelo.md` |

## Histórico de revisões
| Data | Alteração | Responsável |
|---|---|---|
| 2026-03-25 | Criação da convenção consolidada de nomenclatura para pastas e arquivos. | Codex |
