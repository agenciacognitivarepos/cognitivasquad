---
task: optimize-linkedin-post
order: 3
input: squads/linkedin-squad/output/linkedin-post.md (partial)
output: squads/linkedin-squad/output/linkedin-post.md
---

# Process: Otimização e Refinamento de Post

1. **Verificação de Anti-Padrões**: Passe o post pelo filtro de `anti-patterns.md`. Remova clichês de IA e termos proibidos.
2. **Polimento de Estilo**: Garanta que cada parágrafo tenha no máximo 3 linhas.
3. **Check de Veto**: Verifique se o post atende a todos os critérios de qualidade do agente.
4. **Finalização Visual**: Adicione 3 a 5 hashtags estratégicas apenas ao final e uma nota sobre o "first comment" para links.

## Output Format
```markdown
# LinkedIn Post Final
{hook}

{body}

{cta}

# Hashtags
#{tag1} #{tag2} #{tag3}
```

## Output Example
```markdown
# LinkedIn Post Final
O fim dos chatbots burros começou hoje.

Segundo o Gartner, a era da IA conversacional passiva está sendo substituída pelos Agentes de Ação...

Na Agência Cognitiva, nosso framework C.O.R.E.™ garante...

O que você delegaria para um agente hoje se soubesse que ele não falharia?

# Hashtags
#AgenticAI #B2BTech #AgenciaCognitiva
```

## Quality Criteria
- [ ] Zero termos como "Revolutionize" ou "Game-changer".
- [ ] O post está visualmente "escaneável".
- [ ] A CTA é a última linha antes das hashtags.

## Veto Conditions
- Se as hashtags forem o foco principal do post.
- Se o post final se assemelhar a um press release corporativo.
