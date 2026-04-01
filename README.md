# Análise de Crédito com Python: Exploração de Dados

Este repositório contém uma aplicação prática de Ciência de Dados voltada para o setor financeiro. O objetivo principal é realizar uma Análise Exploratória de Dados (EDA) em um conjunto de dados de 30.000 clientes de cartões de crédito para compreender o perfil dos usuários e identificar padrões de inadimplência.

---

## Objetivos do Projeto

* **Configuração de Ambiente**: Demonstração de uso do Python em ambiente local (VS Code/Terminal).
* **Manipulação de Dados**: Utilização da biblioteca Pandas para carregamento e estruturação de arquivos Excel.
* **Engenharia de Recursos**: Classificação automatizada de variáveis entre Categóricas e Numéricas baseada na cardinalidade dos dados.
* **Diagnóstico de Integridade**: Identificação de valores ausentes e análise da qualidade do dataset.

---

## Tecnologias e Ferramentas

| Ferramenta | Descrição |
| :--- | :--- |
| **Linguagem** | Python 3.x |
| **Biblioteca** | Pandas (Manipulação de dados) |
| **Biblioteca** | xlrd / openpyxl (Motores de leitura Excel) |
| **IDE** | Visual Studio Code (VS Code) |

---

## Estrutura do Repositório

```text
Trabalho_de_Dados/
├── Data/
│   └── default_of_credit_card_clients__courseware_version_1_21_19.xls
├── analise_credito.py
└── README.md
Funcionamento do Código
O script executa um fluxo de trabalho estruturado em quatro etapas principais:

Carregamento: Importação dos dados e verificação das dimensões iniciais (linhas e colunas) através do atributo .shape.

Mapeamento de Variáveis: O algoritmo percorre as colunas do DataFrame utilizando uma estrutura de repetição e condicional:

Colunas com menos de 15 valores únicos são classificadas como Categóricas.

Colunas com 15 ou mais valores únicos são tratadas como Numéricas.

Análise Estatística:

Numéricas: Cálculo de métricas descritivas (média, desvio padrão, valores mínimos e máximos) via .describe().

Categóricas: Cálculo de frequência absoluta e relativa via .value_counts().

Verificação de Dados Faltantes: Checagem sistemática de valores nulos utilizando .isnull().sum().

Como Executar o Projeto
Clone o repositório:

Bash
git clone [https://github.com/Davi-Silva-Developer/analise-credito-python.git](https://github.com/Davi-Silva-Developer/analise-credito-python.git)
Instale as dependências necessárias:

Bash
pip install pandas xlrd openpyxl
Execute o script Python:

Bash
python analise_credito.py
Desenvolvido por Davi Silva
