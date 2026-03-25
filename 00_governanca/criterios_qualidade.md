# Critérios de Qualidade PPMC

## Metadados
- Contexto: necessidade de garantir consistência e qualidade mínima dos artefatos da área.
- Objetivo: definir critérios objetivos de validação antes de considerar um documento pronto para uso.
- Escopo: documentos de governança, projetos, processos e melhoria contínua.
- Responsável(is): área de Projetos, Processos e Melhoria Contínua (PPMC).
- Data de criação: 2026-03-25.
- Data da última atualização: 2026-03-25.
- Status: ativo.
- Referências relacionadas: `AGENTS.md`, `README.md`, `00_governanca/glossario.md`, `00_governanca/padroes_documentais.md`.
- Próximo passo: aplicar estes critérios nos próximos artefatos revisados pela área.
- Prazo: 2026-04-15.
- Riscos ou bloqueios: avaliação subjetiva sem evidência mínima de qualidade.
- Decisões pendentes: formalizar periodicidade de auditoria de qualidade documental.

## Regras de aprovação mínima
Um documento só deve ser considerado pronto quando atender simultaneamente:
- completude mínima;
- clareza e consistência;
- rastreabilidade;
- orientação à execução.

## Matriz de critérios
| Critério | Pergunta de validação | Evidência mínima esperada |
|---|---|---|
| Pasta correta | O conteúdo está na frente adequada (`00` a `04`)? | Arquivo salvo na estrutura oficial. |
| Metadados obrigatórios | Os campos essenciais estão preenchidos? | Contexto, objetivo, escopo, responsável, datas, status, referências, próximo passo, prazo, riscos/bloqueios, decisões pendentes. |
| Clareza | Alguém fora do contexto imediato entende o documento? | Texto objetivo, sem ambiguidades críticas. |
| Classificação da informação | Fato, hipótese, análise e recomendação estão separados quando aplicável? | Seções ou marcações explícitas. |
| Orientação à execução | Existe encaminhamento concreto? | Próximo passo com responsável e prazo definido. |
| Rastreabilidade | Há vínculo com documentos relacionados e histórico de mudanças relevantes? | Referências e histórico registrados. |
| Coerência terminológica | Termos críticos seguem o glossário? | Uso aderente a `00_governanca/glossario.md`. |
| Status atualizado | O status reflete o estágio real do documento? | Valor coerente com `rascunho`, `em revisão`, `ativo` ou `arquivado`. |

## Critérios adicionais por frente
### Projetos (`01_projetos`)
- objetivo, escopo, entregas, riscos, dependências e status claramente descritos;
- decisões pendentes e bloqueios destacados;
- próximo passo orientado à gestão e execução.

### Processos (`02_processos`)
- separação explícita entre As Is e To Be;
- gatilho, entradas, saídas, papéis, regras, exceções, indicadores, controles e sistemas identificados;
- ganho esperado e forma de validação registrados.

### Melhoria contínua (`03_melhoria_continua`)
- problema, evidência, hipótese de causa, ação proposta, benefício esperado, responsável, prazo e métrica presentes;
- priorização por impacto, esforço e risco;
- recomendações convertidas em ações verificáveis.

## Resultado da revisão de qualidade
Usar uma das classificações abaixo:
- aprovado: atende aos critérios mínimos.
- aprovado com ressalvas: utilizável, mas com ajustes obrigatórios de curto prazo.
- reprovado: não atende aos critérios mínimos e exige revisão antes de uso.

## Registro mínimo de revisão
```md
## Revisão de qualidade
- Data da revisão:
- Revisor(a):
- Resultado:
- Principais ajustes necessários:
- Prazo para regularização:
```

## Histórico de revisões
| Data | Alteração | Responsável |
|---|---|---|
| 2026-03-25 | Criação da versão inicial dos critérios de qualidade. | Codex |
