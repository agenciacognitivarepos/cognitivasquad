---
name: "Find News"
order: 1
input: "research-focus.md"
output: "raw-news.md"
---

# Find News

## Process
1. Ler o arquivo `research-focus.md` para entender o tema e o período da pesquisa.
2. Usar `web_search` para encontrar as notícias mais recentes e relevantes sobre o tema, focando em portais de tecnologia e negócios conceituados.
3. Extrair o título, a URL, a data e um parágrafo de resumo para cada notícia encontrada (mínimo de 5).
4. Salvar os resultados formatados em `raw-news.md`.

## Output Format (YAML schema)
```yaml
news:
  - title: string
    url: string
    date: date
    summary: string
    source: string
```

## Output Example
```yaml
news:
  - title: "OpenAI lança novos Agentes Autônomos"
    url: "https://openai.com/blog/agents"
    date: "2024-03-24"
    summary: "Novos agentes que podem navegar pela web e realizar tarefas complexas em nome do usuário."
    source: "OpenAI Blog"
```

## Quality Criteria
- Mínimo de 5 notícias.
- Fontes confiáveis e datas recentes.
- Resumo claro e objetivo.

## Veto Conditions
- Se houver menos de 3 notícias relevantes.
- Se os links estiverem quebrados.
