# Glossário 

## A
ACID (Atomicidade, Consistência, Isolamento e Durabilidade): Conjunto de propriedades que garante a confiabilidade das transações de dados, evitando corrupção em caso de falhas de escrita

Alerta SQL: Recurso que monitora consultas e envia notificações automáticas quando os dados atingem um limite específico (ex: um valor estático ou agregação como SOMA ou MÉDIA)

Apache Spark: Motor de processamento distribuído de código aberto que alimenta clusters de computação e SQL warehouses no Databricks

Arquitetura Medalhão (Medallion Architecture): Padrão de design de dados que organiza o lakehouse em camadas (Bronze, Silver e Gold) para o refinamento progressivo da qualidade e estrutura dos dados

Auto Loader: Ferramenta escalonável para ingestão incremental e idempotente de arquivos do armazenamento de objetos em nuvem (S3, Azure Blob) para o lakehouse


## B
Bronze (Camada): Primeira camada da arquitetura medalhão; armazena dados brutos vindos de sistemas externos "como estão", servindo como arquivo histórico e fonte de auditoria


## C
Catalog Explorer: Interface de usuário para descobrir, gerenciar e conceder permissões sobre ativos de dados e IA registrados no Unity Catalog

Clustering Líquido (Liquid Clustering): Técnica de otimização que simplifica a disposição dos dados e melhora o desempenho das consultas sem a necessidade de particionamento manual

Cluster de Computação: Grupo de recursos de computação que executam as cargas de trabalho do Spark, como notebooks e jobs


## D
Data DataFrame: Coleção distribuída de dados organizados em colunas nomeadas, disponível em APIs para Python (PySpark), SQL, R e Scala

Data Intelligence Platform: Evolução da plataforma lakehouse que utiliza IA generativa para entender a semântica dos dados, otimizar desempenho e facilitar a assistência em linguagem natural

Data Lakehouse: Arquitetura que unifica os melhores elementos de data lakes (escala e suporte a dados não estruturados) e data warehouses (performance e transações ACID)

Delta Lake: Camada de armazenamento otimizada de código aberto que fornece a base para tabelas no lakehouse, garantindo transações ACID e manipulação escalonável de metadados


## G
Genie Code: Assistente de IA para desenvolvedores e técnicos; gera código, constrói pipelines, depura erros e oferece sugestões automáticas (Quick fix) em notebooks e editores SQL

Genie Spaces: Interface de chat em linguagem natural voltada para domínios específicos de negócio, permitindo que usuários façam perguntas e recebam respostas baseadas em dados sem saber SQL

Gold (Camada): Camada final da arquitetura medalhão; contém dados curados, agregados e prontos para o consumo por ferramentas de BI e aplicações de IA


## L
Lakebase Postgres: Banco de dados de processamento de transações online (OLTP) totalmente gerenciado e integrado ao ambiente do lakehouse

LakeFlow: Solução de engenharia de dados unificada de ponta a ponta que engloba ingestão (Connect), transformação (Spark/Designer) e orquestração (Jobs)

Linhagem de Dados (Lineage): Rastreamento automático do fluxo e transformação dos dados, desde a origem até o dashboard final


## M
Metric Views: Implementação de semântica de negócios no Unity Catalog que separa a definição da métrica (ex: soma da receita) dos campos usados para agrupamento ou filtragem


## O
Objeto Protegível (Securable Object): Qualquer entidade no Unity Catalog (tabela, volume, função, etc.) na qual permissões podem ser concedidas a usuários ou grupos


## P
Photon: Mecanismo de consulta vetorizada nativo de alto desempenho integrado ao Databricks Runtime para acelerar cargas de trabalho SQL e Spark

PySpark: API de interface para o Apache Spark em Python, permitindo o uso da linguagem para processamento distribuído


## S
Schema Evolution (Evolução de Esquema): Capacidade do Delta Lake de atualizar o esquema de uma tabela de forma automática ou manual sem a necessidade de sobrescrever dados existentes

Silver (Camada): Camada intermediária da arquitetura medalhão; fornece uma "visão corporativa" com dados limpos, padronizados e integrados vindos da camada Bronze

Spark Connect: Arquitetura que separa o cliente do servidor no Spark, facilitando o desenvolvimento remoto e integrações com IDEs

Streaming Table: Tabela Delta otimizada para o processamento de dados incrementais ou de transmissão (streaming) com baixa latência


## T
Time Travel (Viagem no Tempo): Recurso do Delta Lake que utiliza o log de transações para consultar versões históricas dos dados ou restaurar estados anteriores


## U
Unity Catalog: Camada de governança unificada integrada para gerenciar segurança, linhagem, controle de acesso e auditoria de todos os ativos de dados e IA


## V
Vacuum: Comando utilizado para remover arquivos de dados obsoletos que não são mais referenciados pelo log de transações, reduzindo custos de armazenamento

View Materializada: Visualização cujos resultados são pré-calculados e armazenados em cache para garantir acesso mais rápido e eficiente em pipelines
