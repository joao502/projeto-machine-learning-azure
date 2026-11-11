
# 🚲 Projeto Machine Learning Azure — Bike Rentals

## 📌 Sobre o projeto

Este projeto tem como objetivo explorar os recursos do Microsoft Azure Machine Learning para criar, configurar e disponibilizar um modelo de Machine Learning capaz de realizar previsões relacionadas ao aluguel de bicicletas.

O projeto foi desenvolvido como prática de aprendizado, utilizando o conjunto de dados Bike Rentals e um modelo baseado em regressão.

---

## 🛠️ Tecnologias e ferramentas utilizadas

- Microsoft Azure
- Azure Machine Learning Studio
- Automated Machine Learning 
- Modelo de Regressão
- Managed Online Endpoint
- JSON
- JavaScript (para consumo do endpoint)

---

## 📚 Passo a passo do desenvolvimento

### 1. Criação da conta Azure

Realizei o cadastro no Microsoft Azure por meio da modalidade Azure Free Trial, que disponibiliza US$ 200 em créditos para experimentar os serviços da plataforma.

### 2. Criação do projeto e carregamento dos dados

Criei um ambiente de trabalho no Azure Machine Learning Studio e utilizei o conjunto de dados Bike Rentals, disponibilizado nos materiais de aprendizado da Microsoft.

O dataset contém informações relacionadas a datas, condições climáticas e características dos dias, utilizadas para estimar a demanda por aluguel de bicicletas.

### 3. Configuração e treinamento do modelo

Configurei o experimento utilizando uma abordagem de regressão, com o objetivo de prever a quantidade de aluguéis de bicicletas com base nas variáveis disponíveis no conjunto de dados.

Entre as informações utilizadas estão:

- Dia, mês e ano;
- Estação do ano;
- Indicadores de feriado e dia útil;
- Condições climáticas;
- Temperatura e sensação térmica;
- Umidade;
- Velocidade do vento.

### 4. Criação e configuração do endpoint

Após a preparação do modelo, realizei a criação de um **Managed Online Endpoint**, permitindo disponibilizar o modelo por meio de uma API.

Durante essa etapa:

- Configurei a infraestrutura necessária para hospedar o modelo.
- Busquei uma configuração de computação economicamente viável para os testes.
- Identifiquei provedores de recursos do Azure que ainda não estavam registrados na assinatura.
- Realizei o registro dos provedores necessários para permitir a utilização dos serviços.

### 5. Teste e validação do endpoint

Com o endpoint configurado, realizei testes para verificar a comunicação entre a API e o modelo.

O teste foi realizado por meio de uma requisição HTTP POST, utilizando um JSON com as variáveis esperadas pelo modelo.

A requisição foi processada com sucesso e retornou o seguinte resultado:

```json
[
  331.3959016889988
]
```

O valor representa a previsão gerada pelo modelo para os dados enviados na requisição.

---

## 📊 Resultado alcançado

Ao final do projeto, consegui:

- Criar um ambiente de Machine Learning no Azure.
- Trabalhar com um conjunto de dados real de aluguel de bicicletas.
- Configurar um modelo de regressão.
- Disponibilizar o modelo em um endpoint online.
- Realizar uma requisição HTTP para consumir o modelo.
- Receber uma previsão como resposta da API.

---

## 🎯 Objetivo de aprendizado

Este projeto foi desenvolvido com o propósito de adquirir conhecimentos práticos sobre Machine Learning na nuvem, compreender o processo de disponibilização de modelos e aprender a realizar inferências por meio de endpoints hospedados no Microsoft Azure.

