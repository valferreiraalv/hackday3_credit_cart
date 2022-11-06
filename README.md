# hackday3_credit_cart
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
