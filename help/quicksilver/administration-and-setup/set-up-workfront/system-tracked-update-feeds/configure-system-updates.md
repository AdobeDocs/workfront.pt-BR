---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar atualizações do sistema
description: O Workfront gera atualizações automáticas do sistema na área [!UICONTROL Atualizações] de um objeto para registrar as alterações que os usuários executam no objeto. Como administrador do  [!DNL Workfront] você pode configurar quais campos de objeto e ações [!DNL Workfront] rastreia para registrar atualizações do sistema.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 8%

---

# Configurar atualizações do sistema

O [!DNL Adobe Workfront] gera atualizações automáticas do sistema na área [!UICONTROL Atualizações] de um objeto para registrar os seguintes eventos:

* Alterações feitas pelos usuários em um campo de objeto
* Ações executadas por usuários em um objeto

Essas atualizações do sistema incluem o seguinte tipo de informação:

* A alteração que foi feita
* O nome do usuário que fez a alteração
* A hora e a data da alteração

Para obter mais informações sobre atualizações do sistema, consulte [Atualizações rastreadas pelo sistema](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Como administrador do [!DNL Workfront], você pode configurar quais campos de objeto e ações [!DNL Workfront] rastreia para registrar atualizações do sistema.

Por exemplo, você pode fazer com que o [!DNL Workfront] rastreie todas as alterações que os usuários fazem nos nomes de problemas em todo o sistema. Qualquer alteração no nome do problema aparece como uma atualização do sistema na área [!UICONTROL Atualizações] do problema.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: [!UICONTROL Padrão]</p>
   Ou
   <p>Atual: [!UICONTROL Plano]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Determinar quais campos [!DNL Workfront] rastreia um tipo de objeto

Você pode determinar quais informações [!DNL Workfront] rastreia quando os usuários alteram as informações associadas a um determinado tipo de objeto em toda a interface [!DNL Workfront]. Para fazer isso, adicione ou remova os campos que você deseja que [!DNL Workfront] rastreie para esse tipo de objeto.

>[!NOTE]
>
>* [!DNL Workfront] não pode acompanhar e registrar atualizações sobre campos personalizados calculados.
>* Você pode personalizar a atualização do sistema para projetos, tarefas, problemas, portfólios, programas e usuários. Você não pode personalizar a atualização do sistema para modelos, documentos ou folhas de horas, mas [!DNL Workfront] registra atualizações do sistema para esses objetos.
>



* [Adicionar campos que você deseja que [!DNL Workfront] rastreie](#add-fields-you-want-workfront-to-track)
* [Remova os campos que você não quer rastrear](#remove-fields-that-you-don-t-want-tracked)

### Adicionar campos que você deseja que [!DNL Workfront] acompanhe {#add-fields-you-want-workfront-to-track}

Você pode adicionar campos que você deseja que [!DNL Workfront] rastreie para um tipo específico de objeto em toda a interface [!DNL Workfront]. Quando os usuários alteram informações nesse campo, o [!DNL Workfront] registra informações sobre a alteração como uma atualização do sistema na área [!UICONTROL Atualizações] do objeto.

>[!NOTE]
>
>É possível rastrear até 300 campos incorporados e personalizados nos feeds de atualização. Se você estiver rastreando o número máximo de campos e quiser rastrear campos adicionais que não são exibidos na subguia [!UICONTROL Todos os campos], remova primeiro alguns dos campos rastreados para rastrear novos campos. Para obter mais informações sobre como remover campos dos campos de atualização, consulte [Remover campos que você não deseja rastrear](#remove-fields-that-you-don-t-want-tracked).

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Ícone do menu principal](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront] e clique no ícone **[!UICONTROL Configuração]** ![Configurações de engrenagem](assets/gear-icon-settings.png).

1. No painel à esquerda, clique em **[!UICONTROL Interface]** > **[!UICONTROL Feeds de Atualização]**.

1. &#x200B;Clique em **[!UICONTROL Adicionar campos]** e depois clique no objeto que você deseja que seja rastreado.

1. Na caixa&#x200B; **[!UICONTROL Feeds de Atualização]** exibida, comece digitando um campo interno (padrão) ou um campo personalizado para o objeto e, em seguida, clique para selecioná-lo quando ele aparecer na lista.

   Se [!DNL Workfront] já estiver rastreando o campo, você não poderá adicioná-lo uma segunda vez da lista.

1. Depois de adicionar todos os campos que você deseja que [!DNL Workfront] rastreie, clique em **[!UICONTROL Adicionar Campos]**.

   Os campos internos adicionados aparecem na subguia **[!UICONTROL Campos Internos]**.

   Os campos personalizados adicionados são exibidos na subguia **[!UICONTROL Campos Personalizados]**.

   A subguia **[!UICONTROL Todos os campos]** mostra os campos internos e personalizados que estão sendo rastreados.

### Remova os campos que você não quer rastrear {#remove-fields-that-you-don-t-want-tracked}

Você pode remover campos que não deseja que o sistema rastreie para um tipo específico de objeto em toda a interface [!DNL Workfront].

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Ícone do menu principal](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront] e clique no ícone **[!UICONTROL Configuração]** ![Configurações de engrenagem](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Interface]** > **[!UICONTROL Feeds de Atualização]**.

1. Na guia **[!UICONTROL Campos Rastreados]**, selecione a subguia **[!UICONTROL Todos os Campos]**.

   Isso mostra os campos incorporados e personalizados que estão sendo rastreados no momento.

1. Selecione o campo que deseja interromper o rastreamento e clique em **[!UICONTROL Remover]**.

1. Na caixa **[!UICONTROL Remover Campo]** exibida, clique em **[!UICONTROL Sim, Remova-o]** para confirmar.

Quaisquer atualizações sobre os campos rastreados anteriormente são preservadas na área [!UICONTROL Atualizações] onde foram gravadas.

## Determinar quais ações [!DNL Workfront] rastreia um tipo de objeto

Você pode fazer com que o [!DNL Workfront] rastreie as seguintes ações que os usuários podem executar em objetos por toda a interface do [!DNL Workfront].

Por exemplo, você pode fazer com que [!DNL Workfront] registre uma atualização sempre que um usuário alterar uma atribuição para uma tarefa ou problema. A alteração aparece como uma atualização do sistema na área [!UICONTROL Atualizações] para a tarefa ou problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Ação</strong> </th> 
   <th><strong>Objetos</strong> </th> 
   <th><strong>Status padrão</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>A atribuição foi alterada</td> 
   <td>Tarefas, Problemas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>A Linha de Base foi excluída</td> 
   <td>Projetos</td> 
   <td> <p>Desabilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Registro de cobrança criado ou excluído</td> 
   <td>Projetos</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Documento criado ou excluído</td> 
   <td>Projetos, tarefas, problemas, portfólios, programas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Despesa criada ou excluída</td> 
   <td>Projetos, tarefas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Hora registrada ou excluída</td> 
   <td>Projetos, tarefas, problemas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Problema excluído</td> 
   <td>Projetos</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Tarefa excluída</td> 
   <td>Projetos</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>O acesso de alguém foi alterado</td> 
   <td>Projetos, Tarefas, Problemas, Portfólios, Programas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Assinar o objeto com comentário</td> 
   <td>Projetos, tarefas, problemas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
 </tbody> 
</table>

Para configurar quais ações você deseja que [!DNL Workfront] rastreie:

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Ícone do menu principal](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront] e clique no ícone **[!UICONTROL Configuração]** ![Configurações de engrenagem](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Interface]** > **[!UICONTROL Feeds de Atualização]**.

1. Clique na guia **[!UICONTROL Ações]**.

1. Selecione uma ação para habilitá-la ou desmarque uma ação para desabilitá-la.
1. Clique em **[!UICONTROL Salvar]**.

Quando você desabilita uma ação, qualquer atualização gravada anteriormente sobre essa ação é preservada na área [!UICONTROL Atualizações] onde ela foi gravada.
