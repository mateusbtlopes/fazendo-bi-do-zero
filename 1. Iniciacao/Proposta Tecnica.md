# Proposta Técnica Projeto de Business Intelligence - Eleições Municipais 2016 #

## 1. Entendimento do Problema ##

### 1.1. Visão Geral ###

<p>Visando atender a demanda proposta pelo professor Rodrigo Vitorino Moravia de apresentarmos no trabalho final da disciplina "OLAP - Projeto e Construção de Aplicações OLAP" um dashboard que permita a visualização consolidada de dados de nossa escolha, busquei informações sobre a apuração das eleições municipais de 2016. Informações estas que são disponibilizadas pelo TRE (Tribunal Regional Eleitoral) em seu repositório de dados eleitorais (vide site: http://www.tse.jus.br/hotSites/pesquisas-eleitorais/candidatos.html), com arquivos referentes a apuração da "Votação nominal por município e zona" arquivo que é disponibilizado em formato ZIP, contendo um arquivo ".TXT" com as apurações nominais por município e zona de cada estado brasileiro.</p>

### 1.2. Objetivos ###

<p>O objetivo deste trabalho é principalmente consolidar o conhecimento adquirido nesta matéria e apresentar uma solução de Business Intelligence com modelagem, ETL (Extract, Transform, Load dos dados) e um painel/dashboard construído em uma ferramenta de Data Visualization que permita reunir, classificar, analisar, monitoramento e correlacionar diferentes candidatos eleitos de diferentes cidades, estados e regiões do Brasil.</p>

## 2. Solução Proposta ##

### 2.1. Visão Geral ###

<p>Propomos disponibilizar uma solução completa de Business Intelligence contemplando planejamento, modelagem de dados, extração dos dados, tranformação dos dados, carga dos dados no banco modelado, criação de paineis de visualização dos dados e testes automatizados para homologação de consistência dos dados apresentados.</p>

### 2.2. Modelagem dos Dados ###

<p>A modelagem dos dados será feita utilizando os conceitos de modelagem dimensional, respondendo aos requisitos do usuário a serem levantados na próxima fase do projeto.</p>

### 2.3. ETL ###

<p>A Extração, Transformação e Carga dos dados no banco de dados modelado, será realizada por meio de alguma ferramenta de mercado baseando-se na experiência e conhecimento prévio do aluno responsável pelo trabalho.</p>

### 2.4. OLAP ###

<p>A visualização dos dados na ferramenta OLAP será realizada por meio de alguma ferramenta de mercado baseando-se na experiência e conhecimento prévio do aluno responsável pelo trabalho.</p>

### 2.5. Homologação ###

<p>A homologação das informações dispostas nos dashboards serão validadas por meio de testes automatizados a serem desenvolvidos com alguma ferramenta de mercado baseando-se na experiência e conhecimento prévio do aluno responsável pelo trabalho.</p>

## 3. Arquitetura ##

### 3.1. Visão Geral ###

<p>Nossa proposta de arquitetura segue algumas diretrizes:</p>
<p>* Queremos uma arquitetura que seja de fácil instalação e manutenção para todas as ferramentas utilizadas neste projeto;</p>

### 3.2. Modelagem dos Dados ###

<p>Nossa proposta de ferramenta para modelagem de dados será a utilização de um banco de dados Microsoft SQL Server versão 2014.</p>

### 3.3. ETL ###

<p>Nossa proposta de ferramenta para extração, transformação e carga dos dados será a utilização do SQL Server Integration Service 2014 (SSIS).</p>

### 3.4. OLAP ###

<p>Nossa proposta de ferramenta para elaboração dos dashboards será a utilização do Tableau, Qlik View ou Power BI.</p>

### 3.5. Homologação ###

<p>Nossa proposta de ferramenta para homologação dos dados do ETL e Dashboard será a utilização do Selenium WebDriver.</p>

### 3.6. Controle de Versão ###

<p>Nossa proposta de ferramenta para controle de versão do código fonte do projeto será a utilização das issues do próprio repositório GitHub.</p>

### 3.7. Controle de Atividades ###

<p>Nossa proposta de ferramenta para controle das atividades será a utilização das issues do próprio repositório GitHub.</p>

## 4. Sobre o Aluno ##

<p>Mateus Bruno T. Lopes é aluno da 8ª oferta do curso de pós-graduação em Business Intelligence da PUC Minas - Belo Horizonte - Minas Gerais.</p>

## 5. Cronograma ##

### 5.1. Cronograma Resumido ###

<p>-</p>

### 5.2. Cronograma Detalhado ###

<p>-</p>