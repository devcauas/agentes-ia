# Agentes de IA Clássica

Coleção de agentes de inteligência artificial implementados em Python durante a
disciplina de Inteligência Artificial do curso de Análise e Desenvolvimento de
Sistemas da FATEC Taubaté, com fundamentação em Russell & Norvig (AIMA).
Todos os notebooks foram avaliados e validados pelo professor da disciplina.

Cada notebook é autocontido: traz a fundamentação teórica, a formulação do
problema (estados, ações, custo), a implementação e a execução comentada.

## Agentes

| Agente | Técnica |
|---|---|
| [Agente Aspirador — Table-Driven Agent](notebooks/01-agente-aspirador-tabela.ipynb) | Agente reativo simples (table-driven) |
| [Mundo do Aspirador — Ambiente, Simulação e Busca](notebooks/02-mundo-do-aspirador-busca.ipynb) | BFS, DFS e busca de custo uniforme |
| [Agente de Caminho Mínimo — Mapa da Romênia](notebooks/03-caminho-minimo-romenia.ipynb) | Busca de custo uniforme |
| [Problema do Caixeiro-Viajante (TSP)](notebooks/04-caixeiro-viajante.ipynb) | Busca exaustiva, heurística gulosa e Dijkstra |
| [Tabuleiro de Peças Deslizantes — 8-Puzzle com A*](notebooks/05-8-puzzle-a-estrela.ipynb) | Busca A* com heurísticas admissíveis |
| [8 Rainhas — Formulação Reduzida (Incremental)](notebooks/06-8-rainhas-formulacao-reduzida.ipynb) | Busca incremental com poda |
| [8 Rainhas — Formulação de Estados Completos](notebooks/07-8-rainhas-estados-completos.ipynb) | BFS com poda e hill climbing |
| [8 Rainhas — Algoritmo Genético](notebooks/08-8-rainhas-algoritmo-genetico.ipynb) | Algoritmo genético |
| [Agente Dinossauros — Algoritmo Genético](notebooks/09-dinossauros-algoritmo-genetico.ipynb) | Algoritmo genético / busca com múltiplos estados |
| [Mundo dos Wumpus — Lógica Proposicional](notebooks/10-mundo-dos-wumpus-logica-proposicional.ipynb) | Representação fatorada e inferência lógica |

## Como executar

Cada agente abre direto no Google Colab pelo badge no topo do notebook, sem
instalação. Para rodar localmente:

```bash
git clone https://github.com/devcauas/agentes-ia.git
cd agentes-ia
pip install -r requirements.txt
jupyter notebook
```

Python 3.10 ou superior. A maior parte dos agentes usa apenas a biblioteca
padrão; apenas o notebook do algoritmo genético das 8 rainhas depende de
matplotlib para o gráfico de evolução do fitness.

## Estrutura

```
agentes-ia/
├── notebooks/        # um agente por notebook, numerados por progressão
├── requirements.txt
├── LICENSE
└── README.md
```

## Licença

MIT — veja [LICENSE](LICENSE).
