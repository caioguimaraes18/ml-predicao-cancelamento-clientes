# 📉 Previsão de Cancelamento de Clientes

Este projeto tem como objetivo desenvolver um modelo de machine learning capaz de prever se um cliente irá cancelar seu contrato com base em variáveis comportamentais, contratuais e financeiras.

---

## 📂 Sobre o Projeto

O modelo foi construído com base em um dataset simulado com mais de 400 mil registros de clientes, contendo informações como:

- Tempo de contrato e atividade
- Pagamentos em atraso ou em dia
- Valor da mensalidade
- Nível de pagamento
- Perfil do cliente (sexo, idade, filhos, etc.)

O foco principal é identificar padrões que indicam **risco de cancelamento**, apoiando ações de retenção e tomada de decisão.

---

## 🛠️ Tecnologias Utilizadas

- Python 3.10
- Pandas
- Seaborn e Matplotlib
- Scikit-Learn
- Jupyter Notebook

---

## 🔍 Etapas do Projeto

1. **Pré-processamento dos dados**
   - Limpeza e seleção de colunas relevantes
   - Conversão de variáveis categóricas para numéricas
   - Criação da variável-alvo `CANCELAMENTO` (1 = cancelou, 0 = não cancelou)

2. **Exploração e análise de dados**
   - Análises visuais com gráficos de distribuição e taxa de cancelamento
   - Avaliação de perfis com maior risco de churn

3. **Criação do modelo de Machine Learning**
   - Separação entre treino e teste (70/30)
   - Treinamento com Random Forest Classifier
   - Avaliação com acurácia, matriz de confusão e F1-score

4. **Geração de insights**
   - Visualização da importância das variáveis
   - Identificação de fatores-chave para cancelamento (como dias ativos e pagamentos em atraso)

---

## 📊 Principais Insights

- A maior taxa de cancelamento está entre **clientes com menos dias ativos**, indicando que **clientes novos têm mais chance de cancelar**.
- Variáveis como `QT_PC_PAGA_ATRASO` e `VL_MENSALIDADE_ATRASO` têm alta influência no cancelamento.
- Clientes com baixo nível de pagamento apresentam maior probabilidade de cancelamento.

---

## 📁 Resultados

- Acurácia do modelo: **(insira aqui, ex: 0.97)**
- Importância das variáveis visualizada em gráfico de barras horizontais
- Gráficos de taxa de cancelamento por sexo e nível de pagamento

---

## 📌 Como rodar o projeto

1. Clone este repositório:
```bash
git clone https://github.com/seu-usuario/projeto-cancelamento-clientes.git
```
2. Instale as dependências:


```bash
pip install -r requirements.txt
```

3.Rode o notebook: 


```bash
jupyter notebook
```

---

## 🧠 Inspiração

Este projeto foi inspirado na aula da [Hashtag Treinamentos](https://www.youtube.com/watch?v=BIMvMC0XqFM&list=PLI-bpOj6_aWGz89aONnhAUT3GpMP2VvW7), onde é demonstrado o passo a passo para construir um modelo de previsão de cancelamento de clientes.

A partir dessa base, acrescentei novas análises, gráficos personalizados e **insights estratégicos** com foco em comportamento de clientes, como:

- Identificação de perfis com maior risco de churn com base em variáveis como tempo de atividade e inadimplência.
- Visualizações adicionais da taxa de cancelamento por categorias como sexo e nível de pagamento.
- Análise da importância das variáveis no modelo de Machine Learning.

