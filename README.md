Repositório do MVP do Spotify.

Título: Análise de dados sobre os hábitos de escuta dos usuários do spotify. Aluno: Igor Klippel Campos MVP (Produto Mínimo Viável) do Sprint: Engenharia de Dados (40530010057_20250_01)

Introdução
O Spotify é uma das principais plataformas de streaming de áudio do mundo, oferecendo acesso a um vasto catálogo de músicas e podcasts. Lançado em 2006, o serviço está presente em mais de 180 países e territórios, com um acervo superior a 100 milhões de faixas. Em julho de 2023, a plataforma contabilizava mais de 527 milhões de usuários ativos globalmente.

Sobre o Dataset:
O conjunto de dados utilizado neste MVP foi obtido no Kaggle em 28 de março de 2025. Ele contém informações diárias sobre as 50 músicas mais tocadas em 73 países, abrangendo o período de 17 de outubro de 2023 até 28 de março de 2025.(dia do download).

Link do dataset:: https://www.kaggle.com/datasets/asaniczka/top-spotify-songs-in-73-countries-daily-updated

Objetivos Principais:
Explorar e analisar os dados para entender as principais tendências musicais no Spotify, utilizando atributos técnicos das faixas. Especificamente, quero saber se músicas com conteúdo explícito são mais populares do que aquelas sem conteúdo explícito ou censuradas.

Sobre a Carga do Dataset:
O dataset foi baixado no formato CSV e carregado no ambiente Databricks via DBFS (Databricks File System), sendo posteriormente processado com Apache Spark.

Qualidade de dados:
Total de 1.869.020 registros distribuídos em 25 colunas.
Presença de valores nulos em algumas colunas.
Algumas faixas possuem duração de 0 segundos, o que exige atenção no tratamento de dados.

Desafios Técnicos:
Utilização do Databricks Community Edition, com recursos de cluster limitados.
Processamento dos dados utilizando Apache Spark ao invés de SQL ou Pandas.
Estruturação do projeto seguindo o modelo de camadas em medalhão (bronze, silver, gold).

Autoavaliação:
Trabalhar em um ambiente em nuvem como o Databricks foi uma experiência enriquecedora. Apesar da limitação da versão gratuita como a necessidade de reinicializar o cluster a cada sessão, foi possível conduzir o projeto de forma eficiente.

Utilizar Spark apresentou um grau maior de complexidade em comparação a ferramentas mais familiares pra mim como Pandas e SQL, mas proporcionou aprendizado sobre processamento distribuído e escalabilidade.

A aplicação do modelo de medalhão foi essencial para estruturar as etapas da pipeline de forma clara e organizada.

A ausência de uma coluna com o gênero musical foi uma limitação para certas análises qualitativas infelizmente, não foi possível inferir com precisão os gêneros apenas com os atributos disponíveis.

Consegui alcançar o objetivo original do projeto. Para trabalhos futuros, pretendo aplicar algoritmos de aprendizado de máquina com o intuito de identificar padrões que contribuam para a popularidade de músicas em diferentes países.
