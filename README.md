# Projeto - AirBnb
Este projeto foi desenvolvido a partir dos meus estudos na Comunidade DS, Curso: Python - Do zero ao DS. 
A ideia do projeto é gerar insights, partindo da organização e exploração dos dados de uma base de dados de locação de imóveis da empresa AirBnb, do ano de 2019.

## 1. Questão de negócio
Identificar as melhores oportunidades de negócio para compra e locação de imóveis pelo melhor preço, visando a melhor rentabilidade e recuperação do investimento.

## 2. Contexto
O projeto busca a solução para um problema fictício: Um investidor gostaria de diversificar seus negócios e começar a investir em imóveis. 

Ele definiu que compraria imóveis na cidade de Nova York, nos Estados Unidos e, por ser um dos locais mais caros para se viver no País, ele acredita que obterá um retorno satisfatório de seus investimentos caso alugue imóveis na cidade. 

Este investidor planeja inicialmente, alugar os imóveis adquiridos e por isso ele definiu que irá utilizar a plataforma Airbnb para esse fim. Para isso, os dados analisados são provenientes de uma base de dados públicos da empresa, contendo os dados do comportamento dos hosts e de seus imóveis.

## 3. As hipóteses
Foram testadas 18 diferentes hipóteses:

* H1 - O imóvel com o maior valor de aluguel (diária) da base de dados é o imóvel que possui mais avaliações na base de dados.
* H2 - O imóvel que possui a menor quantidade mínima de diárias para locação é também o imóvel que possui o aluguel mais caro.
* H3 - A média do número mínimo de diárias para locação de um imóvel é 7 diárias.
* H4 - O host que possui mais imóveis alugados, possui 100 imóveis.¶
* H5 - O host que possui mais imóveis é o host que também possui mais avaliações.
* H6 - A categoria que mais possui imóveis dentro da base de dados é a 'Private room'
* H7 - A região de Manhattan é a região que mais possui imóveis ativos para locação, da categoria Private room.
* H9 - Na região do Bronx, os imóveis ativos, do tipo 'Entire home/ap', possuem a maior média de tempo de disponibilidade para serem locados.
* H10 - No total e na média, a categoria de imóvel “Private Room“ é a categoria que fica mais tempo disponível para locação.
* H11 - A categoria de imóvel Entire home/apt é a categoria que possui, em média, menos locações.
* H12 - A categoria de imóvel Private Room na região de Manhattan, na média, é a categoria que possui o menor valor de locação, comparado às outras categorias na mesma região.
* H13 - A região que possui maior número de imóveis é Manhattan.
* H14 - A região que possui a maior quantidade de imóveis é também a região que possui os imóveis mais locados.
* H15 - Manhattan é a região que possui, em média, os maiores aluguéis (diárias) dentro da base de dados.
* H16 - Na média,  os imóveis da região do Broklin, ficam menos tempo disponíveis para aluguel, ou seja, são alugados mais rapidamente.
* H17 - O Bairro 'Upper West Side', na região de Manhattan, é o bairro que possui, na média, o maior aluguel dentro da base de dados.
* H18 - 'Tribeca' (Manhattan) é o bairro que possui, na média, o aluguel mais caro da base de dados.

## 4. Premissas sobre o problema de negócio:
* A coluna price possui alguns valores de diária = zero, esses valores serão excluídos e considerados outliers;
* A coluna 'availability_365' indica o número de dias em que o imóvel ficou disponível (sem ser locado) no ano de 2019;
* A coluna'calculated_host_listings_count' indica a quantidade de dias que o imóvel esteve locado no ano de 2019;
* São considerados os imóveis com maior rentabilidade, aqueles que possuem o maior valor das diárias de aluguel e passam o menor tempo desocupados, ou seja, são alugados mais rapidamente.

## 5.  Planejamento da solução:
5.1. Produto final: 

a) Relatórios em formato .csv, trazendo as seguintes informações:
* Rentabilidade por imóveis.
* Rentabilidade por região.
* Rentabilidade - Roosevelt Island/Manhattan:
* Roi (Recuperação do investimento) - Roosevelt Island/Manhattan:

b) Mapa por região, categoria de imóvel e rentabilidade

5.2. Ferramentas: Linguagem Python, Jupyter Notebook, VisualStudioCode

5.3.  Processo: 
- Coletar os dados do site kaggle, limpeza e organização dos dados e atributos;
- Agrupar os imóveis por região, bairro e tipo de imóveis;
- Calcular a média de preço;
- Verificar as melhores possibilidades de rentabilidade:

a) Serão considerados somente os imóveis ativos; 

b) Identificação dos imóveis com menor tempo de desocupação, ou seja, aqueles imóveis que alugam mais rapidamente;

c) Identificação dos imóveis com maior valor da diária;

d) Identificação da região/bairro dos melhores imóveis;

e) Construção de um mapa por localizando os imóveis por preço e categoria.

## 6. Principais insights:
* A região de Manhattam oferece a maioria e os melhores imóveis (mais rentáveis);
* Os imóveis da categoria Entire home/apt possuem o valor da diária mais alta;
* O tipo de imóvel que passa mais tempo disponível é 'shared room';
* O bairro mais rentável é Roosevelt Island, na região de Manhattan.
  

## 7. Resultados financeiros:
Através do relatório de rentabilidade é possível identificar o retorno do valor investido, de acordo com o imóvel adquirido. 

Por exemplo, na simulação de investimento de 1 milhão de dólares, para o imóvel mais rentável (mais rapidamente ocupado, pelo melhor valor da diária), identificou-se 7 locações para alcançar o valor investido (roi).

## 8. Conclusão:
O objetivo do projeto era gerar insights para viabilizar o aluguel de imóveis, encontrando imóveis que oferecessem a oportunidade de um bom negócio, sendo alugados rapidamente, em boa localização e preço, visando a melhor rentabilidade e retorno do valor investido. 

De acordo com as análises realizadas, o projeto cumpriu seu objetivo, trazendo relatórios que possibilitaram a identificação das melhores oportunidades de negócios, além de um mapa interativo por região. 
