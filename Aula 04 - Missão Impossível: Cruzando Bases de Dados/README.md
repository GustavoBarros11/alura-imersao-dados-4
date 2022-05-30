# Aula 4 - Missão Impossivel: Cruzando bases de Dados

Boas-vindas à quarta aula da **Imersão Dados 4ª Edição**!

Chegamos a famosa quarta aula da Imersão, apelidada carinhosamente pelo Paulo Silveira como Missão Impossível. Mas não se preocupe! Ela é mais complexa que as outras aulas, entretanto não há o que temer. No notebook da aula está todo passo a passo. Você pode primeiro acompanhar o vídeo e depois reproduzir o código.

Na nossa base de dados temos algumas poucas informações sobre o imóvel. Uma opção que temos é vincular e enriquecer os nossos dados com informações extras. É exatamente isso que faremos hoje: vamos cruzar os dados que temos com dados do IBGE.

Para executar essa tarefa vamos trabalhar com dados de geolocalização, CEPs, conceitos geometria computacional e muito mais.

## Para ver os exercícios e todo o conteúdo que foi dado em aula, siga os passos abaixo
* Acesse [notebook da aula 04, com todo código trabalhando em aula](https://colab.research.google.com/drive/1WzaYKTJuVoQ1_WeVdBwKsmkCV9PU7IGD?usp=sharing).
* Se você está cheio de dúvidas de como realizamos os cruzamentos entre as bases de dados, esse [artigo da Creditas](https://medium.com/creditas-tech/incrementando-dados-geogr%C3%A1ficos-com-o-censo-nacional-do-ibge-54d342c4bdcf) pode te ajudar!
* Nesta aula vamos precisar da base de dados de endereços. Baixe [neste link](https://drive.google.com/file/d/1u2qPFtYaE4of3Vb3d7yQEVEbS5FdQ_FP/view?usp=sharing) e salvar no seu drive.
* Também precisaremos dos dados dos [setores censitários](https://drive.google.com/drive/folders/1CycoanzYN2oxKHPO6zxvIQ6Og1LBcujv?usp=sharing). Não esqueça que você precisa dos 4 arquivos na mesma pasta para leitura.
* Se você não reproduziu o código sozinho, não se preocupe! Aqui você acessa a [base dados_geo](https://drive.google.com/file/d/1KyaCnwYt3vVV_7O0VktZorRhsMWD9hQQ/view?usp=sharing) e aqui a base [dados_vendas_censo](https://drive.google.com/file/d/1iAFJhgMUquxsbGxM1pWz9BLjpC9SULKr/view?usp=sharing)
* Na parte superior esquerdo, clique em >File, logo depois em >Save a copy in Drive.
* Se você não estiver logado em uma conta Gmail, um pop-up solicitará que você crie ou faça login de em uma conta Google.
* Feito o login uma cópia da aula é criada em seu drive (pasta Colab Notebook, criada automaticamente).
* Abra o notebook e boa diversão.

## Desafios desta aula
1 - Realizar uma análise dos dados do IBGE por mapa, [analisando a distribuição de renda](https://medium.com/creditas-tech/dados-georreferenciados-explora%C3%A7%C3%A3o-e-visualiza%C3%A7%C3%A3o-com-python-edd51e7c53da).

2 - Repassar a aula para entender melhor o que foi realizado.

3 - Aprofundar a análise entre dados de vendas e renda.

4 - Realizar a análise exploratória e encontrar variáveis relevantes para solução do problema.

## Alguns lembretes e dicas
* Que tal aprender mais sobre Geopandas com este [artigo da Creditas](https://medium.com/creditas-tech/dados-georreferenciados-explora%C3%A7%C3%A3o-e-visualiza%C3%A7%C3%A3o-com-python-edd51e7c53da)!
* Podemos usar dados do IBGE para criar novas features, de uma maneira diferente que fizemos em aula. Se liga [neste artigo](https://medium.com/creditas-tech/criando-features-de-machine-learning-a-partir-de-nomes-de-cidades-7149fae7778e)!
* Quer entender mais sobre Boxplot? [Acesse este artigo da Alura](https://www.alura.com.br/artigos/melhorando-a-analise-com-o-boxplot).
* Para baixar os dados do IBGE você pode acessar [esse link](https://gist.githubusercontent.com/tgcsantos/85f8c7b0a2edbc3e27fcad619b37d886/raw/a4954781e6bca9cb804062a3eea0b3b84679daf4/Basico_SP1.csv)
* Para acessar o dicionário de dados do IBGE que estamos trabalhando, é só [clicar aqui](https://drive.google.com/file/d/1WVTqfKtHOOk5X1AWaSOn6NLaO7cix2m4/view?usp=sharing)
* Que tal explorar mais sobre [GeoPandas](https://geopandas.org/en/stable/)
* Quer conhecer um pouco mais sobre String, se [liga neste material](https://panda.ime.usp.br/pensepy/static/pensepy/08-Strings/strings.html).
* Um [guia rápido](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf) para o Pandas.

## Discord e redes sociais
Participe do nosso [Discord](https://discord.gg/UX5ejkABgw), tire suas dúvidas e ajude as outras pessoas que estão participando da Imersão. A melhor forma de aprender é ensinando!

Aproveite também para compartilhar sua participação na Imersão Dados em suas redes sociais! Poste sobre seus projetos no LinkedIn, Twitter e Instagram com as hashtags #ImersãoDados e #ImersãoDados4.

Bons estudos e até a próxima aula!