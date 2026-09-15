# 📊 Processamento de Linguagem Natural e Análise de Dados (Aula_Banco_Dados)

Este repositório contém os projetos, atividades práticas e scripts desenvolvidos durante a graduação em **Ciência de Dados**, cobrindo desde a manipulação e visualização de dados até técnicas introdutórias de **Processamento de Linguagem Natural (PLN)** e integração com bancos de dados.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

* **Linguagem:** Python 3.9+
* **Ambiente de Desenvolvimento:** VS Code, Jupyter Notebook (`.ipynb`)
* **Controle de Versão:** Git & GitHub Desktop
* **Bibliotecas Principais:**
  * `pandas` — Manipulação e análise de dados estruturados (CSV/Excel)
  * `matplotlib` — Criação de gráficos e visualizações de dados em 3D
  * `openpyxl` — Suporte para leitura e escrita de arquivos Excel (`.xlsx`)

---

## 📂 Conteúdo do Repositório

* **`cubo_dados_para_analise.ipynb`**: Análise multidimensional e visualização em gráfico 3D da linha de produtos, preços unitários, quantidades e totais de vendas.
* **`Automacao-banco-dados_escola-1.ipynb`**: Scripts de automação e integração de dados estruturados.
* **`SuperMercados.xlsx` / `dados_escola.csv` / `dados.csv`**: Conjuntos de dados utilizados para testes e análises práticas.
* **`amostra_avaliacao_loja.csv`**: O repositório também conta com um pipeline de mineração de dados textuais aplicados à análise de feedbacks de clientes (*e-commerce* / avaliações de lojas).

---

## 🚀 Como Executar o Projeto Localmente

1. **Clone o repositório:**
   ```bash
  git clone [https://github.com/SEU_USUARIO/Aula_Banco_Dados.git](https://github.com/Crisstudy/Aula_Banco_Dados.git)
   cd Aula_Banco_Dados

2. Crie e ative o ambiente virtual (venv):
   macOS / Linux:
   python3 -m venv venv
   source venv/bin/activate

   Windows:
   python -m venv venv
   venv\Scripts\activate

3. Instale as dependências:
   pip install pandas matplotlib openpyxl ipykernel

4. Execute os Notebooks:
   Abra o VS Code na pasta do projeto:
   code .
   Selecione o Kernel do Jupyter para apontar para o seu ambiente virtual
   ./venv/bin/python
   
## ⛏️ Mineração de Dados de Texto (Text Mining & PLN)

O repositório também conta com um pipeline de mineração de dados textuais aplicados à análise de feedbacks de clientes (*e-commerce* / avaliações de lojas).

### 🛠️ Etapas do Processo de Mineração:
* **Limpeza e Tratamento:** Tratamento de valores nulos (`NaN`) e padronização dos tipos de dados com `pandas`.
* **Tokenização e Normalização:** Divisão de textos em tokens e conversão para caixa baixa para evitar duplicidade de contagens.
* **Contagem de Frequência (Bag-of-Words):** Mapeamento e estruturação do vocabulário do dataset utilizando a classe `Counter` da biblioteca `collections`.
* **Processamento de Linguagem Natural com spaCy:** Aplicação do modelo em português (`pt_core_news_sm`) para tarefas avançadas de PLN.

### 📋 Principais Bibliotecas Utilizadas nesta Etapa:
```python
import pandas as pd
from collections import Counter
import spacy
