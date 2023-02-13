---
title: Arquivo de teste oculto
description: Oculto da pesquisa e da navegação à esquerda
hidefromtoc: true
hide: true
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: ea2fef66d50f07b05648356179d996d3aa4d23df
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 3%

---

# Visão geral da autenticação aprimorada

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

A Adobe Workfront está alterando o gerenciamento de sistema de usuários e senhas. Essas alterações serão implementadas em uma versão em fases chamada **Autenticação aprimorada** experiência. A Autenticação aprimorada oferece aos usuários uma experiência de logon mais consistente e segura em todos os produtos e serviços da Workfront.

A tabela a seguir fornece detalhes sobre a funcionalidade atual e futura:

>[!IMPORTANT]
>
>A maioria dos clientes está usando atualmente a Autenticação herdada e alguns estão usando a Autenticação aprimorada 1.0.
> 
>Para verificar qual tipo de autenticação você está usando atualmente, acesse *your_domain*.my.workfront.com/login. Se você for redirecionado para /auth/login, estará usando a Autenticação aprimorada 1.0.
> 
>Se você for redirecionado para https://login-a-xx.workfront.com/, onde &#39;xx&#39; pode ser EUA (Estados Unidos), UE (Europa) ou GCP (Google Cloud Platform) dependendo da sua localização/plataforma, você estará usando a Autenticação aprimorada 2.0.
>
>Todos os clientes serão transferidos para o Enhanced Authentication 2.0 até o final de 2021.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Recurso</strong> </p> </th> 
   <th><strong>Autenticação herdada</strong> </th> 
   <th><strong>Autenticação aprimorada 1.0</strong> </th> 
   <th> <p>Autenticação aprimorada 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Opções de logon</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que um único nome de usuário seja usado para todos os produtos e serviços da Workfront, incluindo treinamento, suporte e outros</p> </td> 
   <td>Não Disponível</td> 
   <td> <p>Não Disponível</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir o uso do mesmo endereço de email em instâncias do Workfront</p> </td> 
   <td> <p>✓</p> <p>Disponível a partir da versão 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponível a partir da versão 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponível a partir da versão 2019.3</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Endereços de email não diferenciam maiúsculas de minúsculas</p> </td> 
   <td> <p>✓</p> <p>Disponível a partir da versão 2019.3</p> </td> 
   <td> <p>✓</p> <p>Vários usuários não podem ter o mesmo endereço de email se o endereço for diferente somente por maiúsculas e minúsculas. </p> </td> 
   <td> <p>✓</p> <p>Vários usuários não podem ter o mesmo endereço de email se o endereço for diferente somente por maiúsculas e minúsculas. </p> <p>Os administradores do Workfront serão notificados até o final de 2019 para começar a corrigir endereços de email duplicados.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Opções de gerenciamento de senha</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Instale um email de redefinição de senha para um usuário como administrador do Workfront</p> </td> 
   <td> <p>Não Disponível </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Definir uma senha temporária para um usuário como administrador do Workfront</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Não planejado</p> <p>Essa funcionalidade não é uma prática recomendada de segurança</p> </td> 
   <td> <p>Não planejado</p> <p>Essa funcionalidade não é uma prática recomendada de segurança</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Requisitos da política de senha</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exigir que os usuários redefinam senhas após um determinado período</p> </td> 
   <td>✓</td> 
   <td> <p>Não planejado</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Restringir a utilização de uma senha anterior por utilizadores </p> </td> 
   <td>✓</td> 
   <td>Não planejado </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proteção contra tentativas incorretas de entrada de senha </p> </td> 
   <td> <p>✓ </p> <p>Bloqueia a conta depois de 5 tentativas incorretas de entrada de senha. O tempo de espera necessário após o bloqueio ser configurado pelo administrador do Workfront</p> </td> 
   <td> <p>✓</p> <p>O tempo de espera aumenta exponencialmente após cada senha sucessiva incorreta, com base nas práticas recomendadas do setor; o tempo necessário não pode ser configurado pelo administrador do Workfront</p> </td> 
   <td> <p>✓</p> <p>Usa um algoritmo de bloqueio que bloqueia proativamente uma variedade de comportamentos suspeitos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exigir uma combinação de caracteres em minúsculas, maiúsculas, números e especiais</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Maior flexibilidade na escolha de requisitos específicos</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Definir o comprimento mínimo da senha </p> </td> 
   <td> Não Disponível </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>Suporte ao protocolo de logon único</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Suporta integrações SSO compatíveis com protocolos Ative Diretory e LDAP</p> </td> 
   <td> ✓ </td> 
   <td> <p> Obsoleto</p> <p>Os sistemas Ative Diretory, Azure e LDAP devem usar SAML 2.0</p> </td> 
   <td> <p>Obsoleto</p> <p>Os sistemas Ative Diretory, Azure e LDAP podem ser configurados com o SAML 2.0 ou OpenID Connect criptografado.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Suporta protocolos SSO compatíveis com SAML 2.0 </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Suporta protocolos Open ID Connect</p> </td> 
   <td> <p>Não Disponível</p> </td> 
   <td> <p>Não Disponível</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Configure a página de logon do Workfront para sempre redirecionar para a página de logon do provedor de identidade </p> </td> 
   <td> Ativado por padrão e não pode ser desativado</td> 
   <td> <p>✓</p> <p>O administrador do Workfront pode configurar a página de logon para redirecionar para a página de logon do provedor de identidade ou pode configurar um botão ou botões de logon.</p> </td> 
   <td> <p>✓</p> <p> Os administradores do Workfront podem configurar a página de logon para redirecionar para a página de logon do provedor de identidade ou podem configurar um botão ou botões de logon.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que cada instância ative vários provedores de SSO</p> </td> 
   <td> <p>N/A</p> </td> 
   <td> <p>Não planejado</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Suporte ao ambiente</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Um único nome de usuário e senha para ambientes de Visualização</p> </td> 
   <td> <p>Não Disponível</p> </td> 
   <td> <p>Não Disponível</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Um único nome de usuário e senha para ambientes Sandbox</p> </td> 
   <td> <p>Não Disponível</p> </td> 
   <td> <p>Não Disponível</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
