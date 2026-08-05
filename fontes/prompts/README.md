## Engenharia de Prompts

Esta seção documenta os principais prompts utilizados durante os estudos no NotebookLM.

O objetivo é registrar as perguntas realizadas, analisar as respostas geradas pela IA e identificar melhorias nos prompts utilizados.

---

# Prompt 01

## Objetivo

Compreender os conceitos fundamentais de Python para Análise de Dados.

## Prompt

Explique os principais conceitos de Python para Análise de Dados utilizando exemplos simples.

## Resultado

Python utiliza **variáveis** como identificadores para armazenar valores e **estruturas de dados** como listas (ex: `['maçã', 'laranja']`) e dicionários (pares de chave-valor) para organizar informações de forma estruturada. O fluxo da análise é gerenciado por **condicionais** (*if/else*), que executam códigos baseados em regras lógicas, e **loops** (*for/while*), que permitem processar grandes volumes de dados de maneira automatizada. A biblioteca **Pandas** é o pilar central ao fornecer o *DataFrame*, uma tabela programável que facilita o agrupamento de categorias (*groupby*) e o preenchimento de valores ausentes (*fillna*). Complementarmente, o **NumPy** otimiza cálculos matemáticos através da **vetorização**, que aplica operações em blocos de dados de uma só vez, enquanto ferramentas como **Matplotlib** e **Seaborn** traduzem esses resultados em gráficos visuais acionáveis.

## Análise

A resposta apresentou uma visão geral dos conceitos e ajudou na compreensão inicial do tema.

---

# Prompt 02

## Objetivo

Entender a utilização da biblioteca Pandas.

## Prompt

Explique o que é um DataFrame e apresente exemplos práticos de utilização.

## Resultado

Um **DataFrame** é a estrutura de dados fundamental da biblioteca **Pandas**, sendo essencial para a análise de dados moderna em Python. Ele representa uma **tabela retangular de dados**, contendo uma coleção ordenada de colunas, onde cada uma pode ter um tipo de valor diferente (como números, strings ou booleanos).

Você pode imaginar um DataFrame como uma **planilha programável** ou uma tabela de banco de dados SQL que reside na memória do computador. Tecnicamente, ele possui índices tanto para linhas quanto para colunas, podendo ser visto como um dicionário de objetos *Series* (colunas individuais) que compartilham o mesmo índice.

Abaixo estão exemplos práticos de como um DataFrame é utilizado no dia a dia:

*   **Carregamento e Criação:** DataFrames podem ser criados manualmente a partir de dicionários e listas, ou importados de fontes externas como arquivos **CSV** (`pd.read_csv`), planilhas **Excel** (`pd.read_excel`) ou consultas a bancos de dados **SQL**.
*   **Exploração de Dados:** Após carregar os dados, funções como `.head()` são usadas para visualizar as primeiras linhas, enquanto o método **`.describe()`** fornece um resumo estatístico instantâneo, incluindo média, valor máximo, mínimo e desvio padrão das colunas numéricas.
*   **Limpeza de Informações:** É comum utilizar DataFrames para remover registros duplicados através do método **`.drop_duplicates()`** ou tratar dados ausentes (nulos) com **`.fillna()`**, que permite preencher lacunas com valores específicos ou médias calculadas.
*   **Análise Agrupada:** O recurso **`.groupby()`** permite dividir os dados em grupos baseados em categorias (como "Gênero" ou "Região") para aplicar funções de agregação, como somar o total de vendas por território ou calcular a média de idade de um grupo.
*   **Visualização de Resultados:** DataFrames integram-se diretamente com bibliotecas gráficas. Com apenas um comando como `.plot()`, é possível gerar **gráficos de barras, linhas ou histogramas** para comunicar visualmente os *insights* extraídos da tabela.

## Análise

O exemplo facilitou o entendimento da manipulação de dados utilizando DataFrames.

---

# Lições Aprendidas

- Prompts objetivos produzem respostas mais precisas.
- Solicitar exemplos práticos melhora a compreensão.
- Pedir resumos facilita futuras revisões.
