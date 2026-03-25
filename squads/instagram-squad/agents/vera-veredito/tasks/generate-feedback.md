---
name: "Generate Feedback"
order: 2
input: "content-score.yaml"
output: "reviewer-feedback.md"
---

# Generate Feedback

## Process
1. Escrever um feedback detalhado explicando as notas dadas no `score-content.yaml`.
2. Se reprovado, listar exatamente o que deve ser alterado (on_reject loop).
3. Se aprovado, celebrar a qualidade e destacar o ponto mais forte.

## Output Format
Markdown document with score table and bullet points.

## Quality Criteria
- Tom polido e construtivo.
- Feedback acionável.
