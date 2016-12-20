# Plano de Testes do Projeto #

| Nome da tarefa | Responsável | Data |
| ------------- | ------------- | ------------- |
| Plano de Teste | Mateus Bruno T. Lopes | 20/12/2016 |

## Testes - Visão Candidatos ##

* Quantidade de candidatos a prefeito e a vereador foram lançados?
	
   SQL:
    --
		SELECT COUNT(*) AS 'QTDE CANDIDATOS', [DESC_CARGO] AS 'DESCRICAO CARGO'
		FROM [DM_ELEICOES].[dbo].[DIM_CANDIDATO]
		GROUP BY [DESC_CARGO], [SIGLA_PARTIDO], [NOME_PARTIDO]

<hr>
   
* Quantidade de candidatos a prefeito e a vereador foram eleitos?
	
   SQL:
    --
		SELECT COUNT(*) AS 'QTDE CANDIDATOS ELEITOS', [DESC_CARGO] AS 'DESCRICAO CARGO'
		FROM [DM_ELEICOES].[dbo].[DIM_CANDIDATO] C
		INNER JOIN DIM_SITUACAO_CANDIDATO S
		ON C.ID_CANDIDATO = S.ID_CANDIDATO
		WHERE S.DESC_SIT_CAND_TOT = 'ELEITO'
   		 OR S.DESC_SIT_CAND_TOT = 'ELEITO POR MÉDIA'
   		 OR S.DESC_SIT_CAND_TOT = 'ELEITO POR QP'
		GROUP BY [DESC_CARGO]

<hr>

* Quantidade de candidatos a prefeito e a vereador foram para o 2º turno?

   SQL:
    --
		SELECT COUNT(*) AS 'QTDE CANDIDATOS 2º TURNO', [DESC_CARGO] AS 'DESCRICAO CARGO'
		FROM [DM_ELEICOES].[dbo].[DIM_CANDIDATO] C
		INNER JOIN DIM_SITUACAO_CANDIDATO S
		ON C.ID_CANDIDATO = S.ID_CANDIDATO
		WHERE S.DESC_SIT_CAND_TOT = '2º TURNO'
		GROUP BY [DESC_CARGO]

<hr>

* Quantidade de candidatos a prefeito e a vereador foram considerados inaptos para concorrer as eleições?

   SQL:
    --
		SELECT COUNT(*) AS 'QTDE CANDIDATOS INAPTOS', [DESC_CARGO] AS 'DESCRICAO CARGO'
		FROM [DM_ELEICOES].[dbo].[DIM_CANDIDATO] C
		INNER JOIN DIM_SITUACAO_CANDIDATO S
		ON C.ID_CANDIDATO = S.ID_CANDIDATO
		WHERE S.DESC_SIT_CAND_SUPERIOR = 'INAPTO'
		GROUP BY [DESC_CARGO]

## Testes - Visão Partidos ##

* Quantidade de candidatos a prefeito e a vereador foram lançados por partido?

   SQL:
    --
		SELECT COUNT(*) AS 'QTDE CANDIDATOS', [DESC_CARGO] AS 'DESCRICAO CARGO', [SIGLA_PARTIDO] AS 'SIGLA PARTIDO', [NOME_PARTIDO] AS 'NOME PARTIDO'
		FROM [DM_ELEICOES].[dbo].[DIM_CANDIDATO]
		GROUP BY [DESC_CARGO], [SIGLA_PARTIDO], [NOME_PARTIDO]

<hr>

* Quantidade de candidatos a prefeito e a vereador foram eleitos lançados por partido?

   SQL:
    --
		SELECT COUNT(*) AS 'QTDE CANDIDATOS ELEITOS', [DESC_CARGO] AS 'DESCRICAO CARGO', [SIGLA_PARTIDO] AS 'SIGLA PARTIDO', [NOME_PARTIDO] AS 'NOME PARTIDO'
		FROM [DM_ELEICOES].[dbo].[DIM_CANDIDATO] C
		INNER JOIN DIM_SITUACAO_CANDIDATO S
		ON C.ID_CANDIDATO = S.ID_CANDIDATO
		WHERE S.DESC_SIT_CAND_TOT = 'ELEITO'
   		 OR S.DESC_SIT_CAND_TOT = 'ELEITO POR MÉDIA'
   		 OR S.DESC_SIT_CAND_TOT = 'ELEITO POR QP'
		GROUP BY [DESC_CARGO], [SIGLA_PARTIDO], [NOME_PARTIDO]

<hr>

* Quantidade de candidatos a prefeito e a vereador foram para o 2º turno por partido?

   SQL:
    --
		SELECT COUNT(*) AS 'QTDE CANDIDATOS 2º TURNO', [DESC_CARGO] AS 'DESCRICAO CARGO', [SIGLA_PARTIDO] AS 'SIGLA PARTIDO', [NOME_PARTIDO] AS 'NOME PARTIDO'
		FROM [DM_ELEICOES].[dbo].[DIM_CANDIDATO] C
		INNER JOIN DIM_SITUACAO_CANDIDATO S
		ON C.ID_CANDIDATO = S.ID_CANDIDATO
		WHERE S.DESC_SIT_CAND_TOT = '2º TURNO'
		GROUP BY [DESC_CARGO], [SIGLA_PARTIDO], [NOME_PARTIDO]

<hr>

* Quantidade de candidatos a prefeito e a vereador foram considerados inaptos para concorrer as eleições por partido?

   SQL:
    --
		SELECT COUNT(*) AS 'QTDE CANDIDATOS INAPTOS', [DESC_CARGO] AS 'DESCRICAO CARGO', [SIGLA_PARTIDO] AS 'SIGLA PARTIDO', [NOME_PARTIDO] AS 'NOME PARTIDO'
		FROM [DM_ELEICOES].[dbo].[DIM_CANDIDATO] C
		INNER JOIN DIM_SITUACAO_CANDIDATO S
		ON C.ID_CANDIDATO = S.ID_CANDIDATO
		WHERE S.DESC_SIT_CAND_SUPERIOR = 'INAPTO'
		GROUP BY [DESC_CARGO], [SIGLA_PARTIDO], [NOME_PARTIDO]