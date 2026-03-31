---
task: generate-feedback
order: 2
input: squads/linkedin-squad/output/review-result.md (partial)
output: squads/linkedin-squad/output/review-result.md
---

# Process: Geração de Feedback Construtivo

1. **Sintetização de Falhas**: Se o veredito for "REJEITADO", identifique os 3 pontos de melhoria mais urgentes.
2. **Instruções de Refação**: Escreva orientações claras para o criador, baseando-se nos arquivos de `anti-patterns.md` e `tone-of-voice.md`.
3. **Elogio de Pontos Fortes**: Identifique o que está bom para garantir que não seja perdido na refação.

## Output Format
```markdown
# Veredito Final: {APROVADO/REJEITADO}

## Resumo da Revisão
{texto_resumo}

## Pontos Positivos
- {ponto_1}
- {ponto_2}

## Melhorias Necessárias (Se REJEITADO)
1. **{item}**: {instrucao}
2. **{item}**: {instrucao}

## Próximos Passos
{proximo_passo}
```

## Output Example
```markdown
# Veredito Final: REJEITADO

## Resumo da Revisão
O post apresenta uma boa profundidade técnica, mas falha gravemente no gancho inicial e na conformidade com o tom de voz pragmático da Agência Cognitiva.

## Pontos Positivos
- Uso correto do framework PAS no corpo do texto.
- Excelente conexão com o serviço de Pilot Agent.

## Melhorias Necessárias
1. **Otimização do Hook**: O gancho atual tem 18 palavras. Reduza para menos de 10 palavras focando no benefício direto ao leitor.
2. **Tom de Voz**: Remova adjetivos como "incrível" e "revolucionário". Substitua por dados ou termos técnicos.

## Próximos Passos
Lucas, por favor refaça a etapa de criação focando nestes pontos de ajuste.
```

## Quality Criteria
- [ ] Feedback é acionável e não apenas crítico.
- [ ] O tom do feedback é profissional e encorajador (Persona Vera).

## Veto Conditions
- Se o feedback instruir o criador a fazer algo que viole os anti-padrões do squad.
- Se não houver feedback em caso de rejeição.
