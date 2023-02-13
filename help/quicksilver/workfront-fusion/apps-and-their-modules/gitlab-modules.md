---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do GitLab
description: O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion além de uma licença da Adobe Workfront.
author: Becky
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: d55ddd97a69f00a1f42d84dc55a12d2017855776
workflow-type: tm+mt
source-wordcount: '4370'
ht-degree: 0%

---


# [!UICONTROL GitLab] módulos

O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion além de uma licença da Adobe Workfront.

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!UICONTROL GitLab], bem como conectá-lo a vários aplicativos e serviços de terceiros.

>[!NOTE]
>
>Este artigo espera alguma familiaridade com a documentação da API e do [!DNL GitLab] em geral.

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Connect [!DNL GitLab] para [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. Em qualquer [!DNL Workfront Fusion] [!DNL Gitlab] módulo, clique em **[!UICONTROL Adicionar]** ao lado do campo de conexão.
1. Configure os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da conexão]</td> 
      <td> <p>Digite um nome para a conexão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>Insira o URL do [!DNL GitLab] instância.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access Token]</td> 
      <td><p>Insira seu [!UICONTROL Private Token] ou [!UICONTROL Personal Access Token].</p><p>Para obter informações sobre como localizar ou criar um token de acesso pessoal em [!DNL GitLab], consulte "Criar um token de acesso pessoal" em <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">Tokens de acesso pessoais</a> no [!DNL GitLab] documentação.</p></td> 
     </tr> 
    </tbody> 
   </table>


1. Clique em **[!UICONTROL Continuar]**.
1. Clique em **[!UICONTROL Autorizar]** para criar a conexão e retornar ao módulo.

## [!DNL GitLab] módulos e seus campos

Ao configurar [!DNL GitLab] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL GitLab] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

+++**[!UICONTROL Monitorar o status de criação]**

Esse módulo de acionador instantâneo inicia um cenário quando o status de uma build é alterado.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook monitore para ver as alterações de status da criação</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Assista aos comentários de commit/MR/issue/snippet]**

Esse módulo de acionador instantâneo inicia um cenário quando um comentário é feito em uma confirmação, solicitação de mesclagem, problema ou trecho de código.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook assista para comentários</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Observar compromissos (empurra)]**

Esse módulo de acionador instantâneo inicia um cenário quando uma confirmação é enviada para um repositório. Esse módulo não inicia um cenário quando uma tag é enviada.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook observe para confirmar</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Observar comentário da edição]**

Esse módulo de acionador instantâneo inicia um cenário quando um comentário é feito em um problema.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook assista para comentários de problemas</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Problemas de observação]**

Essa [!UICONTROL acionador instantâneo] O módulo inicia um cenário quando um problema é criado ou quando um problema existente é atualizado, fechado ou reaberto.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook observe para solucionar problemas</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Assista às solicitações de mesclagem]**

Esse módulo de acionador instantâneo inicia um cenário quando um dos seguintes ocorre:

* Uma nova solicitação de mesclagem é criada
* Uma solicitação de mesclagem existente é atualizada, mesclada ou fechada
* Uma confirmação é adicionada na ramificação de origem


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook observe para solicitações de mesclagem</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Observar comentários de solicitação de mesclagem]**

Esse módulo de acionador instantâneo inicia um cenário quando um comentário é feito em uma solicitação de mesclagem.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook assista para obter comentários de solicitação de mesclagem</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Monitorar o status do pipeline]**

Esse módulo de acionador instantâneo inicia um cenário quando o status de um pipeline muda.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook monitore para ver as alterações de status do pipeline</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver projetos]**

Esse módulo de acionador agendado inicia um cenário quando um novo projeto é adicionado, do qual o usuário autenticado é membro.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL GitLab] para [!DNL Workfront] Fusão, consulte <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] para [!DNL Workfront] Fusão</a> neste artigo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Máximo de Resultados</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo assista durante cada ciclo de execução de cenário.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Assistir ramificações do repositório]**

Esse módulo de acionador agendado inicia um cenário quando uma nova ramificação é adicionada a um repositório.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL GitLab] para [!DNL Workfront] Fusão, consulte <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] para [!DNL Workfront] Fusão</a> neste artigo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Máximo de Resultados</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo assista durante cada ciclo de execução de cenário.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Assista às tags de repositório]**

Esse módulo de acionador instantâneo inicia um cenário quando uma tag é criada ou excluída em um repositório.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook procure por tags</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver comentários do trecho]**

Esse módulo de acionador instantâneo inicia um cenário quando um novo comentário é feito em um trecho.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook assista para comentários</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Assista a todos]**

Este módulo de acionador agendado inicia um cenário quando uma nova tarefa é adicionada. Quando nenhum filtro é aplicado, o acionador é executado quando uma nova tarefa pendente é adicionada.

Para obter informações sobre campos, consulte [Obter uma lista de tarefas](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Assista à página wiki]**

Esse módulo de acionador instantâneo inicia um cenário quando uma página wiki é criada ou editada.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecione o webhook que deseja usar para este acionador ou adicione um novo webhook. </p><p>Para adicionar um novo webhook, <ol><li>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL webhook] .</li><li>Insira o seguinte: <ul><li>Um nome para o webhook</li><li>A conexão que você deseja usar para este webhook</li><li>O projeto que você deseja que o webhook assista para páginas wiki</li></ul></li><li>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo . </td> 
   </tr> 
   </tbody> 
</table>

+++

### Ações

+++**[!UICONTROL Aceitar solicitação de mesclagem]**

Esse módulo de ação mescla as alterações enviadas com a solicitação de mesclagem fornecida.

Para obter informações sobre campos, consulte [Aceitar solicitação de mesclagem](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Cancelar uma criação]**

Esse módulo de ação cancela uma única build de um projeto.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL GitLab] para [!DNL Workfront] Fusão, consulte <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] para [!DNL Workfront] Fusão</a> neste artigo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID do projeto]</td> 
   <td> <p>Selecione ou mapeie o projeto que contém a build que deseja cancelar.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td>Selecione ou mapeie a build que deseja cancelar.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Mesclar mensagem de confirmação]</td> 
   <td> Insira ou mapeie uma mensagem de confirmação para a mesclagem.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Deve remover a ramificação de origem]</td> 
   <td>Selecione se deseja remover a ramificação de origem quando a mesclagem estiver concluída.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Mesclar ao criar com êxito]</td> 
   <td>Selecione se deseja mesclar a solicitação de mesclagem assim que a build for concluída.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>Se estiver presente, esse SHA deverá corresponder ao HEAD da ramificação de origem. Se não corresponder, a mesclagem falhará.</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Cancelar as criações de um pipeline]**

Esse módulo de ação cancela as criações de um único pipeline.

Para obter informações sobre campos, consulte [Cancelar os trabalhos de um pipeline](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Cancelar mesclagem quando o pipeline tiver êxito]**

Se uma solicitação de mesclagem for definida para mesclar quando um pipeline tiver êxito, esse módulo de ação cancelará essa ação.

Para obter informações sobre campos, consulte [Cancelar mesclagem quando o pipeline tiver êxito](https://docs.gitlab.com/ee/api/merge_requests.html) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Cherry escolhe um compromisso]**

Essa cereja do módulo de ação escolhe uma confirmação para uma determinada ramificação.

Para obter informações sobre campos, consulte [Cherry escolhe um compromisso](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar um novo rótulo]**

Esse módulo de ação cria um novo rótulo para o repositório em questão.

Para obter informações sobre campos, consulte [Criar um novo rótulo](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar um novo pipeline]**

Esse módulo de ação cria um novo pipeline para o projeto em questão.

Para obter informações sobre campos, consulte [Criar um novo pipeline](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar uma nova versão]**

Esse módulo de ação adiciona notas de versão à tag git existente.

Para obter informações sobre campos, consulte [Criar uma versão](https://docs.gitlab.com/ee/api/releases/#create-a-release) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar uma nova tag]**

Esse módulo de ação cria uma nova tag no repositório que aponta para a referência fornecida.

Para obter informações sobre campos, consulte [Criar uma nova tag](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar uma tarefa]**

Este módulo de ação cria uma tarefa para o usuário atual sobre o problema selecionado. O usuário atual é o usuário identificado pelas credenciais na conexão usada para este módulo.

Para obter informações sobre campos, consulte [Criar um para fazer](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar uma tarefa em uma solicitação de mesclagem]**

Este módulo de ação cria uma tarefa para o usuário atual na solicitação de mesclagem selecionada. O usuário atual é o usuário identificado pelas credenciais na conexão usada para este módulo.

Para obter informações sobre campos, consulte [Criar um item a fazer](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar solicitação de mesclagem]**

Esse módulo de ação cria uma nova solicitação de mesclagem em um projeto.

Para obter informações sobre campos, consulte [Criar solicitação de mesclagem](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar novo arquivo no repositório]**

Este módulo de ação cria um novo arquivo no repositório selecionado.

Para obter informações sobre campos, consulte [Criar novo arquivo no repositório](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar nova nota de edição]**

Esse módulo de ação cria uma nota de problema para um único problema de projeto.

Para obter informações sobre campos, consulte [Criar nova nota de edição](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar nova nota de solicitação de mesclagem]**

Esse módulo de ação cria notas para uma única solicitação de mesclagem.

Para obter informações sobre campos, consulte [Criar nova nota de solicitação de mesclagem](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar um novo marco]**

Esse módulo de ação cria um novo marco para um projeto.

Para obter informações sobre campos, consulte [Criar novo marco](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar nova nota de trecho]**

Esse módulo de ação cria uma nova nota para um único trecho. Notas de trecho são comentários que os usuários podem publicar em um trecho.

Para obter informações sobre campos, consulte [Criar nova nota de trecho](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar ramificação de repositório]**

Esse módulo de ação cria uma única ramificação de repositório.

Para obter informações sobre campos, consulte [Criar ramificação de repositório](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Criar variável de compilação]**

Esse módulo de ação cria uma nova variável de build.

Para obter informações sobre campos, consulte [Criar variável](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Excluir uma solicitação de mesclagem]**

Este módulo de ação é somente para administradores e proprietários de projetos. Ele exclui a solicitação de mesclagem em questão

Para obter informações sobre campos, consulte [Excluir uma solicitação de mesclagem](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Excluir arquivo existente no repositório]**

Esse módulo de ação exclui um arquivo existente do repositório.

Para obter informações sobre campos, consulte [Excluir arquivo existente no repositório](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Excluir ramificação de repositório]**

Esse módulo de ação exclui uma ramificação do repositório.

Para obter informações sobre campos, consulte [Excluir ramificação de repositório](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Editar problema]**

Este módulo de ação atualiza um problema de projeto existente. Essa chamada também é usada para marcar um problema como fechado.

Para obter informações sobre campos, consulte [Editar problema](https://docs.gitlab.com/ee/api/issues.html#edit-issue) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Editar marco]**
Este módulo de ação atualiza um marco de projeto existente.

Para obter informações sobre campos, consulte [Editar marco](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Apagar uma criação]**

Esse módulo de ação apaga uma criação de um projeto (remove artefatos de trabalho e registro de tarefas).

Para obter informações sobre campos, consulte [Apagar uma tarefa](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter uma lista de todos]**

Este módulo de pesquisa recupera uma lista de itens a fazer.

Para obter informações sobre campos, consulte [Obter uma lista de tarefas](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter uma única build]**

Esse módulo de ação recupera um único trabalho de um projeto.

Para obter informações sobre campos, consulte [Obter um único trabalho](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter uma única tag de repositório]**

Esse módulo de ação recupera uma tag de repositório específica determinada por seu nome.

Para obter informações sobre campos, consulte [Obter uma única tag de repositório](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter uma implantação específica]**

Esse módulo de ação recupera uma implantação específica.

Para obter informações sobre campos, consulte [Obter uma implantação específica](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter todos os problemas atribuídos a um único marco]**

Este módulo de pesquisa recupera todos os problemas atribuídos a um único marco do projeto.

Para obter informações sobre campos, consulte [Obter todos os problemas atribuídos a um único marco](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter arquivo do repositório]**

Esse módulo de ação recupera informações sobre um arquivo no repositório, como nome, tamanho ou conteúdo.

Para obter informações sobre campos, consulte [Obter arquivo do repositório](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter usuários do projeto]**

Esse módulo de pesquisa recupera os usuários do projeto.

Para obter informações sobre campos, consulte [Obter usuários do projeto](https://docs.gitlab.com/ee/api/projects.html#get-project-users) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter um único problema]**

Esse módulo de ação recupera detalhes do problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para criar uma nova conexão, consulte <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] para o Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td> <p>Selecione o projeto que contém o problema sobre o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do problema]</td> 
   <td> <p>Insira ou mapeie o nome do problema sobre o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Obter nota de problema único]**

Esse módulo de ação recupera uma única nota para um problema específico do projeto.

Para obter informações sobre campos, consulte [Obter nota de problema único](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter solicitação de mesclagem única]**

Esse módulo de ação recupera informações sobre uma única solicitação de mesclagem.

Para obter informações sobre campos, consulte [Obter solicitação de mesclagem única](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter alterações de solicitação de mesclagem única]**

Esse módulo de pesquisa recupera informações sobre a solicitação de mesclagem, incluindo seus arquivos e alterações.

Para obter informações sobre campos, consulte [Obter alterações de solicitação de mesclagem única](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter compromissos de solicitação de mesclagem única]**

Esse módulo de ação recupera uma lista de confirmações de solicitação de mesclagem.

Para obter informações sobre campos, consulte [Obter compromissos de solicitação de mesclagem única](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter nota de solicitação de mesclagem única]**

Esse módulo de ação retorna uma única nota para uma determinada solicitação de mesclagem.

Para obter informações sobre campos, consulte [Obter nota de solicitação de mesclagem única](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter um marco]**

Esse módulo de ação recupera detalhes do marco.

Para obter informações sobre campos, consulte [Obter um único marco](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter projeto único]**

Este módulo de ação recupera os detalhes do projeto.

Para obter informações sobre campos, consulte [Obter projeto único](https://docs.gitlab.com/ee/api/projects.html#get-single-project) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter uma única ramificação de repositório]**

Esse módulo de ação recupera detalhes da ramificação do repositório.

Para obter informações sobre campos, consulte [Obter uma única ramificação de repositório](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter nota de trecho]**

Esse módulo recupera uma única nota para um determinado trecho.

Para obter informações sobre campos, consulte [Obter uma única nota de trecho](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter os comentários de um compromisso]**

Esse módulo de pesquisa recupera comentários de uma confirmação em um projeto.

Para obter informações sobre campos, consulte [Obter os comentários de um compromisso](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter o diferencial de um commit]**

Esse módulo de ação obtém o diferencial de uma confirmação em um projeto.

Para obter informações sobre campos, consulte [Obter o diferencial de um commit](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Manter artefatos]**

Impede que artefatos sejam excluídos quando a expiração for definida.

Para obter informações sobre campos, consulte [Manter artefatos](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar todas as notas de solicitação de mesclagem]**

Este módulo de pesquisa recupera uma lista de todas as notas para uma única solicitação de mesclagem.

Para obter informações sobre campos, consulte [Listar todas as notas de solicitação de mesclagem](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar todas as notas de trecho]**

Este módulo obtém uma lista de todas as notas para um único snippet. Notas de trecho são comentários que os usuários podem publicar em um trecho.

Para obter informações sobre campos, consulte [??](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar criações de confirmação]**

Este módulo de pesquisa retorna uma lista de builds para uma confirmação específica em um projeto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para criar uma nova conexão, consulte <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] para o Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do projeto]</td> 
   <td> <p>Selecione o projeto que contém a confirmação para a qual deseja listar as criações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escopo]</td> 
   <td> Para limitar a pesquisa a ser criada com um status específico, selecione o status . Deixar esse campo em branco retorna todas as criações da confirmação.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Listar problemas]**

Este módulo de pesquisa retorna todos os problemas pelas configurações de filtro especificadas.

Para obter informações sobre campos, consulte [Listar problemas](https://docs.gitlab.com/ee/api/issues.html#list-issues) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar problemas que fecham na mesclagem]**

Esse módulo de pesquisa recupera todos os problemas que seriam fechados ao mesclar a solicitação de mesclagem fornecida.

Para obter informações sobre campos, consulte [Listar problemas que serão fechados na mesclagem](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Rótulos de lista]**

Esse módulo de pesquisa recupera todos os rótulos no projeto.

Para obter informações sobre campos, consulte [Listar rótulos](https://docs.gitlab.com/ee/api/labels.html#list-labels) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar solicitações de mesclagem]**

Esse módulo de pesquisa recupera todas as solicitações de mesclagem pelas configurações de filtro.

Para obter informações sobre campos, consulte [Listar solicitações de mesclagem](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar projetos próprios]**

Esse módulo de pesquisa recupera projetos em que o usuário autenticado é definido como proprietário.

Para obter informações sobre campos, consulte [Listar projetos de usuários](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar criações de projeto]**

Esse módulo de pesquisa recupera uma lista de builds em um projeto.

Para obter informações sobre campos, consulte [Listar trabalhos de projeto](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar implantações de projeto]**

Este módulo de pesquisa recupera uma lista de implantações em um projeto.

Para obter informações sobre campos, consulte [Listar implantações de projeto](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar notas de problema do projeto]**

Esse módulo de pesquisa recupera uma lista de todas as notas de um único problema.

Para obter informações sobre campos, consulte [Listar notas de problema do projeto](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar problemas do projeto]**

Este módulo de pesquisa retorna todos os problemas em um projeto especificado.

Para obter informações sobre campos, consulte [Listar problemas do projeto](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar etapas do projeto]**

Esse módulo de pesquisa recupera todos os marcos do projeto.

Para obter informações sobre campos, consulte [Listar etapas do projeto](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar pipelines de projeto]**

Esse módulo de pesquisa recupera todos os pipelines do projeto.

Para obter informações sobre campos, consulte [Listar pipelines de projeto](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar tags de repositório do projeto]**

Esse módulo de pesquisa recupera uma lista de tags de repositório de um projeto, classificadas por nome em ordem alfabética reversa.

Para obter informações sobre campos, consulte [Listar tags de repositório do projeto](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar variáveis de projeto]**

Esse módulo de pesquisa recupera uma lista das variáveis de um projeto.

Para obter informações sobre campos, consulte [Listar variáveis de projeto](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar projetos]**

Esse módulo de pesquisa recupera todos os projetos dos quais o usuário autenticado é membro.

Para obter informações sobre campos, consulte [Listar todos os projetos](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar ramificações de repositório]**

Esse módulo pesquisa ramificações de repositório pelo termo de pesquisa.

Para obter informações sobre campos, consulte [Listar ramificações de repositório](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar confirmações do repositório]**

Esse módulo de pesquisa recupera uma lista de confirmações de repositório em um projeto.

Para obter informações sobre campos, consulte [Listar confirmações do repositório](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Listar colaboradores do repositório]**

Este módulo de pesquisa recupera uma lista de contribuidores do repositório.

Para obter informações sobre campos, consulte [Contribuidores](https://docs.gitlab.com/ee/api/repositories.html#contributors) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Árvore do repositório de lista]**

Esse módulo de pesquisa recupera uma lista de arquivos e diretórios de repositório em um projeto.

Para obter informações sobre campos, consulte [Árvore do repositório de lista](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Marcar um todo como feito]**

Esse módulo de ação marca um único item pendente fornecido pela ID para o usuário atual, conforme concluído.

Para obter informações sobre campos, consulte [Marcar um item para fazer como concluído](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Modificar nota de problema existente]**

Modifica uma nota existente de um problema.

Para obter informações sobre campos, consulte [Modificar nota de problema existente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Modificar nota de solicitação de mesclagem existente]**

Modifica a nota existente de uma solicitação de mesclagem.

Para obter informações sobre campos, consulte [Modificar nota de solicitação de mesclagem existente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Modificar nota de trecho existente]**

Este módulo de ação modifica uma nota existente de um trecho.

Para obter informações sobre campos, consulte [Modificar nota de trecho existente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Novo problema]**

Esse módulo de ação cria um novo problema de projeto.

Para obter informações sobre campos, consulte [Novo problema](https://www.integromat.com/en/help/app/gitlab) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Reproduzir uma criação]**

Esse módulo de ação aciona uma ação manual para iniciar uma tarefa.

Para obter informações sobre campos, consulte [Reproduzir um trabalho](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Publicar comentário para confirmação]**

Esse módulo de ação adiciona um comentário a uma confirmação.

Para obter informações sobre campos, consulte [Publicar comentário para confirmação](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Remover variável]**

Esse módulo de ação remove a variável de um projeto.

Para obter informações sobre campos, consulte [Remover variável](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Repetir uma criação]**

Este módulo de ação tenta novamente uma única build em uma confirmação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para criar uma nova conexão, consulte <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] para o Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do projeto]</td> 
   <td> <p>Selecione o projeto que contém a build que você deseja repetir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td> Selecione a build que deseja repetir. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Repetir tarefas com falha em um pipeline]**

Este módulo de ação tenta compilações com falha em um pipeline.

Para obter informações sobre campos, consulte [Repetir tarefas em um pipeline](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Obter uma variável]**

Esse módulo recupera detalhes da variável específica de um projeto.

Para obter informações sobre campos, consulte [Mostrar detalhes da variável](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Atualizar uma versão]**

Este módulo de ação atualiza uma versão.

Para obter informações sobre campos, consulte [Atualizar uma versão](https://docs.gitlab.com/ee/api/releases/#update-a-release) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Atualizar solicitação de mesclagem]**

Esse módulo de ação atualiza uma solicitação de mesclagem existente. Você pode alterar a ramificação de destino, o título ou até mesmo fechar o MR.

Para obter informações sobre campos, consulte [Atualizar solicitação de mesclagem](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) no [!DNL GitLab] documentação.

+++

+++**[!UICONTROL Atualizar uma variável]**

Esse módulo de ação atualiza a variável de um projeto.

Para obter informações sobre campos, consulte [Atualizar variável](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) no [!DNL GitLab] documentação.

+++
