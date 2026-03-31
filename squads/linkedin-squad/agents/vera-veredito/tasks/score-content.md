---
task: score-content
order: 1
input: squads/linkedin-squad/output/linkedin-post.md
output: squads/linkedin-squad/output/review-result.md (partial)
---

# Process: Escaneamento e Pontuação de Qualidade

1. **Auditoria de Critérios**: Avalie o post contra o arquivo `quality-criteria.md`.
2. **Dimensionamento**: Atribua notas (1-10) para:
   - **Hook**: Poder de parada de scroll.
   - **Autoridade**: Nível de insight técnico/mercado.
   - **Engajamento**: Qualidade da CTA.
   - **Legibilidade**: Formatação mobile e fluidez.
   - **Conformidade**: Ausência de anti-padrões e tom de voz correto.
3. **Cálculo da Média**: Calcule a nota final.

## Output Format
```yaml
scoring:
  hook: number
  authority: number
  engagement: number
  readability: number
  compliance: number
  overall_score: number
  verdict: "APROVADO" | "REJEITADO"
```

## Output Example
```yaml
scoring:
  hook: 9
  authority: 8
  engagement: 8
  readability: 10
  compliance: 9
  overall_score: 8.8
  verdict: "APROVADO"
```

## Quality Criteria
- [ ] Notas justificadas com base nos arquivos de referência.
- [ ] O veredito "REJEITADO" é obrigatório se a nota Compliance for < 7.

## Veto Conditions
- Se houver pontuações máximas (10) em todos os campos sem uma justificativa excepcional.
- Se o veredito ignorar violações claras de anti-padrões.
