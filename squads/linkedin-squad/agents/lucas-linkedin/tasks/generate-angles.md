---
task: generate-angles
order: 1
input: squads/linkedin-squad/output/selected-story.md
output: squads/linkedin-squad/output/content-angles.md
---

# Process: Geração de Ângulos Estratégicos

1. **Contextualização**: Estude a notícia selecionada e identifique o "core" técnico e de mercado.
2. **Brainstorming de Perspectivas**: Crie 5 ângulos distintos baseados no framework sugerido:
   - **Medo**: Qual o custo da inércia?
   - **Oportunidade**: Qual a vantagem injusta de agir agora?
   - **Educacional**: Como isso funciona na prática técnica?
   - **Contrário**: Por que o mercado está exagerando ou ignorando um ponto vital?
   - **Inspiracional**: Como será o futuro após essa mudança?
3. **Justificativa**: Escreva uma frase para cada ângulo explicando por que ele funcionaria no LinkedIn hoje.

## Output Format
```yaml
angles:
  - type: "Medo" | "Oportunidade" | "Educacional" | "Contrário" | "Inspiracional"
    headline: string
    hook_preview: string (first line)
    summary: string
    justification: string
```

## Output Example
```yaml
angles:
  - type: "Contrário"
    headline: "O fim dos chatbots burros"
    hook_preview: "Chatbots estão mortos. E isso é a melhor notícia para o seu negócio."
    summary: "Desmistifica a ideia de que LLMs sozinhos resolvem tudo e introduz o conceito de agentes orquestrados."
    justification: "Ângulos contrários geram alto 'dwell time' e comentários de especialistas no LinkedIn."
```

## Quality Criteria
- [ ] Pelo menos 5 ângulos distintos gerados.
- [ ] Cada ângulo possui um gancho (hook) provocador.
- [ ] Os ângulos cobrem desde o espectro emocional até o técnico.

## Veto Conditions
- Se os ângulos forem variações superficiais da mesma ideia.
- Se não houver clareza sobre qual persona o ângulo atrai.
