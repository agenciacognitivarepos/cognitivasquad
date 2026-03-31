---
task: find-news
order: 1
input: squads/linkedin-squad/output/research-focus.md
output: squads/linkedin-squad/output/news-found.md (partial)
---

# Process: Descoberta de Notícias Estratégicas

1. **Análise do Foco**: Leia o tema e o período em `research-focus.md`.
2. **Execução da Pesquisa**: Use `web_search` com uma query otimizada (ex: "{tema} tendências mercado tecnologia {ano}").
3. **Seleção Inicial**: Escolha os 5 links mais promissores e use `web_fetch` para ler o conteúdo.
4. **Extração de Dados**: Capture: Título, Data, Link, Resumo e os pontos técnicos principais.

## Output Format
```yaml
raw_news:
  - title: string
    source: string
    url: string
    date: date
    technical_points: [string, string]
    summary: string (min 3 sentences)
```

## Output Example
```yaml
raw_news:
  - title: "Gartner Predicts 40% Growth in Agentic AI Adoption by 2026"
    source: "Gartner Newsroom"
    url: "https://www.gartner.com/en/newsroom/..."
    date: "2025-03-25"
    technical_points:
      - "Shift from conversational to agentic interfaces"
      - "Need for robust orchestration layers"
    summary: "O Gartner indica uma mudança massiva para interfaces agênticas que realmente realizam tarefas. O relatório destaca que a governança de dados será o maior gargalo para essa adoção. Isso valida a abordagem da Agência Cognitiva em focar em dados antes dos agentes."
```

## Quality Criteria
- [ ] Mínimo de 3 notícias variadas encontradas.
- [ ] Nenhuma notícia é puramente promocional ou "press release" vazio.
- [ ] Fontes são reconhecidas no setor de tecnologia.

## Veto Conditions
- Se a pesquisa não retornar nenhuma notícia recente (últimos 30 dias se não especificado).
- Se os resumos forem copiados integralmente da fonte original sem análise.
