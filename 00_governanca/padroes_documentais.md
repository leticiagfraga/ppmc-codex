# Padrões Documentais PPMC

## Metadados
- Contexto: necessidade de uniformizar estrutura, linguagem e rastreabilidade dos artefatos da área.
- Objetivo: estabelecer padrão mínimo para documentos claros, comparáveis e executáveis.
- Escopo: todos os documentos produzidos no repositório `ppmc-codex`.
- Responsável(is): área de Projetos, Processos e Melhoria Contínua (PPMC).
- Data de criação: 2026-03-25.
- Data da última atualização: 2026-03-25.
- Status: ativo.
- Referências relacionadas: `AGENTS.md`, `README.md`, `00_governanca/glossario.md`, `00_governanca/criterios_qualidade.md`.
- Próximo passo: validar este padrão nos próximos documentos criados nas frentes de projeto, processo e melhoria.
- Prazo: 2026-04-15.
- Riscos ou bloqueios: adoção parcial dos padrões e manutenção de formatos legados sem convergência.
- Decisões pendentes: definir responsável formal pela revisão periódica deste padrão.

## Estrutura mínima obrigatória
Todo documento novo deve conter, quando aplicável:
- contexto;
- objetivo;
- escopo;
- responsável(is);
- data de criação;
- data da última atualização;
- status;
- referências relacionadas;
- próximo passo;
- prazo;
- riscos ou bloqueios;
- decisões pendentes.

## Padrão de linguagem
- Escrever em português do Brasil, com linguagem clara, prática e profissional.
- Priorizar frases objetivas e evitar termos vagos sem definição.
- Evitar jargão não padronizado; quando necessário, usar definição do glossário.
- Não registrar suposições como fatos.
- Quando o público for gerencial, iniciar com resumo executivo.

## Padrão de classificação do conteúdo
Para reduzir ambiguidades, separar explicitamente:
- Fato: informação com evidência verificável.
- Hipótese: suposição ainda não validada.
- Análise: interpretação estruturada de fatos e hipóteses.
- Recomendação: ação sugerida com base na análise.

## Padrão de status
Usar valores padronizados:
- rascunho: em elaboração inicial.
- em revisão: aguardando validação.
- ativo: aprovado para uso corrente.
- arquivado: obsoleto, mantido apenas para rastreabilidade.

## Padrão de nomenclatura
- Pastas em `snake_case`, curtas e sem ambiguidade.
- Arquivos em minúsculas com `_` separando termos.
- Quando fizer sentido, prefixar com data no formato `AAAA-MM-DD`.
- Evitar abreviações pouco óbvias.

## Padrão de rastreabilidade e histórico
- Referenciar documentos relacionados em seção própria.
- Não apagar conteúdo relevante sem justificativa registrada.
- Em revisões significativas, registrar histórico com data, alteração e responsável.
- Ao substituir material, preferir nova versão ou documento derivado.

## Modelo de bloco inicial recomendado
```md
## Metadados
- Contexto:
- Objetivo:
- Escopo:
- Responsável(is):
- Data de criação:
- Data da última atualização:
- Status:
- Referências relacionadas:
- Próximo passo:
- Prazo:
- Riscos ou bloqueios:
- Decisões pendentes:
```

## Checklist rápido antes de publicar
- O documento está na pasta correta?
- Os campos obrigatórios estão preenchidos?
- Há separação clara entre fato, hipótese, análise e recomendação?
- Existe responsável e prazo para o próximo passo?
- O status está atualizado?
- As referências estão registradas?

## Histórico de revisões
| Data | Alteração | Responsável |
|---|---|---|
| 2026-03-25 | Criação da versão inicial do padrão documental. | Codex |
