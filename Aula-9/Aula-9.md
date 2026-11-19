# ATIVIDADE - AULA 9

## Sistema: Sistema de chamados de TI

**Arquivos:** `Aula-9.drawio` (diagrama de casos de uso), `Aula-9.svg` (imagem do diagrama) e este arquivo, com a especificação do caso de uso Abrir chamado.

### Diagrama de casos de uso

- **Fronteira:** Sistema de chamados de TI.
- **Casos de uso:** Abrir chamado, Acompanhar chamado, Confirmar solução, Atender chamado e Registrar solução.
- **Atores principais:** Colaborador e Técnico de suporte.
- **Ator secundário:** «sistema» Inventário de TI.
- **Associações:** o Colaborador participa de Abrir chamado, Acompanhar chamado e Confirmar solução. O Técnico de suporte participa de Atender chamado e Registrar solução. O Inventário de TI participa de Abrir chamado e Registrar solução.

### Especificação do caso de uso: Abrir chamado

| Campo | Descrição |
| --- | --- |
| **Caso de uso** | Abrir chamado |
| **Ator principal** | Colaborador |
| **Ator secundário** | Inventário de TI (sistema) |
| **Descrição** | O colaborador descreve um problema de equipamento, sistema, acesso ou rede e envia o chamado para a equipe de suporte atender. |
| **Gatilho** | O colaborador tem um problema que atrapalha o seu trabalho e precisa da ajuda da TI. |
| **Pré-condição** | O colaborador entrou no sistema com o seu usuário da rede. |
| **Pós-condição** | O chamado fica registrado com número e prioridade, aguardando atendimento, e os técnicos de suporte são avisados. |

#### Fluxo principal

1. O colaborador pede para abrir um novo chamado.
2. O sistema mostra as categorias: equipamento, sistema, acesso e rede.
3. O colaborador escolhe a categoria, descreve o problema e informa o número de patrimônio do equipamento.
4. O sistema confere se a descrição foi preenchida e busca o equipamento no inventário de TI.
5. O sistema define a prioridade e mostra um resumo do chamado com o prazo de atendimento.
6. O colaborador confirma o chamado.
7. O sistema registra o chamado, mostra o número e avisa os técnicos de suporte.

#### Fluxo alternativo: abrir chamado para um colega

**Quando.** No passo 3, o problema é no equipamento de outro colaborador.

**Passos.**

1. O colaborador informa o usuário do colega.
2. O sistema busca o colega e mostra os equipamentos dele.
3. O colaborador escolhe o equipamento e descreve o problema.

**Retorno.** O fluxo volta ao passo 4.

#### Exceções

##### Equipamento não encontrado

**Quando.** No passo 4, o número de patrimônio não existe no inventário de TI.

**Passos.**

1. O sistema avisa que não encontrou o equipamento e mostra onde fica a etiqueta de patrimônio.
2. O colaborador corrige o número ou segue sem informar o equipamento.

**Retorno.** O fluxo volta ao passo 4.

##### Desistência

**Quando.** Antes do passo 6, o colaborador desiste.

**Passos.**

1. O colaborador cancela o chamado.
2. O sistema descarta o chamado.

**Retorno.** O caso de uso termina sem registrar o chamado.
