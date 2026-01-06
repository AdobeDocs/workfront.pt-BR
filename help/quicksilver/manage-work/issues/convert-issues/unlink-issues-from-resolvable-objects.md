---
product-area: projects
navigation-topic: convert-issues
title: Desvincular problemas de seus objetos de resolução
description: Ao criar um projeto ou uma tarefa convertendo um problema em um projeto ou tarefa, você tem a opção de manter o problema original. O administrador do Adobe Workfront deve habilitar essa preferência para que você tenha essa opção durante a conversão do problema. Para obter mais informações sobre a conversão de problemas em projetos e tarefas, consulte Visão geral da conversão de problemas no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 3%

---

# Desvincular problemas de seus Objetos de resolução

<!--Audited: 08/2025-->

Ao criar um projeto ou uma tarefa convertendo um problema em um projeto ou tarefa, você tem a opção de manter o problema original. O administrador do Adobe Workfront deve habilitar essa preferência para que você tenha essa opção durante a conversão do problema.\
Para obter mais informações sobre a conversão de problemas em projetos e tarefas, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Quando você decide manter o problema que foi convertido para o projeto ou a tarefa, a resolução do problema é vinculada ao projeto ou à tarefa. O problema se torna o Objeto resolvível do projeto ou da tarefa. O projeto ou tarefa são os Objetos de resolução do problema.

Você também pode vincular manualmente um problema a outro problema. O segundo problema torna-se o Objeto de resolução do primeiro problema, neste caso.\
Para obter mais informações sobre Objetos de Resolução, consulte [Visão Geral de Objetos de Resolução e Resolução](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>O status do problema não pode ser alterado, pois ele muda automaticamente com o status do Objeto de resolução.

Você pode desvincular a resolução de uma ocorrência daquela de um projeto, tarefa ou ocorrência removendo o projeto, tarefa ou ocorrência da ocorrência.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <td> <p>Colaborador ou superior</p>
   <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Visualizar acesso a tarefas e projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no problema</p> <p>Exibir permissões na tarefa ou no projeto</p> </td> 
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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Desvincular um problema de um projeto, tarefa ou problema

1. Vá para o problema que está vinculado a um projeto, tarefa ou problema.
1. Clique na seção **Detalhes do problema**.
1. Vá para a área **Visão geral** da seção **Detalhes do Problema**.
1. No campo **Resolvido por**, remova o tipo de objeto que pode ser resolvido.\
   Um problema pode ser resolvido por um projeto, tarefa ou problema.

   Isso remove o objeto de resolução do problema.

1. Clique em **Salvar** **Alterações**.\
   O problema não está mais vinculado a um projeto, tarefa ou problema, e agora você pode resolvê-lo independentemente.
