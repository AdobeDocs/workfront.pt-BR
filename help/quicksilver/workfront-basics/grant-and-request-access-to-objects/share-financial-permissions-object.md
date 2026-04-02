---
title: Compartilhar permissões financeiras em um objeto
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront pode conceder acesso para exibir ou editar dados financeiros ao atribuir seu nível de acesso. Para obter mais informações, consulte Conceder acesso a dados financeiros.
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 17%

---

# Compartilhar permissões financeiras em um objeto

{{highlighted-preview}}

O administrador do Adobe Workfront pode conceder acesso para exibir ou editar dados financeiros ao atribuir seu nível de acesso. Para obter mais informações, consulte [Conceder acesso a dados financeiros](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Juntamente com o nível de acesso concedido aos usuários, você também pode conceder a eles permissões para Exibir ou Gerenciar finanças de projetos, tarefas ou problemas específicos que você tenha acesso para compartilhar.

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com dados financeiros, consulte a seção [Dados financeiros](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) no artigo [Funcionalidade disponível para cada tipo de objeto](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Requisitos de acesso

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial  Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Padrão</p> 
   <p>Plano</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar ou ter maior acesso a Projetos, Tarefas, Problemas e Dados Financeiros</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões superiores para projetos, tarefas e problemas que incluam pelo menos permissões de Exibir Finanças</p>
   <p><span class="preview">Exibir permissões ou permissões superiores para projetos, tarefas e problemas que incluam pelo menos Exibir taxas de faturamento, Exibir taxas de custo ou Exibir permissões financeiras gerais</span></p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartilhar um objeto e conceder permissões financeiras

Considere o seguinte ao conceder permissões financeiras a objetos:

* Você pode conceder permissões financeiras a projetos, tarefas e problemas.
* As permissões podem ser herdadas: se você tiver permissões do View General Finance para um projeto, herdará automaticamente permissões do View General Finance para as tarefas e problemas no projeto.

Para conceder permissões financeiras a um objeto:

1. Vá para uma tarefa, projeto ou problema que você deseja compartilhar com outras pessoas.
1. Próximo ao nome do objeto, clique em **Compartilhar**.

1. No campo **Conceder acesso a `<Object name>` para**, comece digitando o nome de um usuário, equipe, função, grupo ou empresa com a qual deseja compartilhar o objeto.

   >[!TIP]
   >
   >Você pode compartilhar um objeto somente com usuários, equipes, funções ou empresas ativos.

1. Clique na lista suspensa à direita do nome do usuário e selecione uma das seguintes opções:

   * **Exibir**
   * **Contribute**
   * **Gerenciar**

1. No mesmo menu suspenso, clique no ícone opções avançadas ao lado do nível de permissão e siga um destes procedimentos:

   * Se você selecionou uma das três opções na etapa anterior, verifique se **Exibir Finanças** está selecionado.
   * Se você selecionou **Gerenciar Finanças** na etapa anterior, verifique se **Gerenciar Finanças** está selecionado.
   * <span class="preview">Para qualquer nível de permissão, selecione **Exibir taxas de cobrança**, **Exibir taxas de custo** e **Exibir finanças gerais** conforme necessário.</span>
   * <span class="preview">Somente para permissões de **Gerenciar**, selecione **Editar taxas de cobrança**, **Editar taxas de custo** e **Editar finanças gerais** conforme necessário.</span>

1. Clique em **Salvar**.

## Permissão financeira para todos os níveis de compartilhamento

A tabela a seguir mostra quais permissões financeiras os usuários obtêm ao conceder a eles permissões de Exibição, Contribute ou Gerenciar em objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Ações</strong> </th> 
   <th><strong>Gerenciar</strong> </th> 
   <th><strong>Contribute</strong> </th> 
   <th><strong>Exibir</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Gerenciar registros de cobrança</td> 
   <td>✓</td> 
   <td> <p>  </p> </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Gerenciar/visualizar taxas de custo e cobrança de função</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Gerenciar/visualizar taxas de custo e cobrança de usuário</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Exibir finanças</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr>
  <tr> 
   <td><span class="preview">Editar taxas de faturamento</span></td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td><span class="preview">Editar taxas de custo</span></td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>  
  <tr> 
   <td><span class="preview">Editar finanças gerais</span></td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>
  <tr> 
   <td><span class="preview">Exibir taxas de faturamento</span></td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td><span class="preview">Exibir taxas de custo</span></td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr>  
  <tr> 
   <td><span class="preview">Exibir finanças gerais</span></td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Exibir informações por Custo nas ferramentas de Planejamento de Recursos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Recursos de orçamento nas ferramentas de planejamento de recursos*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Exibir recursos nas ferramentas de Planejamento de recursos*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Requer acesso adicional ao Gerenciamento de Recursos.

Para obter informações sobre o acesso de Gerenciamento de Recursos, consulte [Conceder acesso ao Gerenciamento de Recursos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
