---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configurar POP no Microsoft Exchange
description: Uma conta de email POP em [!DNL Microsoft Exchange] está desativado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Configurar POP em [!DNL Microsoft Exchange]

## Problema

Uma conta de email POP em [!DNL Microsoft Exchange] está desativado.

## Solução

Antes de gastar tempo solucionando o problema, verifique se a conta POP do usuário está configurada corretamente. Se você continuar tendo problemas depois de confirmar que a conta do POP está configurada corretamente, entre em contato com [!DNL Microsoft] Suporte ou um de seus parceiros para obter ajuda adicional.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar POP em [!DNL Microsoft Exchange]

>[!NOTE]
>
>As etapas a seguir podem ser usadas como um guia geral para configurar o POP no [!DNL Microsoft Exchange] para uma produção [!DNL Workfront] sistema. As etapas podem diferir significativamente, dependendo da versão do Exchange ou das alterações de código feitas pelo Microsoft.

1. Inicie e habilite o serviço POP3 no servidor Exchange 2010.

   >[!NOTE]
   >
   >Por padrão, o serviço POP3 não é iniciado.

   1. Iniciar [!DNL Microsoft]Gerenciador do Servidor do .
   1. Navegar: **[!UICONTROL Gerenciador do servidor]** > **[!UICONTROL Configuração]** >**[!UICONTROL Firewall do Windows com Segurança Avançada]** > **[!UICONTROL Serviços]**.

   1. Clique com o botão direito do mouse **[!DNL Microsoft Exchange]POP3**, depois clique em **[!UICONTROL Propriedades]**.

   1. (Condicional) Para garantir que o serviço POP seja iniciado automaticamente, no **[!UICONTROL Geral]** , defina a variável **[!UICONTROL Inicialização]** digitar para [!UICONTROL Automático].

1. Configure o POP3 para o servidor.

   1. Inicie o [!DNL Microsoft Exchange] Console de gerenciamento.
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange no local]** > **[!UICONTROL Configuração do servidor]** > **[!UICONTROL Acesso ao cliente]**.

   1. Choose **[!UICONTROL POP3]**.

      O POP3 está na lista abaixo do [!UICONTROL POP3] e [!UICONTROL IMAP4] guias.

   1. Do lado direito embaixo **[!UICONTROL Ações]**, selecione **[!UICONTROL POP3]** e escolha **[!UICONTROL Propriedades]**.

   1. Clique em **[!UICONTROL Propriedades POP3]**, em seguida, abra o **[!UICONTROL Vínculo]** guia .

      Todos os endereços IP e números de porta disponíveis configurados para o servidor POP3 são exibidos. A caixa superior mostra o arquivo Não criptografado e a caixa inferior mostra o IP e as portas para conexões SSL/TLS.

   1. Clique em **[!UICONTROL Propriedades POP3]**, em seguida, abra o **[!UICONTROL Autenticação]** guia .

   1. **[!UICONTROL Selecionar seguro]** fazer logon.

      É necessária uma conexão TLS para o cliente se autenticar no servidor.

1. Habilite ou permita que usuários se conectem ao POP.

   1. Inicie o [!DNL Microsoft Exchange] Console de gerenciamento.
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange no local]** > **[!UICONTROL Configuração do destinatário]** > **[!UICONTROL Caixa de Correio]**.

      Uma lista de caixas de correio ou usuários é exibida.

   1. Destaque o email que está sendo usado em [!DNL Workfront].
   1. Do lado direito embaixo **[!UICONTROL Ações]**, selecione **[!UICONTROL Propriedades]**, em seguida, abra o **[!UICONTROL Recursos da Caixa de Correio]** guia .

   1. (Condicional) Se POP3 estiver desativado, clique em **[!UICONTROL POP3]**, depois clique em **[!UICONTROL Habilitar]**.

      Uma lista de caixas de correio ou usuários é exibida.

1. Configurar conectores de recepção.

   1. Iniciar [!DNL Microsoft Exchange] Console de gerenciamento.
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange no local]** > **[!UICONTROL Configuração do servidor]** > **[!UICONTROL Transporte de Hub]**.

      Uma lista de conectores de recepção é exibida.

   1. Confirmar o conector de recepção *Cliente* *EX01* estiver ativado.

      Onde *Cliente* *EX01* é o nome do seu servidor Exchange.

   1. Selecionar *EX01 do cliente*, em seguida à direita sob **[!UICONTROL Ações]**, selecione **[!UICONTROL Propriedades]**.

   1. Abra o **[!UICONTROL Autenticação]** e, em seguida, verifique **[!UICONTROL Segurança da camada de transporte (TLS)]** está marcada.

      >[!NOTE]
      >
      >Para ter a Autenticação Básica, talvez seja necessário iniciar o TLS e a Autenticação Integrada do Windows.
