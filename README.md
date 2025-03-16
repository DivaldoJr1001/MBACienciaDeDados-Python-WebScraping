<img src='https://www.unifor.br/o/unifor-theme/images/unifor-logo-horizontal.svg' width="250px">

# MBA em Ciência de Dados - Universidade de Fortaleza

## Data Harvesting - Projeto de Disciplina

### Prof. Ms. Alex Lima

#### <b>(Março/2025)</b>

-------------------------

### <b>Aluno:</b> Divaldo Aderaldo de Oliveira Júnior (2419413)<br>

### Scraping de dados e comparação de preços em múltiplos sites com base em uma string de pesquisa.

-------------------------

## 1. Introdução
Este projeto tem como objetivo realizar a coleta de dados de preços de produtos em múltiplos sites de comércio eletrônico, utilizando técnicas de web scraping. O foco principal é comparar os preços de um produto específico (no caso, o iPhone 15) em diferentes plataformas.

O projeto foi desenvolvido em Python, utilizando as bibliotecas Selenium, Pandas e Matplotlib juntamente a Seaborn para a coleta, organização e visualização dos dados.

## 2. Fontes dos Dados
Os dados foram coletados diretamente dos seguintes sites de comércio eletrônico:
- [**Mercado Livre**](https://lista.mercadolivre.com.br)
- [**Kabum**](https://www.kabum.com.br)
- [**Horizon Play**](https://www.horizonplay.com.br)
- [**XonGeek**](https://www.xongeek.com.br)
- [**Bne Store**](https://www.bnestore.com.br/loja)

Os sites foram escolhidos por não possuir Captcha para interferir com a coleta de dados.

## 3. Ferramentas Utilizadas
- **Python**: Linguagem de programação utilizada para desenvolver o script de web scraping.
- **Selenium**: Biblioteca utilizada para automatizar a navegação e coleta de dados nos sites.
- **Pandas**: Biblioteca para manipulação e análise de dados.
- **Matplotlib/Seaborn**: Bibliotecas para visualização de dados.
- **Google Colab**: Ambiente de execução do código, que permite a execução de scripts Python diretamente no navegador.

## 4. Instruções para Execução do Projeto

### 4.1. Pré-requisitos
- **Python 3.x**: Certifique-se de ter o Python instalado.
- **Bibliotecas Python**: Os comandos de instalação de bibliotecas estão inclusos no código.

### 4.2.1. Execução do Projeto
1. **Clone o repositório** (se estiver utilizando Git):
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio
   ```
2. **Execute o script**:
   - Se estiver executando localmente, utilize o comando:
     ```bash
     python nome_do_script.py
     ```
Alternativamente, o projeto pode ser aberto em Google Colab e executado em nuvem.

### 4.3. Configurações Adicionais
- **Produto a ser pesquisado**: No código, o produto a ser pesquisado é definido na variável `produto_a_pesquisar`. Você pode alterar essa variável para pesquisar outros produtos.
- **Filtragem de Outliers**: O código inclui uma função para filtrar outliers com base no preço dos produtos. Você pode ajustar o limiar de filtragem conforme necessário.

## 5. Resultados Obtidos

### 5.1. Coleta de Dados
O script coleta os preços do produto em cada um dos sites mencionados. Os dados são armazenados em um DataFrame do Pandas, que é posteriormente filtrado para remover outliers que normalmente se referem a produtos diferentes.

### 5.2. Visualização dos Dados
Os dados coletados são visualizados em um gráfico de barras, que compara os preços médios em cada plataforma. O gráfico é gerado utilizando a biblioteca Matplotlib.

### 5.3. Análise dos Resultados com Base no Produto Padrão (iPhone 15)
- **Mercado Livre**: Apresentou os preços mais altos em média.
- **Kabum**: Apresentou os preços mais baixos entre as plataformas analisadas.
- **Horizon Play**: Apresentou preços competitivos, próximos aos do Kabum.
- **XonGeek**: Apresentou preços altos, próximos aos do Mercado Livre.
- **Bne Store**: Apresentou preços intermediários.

### 5.4. Conclusão
Analisando o produto padrão, o projeto demonstra que há uma variação significativa nos preços do iPhone 15 entre diferentes plataformas de comércio eletrônico. A ferramenta desenvolvida pode ser utilizada para monitorar preços e identificar oportunidades de compra mais vantajosas.

## 6. Referências
- [Documentação do Selenium](https://www.selenium.dev/documentation/)
- [Documentação do Pandas](https://pandas.pydata.org/pandas-docs/stable/)
- [Documentação do Matplotlib](https://matplotlib.org/stable/contents.html)
- [Documentação do Seaborn](https://seaborn.pydata.org/tutorial.html)
