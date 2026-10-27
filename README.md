## Portfólio de Análise de Dados — Relatórios Power BI

Projeto de análise de dados de ponta a ponta: modelagem, tratamento e visualização de indicadores de negócio em cinco frentes — Marketing, Comercial, Recursos Humanos, Logística e Financeiro. Cada relatório foi construído a partir de dados brutos, com definição de KPIs, limpeza de base e publicação de dashboards interativos.

🎯 Objetivo
Transformar bases operacionais em painéis de decisão, respondendo a perguntas de negócio específicas de cada área e reduzindo a dependência de planilhas manuais para o acompanhamento de indicadores.

🛠 Ferramentas e técnicas
Power BI (modelagem, DAX, publicação) · Power Query (ETL e limpeza) · Excel/CSV como fonte de dados · Git/GitHub para versionamento do portfólio.

Modelagem em esquema estrela quando aplicável, medidas DAX para indicadores calculados e segmentações para análise por período, área e perfil.

📁 Projetos
Análise de Marketing
Relatório: 
Visão Cliente / Comportamento / Pontos de Venda

Análise da base de clientes e do comportamento de compra, com três visões: perfil do cliente, comportamento e desempenho por ponto de venda.

Indicadores: total de clientes por escolaridade · total de clientes por estado civil · distribuição por país · comportamento de consumo por perfil.

Resultado: [ex.: identificação dos segmentos de maior ticket para direcionamento de campanha] · [ex.: X% da base concentrada em N perfis, direcionando a comunicação].

 Análise Comercial
Relatório: 
abrir dashboard

Indicadores: [receita por período/vendedor] · [meta vs. realizado] · [ranking de produtos] · [taxa de conversão].

Resultado: [ex.: painel passou a mostrar diariamente o atingimento de meta, permitindo ação corretiva dentro do mês].

 Análise de Recursos Humanos
Relatório: 
abrir dashboard

Indicadores: total de funcionários · salário médio · total de funcionários por função · envolvimento no trabalho (baixo, médio, alto, ruim) · disponibilidade para hora extra · distribuição por gênero.

Resultado: [ex.: mapeamento dos setores com maior índice de desengajamento, embasando ação de retenção].

 Análise de Logística
Relatório: 
abrir dashboard

Indicadores: [OTIF / prazo de entrega] · [custo de frete] · [volume por região ou centro de distribuição] · [lead time].

Resultado: [ex.: visibilidade do atraso por rota, reduzindo prazo de entrega em X%].

Dados Financeiros
Relatório: 
abrir dashboard

Indicadores: [receita vs. despesa] · [margem] · [fluxo de caixa] · [variação mês a mês].

Resultado: [ex.: identificação dos centros de custo que puxavam a margem para baixo].

Detecção de Anomalias
A análise buscou identificar transações com padrão atípico em uma base histórica de transações bancárias, tratando o problema como detecção de fraude. Foi aplicado um modelo de detecção de anomalias — o score vai de 0 a 1, e quanto mais alto, mais atípico o registro — sobre 2,53 mil transações. O modelo classificou 1,9% da base como anomalia (cerca de 50 transações) e 98,1% como normal.

O resultado mais relevante é a separação clara entre os dois grupos. As transações marcadas como anômalas têm score médio de 0,65, contra 0,59 das normais, e o maior score da base chega a 0,75. O boxplot confirma que não é sobreposição: a caixa das anômalas fica bem acima da das normais, com mediana em torno de 0,675 contra 0,60. A distribuição do score mostra concentração massiva entre 0,58 e 0,61 — ou seja, a maior parte da base é homogênea, e as anomalias se destacam justamente na cauda direita da curva, onde há pouquíssimos registros.

A leitura de negócio: o modelo conseguiu isolar um grupo pequeno e bem definido de transações fora do padrão, o que permite direcionar a investigação humana para cerca de 2% da base em vez de revisar tudo. Numa operação de antifraude, isso é o ganho real — reduz o esforço de análise e aumenta a chance de pegar o caso relevante. A limitação é o volume absoluto: com apenas ~50 registros classificados como anomalia, cada falso positivo custa caro em proporção, o que recomenda calibrar o threshold do score com a área de negócio antes de usar em decisão real — e não tratar o resultado como veredito, mas como fila priorizada de investigação.

📈 Metodologia de trabalho
Entendimento do negócio — definição das perguntas e dos indicadores antes de montar qualquer visual.
Tratamento de dados — limpeza, padronização de tipos e categorias e consolidação das fontes no Power Query.
Modelagem — relacionamentos, tabela calendário e medidas DAX para os KPIs.
Visualização — layout com hierarquia de informação, segmentações e navegação entre visões.
Validação — conferência dos totais contra a base de origem ([ex.: redução de X% de inconsistências identificadas]).
Publicação — relatórios interativos disponíveis publicamente, com atualização [diária/semanal/mensal].
🔍 O que os projetos demonstram
Tratamento de dados de diferentes domínios (pessoas, vendas, operações e finanças), tradução de regra de negócio em medida DAX, capacidade de construir visão executiva por segmentação e entrega de um padrão visual consistente entre cinco relatórios.

🧩 Competências aplicadas
Power BI · DAX · Power Query · modelagem dimensional · ETL · análise exploratória · definição de KPIs · storytelling com dados.

👤 Sobre
Vincius Vieira Nogueira — analista de dados. Contato: viniciusvnogueira@hotmail.com
