# invest-smells-llm-evaluation

## Avaliação de Histórias de Usuário via Requirements Smells com LLMs

Dataset e resultados do estudo empírico conduzido como Trabalho de Conclusão 
de Curso (TCC) em Engenharia de Software — UFC Campus Quixadá.

---

## Sobre o estudo

Este repositório contém os dados produzidos no experimento que investigou como 
diferentes estratégias de Engenharia de Prompts influenciam a capacidade de 
Modelos de Linguagem de Grande Escala (LLMs) de avaliar a qualidade de histórias 
de usuário segundo o modelo INVEST, utilizando um protocolo determinístico 
baseado em Requirements Smells.

## Modelos avaliados

- ChatGPT (GPT-5.5) — OpenAI
- Gemini (3.1 Pro) — Google DeepMind
- Claude (Sonnet 4.6) — Anthropic

## Técnicas de prompting

- Zero-Shot
- Few-Shot
- Chain-of-Thought (CoT)

## Dataset de histórias de usuário

30 histórias reais extraídas de três sistemas de código aberto do repositório 
público [Requirements data sets](https://data.mendeley.com/datasets/7zbk8zsd8y/1) 
(Dalpiaz, 2018), cobrindo os domínios:

- **Federal Spending** — gestão de gastos públicos federais
- **Recycling** — localização de pontos de coleta de recicláveis
- **Planning Poker** — estimativa ágil colaborativa

## Estrutura do experimento

- 30 histórias × 3 LLMs × 3 técnicas = **270 avaliações automatizadas**
- 1 avaliação humana como *baseline* (129 smells detectados)
- Protocolo binário de 30 Requirements Smells distribuídos entre os 6 
  critérios do modelo INVEST (I, N, V, E, S, T)

## Métricas utilizadas

- Concordância geral e Kappa de Cohen
- Erro Médio Absoluto (MAE) por critério INVEST
- Falsos Positivos (FP) e Falsos Negativos (FN)
- Teste de Wilcoxon pareado (comparação entre modelos e técnicas)
- Teste de Friedman (comparação multicondicional)

## Autor

Felipe Oliveira Nogueira  
Engenharia de Software — UFC Campus Quixadá  
Orientador: Prof. Dr. Enyo José Tavares Gonçalves

## Licença

Este dataset está disponível para fins acadêmicos e de pesquisa.
