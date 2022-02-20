# Challenge BI Alura 2022 - Semana 1
## Dashboard sobre filmes

<p align="center"> 
<img src="https://images.unsplash.com/photo-1536440136628-849c177e76a1?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=725&q=80" </a>

<p align="center">
Photo by: </a> <a href="https://unsplash.com/@myke_simon"> @mike_simon </a>

Elaborado por Francico Foz

<a href="https://img.shields.io/badge/author-gustavolq-blue.svg)](https://www.linkedin.com/in/francisco-tadeu-foz/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>  

---

## Sobre o challenge

O challenge é uma iniciativa da Alura para seus alunos desenvolverem projetos baseado em desafios reais.

### **Contexto de todo o mês**

Três empresas nos contrataram para entender suas bases de dados e exibir informações relevantes com o objetivo de auxiliar suas tomada de decisões.

Conceitos e técnicas de BI serão utilizados para desenvolver um dashboard para uma das empresas.

**A primeira empresa, Alura Films, necessita analisar dados sobre o IMDB (Internet Movie Database) dos filmes e suas informações.**

A segunda empresa, Alura Food, precisa de um dashboard para analisar o mercado de restaurantes na Índia.

A terceira empresa, Alura Skimo, precisa analisar as métricas de suas vendas.

## Descrição semana 1

A Alura Films contratou você para fazer uma pesquisa de mercado, com a finalidade de identificar a seleção ideal de elenco e produção. Para isso, ela disponibilizou uma base de dados do IMDB com 1000 filmes. Use suas habilidades e conhecimentos para explorar, tratar e transformar os dados em informações relevantes que auxiliem na tomada de decisão da empresa.

## Projeto

Para este projeto utilizei a ferramenta [Google Data Studio](https://datastudio.google.com/) e o [Google SpreadSheets](https://docs.google.com/spreadsheets/)

### **Bases de dados**

Os dados fornecidos foram dois arquivos .csv, com as informações da tabela de filmes e outra de posters, com a descrição conforme o [pdf](https://github.com/FranciscoFoz/Challenge_BI_Alura_2022_Semana_1/blob/main/Dados_Fornecidos/Informac%C3%B5es%20sobre%20a%20base%20de%20dados.pdf)

Você pode encontrar os dados iniciais [aqui](https://github.com/FranciscoFoz/Challenge_BI_Alura_2022_Semana_1/tree/main/Dados_Fornecidos)


###     **Limpeza de dados**

Para a construção do dashboard, realizei o tratamento dos dados para que eles ficassem corretos.

#### Etapas:

1. Tradução da coluna "Overview" e "Genre_PT-BR": 

Inseri uma nova coluna no conjunto de dados chamada "Overview_PT-BR" com a tradução das colunas "Overview" e "Genre". Utilizei a função "=GOOGLETRANSLATE()" do google sheets. 

2. Formatação da coluna "Gross":

Formatei os valores que estavam com formato norte americano de "," no lugar do ".", usando a função SUBSTITUIR() e depois acrescentei mais ",00" e formatei a coluna para moeda.

3. Padronização da coluna "Certificate":

Após algumas pesquisas, encontrei os valores equivalentes das classificações indicativas dos filmes e subistituí para que todos ficassem no padrão do Brasil mais os não Classificados:

U: Livre , UA:	10, A: 18, PG-13:	14, Passed:	Não Classificado, PG:	10, R: 18, G:	Livre, not rated:	Não Classificado, Approved:	Livre, PG-12:	14, U/A:	10, 12A:	14, TV-14:	14, GP:	10, Unrated:	Não Classificado, TV-PG:	10, TV-MA:	18, 

###     **Modelagem de dados**


