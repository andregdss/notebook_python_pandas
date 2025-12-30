# Notebook Didático de Análise de Dados com Python Pandas

Este repositório contém um guia avançado e prático sobre a biblioteca **Pandas**, amplamente adotada como padrão industrial para Ciência de Dados em Python.  
O material foi estruturado para cobrir **todo o ciclo de vida do dado**, desde a ingestão de múltiplas fontes (IO) até a análise estatística e a persistência em bancos de dados relacionais.

## 🏛️ Filosofia do Projeto

O notebook é organizado a partir da premissa de que o Pandas vai além da simples visualização de dados, configurando-se como um **ecossistema completo de Data Wrangling**.  
O conteúdo explora os quatro pilares operacionais fundamentais da biblioteca:

- **Filtragem**  
  - Seleção estratégica e condicional de subconjuntos de dados
- **Ordenação**  
  - Organização lógica de registros para análise de tendências
- **Agregação**  
  - Consolidação de informações para extração de métricas analíticas e gerenciais
- **Transformação**  
  - Reestruturação de tipos, formatos e arquitetura dos dados

## 🛠️ Seção Especial: Domínio de Pandas IO (Input/Output)

A parte central do projeto é dedicada à capacidade do Pandas de atuar como um **conector universal de dados**, integrando diferentes formatos e fontes.

### Ingestão de Dados de Diversas Fontes

- **Arquivos Delimitados (CSV)**
  - Uso aprofundado de `read_csv()`
  - Parâmetros de otimização de memória (`nrows`, `usecols`)
  - Tratamento de `encoding` e separadores personalizados
- **Planilhas Complexas (Excel)**
  - Leitura de arquivos `.xlsx` com motores como `openpyxl`
  - Seleção de abas específicas e ajuste de cabeçalhos
- **Dados Semi-estruturados (JSON)**
  - Normalização de dados aninhados com `json_normalize`
  - Conversão de listas e objetos hierárquicos em DataFrames tabulares
- **Web Scraping (HTML)**
  - Coleta automatizada de tabelas diretamente de URLs com `read_html`

### Integração com Bancos de Dados Relacionais (SQL)

O material demonstra a integração entre Python e SQL por meio da biblioteca **SQLAlchemy**:

- **Conexão**
  - Criação de *engines* para comunicação com bancos de dados (ex: SQLite)
- **Persistência (`to_sql`)**
  - Armazenamento de DataFrames como tabelas relacionais
  - Definição de estratégias de substituição ou inserção incremental
- **Consultas Diretas (`read_sql`)**
  - Execução de queries SQL customizadas retornando DataFrames prontos para análise

## 📂 Estrutura de Tópicos e Seções

### 1. Exploração e Diagnóstico (EDA)

Antes da análise, o notebook apresenta técnicas para avaliação inicial da qualidade dos dados:

- **Metadados**
  - Uso de `.info()`, `.dtypes` e `.shape`
- **Qualidade do Dado**
  - Identificação de valores ausentes (`isnull().sum()`)
  - Análise de frequência com `value_counts()`

### 2. Tratamento e Higienização (Data Cleaning)

- **Gestão de Valores Nulos**
  - Preenchimento inteligente (`fillna`)
  - Remoção seletiva (`dropna`)
  - Interpolação de séries temporais
- **Manipulação de Texto**
  - Limpeza de strings com expressões regulares (Regex)
  - Padronização de caracteres e remoção de espaços
- **Séries Temporais**
  - Conversão de datas com `to_datetime`
  - Extração de componentes temporais (dia, mês, ano)

### 3. Transformação e Reshape de Dados

- **Junções (Joins)**
  - Combinação de tabelas com `merge()` e `concat()`
  - Lógicas de *Inner*, *Left*, *Right* e *Outer Join*
- **Reorganização de Dados**
  - Uso de `melt()` para transformação de colunas em linhas
  - Criação de tabelas resumo com `pivot_table()`
- **Lógica Customizada**
  - Aplicação de funções complexas via `.apply()` e expressões `lambda`

### 4. Análise Estatística e Agrupamento

- **Group By**
  - Agregações segmentadas para identificação de padrões
- **Estatística Descritiva**
  - Geração de sumários estatísticos com `.describe()`
- **Multi-Index**
  - Manipulação de índices hierárquicos para dados multidimensionais

## 📈 Estudos de Caso e Aplicações Reais

Os conceitos são consolidados por meio de estudos de caso baseados em dados reais, incluindo:

- **Imobiliário**
  - Análise de precificação de aluguéis e classificação de imóveis
- **Ambiental**
  - Processamento de séries históricas de emissões de CO₂
- **Acadêmico e Saúde**
  - Avaliação de desempenho escolar
  - Análise exploratória de dados hospitalares

## 🚀 Tecnologias Utilizadas

- **Python 3.x**
- **Pandas** — núcleo do processamento de dados
- **NumPy** — operações vetoriais e suporte numérico
- **SQLAlchemy** — interface com bancos de dados SQL
- **Matplotlib** — visualização exploratória de dados

## Como Utilizar

Para executar o notebook, recomenda-se:

- Utilizar o **Google Colab**, ou
- Executar localmente em um ambiente **Jupyter Notebook**

Basta abrir o arquivo `python_pandas.ipynb` e executar as células sequencialmente para acompanhar os exemplos e exercícios.
