# Modelagem do Banco de Dados #

<p> Para melhor a organização dos dados, alguns bancos de dados conhecidos como "STAGES" foram implementados.</p>

#### DM_STAGE_1 ####

<p> Criado com apenas uma tabela denominada "VOTACAO_CANDIDATO_MUN_ZONA", este banco tem como objetivo representar fielmente a estrutura e armazenar os dados retirados do [Repositório de Dados Eleitorais - TSE - Tribunal Superior Eleitoral](http://www.tse.jus.br/hotSites/pesquisas-eleitorais/index.html) em arquivos de formato ".txt".</p>

<p><strong>Representação Física do Banco:</strong></p>

![diagrama_fisico_stage_1](./img/diagrama_fisico_stage_1.png)

<p> Faça aqui <strong>[Download](https://github.com/mateusblopes/fazendo-bi-do-zero/tree/master/3.%20Execucao/3.2.%20Modelagem/scripts/Criando%20DM_STAGE_1.sql)</strong> do script de criação da tabela "VOTACAO_CANDIDATO_MUN_ZONA" do "DM_STAGE_1"</p>

#### DM_STAGE_2 ####

<p> Criado com apenas uma tabela resumida denominada "VOTACAO_CANDIDATO_MUN_ZONA", este banco tem como objetivo representar de forma suscinta os dados de formo a facilitar a criação de dashboards por conter apenas os dados que são relevantes para a criação do mesmo.</p>

<p><strong>Representação Física do Banco:</strong></p>

![diagrama_fisico_stage_1](./img/diagrama_fisico_stage_2.png)

<p> Faça aqui [Download](https://github.com/mateusblopes/fazendo-bi-do-zero/tree/master/3.%20Execucao/3.2.%20Modelagem/scripts/Criando%20DM_STAGE_2.sql) do script de criação da tabela "VOTACAO_CANDIDATO_MUN_ZONA" do "DM_STAGE_2"</p>
