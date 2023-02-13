---
product-area: projects
navigation-topic: manage-issues
title: Copiar problemas
description: Você pode copiar um problema ou uma solicitação e salvá-los no mesmo projeto ou em outro. Também é possível copiar um problema de uma tarefa para outro projeto.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 1%

---

# Copiar problemas

Você pode copiar um problema ou uma solicitação e salvá-los no mesmo projeto ou em outro. Também é possível copiar um problema de uma tarefa para outro projeto.

Você pode copiar problemas dos seguintes objetos:

* De um projeto para o mesmo projeto (duplique no mesmo projeto)
* De uma tarefa para a mesma tarefa (duplicar se na mesma tarefa)
* De um projeto para outro
* De uma tarefa a um projeto

>[!TIP]
>
>&quot;Problemas&quot; e &quot;solicitações&quot; são usadas alternadamente no Workfront. Você pode registrar problemas em projetos e tarefas para indicar trabalhos imprevistos que precisam ser abordados. Também é possível enviar solicitações registradas como problemas em um projeto designado como Fila de solicitações.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> <p>Revise uma licença ou licença superior para copiar um problema na seção Problemas de um projeto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Editar acesso a problemas</p> <p>Visualizar ou aumentar o acesso a Projetos e Tarefas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a problemas no Nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para o problema</p> <p>Contribua com permissões para o item para o qual você está copiando o problema com a capacidade de adicionar problemas.</p> <p> Para obter informações sobre a concessão de permissões para problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a></p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações para problemas associados a documentos ou filas de solicitações

Considere o seguinte ao copiar problemas que contêm documentos ou que estão associados a uma fila de solicitações:

* **Quando um problema é associado a uma fila de solicitações:** Ao copiar um problema para outro objeto e o problema estiver associado a uma fila de solicitações, o problema copiado não será mais associado à fila original do qual o primeiro problema foi originado.
* **Quando um documento é anexado ao problema:** Ao copiar um problema para outro objeto e o problema tiver um documento anexado a ele, o documento e suas versões também serão movidos para o novo problema. As provas ou aprovações associadas ao documento não são movidas.
* **Quando um problema é vinculado a um documento ou uma pasta:** Ao copiar um problema que tenha documentos ou pastas vinculados a um serviço de terceiros, como o Google Drive, os links para os documentos são transferidos para o problema copiado. 

## Copiar problemas em uma lista

É possível copiar um ou vários problemas de uma lista de problemas ou de um relatório de problemas.

1. Vá para o projeto que contém o problema ou os problemas que deseja copiar.

   Ou

   Vá para um relatório de problema.

1. Se você selecionou ir para um projeto, clique em **Problemas** no painel esquerdo.
1. Selecione o problema ou problemas que deseja copiar e clique no botão **Menu Mais** na parte superior da lista de problemas, em seguida, clique em **Copiar para**.

   ![](assets/copy-issue-in-list-nwe-350x169.png)

1. Continue copiando o problema, conforme descrito na seção [Copiar um único problema](#copy-a-single-issue) a partir da Etapa 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:&nbsp;ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## Copiar um único problema {#copy-a-single-issue}

Você pode copiar um problema ao exibi-lo.

1. Vá para um problema que deseja copiar e clique no link **Mais** menu ![](assets/more-icon.png) à direita do nome da ocorrência, em seguida **Copiar** a.

   ![](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   O **Problema de cópia** será exibida.

   ![](assets/copy-issue-box-nwe-350x285.png)

1. No **Selecionar projeto de destino** , especifique o nome do projeto no qual deseja copiar os problemas. O nome do projeto atual é exibido por padrão.

   >[!TIP]
   >
   >Somente 100 projetos são exibidos na lista.

1. (Condicional) Clique em **solicitar acesso** se você não tiver acesso para copiar problemas para o projeto.
1. (Condicional) Continue copiando o problema para o projeto de destino selecionado sem solicitar acesso se tiver acesso para adicionar problemas a uma das tarefas no projeto de destino.

   ![](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Mensagens semelhantes são exibidas se o projeto selecionado estiver com aprovação pendente, concluído ou inativo, quando o administrador do Workfront impede a adição de problemas a esses projetos. Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Opcional) Na seção **Opções** desmarque qualquer um dos itens listados na tabela abaixo para removê-los do novo problema. Todas as opções são selecionadas por padrão.

   >[!NOTE]
   Isso afeta apenas os problemas copiados, não os problemas originais.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Atribuições</td> 
      <td>Remove usuários, funções de trabalho ou equipes atribuídas ao problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progresso</td> 
      <td>Remove a porcentagem concluída, se houver, do problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td><span style="line-height: 1.5;">Remove tudo na guia documentos, incluindo versões de documentos, documentos vinculados e pastas.</span> <br>Por padrão, provas e aprovações de documentos não podem ser copiadas para outro problema.</td> 
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
      <td>Remove as informações do formulário personalizado sobre o problema, bem como as informações sobre os formulários personalizados associados a Documentos anexados ao problema, se também forem copiados com o problema. Os formulários personalizados permanecerão anexados às questões e aos documentos, mas as informações sobre os formulários não serão repassadas para a nova edição. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Na seção **Selecionar tarefa** selecione a tarefa na qual deseja mover o problema.
1. Clique em **Copiar problema** ou **Copiar problemas** se você selecionou vários problemas em uma lista.

   Os problemas copiados são adicionados ao projeto especificado.

 
