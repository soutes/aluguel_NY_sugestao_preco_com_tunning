# Projeto de Ciências de Dados - Rental Price NY

Desenvolvi este projeto como teste para o Programa Lighthouse da Indicium Tech (saiba mais sobre este programa em https://materiais.indicium.tech/lighthouse-aguardar-nova-turma).

## Objetivo
Desenvolver um modelo de previsão de preços a partir do dataset oferecido, e avaliar
tal modelo utilizando as métricas de avaliação
que mais fazem sentido para o problema.

## Entregas
1. Faça uma análise exploratória dos dados (EDA), demonstrando as principais características entre as variáveis e apresentando algumas hipóteses de negócio relacionadas.
2. Supondo que uma pessoa esteja pensando em investir em um apartamento para alugar na
plataforma, onde seria mais indicada a compra?
3. O número mínimo de noites e a disponibilidade ao longo do ano interferem no preço?
4. Existe algum padrão no texto do nome do local para lugares de mais alto valor?
5. Explique como você faria a previsão do preço a partir dos dados. Quais variáveis e/ou suas transformações você utilizou e por quê? Qual tipo de problema estamos resolvendo (regressão, classificação)? Qual modelo melhor se aproxima dos dados e quais seus prós e contras? Qual medida de performance do modelo foi escolhida e por quê?
6. Sugestão de preço para um apartamento


## Estrutura do Projeto

A estrutura do projeto segue uma organização clara e lógica para facilitar a navegação:

├── docs

    - rental_ny_baseline.csv

    - rental_ny_clean.csv

    - teste_indicium_precificacao.csv

├── files

    - [Lighthouse] Desafio Ciência de Dados 2025-3.docx

├── models

    - model_rfe_xgb_ajustado.pkl

    - model_rfe_lgb_tunnig.pkl (inluído após o prazo de envio com fins educativos. Não deve ser considerado na seletiva do Lighthouse.)

├── notebooks

    - rental_price_ny_EDA.ipynb

    - rental_price_ny_model.ipynb

    - rental_price_ny_model_tunning.ipynb (inluído após o prazo de envio com fins educativos. Não deve ser considerado na seletiva do Lighthouse.)

├── LH_CD_LUIZSOUTES_EDA.pdf

└── README.md


- **`docs`**: Diretório com o arquivo em CSV fornecido para o desenvolvimento deste teste e outros dois CSVs com os dataframes manipulados que foram utilizados no projeto.
- **`notebooks`**: Contém o notebook Jupyter `rental_price_ny_EDA.ipynb` com o tratamento visualização e análises dos dados. Além disso, contém o arquivo 'rental_price_ny_model.ipynb' com a criação e treinamento do modelo que utiliza a biblioteca XG Boost Regressor. No final deste consta um teste com uma sugestão de valor para uma nova propriedade.
- **`LH_CD_LUIZSOUTES_EDA.pdf`**: Este arquivo possui a Expoloração e Análise dos Dados completa. Para melhor navegabilidade neste arquivo, faça o download e utilize o Adobe Acrobat.

## Pré-requisitos

- Python 3.12 ou superior.
- Bibliotecas com versão igual ou superior a:
### Pythonic 
numpy = 2.2.2

pandas = 2.2.3

matplotlib = 3.10.0

seaborn = 0.13.2

scikit-learn = 1.6.1

xgboost = 2.1.3

plotly = 6.0.0

## Funcionalidades
### Tratamento de Dados:
- Ajuste no nome de colunas para ficarem com apenas um idioma.
- Limpeza de valores ausentes.
- Tratamento de outliers.

### Visualização:
- Identificação de outliers por meio de boxplots.
- Análises em relação ao grupo de bairros, preço, influência de pontos turísticos, entre outros.
- A Análise Exploratória de Dados (EDA) completa pode ser visualizada no arquivo LH_CD_LUIZSOUTES_EDA.pdf


## Previsão com Machine Learning:
    
**Modelagem e Sugestão de preço:**
    - O modelo foi criado, treinado e ao final avaliado.
    - Uma nova base de dados foi inserida e nesta foi aplicado o modelo com o intuito de receber a sugestão do preço.
    
**Possibilidade de expansão:**
    - Atualização da base com dados mais atuais
    - Refinar os hiper-parâmetros do modelo XGBoost

# Atualização no projeto
Após o prazo para envio, estudei sobre como refinar os hiper parâmetros.
Foi durante estes estudos que tive conhecimento sobre as vantagens do LGBMRegressore e também do **Bayesian Optimization.**
Então apliquei os mesmos no projeto e consegui melhores resultados, conforme demonstro no final do arquivo rental_price_ny_model_tunning.ipynb. Após isto, exportei o modelo para pkl (models/model_rfe_lgb_tunnig.pkl).

## Observação:
Estes arquivos (rental_price_ny_model_tunning.ipynb. e model_rfe_lgb_tunnig.pkl) servem apenas para aprimorar meu conhecimento e não para a seletiva do Programa Lighthouse da Indicium Tech. 

## Contato
Desenvolvedor: Luiz Soutes
LinkedIn: https://www.linkedin.com/in/soutes/
