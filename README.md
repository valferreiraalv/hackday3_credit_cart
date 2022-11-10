# Hackday3_credit_cart_limit
Projeto de data science de classificação de clientes para aumento de limite de cartão de crédito, realizado na terceira edição do Hackday, promovida pela Comunidade DS.

# Contexto 
O Billion Bank é um banco digital brasileiro, fundado em 2021. Trabalha hoje com contas digitais, e cartões de crédito.

Quando um cliente solicita aumento de limite no cartão de crédito, o banco consulta uma empresa de crédito terceira, que retorna uma recomendação: "negar" ou "conceder". Essa resposta é repassada ao cliente.

Dado que a empresa de crédito precisa levantar maiores informações de histórico financeiro do cliente com terceiros, o retorno da recomendação ao banco leva até 5 dias úteis!

Tratando-se de um serviço, a cada solicitação de aumento de limite feita por um cliente, o banco tem um custo adicional de consulta. Visando reduzir este custo, em 2022, o banco passou a só aceitar novos pedidos de aumento de limite a cada 3 meses.

O banco viu um aumento leve do churn no primeiro semestre, que se acentuou mais no segundo, chegando a um ponto já preocupante. O time de CS fez contato com antigos clientes, e constatou que o principal motivo do churn foi a percepção de burocracia relacionada ao aumento nos limites.

Para reverter o cenário, o banco traçou um plano de ação com dois objetivos:
1 - Desburocratizar o processo, permitindo que o cliente possa solicitar um novo limite uma vez por semana, tendo uma resposta instantânea.
2 - Desativar as consultas de recomendação de aumento de limites feitas hoje com a empresa terceira, que são demoradas e custosas.

Para concretizar o plano, foi solicitado ao time de cientistas de dados, que com base no histórico de recomendações ("negar" ou "conceder") da empresa de crédito, aliado ao histórico financeiro dos clientes, desenvolvam um modelo de avaliação de aumento de limite de cartão de crédito dentro de casa.

O modelo de classificação, deve informar se o Billion Bank deve "negar" ou "conceder" o aumento no limite solicitado pelo cliente.

# Questão de Negócio
Desenvolver um modelo de avaliação de limite de cartão de crédito com base no histórico de recomendações ("negar" ou "conceder") da empresa de crédito, aliado ao histórico financeiro dos clientes, para evitar que o banco dependa de terceiros para atender as solicitações e assim, reduzir o churn por esse motivo. 


# Entendimento do Negócio 
O Bilion Bank precisa atender as solicitações de aumento de limite de crédito com agilidade para seus clientes e segurança para o banco. Além disso, pretende reduzir o custo de consultas adicionais por cliente e a burocracia relacionada a cada processo. 
Para atender a demanda será necessário utilizar o histórico de recomendações ("negar" ou "conceder") da empresa de crédito, aliado ao histórico financeiro dos clientes e desenvolver um modelo de avaliação de aumento de limite de cartão de crédito pela própria instituição. 

# Dados 
- id_cliente
- idade	
- saldo_atual	
- divida_atual	
- renda_anual	
- valor_em_investimentos	
- taxa_utilizacao_credito	
- num_emprestimos	
- num_contas_bancarias	
- num_cartoes_credito	
- dias_atraso_dt_venc	
- num_pgtos_atrasados	
- num_consultas_credito	
- taxa_juros	
- investe_exterior	
- pessoa_polit_exp	
- limite_adicional

# Hipóteses 
<b>H1 - Clientes com maior idade tem menor pagamentos em atraso</b>
- Hipótese é falsa, pois os clientes mais velhos apresentam alto número de pagamentos em atraso.

<b>H2 - Clientes mais novos recebem mais negativas de limite adicional</b>
- Hipótese falsa, pois clientes mais velhos também recebem negativas de limite adicional.

<b>H3 - Clientes com maior investimento possuem menor dias de atraso</b>
- Hipótese falsa porque mesmo com maior investimento, clientes apresentam maior dias de atraso

<b>H4 - Clientes com menor número de empréstimos possuem maior renda anual</b>
- Hipótese verdadeira, pois clientes com maior renda anual, apresentam menor número de empréstimos.

<b>H5 - Clientes com maior solicitação de limite de crédito possuem maior dívida</b>
- Hipótese verdadeira, pois clientes que possuem maior dívida são aqueles que solicitam maior crédito.

# Etapas de Solução 
- [Notebook](https://github.com/valferreiraalv/hackday3_credit_cart/blob/main/notebook/hackday3_credit_card.ipynb)

<b>1. Análise Descritiva dos Dados</b>

<b>2. Engenharia de Atributos</b>

<b>3. Análise Exploratória de Dados</b>

<b>4. Preparação dos Dados</b>

<b>5. Seleção de Atributos</b>

<b>6. Treinamento de Modelos de Machine Learning</b>

<b>7. Submissão</b>

# Considerações

# Referências 
Disponível em: https://www.kaggle.com/competitions/cdshackdays3/leaderboard


