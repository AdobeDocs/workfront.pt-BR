---
title: Configurar a Integração  [!DNL Workfront]  e  [!DNL Frame.io]
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Como administrador do  [!DNL Adobe Workfront] você pode integrar o [!DNL Workfront] com o [!DNL Frame.io] e fornecer à sua organização uma maneira simples de revisar e aprovar ativos.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Configurar a integração do [!DNL Workfront] e do [!DNL Frame.io]

O administrador do Workfront habilita a integração entre o Workfront e o Frame.io, configurando a conta padrão Frame.io na área Configuração e designando os usuários do Frame.io no Workfront. Isso permite que o coordenador do projeto planeje e inicie o trabalho usando projetos do Workfront e fluxos de trabalho de revisão e aprovação.


## Requisitos de acesso

>[!IMPORTANT]
>
>Essa funcionalidade está disponível somente para organizações que foram integradas ao [!DNL Adobe Admin Console].

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] plano</td>
   <td>Qualquer</td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licenças
   </td>
   <td><p>Atual: [!UICONTROL Plano]</p>
   <p>Novo: [!UICONTROL Padrão]</p></td>
  </tr>
  <tr>
   <td>Configurações de nível de acesso
   </td>
   <td>Você deve ser um administrador [!DNL Workfront].
   </td>
  </tr>

</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure uma conta [!DNL Frame.io] padrão [!BADGE Em breve]{type=Informative}

Uma vez configurada uma conta padrão do [!DNL Frame.io], qualquer projeto criado no [!DNL Workfront] terá um projeto espelho criado no Frame.io.

>[!IMPORTANT]
>
>Esse recurso será adicionado em breve. Por enquanto, contas Frame.io são adicionadas manualmente pela equipe do Workfront. Entre em contato com o representante de conta Adobe para obter ajuda.

## Configurar uma única conta Frame.io com um grupo Workfront

Você pode conectar um único grupo do Workfront com uma única conta Frame.io diferente da conta padrão.

Para configurar uma única conta Frame.io com um grupo Workfront:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos**.
1. Escolha um grupo existente ou clique em **Criar grupo**.
1. No painel esquerdo, clique em **Conectar ao Frame.io**.
1. Insira o token do desenvolvedor de API.
1. Clique em **Iniciar conexão**.
1. (Condicional) Se você for o administrador de mais de uma conta Frame.io, selecione a conta que deseja usar.

## Habilitar usuários do Frame.io

Os usuários do Workfront que usam regularmente o Frame.io devem ser marcados como usuários do Frame.io. Os administradores do Workfront podem designar usuários do Frame.io no Perfil de usuário do Workfront.

>[!TIP]
>
>Recomendamos permitir que os usuários que trabalham regularmente em ferramentas criativas e fazem upload de ativos para revisão e aprovação como usuários do Frame.io.

Quando um usuário é marcado como um usuário do Frame.io no Workfront e adicionado a um projeto:

* Eles são adicionados como um Colaborador no Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Eles podem enviar ativos do Frame.io para o Workfront para revisão e aprovação formais.
* Eles podem exibir informações na pasta de sincronização unidirecional do Workfront. [!BADGE Em breve]{type=Informative}

Para habilitar usuários do Frame.io:

{{step-1-to-users}}

1. Selecione um ou mais usuários e clique no ícone **Editar** ![](assets/edit-icon.png).
1. Na seção Acesso, ative a caixa de seleção Adicionar aos projetos no Frame.io e selecione **Sim** no menu suspenso.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Se esta caixa estiver desmarcada, o usuário retém o acesso a atribuições passadas e é adicionado aos projetos Frame.io dali em diante.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->
