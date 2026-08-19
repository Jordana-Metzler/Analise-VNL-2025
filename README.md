# Análise da Fase Classificatória — VNL Feminina 2025

Projeto de análise de dados desenvolvido no **Power BI** utilizando dados oficiais da fase classificatória da Volleyball Nations League Feminina 2025.

## Sobre o projeto

Depois de concluir meu curso de Power BI, decidi colocar os conhecimentos adquiridos à prova em um projeto completo e unir esse aprendizado a algo que sempre fez parte da minha vida: o voleibol.

Durante cerca de 10 anos, vivi o esporte dentro de quadra. Neste projeto, tive a oportunidade de analisá-lo por uma nova perspectiva: os dados.

O objetivo foi transformar as estatísticas da fase classificatória da VNL Feminina 2025 em informações claras sobre o desempenho das seleções e das atletas, passando pelas principais etapas de um projeto de Business Intelligence: coleta, tratamento, modelagem, criação de medidas, análise e visualização.

## Perguntas respondidas

O dashboard foi construído para responder perguntas como:

- Quais seleções conquistaram mais pontos na fase classificatória?
- Quais campanhas foram mais dominantes ou equilibradas?
- Quais equipes venceram mais partidas por 3–0?
- Quais seleções disputaram e venceram mais tie-breaks?
- Como foi a campanha de cada seleção?
- Quem foram as maiores pontuadoras da competição?
- Como os pontos foram distribuídos entre ataque, bloqueio e saque?
- Quais atletas se destacaram em passe, defesa e levantamento?
- Como foi construída a campanha do Brasil?
- Quais foram os principais destaques individuais da seleção brasileira?

## Escopo

A análise considera exclusivamente a **fase classificatória da VNL Feminina 2025**. Os jogos eliminatórios e a fase final não fazem parte deste projeto.

Essa separação foi adotada para manter as comparações consistentes, considerando que todas as seleções disputaram a mesma quantidade de partidas durante a fase classificatória.

## Fonte dos dados

Os dados foram coletados nas páginas oficiais da [Volleyball World — VNL 2025](https://en.volleyballworld.com/volleyball/competitions/volleyball-nations-league/2025).

Foram utilizadas informações de:

- Classificação das seleções;
- Resultados por placar;
- Sets e pontos conquistados e sofridos;
- Pontuação das atletas;
- Ataque;
- Bloqueio;
- Saque;
- Passe;
- Defesa;
- Levantamento.

## Desenvolvimento

### Coleta e transformação

Os dados foram importados para o Power BI e tratados no **Power Query**. Entre os principais procedimentos realizados estão:

- Promoção e padronização dos cabeçalhos;
- Remoção de colunas desnecessárias;
- Ajuste dos tipos de dados;
- Separação do nome e da sigla das seleções;
- Padronização dos nomes das atletas;
- Criação de identificadores;
- Organização das tabelas por fundamento.

### Modelagem

O modelo foi organizado com dimensões compartilhadas e tabelas de estatísticas.

**Dimensões:**

- `Dim_Selecao`
- `Dim_Atleta`

**Tabelas de dados:**

- `Classificacao`
- `Pontuacao`
- `Ataque`
- `Bloqueio`
- `Saque`
- `Passe`
- `Defesa`
- `Levantamento`

As relações foram configuradas, sempre que aplicável, como **um para muitos**, com a propagação dos filtros partindo das dimensões para as tabelas de dados.

### Medidas em DAX

Foram desenvolvidas medidas para calcular e analisar:

- Total de jogos, sets e pontos disputados;
- Pontos na classificação;
- Vitórias e derrotas;
- Taxa de vitórias;
- Resultados por placar;
- Jogos com tie-break;
- Saldo de sets e de pontos;
- Saldo médio de sets por jogo;
- Pontuação por ataque, bloqueio e saque;
- Efetividade em ataque, passe, defesa e levantamento;
- Rankings Top 5 e Top 10 com critério de desempate.

## Páginas do dashboard

### Menu interativo

Página inicial com navegação para todas as áreas do relatório.

### Análise geral

Apresenta a classificação da fase preliminar, os principais indicadores da competição e rankings de vitórias por 3–0, tie-breaks e aproveitamento.

### Desempenho por seleção

Permite selecionar uma equipe e analisar sua classificação, vitórias, derrotas, taxa de aproveitamento e distribuição dos resultados por placar.

### Desempenho ofensivo

Analisa as maiores pontuadoras e os principais destaques em ataque, bloqueio e saque.

### Passe, defesa e levantamento

Apresenta as atletas mais efetivas nesses fundamentos, considerando desempenho e volume de ações.

### Brasil em foco

Reúne os principais números da campanha brasileira, a distribuição das vitórias por placar, a única derrota da equipe e os destaques individuais do Brasil.

## Principais resultados

- A Itália terminou a fase classificatória invicta, com **12 vitórias e 33 pontos**;
- O Brasil ficou na segunda colocação, com **31 pontos e 11 vitórias em 12 jogos**;
- A seleção brasileira alcançou **91,67% de aproveitamento**;
- O Brasil terminou a fase com **saldo de 22 sets** e **saldo de 145 pontos**;
- A única derrota brasileira foi por **3 sets a 0 para a França**;
- A decomposição da pontuação mostrou o peso do ataque, bloqueio e saque na produção das atletas;
- As análises de passe, defesa e levantamento mostraram a importância de avaliar tanto a efetividade quanto o volume de ações.

## Ferramentas utilizadas

- **Power BI Desktop** — desenvolvimento do relatório;
- **Power Query** — coleta, limpeza e transformação;
- **DAX** — criação das medidas e regras de análise;
- **Volleyball World** — fonte oficial dos dados.

## Aprendizados

Este projeto permitiu praticar e desenvolver conhecimentos em:

- Tratamento e qualidade de dados;
- Modelagem dimensional;
- Criação e validação de medidas DAX;
- Contexto de filtro no Power BI;
- Rankings com critérios de desempate;
- Escolha de indicadores e visualizações;
- Storytelling com dados;
- Transformação de perguntas sobre o esporte em análises orientadas por dados.


## Autoria

Desenvolvido por **Jordana Metzler**.

---

Este é um projeto independente, desenvolvido para fins educacionais e de portfólio. Não possui vínculo oficial com a Volleyball World ou com a FIVB.
