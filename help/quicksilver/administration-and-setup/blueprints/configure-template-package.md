---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configurar um blueprint
description: Você pode configurar os detalhes do modelo de projeto ou da estrutura organizacional antes de instalar o blueprint.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1824'
ht-degree: 0%

---

# Configurar um blueprint

Você pode configurar detalhes de um blueprint antes de instalá-lo. O modelo do projeto e os tipos de blueprint da estrutura organizacional geralmente exigem que algumas preferências sejam definidas e algumas propriedades sejam mapeadas. Outros tipos de blueprint podem não exigir configuração e você os instalará como estão. Para obter mais informações sobre instalação, consulte [Instalar um blueprint](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano</strong></td>
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licença</strong></td>
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td>
   <td> <p>[!UICONTROL Administrador do sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar um blueprint do modelo de projeto

1. Encontre o blueprint que deseja usar.
1. Clique em **[!UICONTROL Instalar]** e escolha um ambiente:

   <table style="table-layout:auto">
        <tr>
        <td><strong>Produção</strong></td>
        <td>A produção é o seu ambiente ativo.</td>
    </tr>
    <tr>
        <td><strong>Visualização da sandbox</strong></td>
        <td>A Visualização de sandbox é um ambiente de teste que serve como réplica do ambiente ativo e é atualizado a cada fim de semana pela Workfront.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 e 2</strong></td>
        <td>A Sandbox de atualização personalizada é um ambiente de teste separado, que é atualizado manualmente por você. Há um custo adicional para obter a Caixa de proteção de atualização personalizada.</td>
    </tr>
   </table>

1. Continue com as seguintes seções:

   * [[!UICONTROL Preferências do modelo]](#template-preferences)
   * [[!UICONTROL Mapeamento de função]](#role-mapping)
   * [[!UICONTROL Mapeamento de equipe]](#team-mapping)
   * [[!UICONTROL Mapeamento da empresa]g](#company-mapping)
   * [[!UICONTROL Mapeamento de grupo]](#group-mapping)

## [!UICONTROL Preferências do modelo] {#template-preferences}

Escolha como deseja instalar o template.

Também é possível designar a propriedade do modelo antes de instalar o blueprint. Você pode fazer alterações nesses campos depois que o modelo for instalado. Para obter mais informações, consulte [Editar modelos de projeto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL Preferências do modelo] seção](assets/Blueprints_TemplatePreferences.png)

1. No [!UICONTROL Preferências do modelo] especifique um novo nome de modelo.
1. Especifique o seguinte:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Proprietário do modelo]<strong></td>
        <td>Esta pessoa recebe as permissões do [!UICONTROL Gerenciar] no modelo e se tornará o proprietário do Projeto quando o modelo for usado para criar um projeto.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Patrocinador de modelo]</strong></td>
        <td>Normalmente, essa pessoa é gerente, executivo ou parte interessada que precisa saber o que está acontecendo com o projeto. O Patrocinador de projeto não obtém acesso adicional ao projeto, mas é adicionado às notificações por email do projeto.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>Esse é o portfólio ao qual o projeto pertencerá ao ser criado.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Program]</strong></td>
        <td>Este é o programa ao qual o projeto pertencerá ao ser criado.</td>
    </tr>
   </table>

1. Selecione se o modelo está instalado como ativo ou inativo.
1. Selecione se deseja usar as preferências de nova edição definidas, se as preferências estiverem disponíveis.

   Clique em **[!UICONTROL Consulte preferências de edição]** para analisar as preferências específicas que serão instaladas com o blueprint. Os projetos criados a partir do modelo importado usam essas preferências para novos problemas adicionados na [!UICONTROL Problemas] seção.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Grupos de tópicos em fila</strong></td> 
      <td> <p>Grupos de tópicos da fila definem o nível mais alto de categorias para problemas ou solicitações. Os usuários visualizam grupos de tópicos como opções de menu ao selecionar onde enviar solicitações. Um grupo de tópicos pode conter vários tópicos de fila. Para obter mais informações, consulte <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Criar grupos de tópicos</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enfileirar tópicos</strong></td> 
      <td> <p>Os tópicos da fila funcionam juntamente com as regras de roteamento para atribuir problemas ou solicitações. São as opções de menu que os usuários selecionam ao inserir um problema ou solicitação, depois de selecionar um grupo de tópicos. Para obter mais informações, consulte <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Criar Tópicos da Fila</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Regras de roteamento</strong></td> 
      <td>As regras de roteamento enviam problemas ou solicitações para funções de trabalho, usuários ou equipes específicas. Eles também podem enviar as solicitações para projetos específicos, diferente daquele associado à fila de solicitações. Para obter mais informações, consulte <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Criar regras de roteamento</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**Exemplo:** As novas preferências de edição neste blueprint fornecem quatro tópicos da fila. O usuário seleciona um desses tópicos ao criar um problema. (Como existe apenas um grupo de tópicos, ele é aplicado automaticamente e o usuário não precisa selecioná-lo.) Quando o usuário conclui e envia o problema, as regras de roteamento determinam a função ou a equipe de trabalho à qual está atribuído.
   >![Exemplo de preferências de nova edição](assets/Blueprints_IssuePrefsDetails.png)
   >![Tópicos da fila para novo problema](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![Problema roteado para a função de trabalho](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* Usar as preferências de edição ajuda a criar consistência na maneira como novos problemas ou solicitações são capturados em seus projetos.
   >* Definir essas preferências não transforma automaticamente os projetos criados a partir do modelo em filas de solicitações. Para obter informações sobre como configurar uma fila de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* Nem todos os blueprints contêm novas preferências de edição.



## [!UICONTROL Mapeamento de função] {#role-mapping}

>[!NOTE]
>
>Esta seção pode não aparecer em alguns blueprints.

Alguns modelos incluem funções de trabalho prescritas. As funções de trabalho ajudam a atribuir as pessoas certas quando o modelo é convertido em um projeto. Você pode personalizar como as funções são mapeadas antes de instalar o blueprint. Clique em **[!UICONTROL Consulte descrições de funções]** para saber mais sobre as funções disponíveis no blueprint.

O blueprint pesquisa pelo nome da função para ver se alguma função existente corresponde. A pesquisa diferencia maiúsculas de minúsculas, portanto, os nomes devem ser uma correspondência exata. Se nenhuma função existente corresponder, você pode fazer com que o blueprint as crie para você.

![[!UICONTROL Mapeamento de função] seção](assets/Blueprints_RoleMapping.png)

1. Se houver uma função, você poderá escolher uma das seguintes opções:

   1. Crie uma nova função com um nome diferente e digite o nome na caixa de texto.
   1. Use a função existente e selecione uma função na caixa de seleção.
   1. Não use função mapeada. Esta opção não é recomendada porque algumas tarefas não terão funções atribuídas.

1. Se uma função não existir, é possível escolher uma das seguintes opções:

   1. Crie uma nova função. Essa opção cria a função recomendada pelo blueprint.
   1. Crie uma nova função com um nome diferente e digite o nome na caixa de texto.
   1. Use a função existente e selecione uma função na caixa de seleção.
   1. Não use função mapeada. Esta opção não é recomendada porque algumas tarefas não terão funções atribuídas.

>[!NOTE]
>
>O processo de instalação não aplica funções a pessoas específicas. Você deve verificar as pessoas nessas funções após instalar a solução do blueprint e atribuir as pessoas, se necessário. Para obter mais informações, consulte [Ações a serem tomadas após a instalação de um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Para obter mais informações sobre funções de job em [!DNL Workfront], consulte [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL Mapeamento de equipe] {#team-mapping}

>[!NOTE]
>
>Esta seção pode não aparecer em alguns blueprints.

Alguns modelos incluem equipes prescritas. O trabalho atribuído a uma equipe pode ser concluído por qualquer membro da equipe. Você pode personalizar como as equipes são mapeadas antes de instalar o blueprint. Clique em **[!UICONTROL Consulte as descrições da equipe]** para saber mais sobre as equipes disponíveis no blueprint.

O blueprint pesquisa pelo nome da equipe para ver se alguma equipe existente corresponde. A pesquisa diferencia maiúsculas de minúsculas, portanto, os nomes devem ser uma correspondência exata. Se nenhuma equipe existente corresponder, você pode ter o blueprint para criá-las para você.

![[!UICONTROL Mapeamento de equipe] seção](assets/Blueprints_TeamMapping.png)

1. Se houver um grupo, você poderá escolher uma das seguintes opções:

   1. Crie uma nova equipe com um nome diferente e digite o nome na caixa de texto.
   1. Use [!UICONTROL equipe existente]e, em seguida, selecione um grupo na caixa de seleção.
   1. Não use equipe mapeada. Esta opção não é recomendada porque algumas tarefas não terão equipes atribuídas.

1. Se um grupo não existir, você pode escolher uma das seguintes opções:

   1. Crie uma nova equipe. Essa opção cria a equipe recomendada pelo blueprint.
   1. Crie uma nova equipe com um nome diferente e digite o nome na caixa de texto.
   1. Use [!UICONTROL equipe existente]e, em seguida, selecione um grupo na caixa de seleção.
   1. Não use equipe mapeada. Esta opção não é recomendada porque algumas tarefas não terão equipes atribuídas.

>[!NOTE]
>
>O processo de instalação não adiciona pessoas às equipes. Você deve verificar as pessoas nas equipes após instalar a solução blueprint e atribuir as pessoas, se necessário. Para obter mais informações, consulte [Ações a serem tomadas após a instalação de um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Para obter mais informações sobre como as equipes funcionam no [!DNL Workfront], consulte [Criar e gerenciar equipes](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Mapeamento da empresa {#company-mapping}

>[!NOTE]
>
>Esta seção pode não aparecer em alguns blueprints.

Alguns projetos incluem empresas prescritas. Uma empresa é uma unidade organizacional que pode representar sua organização, um departamento dentro da organização ou um cliente com o qual você trabalha. Você pode personalizar como as empresas são mapeadas antes de instalar o blueprint. Clique em **[!UICONTROL Consulte as descrições da empresa]** para saber mais sobre as empresas disponíveis no blueprint.

O blueprint pesquisa pelo nome da empresa para ver se alguma empresa existente corresponde. A pesquisa diferencia maiúsculas de minúsculas, portanto, os nomes devem ser uma correspondência exata. Se nenhuma empresa existente corresponder, você pode fazer com que o blueprint as crie para você. A empresa principal no blueprint é mapeada para a empresa principal em seu ambiente, mesmo que não tenha o mesmo nome.

![[!UICONTROL Mapeamento da empresa] seção](assets/Blueprints_CompanyMapping.png)

1. Se uma empresa existir, você poderá escolher uma das seguintes opções:

   1. Crie uma nova empresa com um nome diferente e digite o nome na caixa de texto.
   1. Use a empresa existente e selecione uma empresa na caixa de seleção.\

      A empresa principal no blueprint é mapeada para a empresa principal em seu ambiente, mesmo que não tenha o mesmo nome.
   1. Não use empresa mapeada. Essa opção não é recomendada, pois as referências da empresa em outros objetos estarão vazias.

1. Se uma empresa não existir, você pode escolher uma das seguintes opções:

   1. Criar uma nova empresa. Essa opção cria a empresa recomendada pelo blueprint.
   1. Crie uma nova empresa com um nome diferente e digite o nome na caixa de texto.
   1. Use a empresa existente e selecione uma empresa na caixa de seleção.
   1. Não use empresa mapeada. Essa opção não é recomendada, pois as referências da empresa em outros objetos estarão vazias.

>[!NOTE]
>
>Para configurar as empresas após instalar o blueprint, consulte [Ações a serem tomadas após a instalação de um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Para obter informações sobre como associar um modelo a uma empresa, consulte [Editar modelos de projeto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Para obter informações sobre como as empresas funcionam em [!DNL Workfront], consulte [Criar e editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL Mapeamento de grupo] {#group-mapping}

>[!NOTE]
>
>Esta seção pode não aparecer em alguns blueprints.

Alguns projetos incluem grupos prescritos. Um grupo é um grupo de usuários que coincide com a estrutura departamental. Os grupos são semelhantes, mas distintos, às equipes e empresas no Workfront. Você pode personalizar como os grupos são mapeados antes de instalar o blueprint. Clique em **[!UICONTROL Consulte as descrições do grupo]** para saber mais sobre os grupos disponíveis no blueprint.

O blueprint pesquisa pelo nome do grupo para ver se algum grupo existente corresponde. A pesquisa diferencia maiúsculas de minúsculas, portanto, os nomes devem ser uma correspondência exata. Se nenhum grupo existente corresponder, o blueprint poderá criá-los para você.

![[!UICONTROL Mapeamento de grupo] seção](assets/Blueprints_GroupMapping.png)

1. Se houver um grupo, você poderá selecionar **[!UICONTROL Remapear grupo]** e escolha uma das seguintes opções:

   1. **[!UICONTROL Criar um novo grupo com um nome diferente]** e digite o nome a ser atribuído a esse grupo. As referências ao grupo na definição do blueprint serão associadas a esse novo grupo.
   1. **[!UICONTROL Substituir por um grupo existente]**, em seguida, pesquise e selecione um grupo na caixa de seleção.

      >[!NOTE]
      >
      >Não é possível renomear um grupo existente.

1. Se um grupo não existir, é possível:

   1. Altere o nome do grupo sugerido digitando-o na caixa de texto.
   1. Selecionar **[!UICONTROL Remapear grupo]** e escolha [!UICONTROL Substituir por um grupo existente], em seguida, pesquise e selecione um grupo na caixa de seleção.
   1. Selecionar **[!UICONTROL Remapear grupo]** e escolha **[!UICONTROL Inserir em um grupo existente]**, em seguida, pesquise e selecione um grupo na caixa de seleção. Essa opção cria um novo subgrupo no grupo existente.

>[!NOTE]
>
>Para configurar os grupos após instalar o blueprint, consulte [Ações a serem tomadas após a instalação de um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Para obter informações sobre como usar grupos em [!DNL Workfront], consulte [Visão geral dos grupos](../../administration-and-setup/manage-groups/groups-overview/groups.md).
