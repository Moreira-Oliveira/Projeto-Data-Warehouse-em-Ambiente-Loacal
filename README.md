# Projeto-Data-Warehouse-em-Ambiente-Local

Para este projeto vamos construir um DW para uma empresa fictícia, a empresa “AlfaMaq Manufatura S.A”.

Uma empresa de manufatura é um tipo de empresa que transforma matéria-prima ou componentes em produtos acabados através do uso de processos industriais. Esse tipo de empresa é responsável por projetar, produzir, montar e testar produtos, tais como automóveis, eletrônicos, alimentos, roupas, máquinas e equipamentos.

As empresas de manufatura geralmente possuem fábricas ou instalações onde os processos produtivos ocorrem. Essas instalações podem envolver o uso de máquinas, equipamentos, ferramentas, robôs e mão-de-obra qualificada para criar produtos que atendam às especificações de qualidade e segurança.

As empresas de manufatura podem atender tanto ao mercado de consumo final quanto ao mercado empresarial, produzindo uma ampla variedade de produtos em diferentes setores. Algumas empresas de manufatura são especializadas em um único produto, enquanto outras produzem uma ampla gama de produtos em diferentes áreas.

A manufatura é uma das principais atividades econômicas em muitos países, empregando milhões de pessoas em todo o mundo. As empresas de manufatura desempenham um papel fundamental na economia, fornecendo produtos essenciais e criando empregos em várias áreas, desde a produção até a administração, vendas e marketing.

A AlfaMaq precisa gerar relatórios para melhor compreensão dos seus processos de negócio. A AlfaMaq tem os seguintes dados disponíveis:

Dados de produção: Informações sobre a produção, incluindo quantidades produzidas, tempo de produção, taxas de defeito, dados de qualidade e informações sobre matérias-primas e processos de fabricação.

Dados de vendas: Informações sobre as vendas de produtos, incluindo preços, quantidades vendidas, locais de venda e dados de clientes.
Dados de fornecedores: Informações sobre fornecedores de matérias-primas e outros insumos necessários para a produção de produtos.
Dados financeiros: Informações sobre as finanças da empresa, incluindo receita, despesas, lucro e fluxo de caixa.

Relatórios que a empresa gostaria para entender melhor o desempenho dos negócios, a eficiência da produção e as necessidades do mercado:

Relatórios de vendas: Relatórios que fornecem informações sobre as vendas por região, produto, canal de vendas e período de tempo, permitindo a empresa identificar os produtos mais vendidos, as tendências de mercado e os canais de vendas mais eficazes.

Relatórios de estoque: Relatórios que mostram informações sobre os níveis de estoque de matérias-primas, produtos em processo e produtos acabados, permitindo que a empresa gerencie seu estoque de forma mais eficiente e reduza os custos de armazenamento.

Relatórios de produção: Relatórios que mostram informações sobre a eficiência da produção, incluindo o tempo de ciclo, taxa de defeito, utilização de máquinas e outros indicadores de desempenho, permitindo que a empresa identifique áreas de melhoria e aumente a eficiência da produção.

Relatórios de manutenção: Relatórios que fornecem informações sobre as atividades de manutenção da empresa, incluindo o tempo de inatividade, manutenção preventiva e corretiva, custos de manutenção e outros indicadores de desempenho, permitindo que a empresa gerencie seus ativos de forma mais eficiente.

Relatórios financeiros: Relatórios que mostram informações financeiras, como receita, despesas, margem de lucro, fluxo de caixa e outras métricas financeiras importantes, permitindo que a empresa avalie sua saúde financeira e tome decisões informadas.

Relatórios de qualidade: Relatórios que fornecem informações sobre a qualidade dos produtos, incluindo os dados de inspeção e teste, o índice de defeito e outros indicadores de qualidade, permitindo que a empresa identifique áreas de melhoria na qualidade e tome medidas corretivas.

📚 Criação de um modelo conceitual

![Captura de tela 2024-12-29 155100](https://github.com/user-attachments/assets/f6bc094b-d8e8-4682-a2d4-7b0552cb4a5c)

![Captura de tela 2024-12-29 155113](https://github.com/user-attachments/assets/cbccf26a-4c70-411f-8c44-e3004924b3ca)

📚 Aqui estão as regras de negócio consideradas para este projeto:

![Captura de tela 2024-12-29 155411](https://github.com/user-attachments/assets/c9f38d04-ee32-422a-b3a4-50c1302ffb27)

📚 Detalhe das entidades

![Captura de tela 2024-12-29 155725](https://github.com/user-attachments/assets/76cd8e28-74c8-4501-ac77-5bdb56242721)
![Captura de tela 2024-12-29 155738](https://github.com/user-attachments/assets/36bd9e0b-4cbd-40ce-b41b-1ebf1848a67b)

Relacionamentos:

• Produto e Venda: Cada venda está associada a um produto. Um produto pode aparecer em várias vendas. Relacionamento Um Para Muitos.

• Cliente e Venda: Cada venda está associada a um cliente. Um cliente pode estar associado a várias vendas. Relacionamento Um Para Muitos.

• Canal de Venda e Venda: Cada venda está associada a um canal de venda. Um canal de venda pode estar associado a várias vendas. Relacionamento Um Para Muitos.

• Data e Venda: Cada ponto no tempo pode registrar várias vendas. Cada venda está associada a um ponto no tempo. Relacionamento Um Para Muitos.

📚 Modelo que será utilizado

![Captura de tela 2024-12-29 160935](https://github.com/user-attachments/assets/6acefbcc-09ec-487b-8663-970c90451ab1)

📚 Modelo Lógico

O modelo lógico traduz um modelo conceitual em uma estrutura que pode ser implementada em um sistema de gestão de banco de dados (SGBD). Ele detalha as tabelas, os tipos de dados de cada coluna e as relações entre essas tabelas através de chaves primárias e estrangeiras. O modelo lógico é independente de tecnologia, é como um template que poderá ser usado em qualquer SGBD.

Transformando o modelo conceitual:

![Captura de tela 2024-12-29 161404](https://github.com/user-attachments/assets/ce541e83-635c-43cc-83e1-79feba818815)

![Captura de tela 2024-12-29 161416](https://github.com/user-attachments/assets/dbf3593d-14e7-4f77-917c-8b6084e03a36)

📚 Programa utilizado

![Captura de tela 2024-12-29 145350](https://github.com/user-attachments/assets/67df7ad9-4113-4a45-851a-1e5a040421bd)

📚 Modelo Star Schema aplicado no PgAdmin

![Captura de tela 2024-12-29 163124](https://github.com/user-attachments/assets/5719049b-d888-419b-bbba-9400c6bd70b2)

📚 Construindo o Processo ETL

![Captura de tela 2024-12-29 164601](https://github.com/user-attachments/assets/6aeb9c4b-8f53-46c3-aeb1-a2472d5cc836)

![Captura de tela 2024-12-29 164619](https://github.com/user-attachments/assets/9763b6d3-901f-4bf9-b2f5-e2e412d6b4c8)

![Captura de tela 2024-12-29 164716](https://github.com/user-attachments/assets/2ff844c4-27f0-437f-a5db-28443ef44b5a)

![Captura de tela 2024-12-29 164743](https://github.com/user-attachments/assets/c7a80d33-7fdf-451a-92c5-e062325c952a)

📚 Views para os relatórios (Codigos na pasta)

Relatório de vendas por produto e canal utilizando Views:

![Captura de tela 2024-12-29 165252](https://github.com/user-attachments/assets/c93b8e66-e54c-4849-973a-f1f75deb8040)

Relatório de vendas para cada cliente em cada mês e ano:

![Captura de tela 2024-12-29 165749](https://github.com/user-attachments/assets/fab48f24-3b82-4c14-b040-e30eebf34499)

📚 Materialized Views

![Captura de tela 2024-12-29 170021](https://github.com/user-attachments/assets/2c7a2ea6-65c8-4a3d-8c74-b581aa030b88)

📚 Relatório de vendas tendo cliente e ano como parâmetro de entrada usando Functions ('João Silva', 2024) 

![Captura de tela 2024-12-29 170320](https://github.com/user-attachments/assets/a92660bf-7a03-4124-961c-ec7c15f71d3f)

📚 Criação de índices em colunas para otimizar a geração de relatórios

![Captura de tela 2024-12-29 170515](https://github.com/user-attachments/assets/21091226-3175-4055-b515-3b91dff27c17)


📚 Substituindo os dados antigos pelos novos (SCD tipo 1)

Substitui os dados antigos pelos novos, sem manter o histórico. Quando um dado é alterado, a versão anterior é sobrescrita, e apenas a versão mais recente é armazenada. Esse tipo é útil quando não há necessidade de preservar o histórico das mudanças, apenas o estado atual dos dados.

![Captura de tela 2024-12-29 171521](https://github.com/user-attachments/assets/6694987a-350a-4f21-8723-b20e6473db07)

A primeira consulta (SELECT * FROM dw.dim_cliente;) exibe os dados atuais da tabela dim_cliente.

A segunda consulta (UPDATE dw.dim_cliente) atualiza os dados de um cliente específico (ID = 1010), alterando as informações de cidade, estado e pais.

A última consulta (SELECT * FROM dw.dim_cliente;) exibe os dados atualizados da tabela dim_cliente.

Este método é utilizado quando não há necessidade de manter um histórico das alterações dos dados.

📚 Substituindo os dados antigos pelos novos mas mantendo os historicos (SCD tipo 2)

Mantém um histórico completo de mudanças ao criar uma nova linha na tabela sempre que um dado é alterado. Ele preserva todas as versões de um dado, utilizando colunas como data_inicio, data_fim ou ativo para indicar a validade de cada versão. Esse tipo de dimensão é ideal quando é necessário manter o histórico completo das alterações ao longo do tempo.

![Captura de tela 2024-12-29 172212](https://github.com/user-attachments/assets/a81da140-3ea3-4208-97f2-44657ba309d5)

📚 SCD Tipo 3. Armazena apenas a versão atual e a anterior dos dados.

O SCD Tipo 3 mantém um histórico limitado, armazenando apenas o valor atual e o valor anterior de um dado. Ele é útil quando é necessário registrar mudanças, mas sem manter um histórico completo. Em geral, o SCD Tipo 3 utiliza colunas separadas para armazenar o valor atual e o anterior, permitindo acompanhar as últimas alterações, mas com um histórico restrito.

![Captura de tela 2024-12-29 172421](https://github.com/user-attachments/assets/15081bd0-05ec-4c87-af08-7b36b49250f0)


