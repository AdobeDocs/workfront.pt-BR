---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,segurança,certificado,Admin,Isenção,configurar,metadados
navigation-topic: security
title: Renovar o certificado de metadados do Adobe Workfront SAML 2.0
description: Os servidores do Adobe Workfront utilizam o protocolo SAML 2.0 para autenticação e autorização. Depois de atualizado, o novo certificado permanece válido por um ano. Quando for a hora de renovar o certificado em seu provedor de identidade, você receberá um aviso na Workfront alertando que essa alteração deve ocorrer. Como administrador do Workfront, você pode gerenciar essa alteração no nível do sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Renovar o certificado de metadados do Adobe Workfront SAML 2.0

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas à Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, nenhuma ação será necessária.
>
>Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Os servidores do Adobe Workfront utilizam o protocolo SAML 2.0 para autenticação e autorização. Depois de atualizado, o novo certificado permanece válido por um ano. Quando for a hora de renovar o certificado em seu provedor de identidade, você receberá um aviso na Workfront alertando que essa alteração deve ocorrer. Como administrador do Workfront, você pode gerenciar essa alteração no nível do sistema.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Isso não estará disponível se a instância Workfront da sua organização estiver habilitada com o Adobe IMS. Consulte o administrador de rede ou de TI se precisar de mais informações.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o SAML 2.0 no Workfront

Para revisar a mensagem de aviso e confirmar a atualização dos metadados do SAML 2.0 no provedor de identidade:

{{step-1-to-setup}}

1. Clique em **Sistema** > **Logon único**.

1. No menu suspenso **Tipo**, selecione **SAML 2.0**.

1. Clique em **Baixar SAML 2.0 Metadata**.

   Isso baixa o certificado Workfront renovado para SAML 2.0, que contém os metadados corretos para o servidor.

1. Em seu provedor de identidade, copie o URL do Serviço do Consumidor de Asserção (ACS) atual (também conhecido como URL de Resposta) para um local seguro.

   >[!CAUTION]
   >
   >Antes de fazer upload dos metadados do Workfront para seu provedor de Logon único (SSO) na Etapa 6, copie seu URL atual do Serviço do consumidor de asserção (ACS) para um local seguro. Esse URL, também conhecido como URL de resposta, é encontrado na página de configuração do Workfront do seu provedor de SSO.
   >
   >
   >Se o URL do ACS for alterado depois que você fizer upload dos metadados do Workfront, significa que os metadados podem conter um URL do ACS incorreto. Você deve alterá-lo de volta para o que você copiou para evitar a interrupção da conexão de Logon único. Seu certificado atualizado ainda estará correto após você fazer isso.

1. No servidor do provedor de identidade, atualize o novo certificado baixado.
1. (Condicional) Se o URL do Serviço de Cliente de Asserção (ACS) ou o URL de Resposta tiver sido alterado no provedor de identidade, altere-o de volta para o URL copiado na Etapa 5.
1. Na Workfront, na **página Logon Único (SSO)**, verifique se esta opção está selecionada: **O novo certificado do Workfront já foi carregado para o Provedor de Identidade**.

   >[!NOTE]
   >
   >* Essa opção estará visível somente se todas as condições a seguir se aplicarem:
   >   * Sua organização já está configurada para SAML 2.0
   >   * O certificado atual está pronto para expirar
   >   * O novo certificado está disponível
   >* Quando esse campo é selecionado, os administradores do Workfront podem fazer logon no Workfront com suas credenciais de SSO ou as credenciais do Workfront.

1. Clique em **Salvar**.

   A mensagem de aviso não é mais exibida porque você confirmou a renovação do certificado SAML 2.0 no servidor do seu provedor de identidade.

1. Clique em **Testar Conexão** para testar sua configuração.

   Você deve ver uma mensagem confirmando que a conexão foi bem-sucedida.

Para obter mais informações ou para obter assistência com a configuração manual de metadados, entre em contato com nossa Equipe de Suporte, conforme explicado em [Entre em contato com o Suporte ao Cliente](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
