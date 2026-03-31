---
task: rank-stories
order: 2
input: squads/linkedin-squad/output/news-found.md (partial)
output: squads/linkedin-squad/output/news-found.md
---

# Process: Ranqueamento Estratégico de Notícias

1. **Análise de Relevância**: Avalie cada notícia do `raw_news` com base na aderência aos serviços da **Agência Cognitiva** (C.O.R.E.™, Agentic AI, Governança).
2. **Atribuição de Score**: Dê uma nota de 1 a 10 para cada item.
3. **Justificativa**: Escreva uma frase explicando por que cada notícia foi ranqueada dessa forma.
4. **Resumo Executivo**: Crie uma tabela final para o usuário selecionar a pauta.

## Output Format
```yaml
ranked_stories:
  - id: number
    title: string
    source: string
    score: number (1-10)
    justification: string
    recommendation: "Recommended" | "Secondary" | "Skip"
```

## Output Example
```yaml
ranked_stories:
  - id: 1
    title: "Gartner Predicts 40% Growth in Agentic AI Adoption"
    source: "Gartner"
    score: 10
    justification: "Conecta perfeitamente com nosso serviço de Pilot Agent e valida nossa tese de mercado."
    recommendation: "Recommended"
```

## Quality Criteria
- [ ] O score reflete a oportunidade real de negócio, não apenas o "hype".
- [ ] A justificativa é específica para a Agência Cognitiva.
- [ ] Existe pelo menos uma história com Recomendação "Recommended".

## Veto Conditions
- Se todos os scores forem idênticos (falta de análise crítica).
- Se a justificativa for genérica (ex: "é importante para tecnologia").
