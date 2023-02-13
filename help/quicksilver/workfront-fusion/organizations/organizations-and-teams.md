---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organizações e equipes do Adobe Workfront Fusion
description: Os recursos de Organização e Equipes do Adobe Workfront Fusion permitem que as empresas controlem o acesso a cenários e outros recursos dentro do Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] organizações e equipes

[!DNL Adobe Workfront Fusion]Os recursos de Organização e Equipes do permitem que as empresas controlem o acesso a cenários e outros recursos dentro da Fusão.

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
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>Workfront Fusion para Automação e Integração do Trabalho,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> 
     <p>Você deve ser um [!DNL Workfront Fusion] administrador da sua organização.</p>
     <p>Você deve ser um [!DNL Workfront Fusion] administrador da sua equipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

<p>**Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] licenças</a></p>


## Organizações

[!DNL Workfront Fusion] Os usuários pertencem a uma organização. Seu [!DNL Fusion] determina quantos cenários ativos e conectores estão disponíveis em sua organização.

[!DNL Fusion] o licenciamento determina o número de cenários ativos e aplicativos ativos disponíveis para uma organização. [!DNL Fusion] exibe a contagem atual de &quot;Cenários ativos&quot; e &quot;Aplicativos ativos&quot; no painel da organização.

* [Funções da organização](#organization-roles)
* [Convidar usuários para uma organização](#inviting-users-to-an-organization)

### Funções da organização

Um usuário tem uma das seguintes funções em uma organização:

* **[!UICONTROL Proprietário]**: O proprietário tem todas as permissões disponíveis na organização.
* **[!UICONTROL Administrador]**: A função de administrador permite que um usuário crie e gerencie equipes e usuários para a organização.
* **[!UICONTROL membro]**: Os membros podem usar [!DNL Workfront Fusion] mas incapaz de fazer alterações organizacionais.
* **[!UICONTROL Contador]**: Uma função de contador permite somente que os usuários vejam as informações da licença no painel da organização.
* **[!UICONTROL Desenvolvedor de aplicativos]**: A funcionalidade para essa função está indisponível no momento e será disponibilizada em breve. Não recomendamos atribuir usuários a essa função no momento.

### Convidar usuários para uma organização

Por padrão, um proprietário de organização (ou usuário autorizado) pode convidar outra pessoa para entrar em sua organização.

Para convidar um usuário para ingressar em uma organização:

1. Clique em **[!UICONTROL Alterar detalhes]** no canto superior direito da tela.
1. Selecionar **[!UICONTROL Convidar um novo usuário]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Preencha o endereço de email e o nome do usuário.
1. Selecione uma função para o usuário. Para obter mais informações sobre funções, consulte [Funções da organização](#organization-roles) neste documento.
1. (Opcional) Adicione uma observação. Essa nota aparece no email de convite recebido pelo usuário.
1. Clique em **[!UICONTROL Salvar]**.

[!DNL Fusion] envia um email com um convite para a organização específica e um [!UICONTROL Aceite A Função] botão.

![](assets/accept-the-role.png)

Quando o recipient clica no botão , ele é redirecionado para a página de convite, onde pode aceitar o convite.

O convite expirará em um dia.

>[!NOTE]
>
>Se o usuário for novo em [!DNL Fusion], [!DNL Fusion] O cria automaticamente uma conta para eles e envia um email com uma senha temporária, direcionando o novo usuário para fazer logon e alterar sua senha.

## Equipes

As equipes são grupos de usuários que compartilham acesso a recursos específicos. Esses recursos podem incluir:

* Cenários
* Conexões
* Webhooks
* Teclas
* Repositórios de dados
* Estruturas de dados
* Configurações de notificação por email

>[!NOTE]
>
>Como as equipes controlam o acesso aos recursos, às vezes é útil que uma equipe tenha apenas um membro. Por exemplo, os usuários em treinamento podem criar conexões com seus indivíduos [!DNL Google] contas. Qualquer membro da equipe também poderá se conectar ao [!DNL Google] , portanto, neste caso, é melhor que o usuário seja o único membro de uma equipe de treinamento.

As organizações podem ter quantas equipes precisarem e os usuários podem pertencer a uma ou mais equipes.

Os usuários podem selecionar sua equipe na lista suspensa no painel de navegação esquerdo. Os usuários só veem equipes das quais são membros. Selecionar uma equipe permitirá que um usuário acesse os recursos dessa equipe.

* [Funções da equipe](#team-roles)
* [Gerenciamento de equipe](#team-management)

### Funções da equipe

Um usuário tem uma das seguintes funções em cada uma de suas equipes:

* **[!UICONTROL Administrador de equipe]**: Além dos recursos das outras funções da equipe, a função de Administrador permite que o usuário adicione, remova ou altere a função de um membro da equipe.
* **[!UICONTROL Membro da Equipe]**: A função de membro da equipe permite que os usuários criem e executem cenários.
* **[!UICONTROL Monitoramento de equipe]**: O [!UICONTROL monitoramento] permite que os usuários acessem informações de execução para cenários, mas não podem projetar cenários ou alterar seu status &quot;Ativo&quot;.
* **[!UICONTROL Operador de Equipe]**: O [!UICONTROL operador] permite que os usuários vejam dados de execução e alterem o status &quot;Ativo&quot; de cenários.
* **[!UICONTROL Membro Restrito da Equipe]**: A funcionalidade para essa função está indisponível no momento e será disponibilizada em breve. Não recomendamos atribuir usuários a essa função no momento.

### Gerenciamento de equipe

* [Criar um grupo](#create-a-team)
* [Definir Opções de Notificação de Equipe](#set-team-notification-options)

#### Criar um grupo

Os proprietários e administradores da organização podem criar equipes.

Para criar uma equipe:

1. No painel de navegação esquerdo, clique em **[!UICONTROL Organização]**
1. Selecione o **[!UICONTROL Equipe]** guia .
1. Clique em **[!UICONTROL Adicionar uma nova equipe]** na lista de equipes.
1. Insira um nome para a nova equipe e clique em **Adicionar**.

#### Definir Opções de Notificação de Equipe

As opções de notificação por email são definidas no nível da equipe.

1. No painel de navegação esquerdo, clique em **[!UICONTROL Equipe]**
1. Selecione o **[!UICONTROL Opções de notificação]** guia .
1. Ative as notificações que deseja que a equipe receba.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Aviso na execução do cenário]'</td> 
      <td> <p>Receba um email quando houver um aviso em uma execução de cenário</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Erros na execução do cenário]</td> 
      <td>Receba um email quando houver um erro em uma execução de cenário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Scenario deativation]</p> </td> 
      <td><p>Receba um email quando um cenário for desativado.</p><p><b>Observação:</b> Você é notificado sobre desativação de cenário somente quando o cenário foi desativado automaticamente devido a erros. Você não recebe notificações sobre cenários que são desativados manualmente.</p><p>Em alguns casos, um cenário pode ser desativado pela variável [!DNL Workfront Fusion] equipe de engenharia porque o cenário está causando desempenho ou outros problemas. Nesses casos, você não recebe notificações em [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Alterações nas opções de notificação salvas automaticamente

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->