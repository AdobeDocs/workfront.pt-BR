---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organizações e equipes do Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] organizações e equipes

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas nos artigos:
>
>* [Visão geral das organizações e equipes do Adobe Workfront Fusion](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/org-and-team-overview.html)
>* [Definir Opções de Notificação de Equipe](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/set-team-notification-options.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Os recursos de Organização e Equipes de [!DNL Adobe Workfront Fusion] possibilitam que as empresas controlem o acesso a cenários e outros recursos no Fusion.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> 
     <p>Você deve ser um administrador do [!DNL Workfront Fusion] para sua organização.</p>
     <p>Você deve ser um administrador [!DNL Workfront Fusion] para sua equipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

<p>**Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] licenças</a></p>


## Organizações

[!DNL Workfront Fusion] usuários pertencem a uma organização.

* [Funções da organização](#organization-roles)
* [Convidar usuários para uma organização](#inviting-users-to-an-organization)
* [Alternar entre organizações](#switch-between-organizations)

### Funções da organização

Um usuário tem uma das seguintes funções em uma organização:

* **[!UICONTROL Proprietário]**: o proprietário tem todas as permissões disponíveis na organização.
* **[!UICONTROL Administrador]**: a função de administrador permite que um usuário crie e gerencie equipes e usuários para a organização.
* **[!UICONTROL Membro]**: os membros podem usar [!DNL Workfront Fusion], mas não podem fazer alterações organizacionais.
* **[!UICONTROL Contador]**: uma função de contador permite que apenas os usuários vejam informações de licença no painel da organização.
* **[!UICONTROL Desenvolvedor de Aplicativos]**: A funcionalidade para esta função está indisponível no momento e será disponibilizada em breve. Não é recomendável atribuir usuários a essa função no momento.

Para obter informações sobre ações específicas disponíveis para usuários em cada função de organização, consulte [Funções de organização e equipe](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Convidar usuários para uma organização

Por padrão, um proprietário de organização (ou usuário autorizado) pode convidar outra pessoa para ingressar em sua organização.

Para convidar um usuário para ingressar em uma organização:

1. Clique em **[!UICONTROL Detalhes da alteração]** no canto superior direito da tela.
1. Selecione **[!UICONTROL Convidar um novo usuário]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Preencha o endereço de email e o nome do usuário.
1. Selecione uma função para o usuário. Para obter mais informações sobre funções, consulte [Funções da organização](#organization-roles) neste documento.
1. (Opcional) Adicione uma observação. Essa nota aparece no email de convite que o usuário recebe.
1. Clique em **[!UICONTROL Salvar]**.

[!DNL Fusion] envia um email com um convite para a organização específica e um botão [!UICONTROL Aceitar a Função].

Quando o recipient clica no botão, ele é redirecionado para a página de convite, onde pode aceitar o convite.

O convite expirará em um dia.

>[!NOTE]
>
>Se o usuário for novo no [!DNL Fusion], o [!DNL Fusion] criará automaticamente uma conta para ele e enviará um email com uma senha temporária, instruindo o novo usuário a fazer logon e alterar a senha.

### Alternar entre organizações

Você pode fazer parte de mais de uma organização no Fusion. Os recursos não são compartilhados entre organizações.

Você pode alternar organizações na Experiência unificada do Adobe clicando no nome da organização no canto superior direito e selecionando a nova organização na lista suspensa. Somente as organizações que têm uma conta do Fusion aparecerão na lista suspensa, mesmo se você for membro de outras organizações no Adobe.

## Equipes

Equipes são grupos de usuários que compartilham acesso a recursos específicos. Esses recursos podem incluir:

* Cenários
* Conexões
* Webhooks
* Chaves
* Armazenamentos de dados
* Estruturas de dados
* Configurações de notificação por email

>[!NOTE]
>
>Como as equipes controlam o acesso aos recursos, às vezes é útil que uma equipe tenha apenas um membro. Por exemplo, os usuários em treinamento podem criar conexões com suas contas individuais do [!DNL Google]. Qualquer membro da equipe também poderá se conectar à conta individual [!DNL Google]. Portanto, neste caso, é melhor que o usuário seja o único membro de uma equipe de treinamento.

As organizações podem ter quantas equipes precisarem e os usuários podem pertencer a uma ou mais equipes.

Os usuários podem selecionar sua equipe na lista suspensa no painel de navegação esquerdo. Os usuários veem somente as equipes das quais são membros. Selecionar uma equipe permitirá que um usuário acesse os recursos dessa equipe.

* [Funções da equipe](#team-roles)
* [Gerenciamento de Equipe](#team-management)

### Funções da equipe

Um usuário tem uma das seguintes funções em cada uma de suas equipes:

* **[!UICONTROL Administrador da Equipe]**: além das funcionalidades das outras funções da equipe, a função de Administrador permite que o usuário adicione, remova ou altere a função de um membro da equipe.
* **[!UICONTROL Membro da Equipe]**: a função de membro da equipe permite que os usuários criem e executem cenários.
* **[!UICONTROL Monitoramento de Equipe]**: A função de [!UICONTROL monitoramento] permite que os usuários acessem informações de execução para cenários, mas não é possível criar cenários nem alterar seu status &quot;Ativo&quot;.
* **[!UICONTROL Operador de Equipe]**: a função [!UICONTROL operador] permite que os usuários vejam os dados de execução e alterem o status &quot;Ativo&quot; dos cenários.
* **[!UICONTROL Membro Restrito à Equipe]**: a funcionalidade para esta função está indisponível no momento e será disponibilizada em breve. Não é recomendável atribuir usuários a essa função no momento.

Para obter informações sobre ações específicas disponíveis para usuários em cada função de equipe, consulte [Funções de organização e equipe](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Gerenciamento de Equipe

* [Criar uma equipe](#create-a-team)
* [Definir opções de notificação da equipe](#set-team-notification-options)

#### Criar uma equipe

Os proprietários e administradores da organização podem criar equipes.

Para criar um grupo:

1. No painel de navegação esquerdo, clique em **[!UICONTROL Organização]**
1. Selecione a guia **[!UICONTROL Equipe]**.
1. Clique em **[!UICONTROL Adicionar nova equipe]** na lista de equipes.
1. Digite um nome para a nova equipe e clique em **Adicionar**.

#### Definir opções de notificação da equipe

>[!NOTE]
>
>Se sua organização tiver sido movida para o Unified Shell, você receberá notificações por meio da área Notificações de Adobe. Você deve usar a experiência do Unified Shell para ver as notificações na área Notificações de Adobe.
>
>Para usar a Experiência do Unified Shell, incluindo a área Notificações do Adobe, clique no botão Tentar Nova Interface do Usuário do Fusion na Experiência Unificada próximo à parte superior da página. Esse botão só estará disponível se sua organização tiver migrado para o Unified Shell.
>
>Para obter mais informações, consulte [Acessar suas notificações](/help/quicksilver/workfront-fusion/fusion-in-admin-console/fusion-unified-experience.md#access-your-notifications) em [!DNL Adobe Unified Experience] para [!DNL Workfront Fusion].

As opções de notificação por email são definidas no nível da equipe.

1. No painel de navegação esquerdo, clique em **[!UICONTROL Equipe]**
1. Selecione a guia **[!UICONTROL Opções de Notificação]**.
1. Ative as notificações que você deseja que a equipe receba.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Aviso na execução do cenário]'</td> 
      <td> <p>Receber um email quando houver um aviso em uma execução de cenário</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Erros na execução do cenário]</td> 
      <td>Receba um email quando houver um erro em uma execução de cenário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Desativação de cenário]</p> </td> 
      <td><p>Receba um email quando um cenário for desativado.</p><p><b>Observação:</b> você será notificado sobre a desativação de cenário somente quando o cenário tiver sido desativado automaticamente devido a erros. Você não recebe notificações sobre cenários que são desativados manualmente.</p><p>Em alguns casos, um cenário pode ser desativado pela equipe de engenharia [!DNL Workfront Fusion] porque está causando desempenho ou outros problemas. Nesses casos, você não recebe notificações em [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

As alterações nas opções de notificação são salvas automaticamente

#### Alternar entre equipes

Você pode fazer parte de mais de uma equipe no Fusion. Como as equipes não compartilham recursos, talvez seja necessário trocar de equipe para acessar cenários específicos ou outros recursos.

Se sua organização não estiver na Experiência unificada do Adobe, você poderá trocar de equipe clicando no nome da equipe na navegação à esquerda e selecionando uma equipe na lista suspensa.

Se sua equipe estiver na Experiência unificada do Adobe, você poderá selecionar uma nova equipe clicando no nome da equipe no cabeçalho e selecionando uma equipe na lista suspensa. Essa opção está disponível em todas as páginas específicas de uma determinada equipe, como uma página de cenário ou a página Conexões.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->