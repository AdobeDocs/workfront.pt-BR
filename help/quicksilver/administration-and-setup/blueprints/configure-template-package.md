---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configurar um blueprint
description: Você pode configurar detalhes do modelo de projeto ou da estrutura organizacional antes de instalar o blueprint.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1841'
ht-degree: 0%

---

# Configurar um blueprint

Você pode configurar detalhes de um blueprint antes de instalá-lo. Os tipos de modelo de projeto e de estrutura organizacional normalmente exigem que algumas preferências sejam definidas e algumas propriedades sejam mapeadas. Outros tipos de blueprint podem não exigir configuração e você os instalará como estão. Para obter mais informações sobre a instalação, consulte [Instalar um blueprint](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>administrador do Workfront </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar um blueprint de modelo de projeto

1. Encontre o blueprint que deseja usar.
1. Clique em **[!UICONTROL Instalar]** e escolha um ambiente:

   <table style="table-layout:auto">
        <tr>
        <td><strong>Produção</strong></td>
        <td>A produção é o seu ambiente ativo.</td>
    </tr>
    <tr>
        <td><strong>Visualização da sandbox</strong></td>
        <td>A visualização da sandbox é um ambiente de teste que serve como uma réplica do seu ambiente ativo e é atualizado todos os finais de semana pela Workfront.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 e 2</strong></td>
        <td>A sandbox de atualização personalizada é um ambiente de teste separado que é atualizado manualmente por você. Há um custo adicional para obter a sandbox de atualização personalizada.</td>
    </tr>
   </table>

1. Continue com as seguintes seções:

   * [[!UICONTROL Preferências do modelo]](#template-preferences)
   * [[!UICONTROL Mapeamento de funções]](#role-mapping)
   * [[!UICONTROL Mapeamento de equipe]](#team-mapping)
   * [[!UICONTROL Mapeamento da empresa]g](#company-mapping)
   * [[!UICONTROL Mapeamento de grupo]](#group-mapping)

## [!UICONTROL Preferências do modelo] {#template-preferences}

Escolha como deseja instalar o modelo.

Você também pode designar a propriedade do modelo antes de instalar o blueprint. Você pode fazer alterações nesses campos após a instalação do template. Para obter mais informações, consulte [Editar modelos de projeto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL Seção &#x200B;] das &#x200B;](assets/Blueprints_TemplatePreferences.png) Preferências de modelo

1. Na seção [!UICONTROL Preferências de Modelo], especifique um novo nome de modelo.
1. Especifique o seguinte:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Proprietário do modelo]<strong></td>
        <td>Esta pessoa recebe permissões de [!UICONTROL Gerenciar] no modelo e se tornará o proprietário do Projeto quando o modelo for usado para criar um projeto.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Patrocinador de modelo]</strong></td>
        <td>Essa pessoa geralmente é um gerente, executivo ou parte interessada que precisa saber o que está acontecendo com o projeto. O Patrocinador do Projeto não obtém acesso adicional ao projeto, mas é adicionado às notificações por email do projeto.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>Este é o portfólio ao qual o projeto pertencerá quando for criado.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Programa]</strong></td>
        <td>Este é o programa ao qual o projeto pertencerá quando for criado.</td>
    </tr>
   </table>

1. Selecione se o modelo está instalado como ativo ou inativo.
1. Selecione se deseja usar as preferências definidas para o novo problema, caso as preferências estejam disponíveis.

   Clique em **[!UICONTROL Ver preferências do problema]** para examinar as preferências específicas que serão instaladas com o blueprint. Os projetos criados a partir do modelo importado usam essas preferências para novos problemas adicionados na seção [!UICONTROL Problemas].

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Grupos de tópicos em fila</strong></td> 
      <td> <p>Os grupos de tópicos da fila definem o nível mais alto de categorias para as ocorrências ou solicitações. Os usuários visualizam grupos de tópicos como opções de menu ao selecionar onde enviar solicitações. Um grupo de tópicos pode conter vários tópicos da fila. Para obter mais informações, consulte <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Criar grupos de tópicos</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enfileirar tópicos</strong></td> 
      <td> <p>Tópicos de fila funcionam em conjunto com regras de roteamento para atribuir problemas ou solicitações. São as opções de menu que os usuários selecionam ao inserir uma ocorrência ou solicitação depois de selecionar um grupo de tópicos. Para obter mais informações, consulte <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Criar tópicos da fila</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Regras de roteamento</strong></td> 
      <td>As regras de roteamento enviam problemas ou solicitações para funções de trabalho, usuários ou equipes específicas. Eles também podem enviar as solicitações para projetos específicos, diferentes daquele associado à fila de solicitações. Para obter mais informações, consulte <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Criar Regras de Roteamento</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**Exemplo:** as novas preferências de problema neste blueprint fornecem quatro tópicos da fila. O usuário seleciona um desses tópicos ao criar uma ocorrência. (Como existe apenas um grupo de tópicos, ele é aplicado automaticamente e o usuário não precisa selecioná-lo.) Quando o usuário conclui e envia o problema, as regras de roteamento determinam a função do cargo ou a equipe à qual está atribuído.
   >![Preferências de exemplo de novo problema](assets/Blueprints_IssuePrefsDetails.png)
   >![Enfileirar tópicos para o novo problema](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![Problema roteado para a função de trabalho](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* Usar as preferências de problema ajuda a criar consistência na maneira como novos problemas ou solicitações são capturados em seus projetos.
   >* A definição dessas preferências não transforma automaticamente os projetos criados a partir do modelo em filas de solicitações. Para obter informações sobre como configurar uma fila de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* Nem todos os blueprints contêm preferências de novos problemas.


## [!UICONTROL Mapeamento de funções] {#role-mapping}

>[!NOTE]
>
>Esta seção pode não aparecer em alguns blueprints.

Alguns modelos incluem funções de trabalho prescritas. As funções de trabalho ajudam a atribuir as pessoas certas quando o modelo é convertido em um projeto. É possível personalizar como as funções são mapeadas antes de instalar o blueprint. Clique em **[!UICONTROL Ver descrições de função]** para saber mais sobre as funções disponíveis no blueprint.

O blueprint pesquisa pelo nome da função para ver se alguma função existente corresponde. A pesquisa diferencia maiúsculas de minúsculas, portanto, os nomes devem ser uma correspondência exata. Se nenhuma função existente for correspondente, você pode fazer com que o blueprint as crie para você.

![[!UICONTROL seção &#x200B;] de Mapeamento de Funções](assets/Blueprints_RoleMapping.png)

1. Se existir uma função, você pode escolher uma das seguintes opções:

   1. Crie uma nova função com um nome diferente e digite o nome na caixa de texto.
   1. Use a função existente, em seguida, selecione uma função na caixa de seleção.
   1. Não usar função mapeada. Esta opção não é recomendada porque algumas tarefas não terão funções atribuídas.

1. Se uma função não existir, você poderá escolher uma das seguintes opções:

   1. Crie uma nova função. Essa opção cria a função recomendada pelo blueprint.
   1. Crie uma nova função com um nome diferente e digite o nome na caixa de texto.
   1. Use a função existente, em seguida, selecione uma função na caixa de seleção.
   1. Não usar função mapeada. Esta opção não é recomendada porque algumas tarefas não terão funções atribuídas.

>[!NOTE]
>
>O processo de instalação não aplica funções a pessoas específicas. Você deve verificar as pessoas nessas funções depois de instalar a solução de blueprint e atribuir pessoas, se necessário. Para obter informações, consulte [Ações a serem executadas após a instalação de um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Para obter mais informações sobre as funções de trabalho em [!DNL Workfront], consulte [Criar e gerenciar funções de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL Mapeamento de equipe] {#team-mapping}

>[!NOTE]
>
>Esta seção pode não aparecer em alguns blueprints.

Alguns modelos incluem equipes prescritas. O trabalho atribuído a uma equipe pode ser concluído por qualquer membro da equipe. Você pode personalizar como as equipes são mapeadas antes de instalar o blueprint. Clique em **[!UICONTROL Ver descrições de equipe]** para saber mais sobre as equipes disponíveis no blueprint.

O blueprint pesquisa pelo nome da equipe para ver se alguma equipe existente corresponde. A pesquisa diferencia maiúsculas de minúsculas, portanto, os nomes devem ser uma correspondência exata. Se nenhuma equipe existente for correspondente, você poderá fazer com que o blueprint as crie para você.

![[!UICONTROL Mapeamento de Equipe] seção](assets/Blueprints_TeamMapping.png)

1. Se houver uma equipe, você pode escolher uma das seguintes opções:

   1. Crie um novo grupo com um nome diferente e digite o nome na caixa de texto.
   1. Use a [!UICONTROL equipe existente] e selecione uma equipe na caixa de seleção.
   1. Não use a equipe mapeada. Esta opção não é recomendada porque algumas tarefas não terão equipes atribuídas.

1. Se não existir uma equipe, você pode escolher uma das seguintes opções:

   1. Criar uma nova equipe. Essa opção cria a equipe recomendada pelo blueprint.
   1. Crie um novo grupo com um nome diferente e digite o nome na caixa de texto.
   1. Use a [!UICONTROL equipe existente] e selecione uma equipe na caixa de seleção.
   1. Não use a equipe mapeada. Esta opção não é recomendada porque algumas tarefas não terão equipes atribuídas.

>[!NOTE]
>
>O processo de instalação não adiciona pessoas às equipes. Você deve verificar as pessoas nas equipes depois de instalar a solução de blueprint e atribuir pessoas, se necessário. Para obter informações, consulte [Ações a serem executadas após a instalação de um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Para obter mais informações sobre como as equipes funcionam em [!DNL Workfront], consulte [Criar e gerenciar equipes](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Mapeamento da empresa {#company-mapping}

>[!NOTE]
>
>Esta seção pode não aparecer em alguns blueprints.

Alguns projetos incluem empresas prescritas. Uma empresa é uma unidade organizacional que pode representar sua organização, um departamento dentro da organização ou um cliente com o qual você trabalha. É possível personalizar como as empresas são mapeadas antes de instalar o blueprint. Clique em **[!UICONTROL Ver descrições da empresa]** para saber mais sobre as empresas disponíveis no blueprint.

O blueprint pesquisa pelo nome da empresa para ver se alguma empresa existente corresponde. A pesquisa diferencia maiúsculas de minúsculas, portanto, os nomes devem ser uma correspondência exata. Se nenhuma empresa existente corresponder, você pode fazer com que o blueprint as crie para você. A empresa principal no blueprint é mapeada para a empresa principal em seu ambiente, mesmo que não tenha o mesmo nome.

![[!UICONTROL seção Mapeamento da Empresa]](assets/Blueprints_CompanyMapping.png)

1. Se existir uma empresa, você poderá escolher uma das seguintes opções:

   1. Crie uma nova empresa com um nome diferente e digite o nome na caixa de texto.
   1. Use a empresa existente e selecione uma empresa na caixa de seleção.\

      A empresa principal no blueprint é mapeada para a empresa principal em seu ambiente, mesmo que não tenha o mesmo nome.
   1. Não usar a empresa mapeada. Essa opção não é recomendada, pois as referências da empresa em outros objetos estarão vazias.

1. Se não existir uma empresa, você poderá escolher uma das seguintes opções:

   1. Crie uma nova empresa. Essa opção cria a empresa recomendada pelo blueprint.
   1. Crie uma nova empresa com um nome diferente e digite o nome na caixa de texto.
   1. Use a empresa existente e selecione uma empresa na caixa de seleção.
   1. Não usar a empresa mapeada. Essa opção não é recomendada, pois as referências da empresa em outros objetos estarão vazias.

>[!NOTE]
>
>Para configurar as empresas após instalar o blueprint, consulte [Ações a serem executadas após instalar um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Para obter informações sobre como associar um modelo a uma empresa, consulte [Editar modelos de projeto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Para obter informações sobre como as empresas funcionam em [!DNL Workfront], consulte [Criar e editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL Mapeamento de grupo] {#group-mapping}

>[!NOTE]
>
>Esta seção pode não aparecer em alguns blueprints.

Alguns blueprints incluem grupos prescritos. Um grupo é um grupo de usuários que coincide com a estrutura departamental. Os grupos são semelhantes, mas distintos das equipes e empresas na Workfront. Você pode personalizar como os grupos são mapeados antes de instalar o blueprint. Clique em **[!UICONTROL Ver descrições de grupo]** para saber mais sobre os grupos disponíveis no blueprint.

O blueprint pesquisa pelo nome do grupo para ver se algum grupo existente corresponde. A pesquisa diferencia maiúsculas de minúsculas, portanto, os nomes devem ser uma correspondência exata. Se nenhum grupo existente for correspondente, você pode fazer com que o blueprint os crie para você.

![[!UICONTROL Mapeamento do Grupo] seção](assets/Blueprints_GroupMapping.png)

1. Se um grupo existir, você poderá selecionar **[!UICONTROL Remapear Grupo]** e escolher uma das seguintes opções:

   1. **[!UICONTROL Crie um novo grupo com um nome diferente]** e digite o nome a ser atribuído a esse grupo. As referências ao grupo na definição de blueprint serão associadas a esse novo grupo.
   1. **[!UICONTROL Substituir por um grupo existente]** e, em seguida, procurar e selecionar um grupo na caixa de seleção.

      >[!NOTE]
      >
      >Não é possível renomear um grupo existente.

1. Se um grupo não existir, você poderá:

   1. Altere o nome do grupo sugerido digitando-o na caixa de texto.
   1. Selecione **[!UICONTROL Remapear Grupo]** e escolha [!UICONTROL Substituir por um grupo existente], depois procure e selecione um grupo na caixa de seleção.
   1. Selecione **[!UICONTROL Remapear Grupo]** e escolha **[!UICONTROL Inserir em um grupo existente]**, depois procure e selecione um grupo na caixa de seleção. Esta opção cria um novo subgrupo no grupo existente.

>[!NOTE]
>
>Para configurar os grupos após instalar o blueprint, consulte [Ações a serem executadas após instalar um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Para obter informações sobre o uso de grupos em [!DNL Workfront], consulte [Visão geral de grupos](../../administration-and-setup/manage-groups/groups-overview/groups.md).
