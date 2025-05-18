# Análise e Predição no Campeonato Brasileiro (2003–2024)

## Quais insights estatísticos podem ser extraídos dos dados do Campeonato Brasileiro Série A, de 2003 até 2024?

## Visão Geral

Este projeto tem como objetivo realizar uma análise aprofundada do Campeonato Brasileiro de Futebol, abrangendo os dados de 2003 a 2024. Além disso, uma parte do projeto é dedicada à aplicação de técnicas de aprendizado de máquina para prever a media de gols ao final do campeonato com base em seu desempenho histórico. A ideia é unir duas paixões pessoais — futebol e ciência de dados — e aplicar os conceitos estudados na disciplina **Sistemas Inteligentes** de maneira prática e com significado real.

## Objetivo

O projeto tem dois grandes objetivos:

1. **Análise de Dados**: Identificar padrões, comportamentos e estatísticas relevantes no Campeonato Brasileiro.
2. **Predição com Machine Learning**: Utilizar algoritmos supervisionados para prever a média de gols de um time com base em características históricas.

## Ferramentas Utilizadas

- **Python**: linguagem principal do projeto.
- **Pandas**: para manipulação de dados.
- **Matplotlib**: para visualização.
- **Scikit-learn**: para aplicação de algoritmos de machine learning (regressão linear e regressão de árvore de decisão).
- **Jupyter Notebook**: para desenvolvimento do projeto.

## Descrição do Projeto

Utilizando dados históricos das partidas do Campeonato Brasileiro, apliquei conceitos de análise de dados e aprendizado de máquina com o objetivo de gerar insights e realizar uma predição simples. Este trabalho une minha paixão por futebol e o aprendizado de ciência de dados, ao mesmo tempo que contribui com minha formação acadêmica e meu portfólio profissional.

## Fonte dos Dados

- **Base de Dados**: `db/campeonato-brasileiro-full.csv`
- **Origem**: Kaggle  
  [Campeonato Brasileiro de Futebol](https://www.kaggle.com/datasets/adaoduque/campeonato-brasileiro-de-futebol/data)

## Limpeza de Dados

Durante o processo de preparação, foram removidas colunas que estavam majoritariamente vazias ou não agregavam valor à análise. São elas:

- `formacao_mandante`
- `formacao_visitante`
- `tecnico_mandante`
- `tecnico_visitante`
- `mandante_Estado`
- `visitante_Estado`
- `hora`

Também foi acrescentada a coluna **`ano`** à base de dados, extraída da coluna de data das partidas, o que permitiu análises por temporada.

## Estrutura da Base de Dados

A base de dados contém as seguintes colunas relevantes:

- `id`: identificador da partida.
- `rodada`: número da rodada.
- `data`: data da partida.
- `dia`: dia da semana.
- `mandante`, `visitante`: times participantes.
- `vencedor`: resultado da partida.
- `placar_mandante`, `placar_visitante`: número de gols marcados.
- `arena`: estádio da partida.
- `estado_mandante`, `estado_visitante`, `estado_vencedor`: estados dos clubes envolvidos.
- `ano`: ano em que a partida foi disputada.

---

## Parte 1: Análise Estatística

A seguir, algumas perguntas guiadoras da análise realizada:

1. **Qual foi a média de gols por partida no Campeonato Brasileiro de 2003 a 2023?**
2. **Qual foi o placar mais comum (moda) no Campeonato Brasileiro?**
3. **Qual o clube que mais venceu partidas como mandante?**
4. **Qual foi o ano com maior média de gols por partida?**
5. **Quantos jogos terminaram 0x0 entre 2003 e 2023?**
6. **Como a média de gols variou ao longo dos anos?**
7. **Qual a proporção de partidas empatadas?**
8. **Qual time mais venceu como visitante?**
9. **Qual time mais fez gols em casa?**
10. **Qual time mais fez gols como visitante?**
11. **Qual foi o maior número de gols marcados em uma única partida?**
12. **Quantas partidas terminaram empatadas no total?**

---

## Parte 2: Análise Preditiva

### Objetivo da Predição

Prever a média de gols do campeonato brasileiro em 2025 usando características como:

- Número de vitórias
- Número de empates
- Número de derrotas
- Média de gols dos anos anteriores

Com base no desempenho dos times em edições anteriores do campeonato, foi criado um modelo simples capaz de estimar a média de gols do campeonato em 2025. Foram usados métodos de previsão em python(Scikit-learn).Essa etapa demonstra como a inteligência artificial pode ajudar a entender padrões e fazer previsões a partir de dados históricos.
---

## Conclusão

Este projeto possibilitou uma análise abrangente e aplicação prática de técnicas de ciência de dados e aprendizado de máquina em um tema de interesse pessoal. Além de gerar insights interessantes sobre o Campeonato Brasileiro, pude experimentar a construção de um modelo preditivo simples e funcional, com resultados promissores.

---

## Sobre o Autor

**Gabriel Campos**  
Estudante de Engenharia da Computação (PUC Minas) e técnico em Automação Industrial. Apaixonado por tecnologia, dados e futebol. Em busca constante de aplicar o conhecimento adquirido em projetos práticos e reais.

- [LinkedIn](https://www.linkedin.com/in/gabrielcamposdev/)

---

*Este projeto foi desenvolvido como parte da disciplina Sistemas Inteligentes no 1º período do curso de Engenharia da Computação da PUC Minas.*

