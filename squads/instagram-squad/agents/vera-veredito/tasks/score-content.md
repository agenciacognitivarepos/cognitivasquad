---
name: "Score Content"
order: 1
input: "optimized-feed.md"
output: "content-score.yaml"
---

# Score Content

## Process
1. Avaliar o conteúdo otimizado contra os critérios em `quality-criteria.md`.
2. Atribuir notas de 1 a 5 para: Alinhamento Estratégico, Contraste, Qualidade do Copy e Tom de Voz.
3. Decidir o veredito final (Aprovado/Reprovado).

## Output Format (YAML schema)
```yaml
scores:
  strategy: integer
  contrast: integer
  copy: integer
  tone: integer
verdict: "Approved" | "Rejected"
```

## Quality Criteria
- Avaliação imparcial e rigorosa.
