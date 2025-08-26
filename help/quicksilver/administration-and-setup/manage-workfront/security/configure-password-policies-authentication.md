---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurar políticas de senha para autenticação
description: Como administrador do Adobe Workfront, você pode configurar opções de política de senha para personalizar a experiência de autenticação para seu sistema Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 3%

---

# Configurar políticas de senha para autenticação

{{important-admin-console-onboard}}

Como administrador do Adobe Workfront, você pode configurar opções de política de senha para personalizar a experiência de autenticação para seu sistema Workfront.

Recomendamos que você configure as preferências de autenticação durante a implementação do Workfront e somente ocasionalmente as revisite posteriormente.

Recursos aprimorados de gerenciamento de senhas serão oferecidos em breve ou já podem estar disponíveis para a sua organização. Use qualquer uma das seções a seguir, dependendo se sua organização tem acesso à nova experiência de autenticação.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurar autenticação (disponível para todos os clientes) {#configure-authentication-available-for-all-customers}

As opções de autenticação são exibidas para todos os clientes. Recursos aprimorados de gerenciamento de senhas serão oferecidos em breve ou já podem estar disponíveis para a sua organização, conforme descrito na seção [Configurar autenticação aprimorada)](#configure-enhanced-authentication-coming-soon) deste artigo.

Para configurar preferências de autenticação:

{{step-1-to-setup}}

1. Clique em **Sistema** > **Autenticação**.

1. Selecione qualquer um dos campos a seguir para estabelecer as configurações de autenticação para sua organização:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Força os usuários a redefinirem suas senhas a cada <em>&lt;value&gt;</em> dias</td> 
      <td>Isso estabelece o período para que os usuários redefinam suas senhas do Workfront. Por padrão, essa opção está desativada. Ao habilitá-lo, você pode escolher entre 30, 60, 90, 120, 180 dias. O padrão é 30 dias.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Não permitir que os usuários definam a mesma senha que qualquer uma de suas <em>&lt;value&gt;</em> senhas anteriores</td> 
      <td> <p>Esse campo proíbe que os usuários reutilizem senhas para um número definido de redefinições. Por padrão, esse campo está desativado. Ao habilitá-lo, você pode definir esse valor como 5, 10 ou 15 redefinições antes que uma senha possa ser reutilizada.</p> <p>Quando essa opção é selecionada, os usuários não podem redefinir suas senhas mais de uma vez em um determinado dia</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Se uma senha incorreta for inserida cinco vezes consecutivas, bloquear a conta por <em>&lt;value&gt;</em> minutos: </td> 
      <td> <p>Selecione por quanto tempo um usuário será bloqueado no Workfront após inserir uma senha incorreta cinco vezes consecutivas. Por padrão, essa opção está ativada e o tempo de espera é de 10 minutos. Você pode bloquear contas por 10 minutos, 30 minutos, 1 hora, 8 horas ou 24 horas. </p> <p>A redefinição manual da senha do usuário substitui esse valor de espera padrão. <br>Os usuários podem redefinir suas próprias senhas quando bloqueados pela tela de logon. Para obter mais informações sobre como eles podem redefinir a senha, caso tenham esquecido, consulte <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Redefinir sua senha</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">As senhas devem conter pelo menos <em>&lt;valor&gt;</em> tipos diferentes de caracteres:</td> 
      <td> <p>Determina a intensidade exigida das senhas de usuário, permitindo selecionar o número de diferentes tipos de caracteres necessários nas senhas.</p> <p>Uma palavra reconhecível do dicionário não pode ser usada como senha.<br>Por padrão, o Workfront exige que pelo menos dois dos seguintes caracteres estejam presentes em senhas (você também pode exigir que três desses caracteres estejam presentes para uma senha válida): </p> 
       <ul> 
        <li>Caracteres em maiúsculas</li> 
        <li>Caracteres em minúsculas</li> 
        <li>Números</li> 
        <li>Símbolos</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

## Configurar autenticação aprimorada{#configure-enhanced-authentication-coming-soon}

Esta seção descreve a experiência de autenticação aprimorada, que pode ainda não estar disponível para a sua organização. Se sua organização não tiver sido migrada para a nova experiência de autenticação, defina as configurações de autenticação, conforme descrito em [Configurar autenticação (disponível para todos os clientes)](#configure-authentication-available-for-all-customers).

Para configurar preferências de autenticação aprimoradas:

{{step-1-to-setup}}

1. Clique em **Sistema** > **Autenticação aprimorada**.
1. Na caixa **Comprimento da Senha**, digite o número mínimo de caracteres necessários para uma senha válida.

   O Workfront exige pelo menos 6 caracteres.

1. (Opcional) Na seção **Requisitos de Senha**, selecione os tipos de caracteres necessários nas senhas do usuário.

   Você pode aumentar a força das senhas de usuários exigindo qualquer um ou todos os tipos de caracteres na seção Requisito de senha. As opções disponíveis são as seguintes:

   | Letras Minúsculas | Exigir pelo menos uma letra minúscula |
   |---|---|
   | Letras Maiúsculas | Exigir pelo menos uma letra maiúscula |
   | Números | Exigir pelo menos um número |
   | Caracteres especiais | Exigir pelo menos um caractere especial |

   {style="table-layout:auto"}

1. Clique em **Salvar**.
