# **Imersão Dados v4.0**
Esta é minha implementação dos notebooks e desafios das aulas da imersão de dados da **Alura**.

![jpg](assets/sp-wallpaper.jpg)

Nesta imersão nós trabalhamos inicialmente com dados de anúncios de imóveis da cidade de São Paulo, explorando esses dados, trabalhando com as bibliotecas do Python para Ciência de Dados, como: Pandas, Numpy, Matplotlib e Searbon, nós criamos visualizações extraímos insights, trabalhamos com o tratamento de dados nulos, extremos e aplicamos estatísticas de dispersão e centralidade. Depois partimos para tópicos mais complexos, tais quais: merging de dois ou mais datasets completamente distintos, transformadno esses dados para que o merge possa ser possível e no final utilizamos da biblioteca Python para Machine Learnin, Scikit-learn, para gerar um modelo de regressão com o intuito de prever os valores dos imóveis utilizando os datasets que nós trabalhamos nas aulas anteriores.

# Tabela de Conteúdos
- [**Imersão Dados v4.0**](#imersão-dados-v40)
- [Tabela de Conteúdos](#tabela-de-conteúdos)
- [Desafios do Projeto](#desafios-do-projeto)
      - [[DESAFIOS Aula 1]](#desafios-aula-1)
      - [[DESAFIOS Aula 2]](#desafios-aula-2)
      - [[DESAFIOS Aula 3]](#desafios-aula-3)
      - [[DESAFIOS Aula 4]](#desafios-aula-4)
      - [[DESAFIOS Aula 5]](#desafios-aula-5)
- [Premissas do Projeto](#premissas-do-projeto)
- [Dicionário de Dados](#dicionário-de-dados)
        - [DATASET - IBGE](#dataset---ibge)
        - [DATASET - IMÓVEIS SÃO PAULO](#dataset---imóveis-são-paulo)
- [Planejamento da Solução](#planejamento-da-solução)
  - [Produto Final](#produto-final)
  - [Tech Stack](#tech-stack)
  - [Process and Methods](#process-and-methods)
- [Insights da Imersão](#insights-da-imersão)
- [Referências](#referências)
- [Próximos Passos](#próximos-passos)

# Desafios do Projeto
#### [DESAFIOS Aula 1]
1. Realizar a média da metragem para cada um dos bairros. (Proposto pelo Paulo)
2. Duas formas de selecionar os dados por bairro (consultar os métodos na documentação do Pandas). (Proposto pelo Thiago)
3. Explorar alguns gráficos na documentação e aplicar nas demais colunas do DF, assim como tentar colocar alguma conclusão. (Proposto pelo Thiago)
4. Pegar outras estatísticas dos dados (como média, mediana, mim, max). (Proposto pela Vivian)
5. Descobrir quais são os bairros que não tem nome de rua. (Proposto pela Vivian)
#### [DESAFIOS Aula 2]
1. Criar uma escala de valores em milhões.
2. Deixar o gráfico do histograma de valores legível (alterar labels, cores, título, escala).
3. Preço do metro quadrado por bairro e plotar em um gráfico ideal.
4. Explorar as bibliotecas de visualizações e colocar as suas conclusão.
5. Pesquisar um visualização para analisar os quartis, mediana e outliers.
#### [DESAFIOS Aula 3]
1. Tentar vincular dados do IBGE com os dados de imóveis.
2. Tratar os outliers e comparar com os resultados.
3. Agrupar por mais de uma categoria e realizar as análises.
4. Organize o colab para deixar com cara de projeto.
#### [DESAFIOS Aula 4]
1. Realizar uma análise dos dados do IBGE por mapa, analisando a distribuição de renda.
2. Repassar a aula para entender melhor o que foi realizado.
3. Aprofundar a análise entre dados de vendas e renda.
4. Realizar a análise exploratória e encontrar variáveis relevantes para solução do problema.
#### [DESAFIOS Aula 5]
1. Adicionar o valor "real" do m² do imóvel.
2. Testar outro modelo de regressão.
3. Criar um modelo baseline com as features originais.
4. Trabalhar mais nos dados e criar novas variáveis.
5. Testar as predições para casos reais.
6. Criar um projeto com os resultados da Imersão e postar nas redes sociais mostrando o trabalho realizado. Lembre-se de marcar a @AluraOnline e utilizar as hashtags #ImersãoDados e #ImersãoDados4.

# Premissas do Projeto
- Nós estamos trabalhando com dados de imóveis de São Paulo.
- Os dados do IBGE utilizados neste projeto são do CENSU 2010, portanto estão **datados**.
- Os resultado deste projeto possuem o objetivo de replicar resultado reais de um projeto de Ciência de Dados, mas por ser um projeto de estudos, diversos valores foram aproximados e até mesmo aleatoriamente selecionados.

# Dicionário de Dados
##### DATASET - IBGE
| Código da variável | Descrição do setor |
| --- | --- |
Cod_setor           | ID
Cod_Grandes_Regiões | Código das Grandes Regiões (Regiões Geográficas)
Nome_Grande_Regiao  | Nome das Grandes Regiões (Regiões Geográficas)
Cod_UF              | Código da Unidade da Federação
Nome_da_UF          | Nome da Unidade da Federação
Cod_meso            | Código da mesorregião
Nome_da_meso        | Nome da mesorregião
Cod_micro           | Código da microrregião
Nome_da_micro       | Nome da microrregião
Cod_RM              | Código da região metropolitana ou RIDE
Nome_da_RM          | Nome da região metropolitana ou RIDE
Cod_municipio       | Código do município
Nome_do_municipio   | Nome do município
Cod_distrito        | Código do distrito
Nome_do_distrito    | Nome do distrito    
Cod_subdistrito     | Código do subdistrito
Nome_do_subdistrito | Nome do subdistrito
Cod_bairro          | Código de bairro
Nome_do_bairro      | Nome do bairro
Situacao_setor      | Código de situação do setor
Tipo_setor          | Tipo ( Situação urbana / Situação rural ) 
V001                | Domicílios particulares permanentes ou pessoas responsáveis por domicílios particulares permanentes
V002                | Moradores em domicílios particulares permanentes ou população residente em domicílios particulares permanentes
V003                | Média do número de moradores em domicílios particulares permanentes (obtida pela divisão de Var2 por Var1)
V004                | Variância do número de moradores em domicílios particulares permanentes
V005                | Valor do rendimento nominal médio mensal das pessoas responsáveis por domicílios particulares permanentes (com e sem rendimento)
V006                | Variância do rendimento nominal mensal das pessoas responsáveis por domicílios particulares permanentes (com e sem rendimento)
V007                | Valor do rendimento nominal médio mensal das pessoas responsáveis por domicílios particulares permanentes (com rendimento)
V008                | Variância do rendimento nominal mensal das pessoas responsáveis por domicílios particulares permanentes (com rendimento)
V009                | Valor do rendimento nominal médio mensal das pessoas de 10 anos ou mais de idade (com e sem rendimento)
V010                | Variância do rendimento nominal mensal das pessoas de 10 anos ou mais de idade (com e sem rendimento)
V011                | Valor do rendimento nominal médio mensal das pessoas de 10 anos ou mais de idade (com rendimento)
V012                | Variância do rendimento nominal mensal das pessoas de 10 anos ou mais de idade (com rendimento)
##### DATASET - IMÓVEIS SÃO PAULO
| Código da variável | Descrição |
| --- | --- |
Rua | Localização da rua de onde o imóvel pertence
Bairro | Bairro onde imóvel está localizado
Cidade | Cidade onde imóvel está localizado
Metragem | Área em metros quadrado
Quartos | Número de quartos no imóvel
Banheiros | Número de banheiros no imóvel
Vagas |  Vagas de estacionamento por veículo
Valor | Preço da casa que está em moeda brasileira BRL


# Planejamento da Solução
## Produto Final
Projeto no Github contendo todos os desafios das 5 aulas da **Imersão Dados 4**. Incluindo visualizações, mapas, dataframes resultantes de merge, e etc.
## Tech Stack
- Python, Pandas, Numpy.
- Matplotlib, Seaborn
- Geopandas

## Process and Methods

# Insights da Imersão

# Referências

# Próximos Passos