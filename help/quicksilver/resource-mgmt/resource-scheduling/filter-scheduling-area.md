---
product-area: resource-management
navigation-topic: resource-scheduling
title: Filtrar informações na área Agendamento
description: Usar um filtro na área Agendamento de Recursos permite determinar quais itens de trabalho são exibidos na linha do tempo do agendamento. Isso inclui quais tarefas e problemas são exibidos na área Não atribuído, bem como quais usuários são exibidos.
author: Alina
feature: Resource Management
exl-id: 974b2515-ed10-459d-a317-36e62c52afc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2452'
ht-degree: 0%

---

# Filtrar informações na área Agendamento

>[!IMPORTANT]
>  
><span class="preview">A funcionalidade de Agendamento descrita neste artigo foi descontinuada e removida do Adobe Workfront a partir da versão 23.1 em janeiro de 2023.   </span>
>  
> <span class="preview"> Este artigo também será removido logo após a versão 23.1, no início de 2023. Nesse momento, recomendamos que você atualize todos os marcadores adequadamente. </span>
> 
><span class="preview"> Agora você pode usar o Balanceador de Carga de Trabalho para agendar o trabalho de seus recursos. </span>
>  
> <span class="preview">Para obter informações sobre como programar recursos usando o Balanceador de Carga de Trabalho, consulte a seção [O Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<p>(SEVERAL SECTIONS BELOW LINKED TO THE PRODUCT. SEE NOTES</p>
-->

Usar um filtro na área Agendamento de Recursos permite determinar quais itens de trabalho são exibidos na linha do tempo do agendamento. Isso inclui quais tarefas e problemas são exibidos na área Não atribuído, bem como quais usuários são exibidos.

Antes de começar a filtrar o conteúdo conforme descrito nesta seção, familiarize-se com o funcionamento do agendamento de recursos no Adobe Workfront.\
Para obter informações sobre a programação de recursos no Workfront, consulte o artigo [Introdução ao Agendamento de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).\
Para obter mais informações sobre a linha do tempo de agendamento, consulte o artigo [Introdução ao Agendamento de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Você pode programar recursos ou uma equipe individual da qual é membro ou para quaisquer projetos para os quais é o Gerenciador de Recursos.

## Requisitos de acesso

Você deve ter o seguinte:

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
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Exibir o acesso ou superior a Projetos, Tarefas e Problemas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores a projetos, tarefas e problemas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

<!--
<p>(NOTE: sections below - LINKED TO THE ui. DO NOT RENAME/ DELETE)</p>
-->

## Criar um filtro na seção Agendamento (para equipes)

As tarefas e os problemas dos projetos, usuários e funções definidos no filtro são exibidos na linha do tempo de agendamento na guia Trabalhando. Use as opções no filtro para determinar quais projetos, usuários e funções são representados na linha do tempo do agendamento.

>[!NOTE]
>
>Não é possível salvar um filtro na guia Trabalhar em (para um grupo). Quando você atualiza a página ou navega para fora, o filtro reverte para as configurações padrão.

Para criar um filtro para a linha do tempo de agendamento na guia Trabalhar em equipes:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Equipes**, selecione um grupo, clique em **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.
1. Clique em **Filtro**.
1. Determine quais projetos são representados na área Não atribuído especificando as seguintes informações:

   <!--
   <p>(NOTE: Alina: there was a note that [This step is linked to from the context-sensitive help] but I could not find from where in the UI it is linked.)&nbsp;</p>
   -->

   * **Prioridades do projeto:** Selecione a prioridade dos projetos que você deseja representar na linha do tempo do agendamento. Tarefas e problemas de projetos com as prioridades selecionadas são exibidos na linha do tempo do agendamento.\
      Somente as prioridades de projetos que incluem tarefas ou problemas atribuídos à equipe estão disponíveis para escolha neste menu.
   * **Status do projeto:** Selecione o status dos projetos que você deseja representar na linha do tempo de programação. Tarefas e problemas de projetos com os status selecionados são exibidos na linha do tempo de agendamento.\
      Somente os status de projetos que incluem tarefas ou problemas atribuídos à equipe estão disponíveis para escolha neste menu.
   * **Projetos:** Selecione os projetos que deseja representar na linha do tempo de programação. Tarefas e problemas dos projetos selecionados são exibidos na linha do tempo do agendamento.\
      Suas seleções nos campos anteriores determinam os projetos que estão disponíveis para seleção.\
      Somente os projetos que incluem tarefas ou problemas atribuídos à equipe estão disponíveis para escolha neste menu.

1. Determine quais usuários são exibidos na linha do tempo do agendamento especificando as seguintes informações. Por padrão, todos os membros da equipe são exibidos.

   <!--
   <p>(NOTE: this step is linked in the UI.)</p>
   -->

   * **Funções:** Selecione as funções que deseja representar na linha do tempo de programação.\
      Somente as tarefas atribuídas a essa função são exibidas na área Não atribuído. Somente os usuários com as funções selecionadas que possam receber essas tarefas são exibidos.\
      Os usuários são exibidos na linha do tempo de agendamento, organizada por função de cargo.
   * **Usuários:** Selecione os usuários individuais que você deseja representar na linha do tempo do agendamento.\
      Somente os usuários selecionados são exibidos, independentemente de terem uma atribuição de função que corresponda à atribuição de função de tarefas na área Não atribuído.\
      Essa opção não afeta quais tarefas e problemas são exibidos na área Não atribuído.

      <!--   
     <p>(NOTE: Alina: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])</p>   
     -->

1. (Opcional) Para fazer modificações adicionais na linha do tempo do agendamento (como alterar o intervalo de datas) e fazer modificações em atribuições de usuários, consulte o artigo [Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

<!--
<p>(NOTE: below - LINKED TO THE UI, DO NOT RENAME/ DELETE/ CHANGE)</p>
-->

## Criar e modificar filtros na seção Agendamento (para vários projetos)

Você pode criar um novo filtro, aplicar um filtro criado anteriormente, modificar um filtro criado anteriormente ou excluir um filtro. Não é possível compartilhar filtros criados com outros usuários.

* [Crie um filtro na seção Agendamento (para projetos)](#create-a-filter-in-the-scheduling-section-for-projects)
* [Aplicar um filtro salvo](#apply-a-saved-filter)
* [Modificar um filtro salvo](#modify-a-saved-filter)
* [Excluir um filtro salvo](#delete-a-saved-filter)

### Crie um filtro na seção Agendamento (para projetos) {#create-a-filter-in-the-scheduling-section-for-projects}

<!--
<p>(NOTE: *****LINKED TO THE PRODUCT FROM THE GLOBAL SCHEDULER >> BOTH THE FIRST AND THE SECOND AREAS) </p>
-->

As tarefas e os problemas dos projetos, usuários e funções definidos no filtro são exibidos na linha do tempo de agendamento na guia Agendamento . Use as opções no filtro para determinar quais projetos, usuários e funções são representados na linha do tempo do agendamento.

Para criar um filtro para a linha do tempo de agendamento na guia Agendamento para vários projetos:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
1. Clique em **Filtro**.\
   ![](assets/scheduling-filter-350x351.png)

1. Deixe o **Filtros salvos** campo em branco.
1. Determine quais projetos são representados na área Não atribuído especificando as seguintes informações:

   <!--
   <p>(NOTE: Alina: this step is linked in the UI.) </p>
   -->

   * **Portfolio:** Selecione os portfólios que incluem programas e projetos que você deseja representar na linha do tempo de programação.

      Somente os programas nos portfólios selecionados estão disponíveis para seleção na **Programa** campo.

   * **Programas:** Selecione quaisquer programas que incluam projetos que você deseja que sejam representados na linha do tempo do agendamento.\
      Suas seleções na **Portfolio** determinam os programas disponíveis para seleção.\
      Somente os projetos dos programas selecionados estão disponíveis para seleção no **Projetos** campo.

   * **Prioridades do projeto:** Selecione a prioridade dos projetos que você deseja representar na linha do tempo do agendamento.\
      Somente os projetos com as prioridades selecionadas são representados.

   * **Status do projeto:** Selecione o status dos projetos que você deseja representar na linha do tempo de programação.\
      Somente os projetos com os status selecionados são representados.

   * **Empresas de projeto:** Tarefas e problemas são exibidos na linha do tempo de agendamento somente quando pertencem a um projeto que corresponde a uma empresa selecionada.

   * **Grupos de projetos:** Tarefas e problemas são exibidos na linha do tempo de agendamento somente quando pertencem a um projeto que corresponde a um grupo selecionado por você.

   * **Projetos:** Selecione os projetos que deseja representar na linha do tempo de programação. Tarefas e problemas dos projetos selecionados são exibidos na linha do tempo do agendamento.\
      Suas seleções nos campos anteriores determinam os projetos que estão disponíveis para seleção.\
      Tarefas e problemas dos projetos selecionados são exibidos na linha do tempo do agendamento. Somente os projetos que incluem tarefas ou problemas atribuídos à equipe estão disponíveis para escolha neste menu.

1. Determine quais usuários são exibidos na linha do tempo do agendamento especificando as seguintes informações: (Por padrão, somente os usuários qualificados para receber uma tarefa ou um problema da área Não atribuído são exibidos. Quando você seleciona usuários individuais, os usuários são exibidos na linha do tempo de agendamento independentemente de estarem qualificados para receber uma tarefa ou um problema da área Não atribuído). 

   <!--
   <p>(NOTE: Alina: this step had a note that it is linked in the UI but I could not find from where.) </p>
   -->

   * **Empresas do usuário:** Este campo permite que você restrinja usuários de outras empresas à exibição na linha do tempo de programação.\
      Deixe esse campo em branco caso deseje que os usuários de qualquer empresa sejam adicionados. Se você especificar empresas individuais, somente os usuários dessas empresas poderão ser adicionados à linha do tempo de programação. Especificar uma empresa não adiciona automaticamente usuários dessa empresa à linha do tempo de agendamento. Em vez disso, use os campos abaixo para adicionar usuários específicos.\
      Essa opção não afeta quais tarefas e problemas são exibidos na área Não atribuído.****

   * **Grupos de usuários:** Todos os usuários de qualquer grupo de usuários especificado são exibidos na linha do tempo de agendamento.

   * **Equipes:** Todos os usuários de qualquer equipe especificada são exibidos na linha do tempo do agendamento.\
      Essa opção não afeta quais tarefas e problemas são exibidos na área Não atribuído.

   * **Funções:** Selecione as funções que deseja representar na linha do tempo de programação.\
      Somente as tarefas atribuídas a essa função são exibidas na área Não atribuído. Somente os usuários com as funções selecionadas que possam receber essas tarefas são exibidos.\
      Os usuários são exibidos na linha do tempo de agendamento, organizada por função de cargo.

   * **Usuários:** Selecione os usuários individuais que você deseja representar na linha do tempo do agendamento.\
      Somente os usuários selecionados são exibidos, independentemente de terem uma atribuição de função que corresponda à atribuição de função de tarefas na área Não atribuído.\
      Essa opção não afeta quais tarefas e problemas são exibidos na área Não atribuído.
   <!--
   <p>NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->

1. Clique em **Salvar novo filtro**.\
   Seus dados são exibidos na linha do tempo do agendamento.

1. (Opcional) Para fazer modificações adicionais na linha do tempo do agendamento (como alterar o intervalo de datas) e fazer modificações em atribuições de usuários, consulte o artigo [Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Aplicar um filtro salvo {#apply-a-saved-filter}

>[!NOTE]
>
>Essa opção se aplica somente ao agendar recursos para vários projetos (na guia Scheduling ); não é possível aplicar um filtro salvo ao agendar recursos para uma equipe (na guia Trabalhar em ) ou ao agendar recursos para um único projeto (na guia Pessoal ).

Você pode aplicar um filtro criado anteriormente.

Para aplicar um filtro salvo para vários projetos:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
1. Clique em **Filtro**.
1. No **Filtros salvos** selecione o filtro que deseja aplicar.\
   Seus dados são exibidos na linha do tempo do agendamento.

1. (Opcional) Para fazer modificações adicionais na linha do tempo do agendamento (como alterar o intervalo de datas) e fazer modificações em atribuições de usuários, consulte o artigo [Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Modificar um filtro salvo {#modify-a-saved-filter}

>[!NOTE]
>
>Essa opção se aplica somente ao agendar recursos para vários projetos (na guia Scheduling ); não é possível modificar um filtro salvo ao agendar recursos para uma equipe (na guia Trabalho em ) ou ao agendar recursos para um único projeto (na guia Pessoal ).

Você pode modificar um filtro criado anteriormente.

Para modificar um filtro salvo para vários projetos:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
1. Clique em **Filtro**.
1. No **Filtros salvos** selecione o filtro que deseja modificar na lista suspensa.
1. Especifique quais dados serão exibidos na linha do tempo do agendamento.
1. Clique em **Salvar**.\
   Seus dados são exibidos na linha do tempo do agendamento.

1. (Opcional) Para fazer modificações adicionais na linha do tempo do agendamento (como alterar o intervalo de datas) e fazer modificações em atribuições de usuários, consulte o artigo [Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Excluir um filtro salvo {#delete-a-saved-filter}

>[!NOTE]
Essa opção se aplica somente ao agendar recursos para vários projetos (na guia Scheduling ); não é possível excluir um filtro salvo ao agendar recursos para uma equipe (na guia Trabalho em ) ou ao agendar recursos para um único projeto (na guia Pessoal ).

Você pode excluir um filtro criado anteriormente.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
1. Clique em **Filtro**.
1. No **Filtros salvos** , na lista suspensa, clique no (x) ao lado do filtro que deseja excluir. 

## Criar e modificar filtros na seção Agendamento (para um único projeto)

<!--
<p>(NOTE: **** LINKED FROM THE PRODUCT FROM THE PROJECT> STAFFING> SCHEDULING AREA) </p>
-->

Tarefas e problemas dos usuários, equipes e funções definidas no filtro são exibidos na linha do tempo de agendamento na guia Pessoal. Use as opções no filtro para determinar quais usuários, equipes e funções são representadas na linha do tempo do agendamento.

>[!NOTE]
Não é possível salvar um filtro na guia Pessoal (para um único projeto). Quando você atualiza a página ou navega para fora, o filtro reverte para as configurações padrão.

Para criar um filtro para a linha do tempo de agendamento na guia Pessoal de um único projeto:

1. Vá para um projeto e clique no botão **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.
1. Determine quais usuários são exibidos na linha do tempo do agendamento especificando as seguintes informações: (Por padrão, somente os usuários qualificados para receber uma tarefa ou um problema da área Não atribuído são exibidos. Quando você seleciona usuários individuais, os usuários são exibidos na linha do tempo de agendamento independentemente de estarem qualificados para receber uma tarefa ou um problema da área Não atribuído). 

   <!--
   <p><span>(NOTE: Alina: [This step is linked to from the context-sensitive help]) </span> </p>
   -->

   * **Empresas do usuário:** Este campo permite que você restrinja usuários de outras empresas à exibição na linha do tempo de programação.\
      Deixe esse campo em branco caso deseje que os usuários de qualquer empresa sejam adicionados. Se você especificar empresas individuais, somente os usuários dessas empresas poderão ser adicionados à linha do tempo de programação. Especificar uma empresa não adiciona automaticamente usuários dessa empresa à linha do tempo de agendamento. Em vez disso, use os campos abaixo para adicionar usuários específicos.\
      Essa opção não afeta quais tarefas e problemas são exibidos na área Não atribuído.

   * **Grupos de usuários:** Todos os usuários de qualquer grupo de usuários especificado são exibidos na linha do tempo de agendamento.

   * **Equipes:** Todos os usuários de qualquer equipe especificada são exibidos na linha do tempo do agendamento.\
      Essa opção não afeta quais tarefas e problemas são exibidos na área Não atribuído.

   * **Funções:** Selecione as funções que deseja representar na linha do tempo de programação.\
      Somente as tarefas atribuídas a essa função são exibidas na área Não atribuído. Somente os usuários com as funções selecionadas que possam receber essas tarefas são exibidos.\
      Os usuários são exibidos na linha do tempo de agendamento, organizada por função de cargo.

   * **Usuários:** Selecione os usuários individuais que você deseja representar na linha do tempo do agendamento.\
      Somente os usuários selecionados são exibidos, independentemente de terem uma atribuição de função que corresponda à atribuição de função de tarefas na área Não atribuído.\
      Essa opção não afeta quais tarefas e problemas são exibidos na área Não atribuído.
   <!--
   <p>(NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->
