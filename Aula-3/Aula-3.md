# A T I V I D A D E

## História 1 - Avaliação do pedido

Como cliente, quero avaliar o pedido depois da entrega, para ajudar outros clientes a escolherem melhor.

Dado que o pedido foi entregue, quando o cliente abre o app, então aparece a opção de avaliar o pedido.

Dado que o cliente avalia com nota e comentário, quando confirma o envio, então a avaliação aparece no perfil do restaurante.

### Requisitos não funcionais

**1. Eficiência de desempenho**

Depois que o cliente confirmar a avaliação, ela deverá aparecer no perfil do restaurante em até 2 segundos, em 95% dos casos.

**2. Confiabilidade**

Caso ocorra uma falha de conexão durante o envio da avaliação, o sistema não deverá cadastrar a mesma avaliação mais de uma vez quando a conexão voltar.

**3. Segurança**

Somente o cliente responsável pelo pedido entregue poderá fazer uma avaliação referente àquele pedido.




## História 2 - Salvar cartão de pagamento

Como cliente, quero salvar um cartão de pagamento, para não digitar os dados a cada compra.

Dado que o cliente cadastra um cartão válido, quando confirma o cadastro, então o cartão fica disponível para escolha no checkout.

Dado que o cliente tem um cartão salvo, quando faz um novo pedido, então pode selecionar esse cartão sem redigitar os dados.

### Requisitos não funcionais

**1. Segurança**

Depois que o cartão for salvo, o sistema deverá mostrar apenas os quatro últimos números do cartão, sem exibir os dados completos.

**2. Eficiência de desempenho**

Os cartões salvos deverão aparecer no checkout em até 2 segundos, em 95% dos acessos.

**3. Confiabilidade**

Depois que o cadastro do cartão for confirmado, ele deverá continuar disponível nas próximas compras mesmo que o cliente feche e abra o aplicativo novamente.



## História 3 - Resumo diário de vendas

Como dono de restaurante, quero ver um resumo diário de vendas, para acompanhar o desempenho do dia.

Dado que o dia comercial termina, quando o restaurante abre o painel de vendas, então vê o total de pedidos e o faturamento do dia.

Dado que o restaurante seleciona um período diferente, quando aplica o filtro, então o resumo é recalculado para aquele período.

### Requisitos não funcionais

**1. Eficiência de desempenho**

O resumo de vendas deverá carregar em até 2 segundos, em 95% dos acessos, para períodos de até 30 dias.

**2. Segurança**

Somente usuários vinculados ao restaurante poderão visualizar os dados de pedidos e faturamento daquele estabelecimento.

**3. Usabilidade**

O usuário deverá conseguir alterar o período do resumo e aplicar o filtro em no máximo três ações dentro do painel.
