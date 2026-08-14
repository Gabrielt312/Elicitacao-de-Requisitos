# A T I V I D A D E
**Making History** 

> Você é PO de um aplicativo de delivery de comida. Chegaram até você três necessidades vagas.

1. | O usuário precisa acompanhar o pedido depois de fazer a compra.

2. | O restaurante precisa avisar quando um item do cardápio fica indisponível.

3. | O entregador precisa reportar um problema durante a entrega.

Para cada uma das três, escreva uma história de usuário, com o INVEST em mente, e três critérios de
aceitação no formato Dado, Quando, Então. Após escrever as histórias e os critérios, ordene as tarefas
usando o MoSCow.


# Historia 1 - Acompanhamento do pedido | Must Have
Dado que o pedido foi aprovado,
quando o cliente acessar a tela de acompanhamento,
então poderá visualizar o status pedido.

Dado que o restaurante atualizou a etapa do pedido,
quando essa atualização for registrada,
então o novo status deverá ser exibido ao cliente.

Dado que o pedido saiu para entrega,
quando o cliente abrir o acompanhamento,
então deverá visualizar a previsão de entrega.

# História 2 — Item indisponível | Must Have

Dado que o restaurante está acessando o cardápio,
quando marcar um item como indisponível,
então o item não deverá mais permitir novas compras.

Dado que um item está indisponível,
quando o cliente visualizar o cardápio,
então o aplicativo deverá informar que o item está indisponível.

Dado que o restaurante voltou a ter o item disponível,
quando alterar seu status para disponível,
então o item deverá voltar a permitir a compra.

# História 3 — Problema durante a entrega | Should Have

Dado que o entregador está em uma entrega,
quando selecionar a opção “Reportar problema”,
então deverá visualizar uma lista dos tipos de ocorrências.

Dado que o entregador selecionou o tipo do problema e informou os detalhes,
quando confirmar o envio,
então a ocorrência deverá ser registrada e vinculada ao pedido.

Dado que a ocorrência foi registrada com sucesso,
quando o envio for concluído,
então o entregador deverá receber uma confirmação e as orientações para prosseguir.


# Priorização MoSCoW

**Could Have** Melhorias futuras: Notificações automáticas, mapa em tempo real, envio de fotos e chat com o suporte.

**Won’t Have agora** Funcionalidades avançadas: Previsões inteligentes e resolução automática de ocorrências ficam fora da primeira versão.