---
product-area: projects
navigation-topic: convert-issues
title: Desvincular problemas de seus Objetos de resolução
description: Ao criar um projeto ou uma tarefa convertendo um problema em um projeto ou tarefa, você tem a opção de manter o problema original. O administrador do Adobe Workfront deve habilitar essa preferência para que você tenha essa opção durante a conversão do problema. Para obter mais informações sobre a conversão de problemas em projetos e tarefas, consulte Visão geral da conversão de problemas no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Desvincular problemas de seus Objetos de resolução

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

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Visualizar acesso a tarefas e projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no problema</p> <p>Exibir permissões na tarefa ou no projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Desvincular um problema de um projeto, tarefa ou problema

1. Vá para o problema que está vinculado a um projeto, tarefa ou problema.
1. Clique na seção **Detalhes do problema**.
1. Vá para a área **Visão geral** da seção **Detalhes do Problema**.
1. No campo **Resolvido por**, remova o tipo de objeto que pode ser resolvido.\
   Um problema pode ser resolvido por um projeto, tarefa ou problema.

   Isso remove o objeto de resolução do problema.

1. Clique em **Salvar** **Alterações**.\
   O problema não está mais vinculado a um projeto, tarefa ou problema, e agora você pode resolvê-lo independentemente.
