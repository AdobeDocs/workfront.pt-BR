---
product-area: projects
navigation-topic: manage-issues
title: Copiar Problemas
description: Você pode copiar um problema ou uma solicitação e salvá-los no mesmo projeto ou em outro. Você também pode copiar um problema de uma tarefa para outro projeto.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# Copiar problemas

<!--Audited: 08/2025-->

Você pode copiar um problema ou uma solicitação e salvá-los no mesmo projeto ou em outro. Você também pode copiar um problema de uma tarefa para outro projeto.

Você pode copiar ocorrências dos seguintes objetos:

* De um projeto para o mesmo projeto (duplique-o no mesmo projeto)
* De uma tarefa para a mesma tarefa (duplicar se estiver na mesma tarefa)
* De um projeto para outro projeto
* De uma tarefa para um projeto

>[!TIP]
>
>&quot;Problemas&quot; e &quot;solicitações&quot; são usados alternadamente no Workfront. Você pode registrar problemas em projetos e tarefas para indicar trabalho imprevisto que precisa ser resolvido. Você também pode enviar solicitações que são registradas como ocorrências em um projeto designado como uma Fila de solicitações.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <ul><li><p>Colaborador ou superior</p> </li>
   <li><p>Licença leve ou superior para copiar um problema na seção Problemas de um projeto</p></li></ul>
   Ou
   <ul><li><p>Solicitante ou superior</p> </li>
   <li><p>Licença de revisor ou superior para copiar um problema na seção Problemas de um projeto</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior a projetos e tarefas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> <p>Contribua com permissões para o item no qual você está copiando o problema com a capacidade de Adicionar problemas.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to copy an issue in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying the issue to with the ability to Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Considerações ao copiar problemas

### Considerações gerais ao copiar problemas

Você pode optar por copiar alguns itens associados à ocorrência para a ocorrência copiada durante o processo de cópia. No entanto, alguns itens são transferidos para o novo problema por padrão, enquanto outros não, conforme descrito nas listas abaixo.

Os seguintes itens são copiados para a nova ocorrência, por padrão:

* Contato Primário
* Formulários personalizados. As informações nos campos personalizados copiam para o novo problema somente quando você seleciona Dados personalizados no processo de cópia.
* Aprovações
* Datas de Início Planejadas e de Término Planejadas

Os seguintes objetos não são copiados para a nova ocorrência, por padrão:

* Horas registradas

### Considerações para problemas associados a documentos ou filas de solicitações

Considere o seguinte ao copiar problemas que contêm documentos ou estão associadas a uma fila de solicitações:

* **Quando um problema está associado a uma fila de solicitações:** Quando você copia um problema para outro objeto e o problema está associado a uma fila de solicitações, o problema copiado não está mais associado à fila original da qual o primeiro problema se originou.
* **Quando um documento é anexado ao problema:** Quando você copia um problema para outro objeto e o problema tem um documento anexado a ele, o documento e suas versões também são movidos para o novo problema. As provas ou aprovações associadas ao documento não são movidas.
* **Quando um problema está vinculado a um documento ou a uma pasta:** Quando você copia um problema que tem documentos ou pastas vinculados a um serviço de terceiros, como o Google Drive, os links para os documentos são transferidos para o problema copiado.

## Copiar problemas em uma lista

Você pode copiar um ou vários problemas de uma lista ou de um relatório de problemas.

1. Vá para o projeto que contém o(s) problema(s) que deseja copiar.

   Ou

   Ir para um relatório de problemas.

1. Se você optou por ir para um projeto, clique em **Problemas** no painel esquerdo.
1. Selecione o(s) problema(s) que deseja copiar e clique no **menu Mais** na parte superior da lista de problemas, depois clique em **Copiar para**.

   ![Copiar problema na lista](assets/copy-issue-in-list-nwe-350x169.png)

1. Continue copiando o problema, conforme descrito na seção [Copiar um único problema](#copy-a-single-issue), começando com a Etapa 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## Copiar um único problema {#copy-a-single-issue}

Você pode copiar um problema ao visualizá-lo.

1. Vá para um problema que você deseja copiar e clique no menu **Mais** ![Mais menu](assets/more-icon.png) à direita do nome do problema e **Copiar para**.

   ![Copiar no nível do problema](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   A caixa **Copiar Problema** é exibida.

   ![Copiar caixa de problemas](assets/copy-issue-box-nwe-350x285.png)

1. Na seção **Selecionar projeto de destino**, especifique o nome do projeto para o qual deseja copiar os problemas. O nome do projeto atual é exibido por padrão.

   >[!TIP]
   >
   >Somente 100 projetos são exibidos na lista.

1. (Condicional) Clique em **solicitar acesso** se você não tiver acesso para copiar problemas para o projeto.
1. (Condicional) Continue a copiar o problema para o projeto de destino selecionado sem solicitar acesso se tiver acesso para adicionar problemas a uma das tarefas no projeto de destino.

   ![Copiar problema e solicitar acesso](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Mensagens semelhantes serão exibidas se o projeto selecionado estiver com aprovação pendente, concluído ou inativo, quando o administrador do Workfront impedir a adição de problemas a esses projetos. Para obter mais informações, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Opcional) Na seção **Opções**, desmarque qualquer um dos itens listados na tabela abaixo para removê-los do novo problema. Todas as opções são selecionadas por padrão.

   >[!NOTE]
   >
   >Isso afetará somente os problemas copiados, não os originais.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Atribuições</td> 
      <td>Remove usuários, funções de trabalho ou equipes atribuídos ao problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progresso</td> 
      <td>Remove o percentual concluído, se houver, do problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td><span style="line-height: 1.5;">Remove tudo na guia de documentos, incluindo versões de documentos, documentos vinculados e pastas.</span> <br>Por padrão, provas e aprovações de documentos não podem ser copiadas para outro problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permissões</td> 
      <td>Remove as entidades com as quais o problema é compartilhado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atualizações</td> 
      <td>Remove comentários da seção Atualizações do problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dados personalizados</td> 
      <td>Remove as informações do formulário personalizado sobre o problema, bem como as informações nos formulários personalizados associados aos Documentos anexados ao problema, se eles também forem copiados com o problema. Os formulários personalizados permanecerão anexados aos problemas e documentos, mas as informações nos formulários não serão transferidas para o novo problema. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Na seção **Selecionar tarefa**, selecione a tarefa para onde deseja mover o problema.
1. Clique em **Copiar problema** ou **Copiar problemas** se você selecionou vários problemas em uma lista.

   Os problemas copiados são adicionados ao projeto especificado.


