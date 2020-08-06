InsurCrawler - Python Web Analyzer for InsurUP
========================

> Insurtech Innovation Program

O InsurCrawler é um rastreador multithread que utiliza os módulos BeautifulSoup e urllib.request para realizar o rastreamento de todas as páginas que são geradas a partir de um determinado site selecionado. 
O InsurCrawler é o princípio do projeto InsurUP, que consiste em um sistema de pesquisas qualificadas em sites de notícias, uma vez que o primeiro passo para a criação de uma ferramenta de busca é um sistema de crawler, sendo a espinha dorsal da execução. 
#
## Instale as pendências
### Windows 
~~~
> pip install -r requirements.txt
~~~
### MacOS & Linux
~~~
> pip3 install -r requirements.txt
~~~
#
## Exemplo de execução do crawler
### Windows
~~~python
> python main.py
> Website > https://peru21.pe
# Performs crawl
# Outputs ->> results.csv 
~~~ 

### MacOS
~~~python
> python3 main.py
> Website > https://peru21.pe
# Performs crawl
# Outputs ->> results.csv 
~~~ 

### Linux
~~~python
> sudo python3 main.py
> Website > https://peru21.pe
# Performs crawl
# Outputs ->> results.csv 
~~~

#

## Features

* Rastreia todos os links de um determinado domínio da web e verifica o código de status da resposta.
* Executa todos os rastreamentos usando práticas simultâneas de  Python.
* Grava o resultados de cada página rastreada em um arquivo results.csv
# 
## ToDo

* Análise de cada página para verificação de conformidade com o SEO.
* Criação de um algoritmo de busca estruturado, filtrando resultados por palavras-chave para a consistência da raspagem de dados.
* Criação de um sistema de índice para geração de um mecanismo de Rating;  
#
## Plus

* Protótipo da interface gráfica: https://github.com/TachibanaNero/insur-up
#
## On-Page Checklist

* Deve conter uma tag `<title>` dentro de `<head>`
* Deve conter `<meta name="description" content="...">`
* As imagens devem conter o atributo `alt="keyword"`
* Relatar as 5 palavras-chave mais utilizadas em todas as páginas
* Reportar o tamanho de cada página e dividir em buckets de js, css, imagens, etc...
* Reportar o número de requisições que cada página leva para carregar e categorizá-las em buckets.
* Realizar a análise de tempo de carregamento de cada página.
* Reportar se o Javascrip e CSS não estiverem minificados.
