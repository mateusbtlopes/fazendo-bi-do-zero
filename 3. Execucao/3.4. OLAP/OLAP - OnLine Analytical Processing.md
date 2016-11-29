# OLAP - OnLine Analytical Processing #

Como já sabemos os dados utilizados neste projeto vem do [Repositório de Dados Eleitorais - TSE - Tribunal Superior Eleitoral](http://www.tse.jus.br/hotSites/pesquisas-eleitorais/index.html) em formato ".txt", com a intensão de fornecer maior confiabilidade no armanezamento destes dados, criamos alguns STAGE's que foram povoadas utilizando o processo que damos o nome de ETL (Extração, Transformação e Carga de Dados), para executar tais tarefas que serão detalhadas abaixo, utilizamos a ferramenta da Microsoft denominada <strong>SSIS - SQL Server Integration Server</strong>, entretanto precisamos exibir os dados de forma organizada e de simples entendimento, para isso utilizamos a ferramenta [Tableau Desktop](https://public.tableau.com/profile/mateusblopes#!/).

### Apuração Eleições Municipais 2016 - Visão Candidatos ###

![SSIS - Exemplo Extração De Dados](./imagens/Dashboard-VisãoGeral-Candidatos.png)

### Apuração Eleições Municipais 2016 - Visão Partidos ###

![SSIS - Exemplo Extração De Dados](./imagens/Dashboard-VisãoGeral-Partidos.png)