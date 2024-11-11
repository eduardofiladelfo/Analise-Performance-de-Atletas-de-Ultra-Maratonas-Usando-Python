# Análise da Performance de Atletas de Ultra Maratonas no ano de 2020

### Overview do Projeto

O objetivo dessa análise é realizar uma EDA (Análise exploratória de dados) do país que realizou a maior quantidade de ultra maratonas do ano de 2020 e também descobrir qual delas teve a maior quantidade de participantes, visando identificar padrões extrair insights da performance dos atletas segmentado por gênero e faixa etária. 

### Dataset

O conjunto de dados usado neste projeto está disponível publicamente no Kaggle:

https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running

Talvez seja necessário criar uma conta do Kaggle para acessar esse conjunto de dados.

### Ferramentas 

- Python: Análise dos dados e visualização dos gráficos.
  
#### Bibliotecas

- Pandas: Manipulação dos dados
- Numpy: Computação numérica
- Matplotlib/Seaborn: Visualização dos dados

### Importação e filtragem dos dados
Nessa fase inicial de preparação, faremos as seguintes tarefas:

1. Carregamento da base.
2. Filtrar quais foram as maratonas realizadas no ano de 2020 entre as categorias de 50km e 50mi.
3. Descobrir qual dos países tiveram a maior quantidade desses eventos.
4. Buscar nesse país o evento com o maior número de participantes.
   
Obs.: Faremos a filtragem dos países já na primeira etapa por se tratar de uma base com diferentes tipos de provas. Convém inicialmente filtrar de acordo com métricas estabelecidas para posteriormente iniciarmos a limpeza e o tratamento dos dados.

### Limpeza e tratamento dos dados

Na etapa de tratamento, faremos as seguintes tarefas:
1. Analisar/Remover os valores em nulo.
2. Limpeza e formatação dos dados.

### Análise exploratória

A EDA explorará perguntas sobre a prova como:

- Qual a quantidade de atletas do sexo masculino e feminino?
- Qual a quantidade desses atletas por categoria de idade? Sendo elas:
  
  - Participantes com menos de 20 anos: 20-
  - Participantes entre 20 e 30 anos: 20 a 30
  - Participantes entre 30 e 40 anos: 31 a 40
  - Participantes entre 40 e 50 anos: 41 a 50
  - Parcitipantes com mais de 50: 50+

 - Dadas as categorias, qual delas teve uma maior quantidade de participantes?
 - Qual a velocidade média dos competidores de acordo com sua categoria e gênero?
 - Quem foi o primeiro e último colocado? Qual o tempo de prova e a velocidade média deles?
 - Qual o tempo de prova desses atletas de acordo com sua velocidade média?

### Resultados

Os resultados da análise foram os seguintes:
1. Dos 632 participantes, 470 eram do gênero masculino, enquanto 162 eram do gênero feminino, que corresponde a 74% e 26%, respectivamente.
2. A maior quantidade de atletas do público masculino se encontra entre 20 e 30 anos, enquanto o público feminino está alocado no grupo de participantes de 31 a 40 anos. Não houve nenhum competidor com menos de 20 anos.
3. Podemos notar que a prova não houve nenhum desistente e nenhum deles quebrou. "Quebrar" é um termo utilizado para quando um atleta em determinado momento da prova e não consegue completar a corrida
(ou precisa diminuir muito o ritmo para chegar até o final). Uma das hipóteses é devido à estação do ano que a prova foi realizada. Na data que a ultra maratona foi realizada era outono, a temperatura é mais amena se comparada ao verão, por exemplo.
4. A faixa de densidade mostra que a maioria dos corredores mantiveram a velocidade entre 6 e 8 milhas por hora (mph), indicando uma convergência nas performances em torno dessa faixa de tempo. A maior velocidade em mph foi do gênero masculino no grupo de 20 a 30 anos, com 15,149 mph. Logo, o vencedor da competição está nessa categoria, percorrendo aproximadamente 80,47 km numa velocidade média de 24,38 km/h. A maior velocidade em mph do grupo feminino está nos participantes de 31 a 40 anos.


