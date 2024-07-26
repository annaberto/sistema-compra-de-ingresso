## Sistema de Compra de Ingressos

Este desenho esquemático representa a estrutura de software de compras de ingressos para o festival Rock in Rio. O esquema se propõe a projetar uma estrutura para vendas de ingressos que lida com a alta demanda de pedidos, garantindo a integridade dos dados e das transações.

Neste esquema, os processos foram separados em algumas etapas. A entrada na fila representa a solicitação de um usuário para a compra de ingressos. Em seguida, é verificada a disponibilidade do ingresso e a requisição é processada. Este é um dos pontos mais sensíveis do sistema, pois essa requisição deve ser capaz de trazer dados íntegros sobre a disponibilidade de ingressos, para que não haja nenhuma compra indevida. Após a verificação de disponibilidade dos ingressos, a reserva temporária é realizada, para que em um prazo definido a reserva possa ser totalmente efetivada. Caso não haja disponibilidade, o usuário é encaminhado novamente à fila para que possa consultar se houve alguma desistência no sistema e a disponibilidade de um novo ingresso. Após a reserva temporária, o usuário é encaminhado para o fluxo de pagamento. Em caso de sucesso no pagamento, a confirmação do ingresso é realizada e uma notificação é enviada ao usuário. Caso o pagamento não seja feito com sucesso, o usuário tem a chance de retornar à fila para que uma nova tentativa seja feita.



![Diagrama sem nome drawio](https://github.com/user-attachments/assets/0bd8900d-dfbf-4084-8795-3e26905557a9)
