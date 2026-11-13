---
product-area: betas
title: Programa Beta de recursos das organizações conectadas
description:
author: Alina
feature: Product Announcements
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 8f8f4e7962bfde525470842caecd49f03b758b29
workflow-type: tm+mt
source-wordcount: '2241'
ht-degree: 1%
---
# Programa beta de recursos de organizações conectadas

>[!IMPORTANT]
>
>O recurso Organizações conectadas está atualmente na fase beta fechada e está aberto a um pequeno número de clientes.
>
>O beta será executado até o final de 2026.
>
>Em caso de dúvidas, entre em contato com o gerente de programa beta da Adobe.

O recurso Organizações conectadas permite que uma empresa e seus parceiros colaborem no trabalho quando ambas as organizações tiverem comprado o Adobe Workfront.

Por exemplo, uma empresa cliente pode enviar uma solicitação à empresa fornecedora para que o trabalho seja feito.

Cada empresa pode continuar trabalhando em sua própria instância do Workfront, com seus próprios usuários, permissões e fluxos de trabalho.

Os objetos de trabalho são espelhados entre as duas instâncias e somente os dados que ambos os lados concordam em compartilhar são sincronizados.

O resultado é uma visualização compartilhada de solicitações, status e decisões sem logons de convidado adicionais, licenças duplicadas ou longos threads de email.

## Visão geral do fluxo de trabalho atual de várias organizações

Quando duas empresas investiram no Workfront, elas devem poder trabalhar juntas sem que uma pague duas vezes ou mude para o sistema da outra.

Atualmente, quando as duas empresas trabalham em dois sistemas separados, sua colaboração pode incluir alguns dos seguintes fluxos de trabalho:

* As solicitações e os resumos viajam por threads de email que são difíceis de seguir.

* As transferências são manuais, com pouca capacidade de auditoria.

* Trabalhar dentro do sistema de outra empresa significa logons de convidado, licenças extras ou ambos.

* Várias cópias de arquivos circulam, e ninguém tem certeza de qual é a fonte da verdade.

* O status é difícil de seguir, portanto, os gerentes de conta gastam tempo criando plataformas e programando reuniões de atualização.

## Visão geral da solução Connected organization

Quando você usa o recurso Connected organization, as duas empresas continuam a trabalhar em dois sistemas separados e sua colaboração incluirá alguns dos seguintes workflows:

* Nenhuma organização acessa um objeto na instância da outra.
* Um objeto, como uma solicitação da organização cliente, é duplicado e publicado na instância do provedor.
* Somente os metadados configurados para sincronização são mantidos atualizados entre as duas cópias.
* Cada empresa gerencia seus próprios usuários, permissões e fluxos de trabalho além desse objeto.

O princípio orientador é compartilhar o mínimo necessário para realizar o trabalho e manter tudo o mais confidencial.

<table>
<tbody>
<tr class="odd">
<td><strong>O que é compartilhado</strong></td>
<td><strong>O que permanece privado</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Resumos e detalhes da solicitação</p></li>
<li><p>Prazos e marcos acordados</p></li>
<li><p>Revisar comentários</p></li>
<li><p>Decisões de aprovação</p></li>
<li><p>Ativos finais aprovados</p></li>
</ul></td>
<td><ul>
<li><p>Relações com outros clientes ou outras agências</p></li>
<li><p>Finanças, taxas e o que é cobrado do cliente</p></li>
<li><p>Planejamento e capacidade de recursos</p></li>
<li><p>Estrutura de projeto interna, tarefas e quaisquer campos não selecionados para compartilhamento</p></li>
</ul></td>
</tr>
</tbody>
</table>

## Recursos disponíveis na versão beta

A primeira fase do programa beta permite conectar as duas instâncias e iniciar o trabalho.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Recurso** | **O que ele faz** |
| **Organizações conectadas** | Vincula as duas instâncias do Workfront entre as duas organizações. Durante a versão beta, o Adobe configura a conexão. Uma configuração de autoatendimento está sendo desenvolvida no momento. |
| **Solicitar formulários** | A empresa cliente cria um formulário de solicitação, publica-o e o compartilha com uma empresa provedora a partir das configurações de Compartilhamento do formulário. |
| **Entrada de solicitação assistida por IA** | O solicitante do cliente pode usar o recurso de preenchimento de formulário de IA para digitar um prompt e anexar arquivos em vez de preencher um formulário longo. O sistema mapeia esse conteúdo para os campos de formulário e mostra o mapeamento para revisão. O solicitante aceita o resultado e envia o formulário. |
| **Solicitações espelhadas** | A solicitação enviada aparece na área Solicitações da empresa fornecedora como uma cópia somente leitura, incluindo valores de campos personalizados. |
| **Conversão de solicitação para projeto** | O provedor converte a solicitação em um projeto e seleciona o portfólio, o programa e o modelo para iniciar o trabalho. O novo objeto na instância do provedor é vinculado de volta à solicitação original do cliente. Os pormenores do trabalho efetivo por parte do prestador não são visíveis para a empresa requerente. |
| **Comentários bidirecionais** | Os comentários sobre o pedido são visíveis de ambos os lados e chegam quase imediatamente, de modo que ambas as partes podem trabalhar para chegar a um acordo em um único lugar. |
| **Solicitar aceitação** | Quando ambos os lados concordarem, o provedor aceitará a solicitação e o cliente poderá ver que ela foi aceita. |
| **Atualizações de status de rascunho de IA** | Quando um solicitante solicita o status em um comentário, o provedor pode usar os comandos da IA para gerar uma resposta de rascunho de maneira rápida e consistente. <br> O rascunho inclui informações dos objetos conectados à solicitação, como a Data de conclusão planejada, a Condição e as horas registradas nas Horas planejadas. <br> É um resumo das informações mais importantes, não uma exportação campo a campo. Uma pessoa a revisa e edita antes de enviar uma resposta ao cliente. |

## Participe da versão beta

Fale com o gerente de programa do Adobe beta para participar do beta.

### O que pedimos aos participantes

* Participe de uma chamada de feedback semanal.

* Reserve cerca de uma hora por semana para testes práticos por conta própria. Sessões de trabalho em tempo real na chamada do são uma opção do.

* Sempre que possível, levar as perspectivas de ambos os parceiros para as reuniões.

* Identifique os ambientes do Workfront a serem conectados e provisione contas de administrador para um pequeno número de engenheiros da Adobe para que eles possam validar a conexão.

### O que queremos aprender

* O espelhamento de um objeto e a sincronização somente dos dados selecionados são o modelo de compartilhamento correto? Ele é flexível o suficiente para cada lado?

* O sequenciamento de fases está correto ou um recurso posterior deve vir antes?

* Quais pontos de contato estão faltando na colaboração?

* Como a nomeação e o mapeamento de campos devem funcionar entre as duas instâncias?

  Hoje, o formulário e a solicitação são de propriedade do cliente e o provedor os vê como somente leitura com os nomes de campo do cliente.

* O que a TI precisa para aprovar e administrar uma conexão?

## Fluxo de trabalho completo

Esta seção descreve o fluxo de trabalho para duas partes envolvidas nessa integração.

Estamos usando um fluxo de trabalho de cliente e provedor como exemplos.

O fluxo de trabalho inclui as seguintes etapas:

1. [Criar uma conexão de instância](#1-create-an-instance-connection)
1. [Confirmar a conexão](#2-acknowledge-the-connection)
1. [Compartilhar um formulário de solicitação com a organização conectada](#3-share-a-request-form-with-the-connected-organization)
1. [Envie uma solicitação](#4-submit-a-request)
1. [Revisar a solicitação e criar um projeto](#5-review-the-request-and-create-a-project)
1. [Colaborar na conversa entre empresas](#6-collaborate-in-the-cross-company-conversation)

### Antes de começar

* Você deve ser um administrador do sistema com acesso total à área **Instalação** em ambas as instâncias.
* A instância solicitante precisa do cliente exclusivo **GUID** da instância de recebimento.
* O formulário que você deseja compartilhar deve ser publicado.

### &#x200B;1. Criar uma conexão de instância

Configure o seguinte na instância solicitante (o cliente):

1. Faça logon no ambiente do cliente e vá para **Instalação** > **Conexões de instância**. A página lista todas as conexões e fica vazia se nenhuma ainda existir.
1. Clique em **Criar conexão**.
1. Na caixa **Criar conexão**, adicione o **GUID da instância de recebimento**. É um campo obrigatório.
1. (Opcional) Defina uma **Data de expiração**. A conexão para de funcionar após essa data.
1. Clique em **Criar conexão**.

   A nova conexão é exibida na lista de conexões com o status **Pendente**.
1. Selecione a nova conexão para ver seus detalhes.

   >[!TIP]
   >
   >Uma conexão pendente não compartilha nada. A instância de recebimento deve confirmá-la primeiro.


### &#x200B;2. Confirmar a conexão

Configure o seguinte na instância de recebimento (o provedor):

1. Faça logon na instância do provedor e acesse **Menu Principal** > **Instalação** > **Conexões de instância**.
1. Clique no nome para abrir a conexão da instância de recebimento. Um banner exibe a seguinte mensagem: **Uma instância deseja se conectar à sua. Escolha pelo menos um recipient elegível e reconheça a conexão. Nada é compartilhado até que você o faça.**
1. Em **Destinatários qualificados**, abra a lista **Grupos e usuários de pesquisa** e escolha quem pode receber trabalho da instância solicitante. Você pode escolher grupos e usuários individuais. <!--asking Anna K if this should be teams and users, instead of groups; it's groups in the UI-->
1. Clique em **Confirmar** para aceitar a conexão ou clique em uma das seguintes opções:

   * **Recusar** para recusar a conexão.
   * **Fechar** para deixar pendente.

   Uma mensagem &quot;Alterações salvas&quot; é exibida, e o status da conexão é alterado para **Ativo**. A lista agora mostra os recipients qualificados, a data de criação e a data de expiração.

   >[!TIP]
   >
   >**Confirmar** permanece esmaecido até que você escolha pelo menos um destinatário qualificado.

### &#x200B;3. Compartilhar um formulário de solicitação da organização solicitante

Na instância do Workfront do cliente:

1. Vá para **Menu principal** > **Solicitações** e clique em **Solicitar formulários**.
1. Abra o formulário publicado que deseja compartilhar.
1. Clique em **Compartilhar**.

   Observe as seguintes guias dentro da caixa **Compartilhar**:

   * **Compartilhamento interno**
   * **Compartilhamento público**
   * **Organizações conectadas**
1. Abra a guia **Organizações conectadas**.
1. No campo **Organização**, selecione a instância do provedor conectado.
1. No campo **Usuários e grupos**, escolha quem nessa organização pode usar o formulário. Adicione usuários e grupos.
1. Clique em **Salvar**.

Uma mensagem **Suas alterações foram salvas com êxito** confirma o compartilhamento. <!--need to submit a UI text change - remove "successfully"-->

### &#x200B;4. Envie uma solicitação

Como um usuário na instância do cliente, envie uma solicitação do fazendo o seguinte:

1. Faça logon na instância Workfront do cliente e acesse **Menu Principal** > **Solicitações**.

   A página **Enviar nova solicitação** lista formulários recentes, incluindo aquele que você acabou de compartilhar.

   Uma observação na parte superior exibe **Solicitação entre empresas: as solicitações enviadas com este formulário estão visíveis para a organização conectada.**
1. Preencha o formulário manualmente ou use **Preencher formulário** para que a IA faça isso por você.
1. (Opcional) Para usar Preencher formulário, faça o seguinte:

   1. Clique em **Preencher formulário**.
   1. Descreva sua solicitação, cole um email relacionado ou clique em **Anexar arquivos** para carregar um arquivo. A IA encontra os detalhes relevantes e os aplica ao formulário.
   1. Clique em **Aplicar ao formulário**. Uma barra de progresso mostra **Preenchendo seu formulário** enquanto os valores de campo são gerados.
   1. Para ignorar a etapa de IA, clique em **Ignorar**.
1. Revise os valores gerados e edite qualquer coisa que precise ser alterada.
1. Clique em **Enviar** para enviar a solicitação.

   Uma mensagem **Solicitação enviada com êxito** é exibida com um link **Exibir sua solicitação**.

   A nova solicitação é adicionada à lista de solicitações com o nome do formulário e um status de **Novo** na instância do cliente e do provedor.

   >[!TIP]
   >
   >As respostas da IA podem ser imprecisas. Sempre verifique novamente os valores preenchidos antes de enviar.

   A solicitação criada é somente leitura na instância do provedor.

### &#x200B;5. Revisar a solicitação e criar um projeto

1. Faça logon na instância Workfront do provedor e acesse **Menu Principal** > **Solicitações**.

A solicitação de entrada é exibida na lista.

O **Tipo** da solicitação está marcado como **Externo: &lt; nome da instância do cliente >**, que a marca como proveniente da organização conectada.

1. Abra a solicitação. Um selo **Compartilhado com: &lt; nome da instância do cliente >** é exibido ao lado do título, e o painel de comentários mostra o seguinte aviso de **Conversação entre empresas**: **Esta discussão está visível para &lt; nome da organização do cliente >.**
1. Revise as informações da solicitação e as respostas do formulário.
1. Clique no menu **Mais** à direita do nome da solicitação e, em seguida, em **Criar objeto**.
1. Na caixa de diálogo **Criar objeto**, atualize os seguintes campos:
   * **Ação**: selecione uma ação no menu. Por exemplo, **Criar um único projeto**
   * **Modelo de projeto**: selecione um modelo disponível.
   * **Proprietário do projeto**: adicione um proprietário de projeto.
   * **Módulo**: escolha um produto onde o objeto será exibido. Se você escolher **Fluxo de trabalho**, um projeto será criado na instância do provedor do Workfront.
   * **Formulários personalizados**: anexe formulários personalizados, se necessário.
   * **Portfolio** e **Programa**: adicionar portfólios ou programas para o novo projeto.
1. Clique em **Criar**.

   A solicitação na instância do provedor agora vincula ao novo projeto, e o status da solicitação muda para **Em andamento**, se o projeto estiver no status Atual. A instância solicitante do cliente vê a alteração de status em sua própria cópia da solicitação.

### &#x200B;6. Colaborar na conversa entre empresas

Os usuários em ambas as organizações podem comentar em suas respectivas solicitações. O banner de **conversa entre empresas** é um lembrete de que tudo o que foi escrito aqui está visível para a outra organização.

Siga um destes procedimentos:

1. Para solicitar uma atualização da instância do cliente:

   1. Abra a solicitação e vá para o painel **Comentários**.
   1. Clique em **Novo comentário**, digite sua mensagem e clique em **Enviar**.

1. Para atualizar a solicitação da instância do provedor:

   1. Abra a solicitação. O novo comentário está realçado com um rótulo **Novo**.
   1. Clique em **Responder**, escreva a resposta e clique em **Enviar**.

1. Para fazer o acompanhamento a partir da instância do cliente:

   1. Abra a solicitação. A resposta do provedor aparece abaixo do comentário original.
   1. Clique em **Curtir** para confirmar a confirmação ou **Adicionar resposta** para continuar a discussão.




<!--
### Client's workflow

As a requestor in the client's organization, you can do the following:  

1. Create or ask an administrator to create a request form, publish it, and share it with the connected provider's organization.

2. Open the published form from the Requests area, enter a prompt, and attach any files.

3. Review how the content maps to the form fields, accept, and submit.

### Provider's workflow

As a work manager in the provider's organization, do the following: 

1. Receive the request in your Requests area as a read-only copy.

2. Discuss the request through comments until both sides are aligned, then accept it.

3. Convert the request into a project, choosing the portfolio, program, and template, if needed.

4. Choose which project fields are mirrored back to the client's request. 

5. Answer status questions in comments, or generate a draft status update, review it, and publish to your request. It will also display on the client's original request. 

    From that point on, the request on the provider's side acts as a replica of the client's original request, so comments and agreed-upon data stay in sync.
-->

## Segurança e governança

Manter os dados de cada organização protegidos é um requisito essencial do projeto.

Uma das linhas de base que queremos que o beta estabeleça é a facilidade com que as equipes de TI e de segurança podem aprovar e administrar uma conexão entre instâncias.

Estes são os benefícios do workflow da organização conectada:

* **Nenhum acesso entre instâncias**: nenhum usuário da organização parceira é necessário em sua instância, portanto, não há logon de convidado nem licenças adicionais.

* **Compartilhamento mínimo necessário**: somente os dados configurados para sincronização são compartilhados. Todo o resto permanece na instância de origem.

* **Controles independentes**: cada organização mantém seus próprios usuários, permissões e fluxos de trabalho.

* **Escopo em nível de equipe**: as solicitações devem alcançar somente as equipes de agência configuradas para trabalhar com esse cliente, usando os controles de acesso existentes do Workfront.

## Perspectivas do roteiro

As fases abaixo descrevem nosso plano atual de desenvolvimento e versão. O sequenciamento pode mudar com base no que aprendemos durante a fase beta. Fases posteriores não são compromissos.

<table>
<tbody>
<tr class="odd">
<td><strong>Fase</strong></td>
<td><strong>Foco e recursos planejados</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Fase 1</strong></td>
<td>Instâncias do Connect e trabalho de início: formulários de solicitação, entrada assistida por IA, solicitações espelhadas, conversão do projeto, comentários e redação de status.</td>
<td>Na versão beta</td>
</tr>
<tr class="odd">
<td><strong>Fase 2</strong></td>
<td><ul>
<li><p>Revisão e aprovação usando o Quadro e a experiência unificada de revisão e aprovação</p></li>
<li><p>As revisões pendentes aparecem no Workfront ou na Estrutura, onde quer que a parte interessada trabalhe</p></li>
<li><p>As anotações permanecem vinculadas ao arquivo de trabalho para que as equipes criativas vejam o feedback em um único lugar</p></li>
</ul></td>
<td>Planejado</td>
</tr>
<tr class="even">
<td><strong>Fase 3</strong></td>
<td><ul>
<li><p>Atribuição de trabalho baseada em tarefa além das solicitações</p></li>
<li><p>Status mais automatizado, informado por campos compartilhados ou não compartilhados</p></li>
<li><p>Um novo tipo de objeto de entrega, com metadados definidos durante o resumo e herdados pelo ativo final aprovado</p></li>
<li><p>Entrega direta de ativos finais aprovados na AEM da marca, reduzindo a entrada manual de metadados</p></li>
</ul></td>
<td>Planejado</td>
</tr>
<tr class="odd">
<td><strong>Fase 4</strong></td>
<td><ul>
<li><p>Contexto compartilhado entre parceiros</p></li>
<li><p>Uso do Adobe Brand Intelligence <!--by the agency--> antes da revisão, com acesso controlado pela equipe</p></li>
<li><p>Recursos informados pelo contexto, como estimativas</p></li>
</ul></td>
<td>Longo prazo</td>
</tr>
</tbody>
</table>






<!--

Original pdf from team:

**ADOBE WORKFRONT | BETA PROGRAM**

**Agency Brand Connectors**

Product overview for beta participants

# **Overview**

Agency Brand Connectors lets a brand and its agency collaborate on work when both organizations run Adobe Workfront. Each side keeps working in its own Workfront instance, with its own users, permissions, and workflows. Work objects are mirrored between the two instances, and only the data both sides agree to share is synchronized.

The result is a shared view of requests, status, and decisions without guest logins, duplicate licenses, or long email threads.

# **The challenge this addresses**

When a brand and an agency are both invested in Workfront, they should be able to work together without either one paying twice or moving into the other's system. Today the collaboration usually looks like this:

  - Requests and briefs travel through email threads that are hard to follow.

  - Handoffs are manual, with little auditability.

  - Working inside a partner's system means guest logins, extra licenses, or both.

  - Multiple copies of files circulate, and no one is sure which is the source of truth.

  - Status is hard to see, so producers and account managers spend time building decks and scheduling update meetings.

# **How it works: the sharing model**

Neither organization accesses an object in the other's instance. Instead, an object such as a request is duplicated and published into the partner's instance, and only the metadata configured for sync is kept up to date between the two copies. Each side manages its own users, permissions, and workflows downstream of that object.

The guiding principle is to share the minimum needed to get the work done, and to keep everything else confidential.

<table>
<tbody>
<tr class="odd">
<td><strong>What is shared</strong></td>
<td><strong>What stays private</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs and request details</p></li>
<li><p>Agreed deadlines and milestones</p></li>
<li><p>Review comments</p></li>
<li><p>Approval decisions</p></li>
<li><p>Final approved assets</p></li>
</ul></td>
<td><ul>
<li><p>Relationships with other clients or other agencies</p></li>
<li><p>Financials, rates, and what is charged to the client</p></li>
<li><p>Resource planning and capacity</p></li>
<li><p>Internal project structure, tasks, and any fields not selected for sharing</p></li>
</ul></td>
</tr>
</tbody>
</table>

# **Features available in the beta**

The first phase of the beta covers connecting two instances and kicking off work.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Feature**                       | **What it does**                                                                                                                                                                                                                                                                                                                      |
| **Connected organizations**       | Links a brand instance and an agency instance. During the beta, Adobe configures the connection. A self-serve setup is being worked on.                                                                                                                                                                                               |
| **Request forms**                 | The brand creates a request form, publishes it, and shares it with a connected organization from the form's Share settings.                                                                                                                                                                                                           |
| **AI-assisted request intake**    | The requester types a prompt and attaches files instead of filling out a long form. The system maps that content to the form fields and shows the mapping for review. The requester accepts the result and submits. This uses Workfront's existing form-filling technology.                                                           |
| **Mirrored requests**             | The submitted request appears in the agency's request area as a read-only copy, including custom field values.                                                                                                                                                                                                                        |
| **Request-to-project conversion** | The agency converts the request into a project and selects the portfolio, program, and template. The new object is linked back to the request. Downstream work on the agency side is not visible to the brand.                                                                                                                        |
| **Two-way comments**              | Comments on the request are visible on both sides and arrive almost immediately, so both parties can work toward agreement in one place.                                                                                                                                                                                              |
| **Request acceptance**            | Once both sides agree, the agency accepts the request and the brand sees that it has been accepted.                                                                                                                                                                                                                                   |
| **AI-drafted status updates**     | When a brand asks for status in a comment, the agency can use a slash command to generate a draft reply. The draft draws on connected objects, such as planned completion date, condition, and hours logged against hours planned. It is a summary, not a field-by-field export, and a person reviews and edits it before publishing. |

# **End-to-end workflow**

## **Brand side**

1.  Create a request form, publish it, and share it with the connected agency.

2.  Open the published form, enter a prompt, and attach any files.

3.  Review how the content maps to the form fields, accept, and submit.

## **Agency side**

1.  Receive the request in the request area as a read-only copy.

2.  Discuss the request through comments until both sides are aligned, then accept it.

3.  Convert the request into a project, choosing the portfolio, program, and template.

4.  Choose which project data is mirrored back to the brand.

5.  Answer status questions in comments, or generate a draft status update, review it, and publish.

From that point on, the request on the agency side acts as a replica of the request on the brand side, so comments and agreed data stay in step.

# **Security and governance**

Keeping each organization's data protected is a core design requirement, and one of the baselines we want the beta to establish is how easily IT and security teams can approve and administer a connection between instances.

  - **No cross-instance access.** No users from the partner organization are needed in your instance, so there are no guest logins and no additional licenses.

  - **Minimum necessary sharing.** Only the data configured for sync is shared. Everything else stays in the originating instance.

  - **Independent controls.** Each organization keeps its own users, permissions, and workflows.

  - **Team-level scoping.** Requests are intended to reach only the agency teams set up to work on that brand, using existing Workfront access controls.

# **Roadmap**

The phases below describe our current plan. Sequencing may change based on what we learn in the beta, and later phases are not commitments.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Focus and planned capabilities</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Connect instances and kick off work: request forms, AI-assisted intake, mirrored requests, project conversion, comments, and status drafting.</td>
<td>In beta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Review and approval using Frame and the unified review and approval experience</p></li>
<li><p>Pending reviews appear in Workfront or Frame, wherever the stakeholder works</p></li>
<li><p>Annotations stay tied to the working file so creative teams see feedback in one place</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Task-based work assignment in addition to requests</p></li>
<li><p>More automated status, informed by shared or unshared fields</p></li>
<li><p>A new deliverable object type, with metadata defined during briefing and inherited by the final approved asset</p></li>
<li><p>Direct delivery of approved final assets into the brand's AEM, reducing manual metadata entry</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Shared context between brand and agency</p></li>
<li><p>Use of Adobe Brand Intelligence by the agency before review, with access controlled by team</p></li>
<li><p>Context-informed capabilities such as estimating</p></li>
</ul></td>
<td>Longer term</td>
</tr>
</tbody>
</table>

# **Participating in the beta**

## **What we ask of participants**

  - Join a weekly feedback call.

  - Set aside about one hour per week for hands-on testing. Live working sessions on the call are an option if time is tight.

  - Bring both the brand and the agency perspective where possible.

  - Identify the Workfront environments to connect, and provision admin accounts for a small number of Adobe engineers so they can validate the connection.

## **What we want to learn**

  - Is mirroring an object and syncing only selected data the right sharing model, and is it flexible enough for each side?

  - Is the phase sequencing right, or should a later capability come sooner?

  - What touchpoints are missing from the collaboration?

  - How should field naming and mapping work between brand and agency instances? Today, the form and request are owned by the brand, and the agency sees them read-only with the brand's field names.

  - What does IT need to approve and administer a connection?

The beta runs through the end of the year. For questions or blockers, contact your Adobe beta program manager.


-->