---
task: create-linkedin-post
order: 2
input: squads/linkedin-squad/output/selected-angle.md
output: squads/linkedin-squad/output/linkedin-post.md (partial)
format: linkedin-post
---

# Process: Composição de Post para LinkedIn

1. **Revisão de Contexto**: Leia o ângulo selecionado em `selected-angle.md` e o framework em `domain-framework.md`.
2. **Construção do Hook**: Crie 3 opções de ganchos iniciais (menos de 12 palavras) e escolha o mais impactante.
3. **Escrita do Corpo**: Utilize o framework PAS (Problema, Agitação, Solução) ou BAB (Antes, Depois, Ponte).
4. **Ponte de Produto**: Conecte o conteúdo a um dos produtos ou serviços da Agência Cognitiva descritos no perfil da empresa.
5. **Call to Action (CTA)**: Finalize com uma pergunta aberta que incentive discussões técnicas ou de negócio.

## Output Format
```yaml
post_content:
  hook: string
  body: string
  cta: string
  format_notes: string
```

## Output Example
```yaml
post_content:
  hook: "A IA não é o fim da sua carreira técnica. É o início da sua era de orquestração."
  body: "Hoje, o mercado exige mais do que apenas código. Exige a capacidade de desenhar ecossistemas produtivos...\n\nNa Agência Cognitiva, acreditamos no C.O.R.E.™..."
  cta: "Você prefere gerenciar linhas de código ou orquestrar agentes autônomos?"
  format_notes: "Usei espaços entre parágrafos e bullet points para leitura mobile."
```

## Quality Criteria
- [ ] O gancho é curto e provocador.
- [ ] A conexão com o produto da empresa é fluida e não soa como "anúncio".
- [ ] O tom de voz segue exatamente o estilo sugerido em `tone-of-voice.md`.

## Veto Conditions
- Se houver links externos no corpo do post.
- Se o post for um bloco de texto único sem quebras de parágrafo.
