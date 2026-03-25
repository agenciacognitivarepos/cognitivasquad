---
name: "Optimize Content"
order: 3
input: "feed-script.md"
output: "optimized-feed.md"
---

# Optimize Content

## Process
1. Revisar o script gerado para garantir fluidez e impacto executivo.
2. Refinar os "hooks" para serem mais curtos e magnéticos.
3. Garantir que o vocabulário "Never Use" foi removido.
4. Adicionar variantes para o título do Slide 1 (A/B Test).

## Output Format (YAML schema)
```yaml
optimized_content:
  slides: list
  caption: string
  variants_title: string[]
```

## Quality Criteria
- Texto mais limpo e impactante que a versão anterior.
- Ganchos A/B consistentes.
