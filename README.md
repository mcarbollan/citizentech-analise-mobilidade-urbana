CitizenTech – Análise de Mobilidade Urbana

Global Solution | MLAM

Integrantes

* Laura Godoy Callegari – RM569181
* Mariana Dreset Carbollan – RM569207

Sobre o projeto

Este projeto foi desenvolvido como parte da Global Solution da disciplina de Modelagem Linear para Aprendizado de Máquina (MLAM).

O trabalho tem como tema a mobilidade urbana e utiliza uma base de dados sobre o aluguel de bicicletas compartilhadas na cidade de Seul, na Coreia do Sul.

O objetivo é analisar como fatores como temperatura, umidade, velocidade do vento e horário podem influenciar a quantidade de bicicletas alugadas, utilizando conceitos de estatística e Machine Learning estudados durante o semestre.

Base de dados

Para realizar as análises, foi utilizada a base de dados Seoul Bike Sharing Demand, disponibilizada pelo UCI Machine Learning Repository.

A base apresenta informações sobre o aluguel de bicicletas entre 2017 e 2018, incluindo:

* Quantidade de bicicletas alugadas por hora;
* Temperatura;
* Umidade;
* Velocidade do vento;
* Visibilidade;
* Precipitação e neve;
* Estações do ano;
* Feriados;
* Funcionamento do serviço.

Fonte: UCI Machine Learning Repository

O que foi desenvolvido

Durante o projeto, foram realizadas cinco etapas principais:

1. Distribuição Normal

Análise da distribuição das temperaturas e cálculo de probabilidades utilizando conceitos de distribuição normal.

2. Testes de Hipótese

Aplicação de testes Z para analisar hipóteses relacionadas à média dos dados.

3. Análise Bivariada

Estudo da relação entre temperatura e quantidade de bicicletas alugadas, utilizando covariância, correlação de Pearson e regressão linear simples.

4. Regressão Linear Múltipla

Análise da influência de diferentes variáveis, como temperatura, umidade, vento e horário, na quantidade de bicicletas alugadas.

5. Regressão Logística

Utilização de um modelo de classificação para analisar o funcionamento do serviço de bicicletas compartilhadas.

Ferramentas utilizadas

* Python
* Google Colab / Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* SciPy
* Statsmodels
* Scikit-learn

Organização dos arquivos

O projeto está organizado da seguinte maneira:

CitizenTech/
│
├── base_seoul_bike.csv
├── MLAM_CitizenTech.ipynb
├── README.md
│
└── resultados/
    ├── gráficos das análises
    ├── tabelas estatísticas
    └── relatorio_estatistico.pdf

Conclusão

Com o desenvolvimento deste trabalho, foi possível aplicar na prática os conteúdos estudados na disciplina, explorando diferentes métodos estatísticos e modelos de Machine Learning.

As análises permitiram observar como as condições climáticas e os horários estão relacionados à demanda por bicicletas compartilhadas, mostrando como a análise de dados pode contribuir para uma melhor compreensão da mobilidade urbana.

Projeto acadêmico desenvolvido para a Global Solution – MLAM.
