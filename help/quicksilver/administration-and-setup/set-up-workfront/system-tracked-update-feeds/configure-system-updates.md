---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar atualizações do sistema
description: O Workfront gera atualizações automáticas do sistema em um objeto [!UICONTROL Atualizações] para registrar as alterações que os usuários executam no objeto. Como um [!DNL Workfront] administrador, você pode configurar quais campos e ações de objeto [!DNL Workfront] rastreia para registrar atualizações do sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 7%

---

# Configurar atualizações do sistema

[!DNL Adobe Workfront] gera atualizações automáticas do sistema em um objeto [!UICONTROL Atualizações] para registrar os seguintes eventos:

* Alterações feitas pelos usuários em um campo de objeto
* Ações executadas pelos usuários em um objeto

Essas atualizações do sistema incluem a alteração feita, o nome do usuário que fez a alteração e a hora e a data da alteração.

Como um [!DNL Workfront] administrador, você pode configurar quais campos e ações de objeto [!DNL Workfront] rastreia para registrar atualizações do sistema.

Por exemplo, você pode ter [!DNL Workfront] rastreie todas as alterações que os usuários fazem nos nomes dos problemas em todo o sistema. Qualquer alteração no nome do problema será exibida como uma atualização do sistema no [!UICONTROL Atualizações] área.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Determine quais campos [!DNL Workfront] rastreia para um tipo de objeto

Você pode determinar quais informações [!DNL Workfront] rastreia quando usuários alteram informações associadas a um determinado tipo de objeto em todo o [!DNL Workfront] interface. Para isso, adicione ou remova os campos desejados [!DNL Workfront] para rastrear esse tipo de objeto.

>[!NOTE]
>
>* [!DNL Workfront] O não pode rastrear e registrar atualizações sobre campos personalizados calculados.
>* Você pode personalizar a atualização do sistema para projetos, tarefas, problemas, portfólios, programas e usuários. Não é possível personalizar a atualização do sistema para modelos, documentos ou folhas de ponto, mas [!DNL Workfront] O registra atualizações de sistema para esses objetos.
>




* [Adicionar campos que deseja [!DNL Workfront] para rastrear](#add-fields-you-want-workfront-to-track)
* [Remover campos que você não deseja rastrear](#remove-fields-that-you-don-t-want-tracked)

### Adicionar campos que deseja [!DNL Workfront] para rastrear {#add-fields-you-want-workfront-to-track}

Você pode adicionar campos desejados [!DNL Workfront] para rastrear um tipo específico de objeto em todo o [!DNL Workfront] interface. Quando os usuários alteram informações nesse campo, [!DNL Workfront] registra informações sobre a alteração como uma atualização do sistema no [!UICONTROL Atualizações] área para o objeto.

>[!NOTE]
>
>É possível rastrear até 300 campos incorporados e personalizados nos feeds de atualização. Se você estiver rastreando o número máximo de campos e quiser rastrear campos adicionais que não são exibidos na variável [!UICONTROL Todos os campos] Subguia , primeiro remova alguns dos campos rastreados para rastrear novos campos. Para obter mais informações sobre como remover campos dos campos de atualização, consulte [Remover campos que você não deseja rastrear](#remove-fields-that-you-don-t-want-tracked).

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel à esquerda, clique em **[!UICONTROL Interface]** > **[!UICONTROL Atualizar feeds]**.

1. Clique em &#x200B; **[!UICONTROL Adicionar campos]**, em seguida, clique no objeto que deseja rastrear.

1. No &#x200B; **[!UICONTROL Atualizar feeds]** for exibida, comece a digitar um campo incorporado (padrão) ou um campo personalizado para o objeto e, em seguida, clique para selecioná-lo quando ele for exibido na lista.

   If [!DNL Workfront] já estiver rastreando o campo , não será possível adicioná-lo uma segunda vez na lista.

1. Após adicionar todos os campos desejados [!DNL Workfront] para rastrear, clique em **[!UICONTROL Adicionar campos]**.

   Os campos incorporados adicionados serão exibidos abaixo da variável **[!UICONTROL Campos incorporados]** subguia .

   Os campos personalizados que você adicionou são exibidos sob a variável **[!UICONTROL Campos personalizados]** subguia .

   O **[!UICONTROL Todos os campos]** A subguia mostra os campos incorporados e personalizados que estão sendo rastreados.

### Remover campos que você não deseja rastrear {#remove-fields-that-you-don-t-want-tracked}

Você pode remover campos que não deseja que o sistema rastreie para um tipo específico de objeto em toda a [!DNL Workfront] interface.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Interface]** > **[!UICONTROL Atualizar feeds]**.

1. No **[!UICONTROL Campos rastreados]** selecione a guia **[!UICONTROL Todos os campos]** subguia .

   Isso mostra os campos incorporados e personalizados que estão sendo rastreados no momento.

1. Selecione o campo que deseja parar de rastrear e clique em **[!UICONTROL Remover]**.

1. No **[!UICONTROL Remover campo]** for exibida, clique em **[!UICONTROL Sim, Remover]** para confirmar.

Todas as atualizações sobre os campos rastreados anteriormente são preservadas na variável [!UICONTROL Atualizações] área onde foram registrados.

## Determine quais ações [!DNL Workfront] rastreia para um tipo de objeto

Você pode ter [!DNL Workfront] rastreie as seguintes ações que os usuários podem executar em objetos em todo o [!DNL Workfront] interface.

Por exemplo, você pode ter [!DNL Workfront] registre uma atualização sempre que um usuário alterar uma atribuição para uma tarefa ou problema. A alteração é exibida como uma atualização do sistema no [!UICONTROL Atualizações] área para a tarefa ou o problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Ação</strong> </th> 
   <th><strong>Objetos</strong> </th> 
   <th><strong>Situação Primária</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>A atribuição foi alterada</td> 
   <td>Tarefas, Problemas</td> 
   <td> <p>Ativado</p> </td> 
  </tr> 
  <tr> 
   <td>A Linha de Base foi excluída</td> 
   <td>Projetos</td> 
   <td> <p>Desabilitado</p> </td> 
  </tr> 
  <tr> 
   <td>O registro de cobrança é criado ou excluído</td> 
   <td>Projetos</td> 
   <td> <p>Ativado</p> </td> 
  </tr> 
  <tr> 
   <td>Documento criado ou excluído</td> 
   <td>Projetos, tarefas, problemas, portfólios, programas</td> 
   <td> <p>Ativado</p> </td> 
  </tr> 
  <tr> 
   <td>Despesa criada ou excluída</td> 
   <td>Projetos, tarefas</td> 
   <td> <p>Ativado</p> </td> 
  </tr> 
  <tr> 
   <td>Hora registrada ou excluída</td> 
   <td>Projetos, tarefas, problemas</td> 
   <td> <p>Ativado</p> </td> 
  </tr> 
  <tr> 
   <td>Problema excluído</td> 
   <td>Projetos</td> 
   <td> <p>Ativado</p> </td> 
  </tr> 
  <tr> 
   <td>Tarefa excluída</td> 
   <td>Projetos</td> 
   <td> <p>Ativado</p> </td> 
  </tr> 
  <tr> 
   <td>O acesso de alguém foi alterado</td> 
   <td>Projetos, Tarefas, Problemas, Portfólios, Programas</td> 
   <td> <p>Ativado</p> </td> 
  </tr> 
  <tr> 
   <td>Assinar o objeto com comentário</td> 
   <td>Projetos, tarefas, problemas</td> 
   <td> <p>Ativado</p> </td> 
  </tr> 
 </tbody> 
</table>

Para configurar quais ações você deseja [!DNL Workfront] para rastrear:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Interface]** > **[!UICONTROL Atualizar feeds]**.

1. Clique no botão **[!UICONTROL Ações]** guia .

1. Selecione uma ação para ativá-la ou desmarque uma ação para desativá-la.
1. Clique em **[!UICONTROL Salvar]**.

Quando você desativa uma ação, qualquer atualização gravada anteriormente sobre essa ação é preservada na variável [!UICONTROL Atualizações] área onde foi gravada.
