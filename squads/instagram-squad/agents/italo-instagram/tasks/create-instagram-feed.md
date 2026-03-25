---
name: "Create Instagram Feed"
order: 2
input: "selected-angle.md"
output: "feed-script.md"
---

# Create Instagram Feed

## Process
1. Ler o ângulo selecionado pelo usuário.
2. Criar um roteiro de carrossel (6-8 slides) seguindo o framework AIDA ou PAS.
3. Usar a pesquisa visual (azul escuro, 3D, minimalismo) para sugerir a descrição de cada imagem/slide.
4. Escrever a legenda completa do post, incluindo hashtags e CTA.

## Output Format (YAML schema)
```yaml
carousel:
  slides:
    - number: integer
      text: string
      visual_description: string
caption: string
hashtags: string[]
cta: string
```

## Output Example
```yaml
carousel:
  slides:
    - number: 1
      text: "Sua IA está presa na Sandbox?"
      visual_description: "Robô 3D atrás de uma barreira de vidro futurista azul."
caption: "O mercado vende projetos, nós construímos produtos. A transição para um ecossistema agêntico exige..."
```

## Quality Criteria
- Mensagem clara e sofisticada.
- Contraste forte entre mercado e Agência Cognitiva.
- CTA direto para liderança.

## Veto Conditions
- Texto infantil ou com excesso de emojis.
- Falta de menção ao método C.O.R.E.
