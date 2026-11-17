# ATIVIDADE - AULA 8

## Processo: Atendimento de RMA (devolução de produto com defeito)

**Arquivos:** `Aula-8.bpmn` (modelo BPMN 2.0) e `Aula-8.svg` (imagem do diagrama).

### Piscinas e raias

- **Piscina Cliente:** solicita o RMA, envia o produto e recebe a decisão.
- **Piscina MULTCABOS (RMA):** duas raias.
  - **Atendimento:** registra o chamado, faz a triagem, decide se há defeito, emite a nota de devolução e notifica o cliente.
  - **Laboratório:** analisa o defeito e registra o laudo.

### Eventos de início e de fim

- Início: "Defeito identificado" (Cliente) e "Solicitação recebida" (mensagem, MULTCABOS).
- Fim: "Atendimento encerrado" (Cliente) e "RMA concluído" (MULTCABOS).

### Tarefas

Solicitar RMA, Enviar produto, Receber decisão, Registrar chamado, Receber produto, Triar produto, Recusar garantia, Emitir nota de devolução, Notificar cliente, Analisar defeito, Registrar laudo.

### Gateways

- **Exclusivo (X):** "Defeito confirmado?". Sim segue para a análise no laboratório. Não segue para a recusa da garantia.
- **Paralelo (+):** abre dois caminhos ao mesmo tempo, a emissão da nota de devolução e o registro do laudo. O segundo `+` espera os dois terminarem antes de notificar o cliente.

### Mensagens entre piscinas

- Cliente envia a solicitação de RMA ao Atendimento.
- Cliente envia o produto para o recebimento do Atendimento.
- Atendimento notifica o cliente sobre a decisão.
