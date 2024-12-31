### API- Cotações Cambiais

### Objetivo 

Python é uma linguagem extremamente versátil, especialmente para a integração de sistemas. Neste projeto, utilizaremos a API fornecida pelo Federal Reserve Bank of St. Louis para explorar esse tipo de conexão e realizar análises financeiras relacionadas ao Brasil.
Nosso foco será desde a implementação do Plano Real segregado por tipo de governo verificar a cotação do Dólar.

Para começar, vamos definir o que é uma API.

Uma API, ou Interface de Programação de Aplicações (do inglês "Application Programming Interface"),é um conjunto de regras e especificações que permite que diferentes softwares se comuniquem entre si. 
Esse processo é feita por meio de:

 - Solicitação: Tudo começa quando uma aplicação faz uma solicitação a uma API. Por exemplo, quando você acessa um aplicativo de previsão do tempo no seu celular, o aplicativo solicita informações a uma API que possui os dados meteorológicos.

 - Processamento: A API recebe a solicitação, processa-a, e então envia a solicitação ao sistema correto, como um banco de dados ou outro servidor.

 - Resposta: O sistema retorna a informação solicitada de volta para a API, que por sua vez envia essa informação de volta para a aplicação inicial.

 - Apresentação: A aplicação recebe a informação e a apresenta ao usuário de uma forma legível, como a previsão do tempo para a semana.


À vista disso, sempre é necessário ler a documentação da requesição que será executada. 

No nosso caso será essa:

Fonte: https://fred.stlouisfed.org/

>  "This product uses the FRED® API but is not endorsed or certified by the Federal Reserve Bank of St. Louis."


Foi usada a biblioteca request para fazer a conexão, ademais, é interessante sempre ver o StatusCode e o Content Type da URL. 
para mais detalhes você pode acessar a documentação : 


Feito toda a conexão e o rateio, foi feito a questão de paginação e offset .


Essa análise pegou todos os anos desde a criação do plano real até os dias atuais cotações do valor do dólar. 

IMAGEM 

Foi feito uma segregração pelo presidente do período.

Baseando-nos nos gráficos e contextualizando os acontecimentos históricos, temos o seguinte panorama:

Durante o governo de Itamar Franco, Fernando Henrique Cardoso (FHC), então ministro da Fazenda, foi o responsável pela implementação do Plano Real. Nos anos 1990, o Brasil enfrentava uma grave crise de hiperinflação, que corroía o poder de compra da população e desestabilizava a economia. Para combater esse cenário, FHC adotou medidas austeras, como o aumento da arrecadação por meio de novos impostos e cortes significativos em áreas como educação e saúde.

Uma das estratégias mais notáveis foi a criação da Unidade Real de Valor (URV), uma moeda virtual que nivelava os preços com a cotação do dólar. Posteriormente, a URV foi convertida no Real, que se tornou a moeda oficial do Brasil e permanece em uso até hoje. Na época de sua implementação, o Real chegou a ter uma valorização expressiva, com 1 dólar valendo R$ 0,83. No entanto, ao final do mandato de FHC, a moeda brasileira sofreu forte desvalorização, atingindo R$ 4,00 por dólar.

Durante os dois mandatos de Luiz Inácio Lula da Silva (2003-2010), o Brasil experimentou uma conjuntura econômica mais favorável, impulsionada pelo boom das commodities no mercado internacional. O governo implementou algumas reformas estruturais e conseguiu manter o dólar relativamente estável, oscilando abaixo de R$ 3,50 durante quase todo o período. Apesar desses avanços, o segundo mandato de Lula foi marcado pelo início de investigações de esquemas de corrupção que abalariam profundamente a credibilidade do governo. Esses esquemas culminaram no déficit trilionário que marcou o período subsequente.

Com a sucessão de Lula, a presidência de Dilma Rousseff enfrentou graves instabilidades políticas e econômicas. A desconfiança do mercado, combinada com escândalos de corrupção e uma rejeição crescente por parte da população, fez o dólar voltar a patamares elevados, alcançando novamente R$ 4,00. A crise culminou no impeachment de Dilma em 2016.

O vice-presidente, Michel Temer, assumiu a presidência e adotou medidas consideradas importantes, como reformas fiscais e trabalhistas. Essas ações ajudaram a estabilizar temporariamente o dólar, que permaneceu abaixo de R$ 4,00 durante o restante de seu mandato.

Com a eleição de Jair Bolsonaro em 2018, o Brasil enfrentou a pandemia de COVID-19, que desestruturou economias em todo o mundo. Durante esse período, o dólar disparou, ultrapassando R$ 5,00. A instabilidade econômica e política, agravada pelo descumprimento do teto de gastos, dificultou a recuperação da moeda.

Em 2023, com o retorno de Lula ao poder, o dólar atingiu um recorde histórico de R$ 6,30. O cenário atual não apresenta perspectivas claras de melhora, refletindo a incerteza política e econômica que o Brasil enfrenta.



## 










 