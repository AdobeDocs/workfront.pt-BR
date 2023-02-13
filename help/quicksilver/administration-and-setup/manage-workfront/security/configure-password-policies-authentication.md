---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurar políticas de senha para autenticação
description: Como administrador do Adobe Workfront, você pode configurar as opções de política de senha para personalizar a experiência de autenticação no seu sistema Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 2%

---

# Configurar políticas de senha para autenticação

{{important-admin-console-onboard}}

Como administrador do Adobe Workfront, você pode configurar as opções de política de senha para personalizar a experiência de autenticação no seu sistema Workfront.

Recomendamos que você configure as preferências de autenticação durante a implementação do Workfront e apenas as revisite ocasionalmente depois.

Os recursos aprimorados de gerenciamento de senha serão disponibilizados em breve ou já podem estar disponíveis para sua organização. Use qualquer uma das seções a seguir, dependendo se sua organização tem acesso à nova experiência de autenticação.

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

## Configurar autenticação (disponível para todos os clientes) {#configure-authentication-available-for-all-customers}

As opções de autenticação são exibidas para todos os clientes. Os recursos aprimorados de gerenciamento de senha serão disponibilizados em breve ou já podem estar disponíveis para a sua organização, conforme descrito na seção [Configurar autenticação aprimorada (em breve)](#configure-enhanced-authentication-coming-soon) neste artigo.

Para configurar preferências de autenticação:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Autenticação**.

1. Selecione qualquer um dos seguintes campos para estabelecer as configurações de autenticação da sua organização:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Forçar usuários a redefinir sua senha a cada <em>&lt;value&gt;</em> dias</td> 
      <td>Isso estabelece o período de tempo para os usuários redefinirem sua senha do Workfront. Por padrão, essa opção está desativada. Ao habilitá-lo, você pode escolher entre 30, 60, 90, 120, 180 dias. O padrão é 30 dias.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Não permitir que os usuários definam a mesma senha que qualquer uma das anteriores <em>&lt;value&gt;</em> senhas</td> 
      <td> <p>Este campo proíbe que os usuários reutilizem senhas para um número definido de redefinições. Por padrão, esse campo está desativado. Ao habilitá-la, você pode definir esse valor como 5, 10 ou 15 redefinições antes que uma senha possa ser reutilizada.</p> <p>Quando essa opção é selecionada, os usuários não podem redefinir suas senhas mais de uma vez em um determinado dia</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Se uma senha incorreta for inserida cinco vezes consecutivas, bloqueie a conta para <em>&lt;value&gt;</em> minutos: </td> 
      <td> <p>Selecione por quanto tempo um usuário ficará bloqueado no Workfront depois de digitar uma senha incorreta cinco vezes consecutivas. Por padrão, essa opção está ativada e a quantidade de tempo de espera é de 10 minutos. Você pode bloquear contas por 10 minutos, 30 minutos, 1 hora, 8 horas ou 24 horas. </p> <p>A redefinição manual da senha do usuário substitui esse valor de espera padrão. <br>Os usuários podem redefinir suas próprias senhas quando bloqueadas pela tela de logon. Para obter mais informações sobre como eles podem redefinir a senha, se esquecerem, consulte <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Redefinir senha</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">As senhas devem conter pelo menos <em>&lt;value&gt;</em> diferentes tipos de caracteres:</td> 
      <td> <p>Determina a força que as senhas devem ter ao permitir que você selecione o número de diferentes tipos de caracteres necessários em suas senhas.</p> <p>Uma palavra de dicionário reconhecível não pode ser usada como senha.<br>Por padrão, o Workfront exige que pelo menos 2 dos seguintes estejam presentes em senhas (você também pode exigir que 3 desses caracteres estejam presentes para uma senha válida): </p> 
       <ul> 
        <li>Caracteres em maiúsculas</li> 
        <li>Caracteres minúsculos</li> 
        <li>Números</li> 
        <li>Símbolos</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

## Configurar autenticação aprimorada (em breve) {#configure-enhanced-authentication-coming-soon}

Esta seção descreve a experiência de autenticação aprimorada, que pode ainda não estar disponível para sua organização. Se sua organização não tiver migrado para a nova experiência de autenticação, você deverá definir as configurações de autenticação, conforme descrito em [Configurar autenticação (disponível para todos os clientes)](#configure-authentication-available-for-all-customers).

Para configurar preferências de autenticação aprimoradas:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Autenticação aprimorada**.
1. No **Comprimento da senha** digite o número mínimo de caracteres necessários para uma senha válida.

   O Workfront requer pelo menos 6 caracteres.

1. (Opcional) Na seção **Requisitos de senha** selecione os tipos de caracteres necessários nas senhas do usuário.

   Você pode aumentar a força das senhas do usuário exigindo qualquer um ou todos os tipos de caracteres na seção Requisito de senha . As seguintes opções estão disponíveis:

   | Letras Minúsculas | Exigir pelo menos uma letra minúscula |
   |---|---|
   | Letras Maiúsculas | Exigir pelo menos uma letra maiúscula |
   | Números | Exigir pelo menos um número |
   | Caracteres especiais | Exigir pelo menos um caractere especial |

   {style=&quot;table-layout:auto&quot;}

1. Clique em **Salvar**.
