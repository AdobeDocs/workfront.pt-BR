---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar atualizações do sistema
description: O Workfront gera atualizações automáticas do sistema no [!UICONTROL Atualizações] para registrar as alterações que os usuários executam no objeto. Como um [!DNL Workfront] administrador, você pode configurar quais campos de objeto e ações [!DNL Workfront] rastreia para registrar atualizações do sistema.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 7%

---

# Configurar atualizações do sistema

[!DNL Adobe Workfront] O gera atualizações automáticas do sistema no [!UICONTROL Atualizações] para registrar os seguintes eventos:

* Alterações feitas pelos usuários em um campo de objeto
* Ações executadas por usuários em um objeto

Essas atualizações do sistema incluem o seguinte tipo de informação:

* A alteração que foi feita
* O nome do usuário que fez a alteração
* A hora e a data da alteração

Para obter mais informações sobre atualizações do sistema, consulte [Atualizações rastreadas pelo sistema](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Como um [!DNL Workfront] administrador, você pode configurar quais campos de objeto e ações [!DNL Workfront] rastreia para registrar atualizações do sistema.

Por exemplo, você pode ter [!DNL Workfront] rastrear todas as alterações que os usuários fazem nos nomes dos problemas no sistema. Qualquer alteração no nome do problema aparece como uma atualização do sistema no [!UICONTROL Atualizações] área.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Determinar quais campos [!DNL Workfront] rastreia um tipo de objeto

Você pode determinar quais informações [!DNL Workfront] rastreia quando os usuários alteram as informações associadas a um determinado tipo de objeto em todo o [!DNL Workfront] interface. Para fazer isso, adicione ou remova os campos desejados [!DNL Workfront] para rastrear esse tipo de objeto.

>[!NOTE]
>
>* [!DNL Workfront] não é possível rastrear e registrar atualizações sobre campos personalizados calculados.
>* Você pode personalizar a atualização do sistema para projetos, tarefas, problemas, portfólios, programas e usuários. Não é possível personalizar a atualização do sistema para modelos, documentos ou folhas de horas, mas [!DNL Workfront] O registra atualizações do sistema para esses objetos.
>



* [Adicione os campos desejados [!DNL Workfront] para rastrear](#add-fields-you-want-workfront-to-track)
* [Remova os campos que você não quer rastrear](#remove-fields-that-you-don-t-want-tracked)

### Adicione os campos desejados [!DNL Workfront] para rastrear {#add-fields-you-want-workfront-to-track}

É possível adicionar os campos desejados [!DNL Workfront] para rastrear um tipo específico de objeto em todo o [!DNL Workfront] interface. Quando os usuários alteram as informações nesse campo, [!DNL Workfront] registra informações sobre a alteração como uma atualização do sistema na [!UICONTROL Atualizações] para o objeto.

>[!NOTE]
>
>É possível rastrear até 300 campos incorporados e personalizados nos feeds de atualização. Se você estiver rastreando o número máximo de campos e quiser rastrear campos adicionais que não são exibidos no [!UICONTROL Todos os campos] Subguia, é necessário remover primeiro alguns dos campos rastreados para rastrear novos campos. Para obter mais informações sobre como remover campos dos campos de atualização, consulte [Remova os campos que você não quer rastrear](#remove-fields-that-you-don-t-want-tracked).

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel à esquerda, clique em **[!UICONTROL Interface]** > **[!UICONTROL Feeds de atualização]**.

1. &#x200B;Clique **[!UICONTROL Adicionar campos]** e, em seguida, clique no objeto que você deseja rastrear.

1. No &#x200B; **[!UICONTROL Feeds de atualização]** que for exibida, comece digitando um campo incorporado (padrão) ou um campo personalizado para o objeto e, em seguida, clique nele para selecioná-lo quando ele aparecer na lista.

   Se [!DNL Workfront] já estiver rastreando o campo, não será possível adicioná-lo uma segunda vez na lista.

1. Depois de adicionar todos os campos desejados [!DNL Workfront] para rastrear, clique em **[!UICONTROL Adicionar campos]**.

   Os campos integrados adicionados aparecem abaixo de **[!UICONTROL Campos predefinidos]** subguia.

   Os campos personalizados adicionados são exibidos na **[!UICONTROL Campos personalizados]** subguia.

   A variável **[!UICONTROL Todos os campos]** A subguia mostra os campos integrados e personalizados que estão sendo rastreados.

### Remova os campos que você não quer rastrear {#remove-fields-that-you-don-t-want-tracked}

Você pode remover campos que não deseja que o sistema rastreie para um tipo específico de objeto em toda a [!DNL Workfront] interface.

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Interface]** > **[!UICONTROL Feeds de atualização]**.

1. No **[!UICONTROL Campos rastreados]** , selecione a **[!UICONTROL Todos os campos]** subguia.

   Isso mostra os campos incorporados e personalizados que estão sendo rastreados no momento.

1. Selecione o campo que deseja interromper o rastreamento e clique em **[!UICONTROL Remover]**.

1. No **[!UICONTROL Remover campo]** for exibida, clique em **[!UICONTROL Sim, remova]** para confirmar.

Quaisquer atualizações sobre os campos rastreados anteriormente são preservadas na [!UICONTROL Atualizações] área onde foram registrados.

## Determinar quais ações [!DNL Workfront] rastreia um tipo de objeto

Você pode ter [!DNL Workfront] rastrear as seguintes ações que os usuários podem executar nos objetos em toda a [!DNL Workfront] interface.

Por exemplo, você pode ter [!DNL Workfront] registre uma atualização sempre que um usuário alterar uma atribuição para uma tarefa ou problema. A alteração aparece como uma atualização do sistema no [!UICONTROL Atualizações] para a tarefa ou problema.

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
   <td>Registro de cobrança criado ou excluído</td> 
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

Para configurar as ações desejadas [!DNL Workfront] para rastrear:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Interface]** > **[!UICONTROL Feeds de atualização]**.

1. Clique em **[!UICONTROL Ações]** guia.

1. Selecione uma ação para habilitá-la ou desmarque uma ação para desabilitá-la.
1. Clique em **[!UICONTROL Salvar]**.

Quando você desativa uma ação, qualquer atualização gravada anteriormente sobre essa ação é preservada na [!UICONTROL Atualizações] área onde foi registrado.
