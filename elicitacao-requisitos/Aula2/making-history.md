
Como Product Owner de um aplicativo de delivery de comida, foram identificadas três necessidades principais:

1. O usuário precisa acompanhar o pedido após realizar a compra.
2. O restaurante precisa informar quando um item do cardápio estiver indisponível.
3. O entregador precisa reportar problemas durante a entrega.

As histórias de usuário abaixo foram elaboradas considerando os princípios **INVEST** e os critérios de aceitação utilizando o formato **Dado, Quando, Então**.

---

## História 1 — Acompanhamento do pedido

**Como** cliente do aplicativo,
**quero** acompanhar o status do meu pedido após a compra,
**para** saber em qual etapa ele está e ter uma previsão sobre a entrega.

### Critérios de aceitação

**Critério 1**
**Dado** que o cliente realizou um pedido com sucesso,
**Quando** acessar a tela de acompanhamento,
**Então** deverá visualizar o status atual do pedido.

**Critério 2**
**Dado** que o restaurante alterou o status do pedido,
**Quando** essa alteração for registrada no sistema,
**Então** o novo status deverá ser exibido ao cliente.

**Critério 3**
**Dado** que o pedido saiu para entrega,
**Quando** o cliente acessar o acompanhamento,
**Então** deverá visualizar que o pedido está a caminho.

---

## História 2 — Item indisponível no restaurante

**Como** restaurante parceiro,
**quero** marcar um item do cardápio como indisponível,
**para** impedir que clientes façam pedidos de produtos que não podem ser preparados.

### Critérios de aceitação

**Critério 1**
**Dado** que o restaurante possui um item cadastrado no cardápio,
**Quando** marcar esse item como indisponível,
**Então** o sistema deverá atualizar a disponibilidade do produto.

**Critério 2**
**Dado** que um item está marcado como indisponível,
**Quando** o cliente visualizar o cardápio,
**Então** não deverá ser possível adicionar esse item ao pedido.

**Critério 3**
**Dado** que um item anteriormente indisponível voltou ao estoque,
**Quando** o restaurante marcá-lo novamente como disponível,
**Então** o item deverá voltar a permitir pedidos dos clientes.

---

## História 3 — Problema durante a entrega

**Como** entregador,
**quero** reportar um problema ocorrido durante uma entrega,
**para** registrar a situação e permitir que o suporte ou o restaurante tome as providências necessárias.

### Critérios de aceitação

**Critério 1**
**Dado** que o entregador está realizando uma entrega,
**Quando** selecionar a opção de reportar problema,
**Então** o sistema deverá apresentar as opções de problemas disponíveis.

**Critério 2**
**Dado** que o entregador selecionou um tipo de problema,
**Quando** confirmar o envio do reporte,
**Então** o problema deverá ser registrado e associado ao pedido.

**Critério 3**
**Dado** que um problema foi reportado com sucesso,
**Quando** o registro for concluído,
**Então** o entregador deverá receber uma confirmação na tela.

---

# Priorização — MoSCoW

A priorização das funcionalidades foi realizada utilizando a técnica **MoSCoW**.

## Must Have

Funcionalidades essenciais para o funcionamento adequado do aplicativo:

* Permitir que o cliente visualize o status atual do pedido.
* Permitir que o restaurante marque um item como indisponível.
* Impedir a compra de itens marcados como indisponíveis.
* Permitir que o entregador reporte um problema durante uma entrega.
* Associar o problema reportado ao pedido correspondente.

## Should Have

Funcionalidades importantes, mas que não impedem o funcionamento básico do sistema:

* Atualizar o status apresentado ao cliente quando o pedido mudar de etapa.
* Permitir que o restaurante torne novamente disponível um item.
* Exibir diferentes categorias de problemas para o entregador selecionar.

## Could Have

Funcionalidades que melhoram a experiência, mas podem ser implementadas posteriormente:

* Exibir uma mensagem de confirmação após o entregador reportar um problema.
* Exibir uma indicação mais detalhada de que o pedido está a caminho.
* Enviar notificações ao cliente sempre que o status do pedido mudar.

## Won't Have

Funcionalidades que não serão desenvolvidas nesta versão:

* Rastreamento em tempo real da localização exata do entregador por GPS.
* Chat em tempo real entre cliente, restaurante e entregador.
* Sugestão automática de substituição para itens indisponíveis.

---

## Considerações sobre INVEST

As histórias foram estruturadas considerando os princípios INVEST:

* **I — Independent:** cada história pode ser desenvolvida de maneira independente.
* **N — Negotiable:** os detalhes de implementação podem ser discutidos com a equipe.
* **V — Valuable:** cada história entrega valor para um usuário do sistema.
* **E — Estimable:** possuem escopo suficientemente definido para permitir estimativas.
* **S — Small:** cada história possui tamanho adequado para ser desenvolvida dentro de uma Sprint.
* **T — Testable:** os critérios de aceitação permitem verificar se as funcionalidades foram implementadas corretamente.
