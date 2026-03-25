---
name: "Rank Stories"
order: 2
input: "raw-news.md"
output: "ranked-news.md"
---

# Rank Stories

## Process
1. Analisar as notícias listadas em `raw-news.md`.
2. Avaliar cada notícia pelo impacto estratégico para executivos (1-5) e relevância para o C-Level (1-5).
3. Selecionar as 3 melhores notícias e justificar a escolha com base no perfil da Agência Cognitiva.
4. Salvar as notícias ranqueadas em `ranked-news.md`.

## Output Format (YAML schema)
```yaml
ranked_news:
  - title: string
    rank: integer
    justification: string
    impact_score: integer
```

## Output Example
```yaml
ranked_news:
  - title: "NVIDIA NIM para microsserviços"
    rank: 1
    justification: "Impacta diretamente a infraestrutura de agentes em escala, diferencial da AC."
    impact_score: 5
```

## Quality Criteria
- Justificativa clara ligando a notícia à Agência Cognitiva.
- Ranqueamento lógico.

## Veto Conditions
- Se não houver justificativa.
- Se o impacto não estiver relacionado a negócios.
