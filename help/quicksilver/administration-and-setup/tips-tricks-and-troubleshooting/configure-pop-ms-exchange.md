---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configurar POP no Microsoft Exchange
description: Uma conta de email POP em  [!DNL Microsoft Exchange]  está desabilitada.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Configurar POP em [!DNL Microsoft Exchange]

## Problema

Conta de email POP em [!DNL Microsoft Exchange] desabilitada.

## Solução

Antes de gastar tempo resolvendo o problema, verifique se a conta POP do usuário está configurada corretamente. Se continuar a ter problemas depois de confirmar que a conta POP está configurada corretamente, contate o Suporte do [!DNL Microsoft] ou um de seus parceiros para obter ajuda adicional.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## Requisitos de acesso

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
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront]. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
