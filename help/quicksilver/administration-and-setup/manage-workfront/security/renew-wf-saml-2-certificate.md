---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,segurança,certificado,Admin,Isenção,configurar,metadados
navigation-topic: security
title: Renovar o certificado de metadados SAML 2.0 do Adobe Workfront
description: O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Renovar o certificado de metadados SAML 2.0 do Adobe Workfront

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, nenhuma ação será necessária.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Os servidores da Adobe Workfront utilizam o protocolo SAML 2.0 para autenticação e autorização. Depois de atualizado, o novo certificado permanece válido por um ano. Quando é hora de renovar o certificado em seu provedor de identidade, você recebe um aviso no Workfront avisando que essa alteração deve ocorrer. Como administrador do Workfront, você pode gerenciar essa alteração no nível do sistema.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Isso não estará disponível se a instância do Workfront de sua organização estiver habilitada com o Adobe IMS. Consulte seu administrador de rede ou de TI se precisar de mais informações.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar o SAML 2.0 no Workfront

Para revisar a mensagem de aviso e reconhecer a atualização dos metadados SAML 2.0 em seu provedor de identidade:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Logon único**.

1. No **Tipo** , selecione **SAML 2.0**.

1. Clique em **Baixar metadados do SAML 2.0**.

   Isso baixa o certificado Workfront renovado para SAML 2.0, que contém os metadados corretos para o servidor.

   >[!CAUTION]
   >
   >Antes de fazer upload dos metadados do Workfront para seu provedor de Logon Único (SSO) na Etapa 5, copie o URL do Serviço de Consumidor de Asserção (ACS) atual para um local seguro. Esse URL, também conhecido como URL de resposta, é encontrado na página de configuração do Workfront do provedor SSO.
   >
   >
   >Se o URL do ACS for alterado após o upload dos metadados do Workfront, isso significa que os metadados podem conter um URL do ACS incorreto. Você deve alterá-lo de volta para o que copiou para evitar quebrar sua conexão de logon único. O certificado atualizado ainda estará correto depois que você fizer isso.

1. Vá para o servidor do provedor de identidade e atualize o novo certificado que você baixou.
1. Na Workfront, no **Página Logon único (SSO)**, verifique se esta opção está selecionada: **O novo certificado da Workfront já foi carregado no Provedor de identidade**.

   Quando esse campo é selecionado, os administradores do Workfront podem fazer logon no Workfront com suas credenciais de SSO ou suas credenciais do Workfront.

1. Clique em **Salvar**.

   A mensagem de aviso não é mais exibida porque você reconheceu a renovação do certificado SAML 2.0 no servidor do seu provedor de identidade.

1. Clique em **Testar conexão** para testar sua configuração.

   Você deve ver uma mensagem confirmando que a conexão foi bem-sucedida.

Para obter mais informações ou ajuda com a configuração manual de metadados, entre em contato com a Equipe de suporte, conforme explicado em [Entre em contato com o Suporte ao cliente](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
