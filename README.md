# Moderador de Tweets com Inteligência Artificial

![Python](https://img.shields.io/badge/Python-Linguagem-3776AB?style=flat-square&logo=python)
![Pysentimiento](https://img.shields.io/badge/Pysentimiento-Análise%20de%20Sentimentos-0052CC?style=flat-square&logo=python)
![OpenAI](https://img.shields.io/badge/OpenAI-Moderação-412991?style=flat-square&logo=openai)
![Requests](https://img.shields.io/badge/Requests-Requisições-2D8CFF?style=flat-square&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Manipulação%20de%20Dados-150458?style=flat-square&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualização%20de%20Dados-11557C?style=flat-square&logo=matplotlib)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat-square&logo=jupyter)

## Descrição

Este projeto tem como objetivo a construção de um sistema de moderação automática de conteúdo de tweets utilizando técnicas de inteligência artificial.  
O sistema é capaz de identificar automaticamente linguagem ofensiva, discurso de ódio e outras categorias de conteúdo inadequado em português.

O projeto oferece duas alternativas para a análise dos textos:

- Alternativa gratuita utilizando a biblioteca `pysentimiento`, que realiza análise de sentimentos e detecção de discurso de ódio.
- Alternativa paga utilizando a API de Moderação da OpenAI, que analisa o conteúdo dos textos e classifica a probabilidade de conter violações em diversas categorias.

Após a análise, os resultados são apresentados em gráficos de barras que exibem a pontuação de cada categoria detectada para cada tweet analisado.

O projeto é útil para moderação de redes sociais, plataformas de conteúdo gerado por usuários ou qualquer sistema que exija monitoramento de linguagem inadequada.

## Funcionalidades

- Analisar tweets automaticamente para detecção de conteúdos inadequados.
- Classificar os textos em múltiplas categorias de moderação, como discurso de ódio, assédio, ameaças, entre outros.
- Visualizar as análises em gráficos de barras que destacam as probabilidades de cada categoria.
- Suporte completo ao idioma português na moderação.
- Opção de escolha entre uma solução gratuita ou uma solução paga (OpenAI API).
- Tratamento de erros para lidar com falhas de autenticação ou requisições externas.
- Organização dos dados de análise em estruturas fáceis de manipular e exportar.
- Código modular para permitir fácil extensão e adaptação para novos tipos de dados.
- Documentação dos métodos utilizados para futuras melhorias.

## Tecnologias Abordadas

- Python 3: Linguagem de programação principal utilizada no projeto.
- Pysentimiento: Biblioteca de processamento de linguagem natural para análise de sentimentos e detecção de discurso de ódio.
- OpenAI Moderation API: Serviço de moderação de conteúdo baseado em inteligência artificial.
- Requests: Biblioteca para realizar requisições HTTP em Python.
- Pandas: Biblioteca para manipulação de dados em formato tabular.
- Matplotlib: Biblioteca para criação de gráficos e visualizações de dados.
- Jupyter Notebook: Ambiente interativo para desenvolvimento e execução do código.

## Estrutura do Projeto

- **Coleta de dados:** Tweets são carregados a partir de uma lista ou de outra fonte.
- **Moderação dos textos:** Cada tweet é submetido ao analisador escolhido (pysentimiento ou OpenAI API).
- **Armazenamento dos resultados:** As saídas de moderação são organizadas em uma estrutura contendo o texto original e o resultado da análise.
- **Visualização:** Para cada tweet, um gráfico de barras é gerado mostrando os scores de cada categoria de risco.
- **Tratamento de exceções:** Em caso de erro nas APIs externas, mensagens descritivas são lançadas.
