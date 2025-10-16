---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configurar POP no Microsoft Exchange
description: Uma conta de email POP em  [!DNL Microsoft Exchange]  está desabilitada.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Configurar POP em [!DNL Microsoft Exchange]

## Problema

Conta de email POP em [!DNL Microsoft Exchange] desabilitada.

## Solução

Antes de gastar tempo resolvendo o problema, verifique se a conta POP do usuário está configurada corretamente. Se continuar a ter problemas depois de confirmar que a conta POP está configurada corretamente, contate o Suporte do [!DNL Microsoft] ou um de seus parceiros para obter ajuda adicional.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar POP em [!DNL Microsoft Exchange]

>[!NOTE]
>
>As etapas a seguir podem ser usadas como um guia geral para configurar POP em [!DNL Microsoft Exchange] para um sistema de produção [!DNL Workfront]. As etapas podem diferir significativamente, dependendo da versão do Exchange ou das alterações de código feitas pelo Microsoft.

1. Inicie e habilite o serviço POP3 no servidor Exchange 2010.

   >[!NOTE]
   >
   >Por padrão, o serviço POP3 não é iniciado.

   1. Inicie o Gerenciador de Servidores do [!DNL Microsoft].
   1. Navegar: **[!UICONTROL Gerenciador do Servidor]** > **[!UICONTROL Configuração]** >**[!UICONTROL Firewall do Windows com Segurança Avançada]** > **[!UICONTROL Serviços]**.

   1. Clique com o botão direito do mouse em **[!DNL Microsoft Exchange]POP3** e em **[!UICONTROL Propriedades]**.

   1. (Condicional) Para garantir que o serviço POP seja iniciado automaticamente, na guia **[!UICONTROL Geral]**, defina o tipo **[!UICONTROL Inicialização]** como [!UICONTROL Automática].

1. Configure o POP3 para o servidor.

   1. Inicie o console de Gerenciamento [!DNL Microsoft Exchange].
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange No Local]** > **[!UICONTROL Configuração Do Servidor]** > **[!UICONTROL Acesso Para Cliente]**.

   1. Escolha **[!UICONTROL POP3]**.

      O POP3 está na lista nas guias [!UICONTROL POP3] e [!UICONTROL IMAP4].

   1. No lado direito, em **[!UICONTROL Ações]**, selecione **[!UICONTROL POP3]** e escolha **[!UICONTROL Propriedades]**.

   1. Clique em **[!UICONTROL Propriedades POP3]** e abra a guia **[!UICONTROL Associação]**.

      Todos os endereços IP e números de porta disponíveis configurados para o servidor POP3 são exibidos. A caixa superior mostra a opção Não criptografado e a caixa inferior mostra as portas e IP para conexões SSL/TLS.

   1. Clique em **[!UICONTROL Propriedades POP3]** e abra a guia **[!UICONTROL Autenticação]**.

   1. **[!UICONTROL Selecione um logon seguro]**.

      Uma conexão TLS é necessária para que o cliente se autentique no servidor.

1. Habilite ou permita que os usuários se conectem a POP.

   1. Inicie o console de Gerenciamento [!DNL Microsoft Exchange].
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange No Local]** > **[!UICONTROL Configuração De Destinatário]** > **[!UICONTROL Caixa De Correio]**.

      Uma lista de caixas de correio ou usuários é exibida.

   1. Realçar o email que está sendo usado dentro de [!DNL Workfront].
   1. No lado direito, em **[!UICONTROL Ações]**, selecione **[!UICONTROL Propriedades]** e abra a guia **[!UICONTROL Recursos da Caixa de Correio]**.

   1. (Condicional) Se o POP3 estiver desabilitado, clique em **[!UICONTROL POP3]** e em **[!UICONTROL Habilitar]**.

      Uma lista de caixas de correio ou usuários é exibida.

1. Configurar conectores de recebimento.

   1. Inicie o console de gerenciamento [!DNL Microsoft Exchange].
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange No Local]** > **[!UICONTROL Configuração Do Servidor]** > **[!UICONTROL Transporte De Hub]**.

      Uma lista de conectores de recebimento é exibida.

   1. Confirme se o conector de recebimento *Client* *EX01* está habilitado.

      Onde *Client* *EX01* é o nome do seu servidor Exchange.

   1. Selecione *Client EX01* e, à direita, em **[!UICONTROL Actions]**, selecione **[!UICONTROL Properties]**.

   1. Abra a guia **[!UICONTROL Autenticação]** e verifique se **[!UICONTROL Transport Layer Security (TLS)]** está marcado.

      >[!NOTE]
      >
      >Para ter a Autenticação Básica, talvez seja necessário iniciar o TLS e a Autenticação Integrada do Windows.
