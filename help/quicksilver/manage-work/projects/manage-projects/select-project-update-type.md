---
product-area: projects
navigation-topic: manage-projects
title: Selecione o tipo de atualização do projeto
description: Selecionando um Tipo de Atualização para um projeto, você pode controlar com que frequência as alterações feitas na linha do tempo do projeto são salvas nas tarefas pai ou no projeto.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Selecione o tipo de atualização do projeto

Selecionando um Tipo de Atualização para um projeto, você pode controlar com que frequência as alterações feitas na linha do tempo do projeto são salvas nas tarefas pai ou no projeto.

Quando a linha do tempo do projeto é atualizada, ela é recalculada com base nas alterações feitas no projeto, em suas tarefas ou em alterações feitas em outro projeto do qual a linha do tempo depende.

Por exemplo, as alterações a seguir nas tarefas do projeto acionam uma atualização na linha do tempo  do projeto:

* Atualizar as datas das tarefas
* Alterar relações predecessoras de tarefas
* Alterar relações pai-filho, adicionando ou removendo atribuições, além de alterar a restrição ou o tipo de duração da tarefa.

## Requisitos de acesso

<!-- drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Atualizar um tipo de atualização do projeto

Quando as tarefas são atualizadas, seus objetos principais (tarefas principais ou o projeto) são atualizados no momento indicado pelo Tipo de Atualização.  Para especificar um Tipo de Atualização para o seu projeto:

1. Vá para o projeto cujo Tipo de Atualização você deseja especificar.
1. Clique no ícone Mais ![Mais](assets/more-icon.png) do menu ao lado do nome do projeto e clique em **Editar**.

1. Clique em **Projeto** **Configurações**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. No campo **Tipo de Atualização**, selecione se deseja que o Workfront calcule a linha do tempo do projeto automaticamente diariamente, quando houver uma alteração ou se deseja que o gerente de projeto a calcule manualmente.

   Selecione entre as opções da lista abaixo. 

   >[!IMPORTANT]
   >
   >Se a linha do tempo de um projeto tiver mais de 15 anos, a Workfront não calculará a linha do tempo automaticamente ou quando houver alteração. O tipo de atualização de um projeto com mais de 15 anos é sempre manual.

   * **Automático e Mediante alteração:** Esta é a configuração padrão. A linha do tempo do projeto é atualizada sempre que ocorre uma alteração no projeto ou em outro projeto do qual a linha do tempo depende. A linha do tempo do projeto também é atualizada todas as noites. \
     Essa é a configuração recomendada, pois garante que a linha do tempo do projeto esteja sempre atualizada.

     Quando você atualiza uma tarefa ou o projeto e aciona um novo cálculo de linha do tempo, todas as datas disponíveis são exibidas imediatamente, permitindo que você continue trabalhando. Em projetos com mais de 100 tarefas, as datas que exigem cálculos mais longos ficam esmaecidas.

     ![](assets/dates-dimmed-when-insline-editing-350x146.png)

     Isso indica que o recálculo ainda não foi concluído e as datas estão sujeitas a alterações.

   * **Alterar Somente:** A linha de tempo do projeto é atualizada sempre que ocorre uma alteração no projeto ou em outro projeto do qual a linha de tempo depende; não ocorrem atualizações agendadas.\
     Você pode selecionar essa opção se estiver preocupado com o desempenho do sistema e se alterações raramente ocorrerem no projeto ou em outros projetos dos quais a linha do tempo dependa.

   * **Somente Automático:** A linha do tempo do projeto é atualizada todas as noites; ela não é atualizada imediatamente após as alterações serem feitas.\
     Você pode querer selecionar esta opção se estiver preocupado com o desempenho do sistema e se muitas alterações ocorrem a cada dia no projeto ou em outros projetos dos quais a linha do tempo depende.

     >[!NOTE]
     >
     >Um projeto não recalcula automaticamente todas as noites se estiver no status Planejamento. Ele só é recalculado quando há alteração.

   * **Somente Manual:** A linha de tempo do projeto é atualizada somente quando você seleciona a opção **Recalcular Linhas de Tempo**, conforme descrito na seção &quot;Recálculo Manual&quot; do artigo [Recalcular linhas de tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
     Você pode selecionar essa opção se estiver fazendo muitas alterações ao projeto de uma vez e quiser que o recálculo da linha do tempo ocorra após todas as alterações terem sido feitas (em vez de após cada alteração individual).

1. Clique em **Salvar**.
