CitizenTech – Análise de Mobilidade Urbana

Global Solution | MLAM – Modelagem Linear para Aprendizagem da Máquina 

1. Integrantes

* Laura Godoy Callegari – RM569181
* Mariana Dreset Carbollan – RM569207

2. Apresentação do problema e objetivo

A mobilidade urbana é um tema importante para o planejamento das cidades. Nesse contexto, os sistemas de bicicletas compartilhadas precisam ter uma quantidade de bicicletas disponível de acordo com a demanda dos usuários.

Este projeto tem como foco a análise do aluguel de bicicletas compartilhadas na cidade de Seul, na Coreia do Sul.

O objetivo é investigar como fatores como temperatura, umidade, velocidade do vento e horário podem estar relacionados à quantidade de bicicletas alugadas e ao funcionamento do serviço.

Para isso, foram aplicados conceitos de estatística e técnicas de Machine Learning estudados durante o semestre, buscando compreender melhor os dados e identificar padrões que possam contribuir para o planejamento da mobilidade urbana.

3. Base de dados e fonte

Para o desenvolvimento do projeto, foi utilizada a base de dados Seoul Bike Sharing Demand, disponibilizada pelo UCI Machine Learning Repository.

A base contém 8.760 registros referentes ao período de dezembro de 2017 a novembro de 2018, com informações sobre o aluguel de bicicletas por hora e diferentes condições climáticas.

Entre as informações disponíveis, estão:

* Quantidade de bicicletas alugadas;
* Temperatura;
* Umidade;
* Velocidade do vento;
* Visibilidade;
* Precipitação e neve;
* Estações do ano;
* Horário;
* Feriados;
* Funcionamento do serviço.

Fonte dos dados: UCI Machine Learning Repository – Seoul Bike Sharing Demand

DOI: 10.24432/C5F62R

Licença: Creative Commons Attribution 4.0 (CC BY 4.0).

4. Organização dos arquivos e execução

O repositório está organizado da seguinte forma:

CitizenTech/
│
├── base_seoul_bike.csv
│
├── MLAM_CitizenTech.ipynb
│
├── README.md
│
└── resultados/
    ├── 01_dispersao_regressao_simples.png
    ├── 02_correlacao_bivariada.png
    ├── 03_correlacao_multivariada.png
    ├── 04_dispersao_multivariada.png
    ├── estatisticas_descritivas.csv
    ├── matriz_confusao.csv
    ├── matriz_correlacao.csv
    ├── matriz_covariancia.csv
    └── relatorio_estatistico.pdf

Como executar o projeto

Para visualizar e executar as análises, é necessário:

1. Baixar ou clonar este repositório.
2. Ter o Python instalado no computador.
3. Abrir o arquivo MLAM_CitizenTech.ipynb pelo Google Colab, Jupyter Notebook ou VS Code.
4. Instalar as bibliotecas necessárias, caso ainda não estejam disponíveis.
5. Executar as células do notebook na ordem apresentada.

É importante manter o arquivo base_seoul_bike.csv na mesma pasta do notebook, pois ele é utilizado para realizar as análises.

Os gráficos, tabelas e o relatório estatístico são gerados automaticamente e armazenados na pasta resultados/.

Caso o arquivo CSV não esteja na pasta, o próprio notebook também possui uma opção para buscar a base original na fonte oficial.

5. Bibliotecas e dependências

O projeto foi desenvolvido utilizando Python e as seguintes bibliotecas:

Biblioteca	Utilização
Pandas	Leitura e organização dos dados
NumPy	Operações e cálculos numéricos
Matplotlib	Criação de gráficos
SciPy	Cálculos estatísticos e probabilidades
Statsmodels	Regressões e análises estatísticas
Scikit-learn	Modelos de Machine Learning
ReportLab	Geração do relatório em PDF
IPython / IPykernel	Execução do notebook

Para instalar as dependências, basta executar o comando abaixo em uma célula do notebook ou no terminal:

pip install numpy pandas matplotlib scipy statsmodels scikit-learn reportlab ipykernel

6. Principais resultados e limitações

Principais resultados

Durante o desenvolvimento do projeto, foram realizadas diferentes análises estatísticas e modelos de Machine Learning.

Entre os principais resultados observados:

* Distribuição Normal: foram analisadas as temperaturas e calculadas probabilidades considerando a distribuição normal.
* Testes de Hipótese: foram realizados dois testes Z unilaterais, um à esquerda e outro à direita, utilizando diferentes tamanhos de amostra e níveis de significância.
* Análise Bivariada: foi identificada uma relação positiva entre temperatura e quantidade de bicicletas alugadas. A regressão linear simples apresentou significância estatística no teste F.
* Regressão Linear Múltipla: a análise mostrou associações entre a quantidade de aluguéis e as variáveis temperatura, umidade, velocidade do vento e horário. No modelo desenvolvido, temperatura e horário apresentaram coeficientes positivos, enquanto umidade e vento apresentaram coeficientes negativos.
* Regressão Logística: foi desenvolvido um modelo de classificação para identificar se o serviço de bicicletas estava em funcionamento ou fechado, utilizando variáveis meteorológicas.

Os resultados também foram apresentados por meio de gráficos, matrizes de correlação, matrizes de covariância, matriz de confusão e relatório estatístico.

Limitações identificadas

Durante as análises, também foram identificadas algumas limitações:

* A base de dados representa apenas a cidade de Seul e o período de 2017 a 2018, portanto, os resultados não podem ser generalizados automaticamente para outras cidades.
* A distribuição normal foi utilizada como hipótese para os cálculos solicitados, mas isso não significa que todos os dados apresentem uma distribuição perfeitamente normal.
* Os modelos de regressão linear podem não representar todas as relações existentes entre as variáveis, principalmente quando existem padrões sazonais ou relações não lineares.
* Foi identificada dependência temporal entre os resíduos das regressões, o que indica que observações próximas no tempo podem estar relacionadas.
* Na regressão logística, existe uma diferença significativa entre a quantidade de registros de funcionamento e de fechamento do serviço, o que exige cuidado na interpretação dos resultados de classificação.

Além disso, as relações identificadas nas análises representam associações entre as variáveis e não comprovam, necessariamente, uma relação de causa e efeito.

Considerações finais

A realização deste projeto permitiu colocar em prática os conteúdos estudados na disciplina de Machine Learning e Análise de Dados, utilizando uma base de dados real para desenvolver diferentes análises estatísticas e modelos de classificação e regressão.

Com isso, foi possível compreender melhor como a análise de dados pode ajudar a identificar padrões e gerar informações relevantes para questões relacionadas à mobilidade urbana.

⸻

Trabalho acadêmico desenvolvido para a Global Solution – MLAM.
