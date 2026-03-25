---
name: "Generate Angles"
order: 1
input: "selected-news.md"
output: "content-angles.md"
---

# Generate Angles

## Process
1. Ler a notícia selecionada em `selected-news.md`.
2. Usar o `domain-framework.md` para entender como aplicar o contraste da Agência Cognitiva.
3. Gerar 5 ângulos de copywriting (Medo, Oportunidade, Pragmático, Contrário, Inspiracional) que tragam uma perspectiva executiva sobre a notícia.
4. Cada ângulo deve conter: Título (gancho), Ideia Central e Argumento de Contraste com o produto da AC.

## Output Format (YAML schema)
```yaml
angles:
  - type: "Medo" | "Oportunidade" | "Pragmático" | "Contrário" | "Inspiracional"
    hook: string
    concept: string
    contrast_argument: string
```

## Output Example
```yaml
angles:
  - type: "Contrário"
    hook: "Por que você não deveria confiar no hype do GPT-5 (ainda)"
    concept: "Modelos são gratuitos, infraestrutura real de produção não é."
    contrast_argument: "Enquanto o mercado espera o próximo modelo, nós construímos Ecossistemas Agênticos que rodam hoje."
```

## Quality Criteria
- Mínimo de 5 ângulos distintos.
- Foco em C-Level (consequências de negócio).
- Contraste claro com a metodologia da Agência.

## Veto Conditions
- Se os ângulos forem repetitivos.
- Se forem puramente técnicos e sem "gancho" comercial.
