---
title: Visão geral da autenticação aprimorada
description: Oculto da pesquisa e da navegação à esquerda
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: bf8e6c2b8a45cf65840a2ac8b3c25d11266d49f9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Visão geral da autenticação aprimorada

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

O Adobe Workfront está alterando o gerenciamento de sistema de usuários e senhas. Essas alterações serão implementadas em uma versão em fases chamada **Autenticação aprimorada** experiência. A Autenticação aprimorada oferece aos usuários uma experiência de logon mais consistente e segura em todos os produtos e serviços da Workfront.

A tabela a seguir fornece detalhes sobre a funcionalidade atual e futura:

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
   <td>Não disponível</td> 
   <td> <p>Não disponível</p> </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir o uso do mesmo endereço de email em instâncias do Workfront</p> </td> 
   <td> <p>✓ µ</p> <p>Disponível a partir da versão 2019.3</p> </td> 
   <td> <p>✓ µ</p> <p>Disponível a partir da versão 2019.3</p> </td> 
   <td> <p>✓ µ</p> <p>Disponível a partir da versão 2019.3</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Os endereços de email não diferenciam maiúsculas de minúsculas</p> </td> 
   <td> <p>✓ µ</p> <p>Disponível a partir da versão 2019.3</p> </td> 
   <td> <p>✓ µ</p> <p>Vários usuários não podem ter o mesmo endereço de email se o endereço for diferente somente por letras maiúsculas e minúsculas. </p> </td> 
   <td> <p>✓ µ</p> <p>Vários usuários não podem ter o mesmo endereço de email se o endereço for diferente somente por letras maiúsculas e minúsculas. </p> <p>Os administradores do Workfront serão notificados no final de 2019 para começar a corrigir endereços de email duplicados.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Opções de gerenciamento de senhas</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Instigar um email de redefinição de senha para um usuário como administrador do Workfront</p> </td> 
   <td> <p>Não disponível </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Defina uma senha temporária para um usuário como administrador do Workfront</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>Não planejado</p> <p>Esta funcionalidade não é uma prática recomendada de segurança</p> </td> 
   <td> <p>Não planejado</p> <p>Esta funcionalidade não é uma prática recomendada de segurança</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Requisitos da política de senha</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exigir que os usuários redefinam senhas após um determinado período</p> </td> 
   <td>✓ µ</td> 
   <td> <p>Não planejado</p> </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Restringir usuários de usar uma senha anterior </p> </td> 
   <td>✓ µ</td> 
   <td>Não planejado </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proteção contra tentativas incorretas de entrada de senha </p> </td> 
   <td> <p>✓ µ </p> <p>Bloqueia a conta após 5 tentativas incorretas de entrada de senha. O tempo de espera necessário após o bloqueio é configurado pelo administrador do Workfront</p> </td> 
   <td> <p>✓ µ</p> <p>O tempo de espera aumenta exponencialmente após cada senha incorreta sucessiva com base nas práticas recomendadas do setor; o tempo necessário não pode ser configurado pelo administrador do Workfront</p> </td> 
   <td> <p>✓ µ</p> <p>Usa um algoritmo de bloqueio que bloqueia proativamente uma variedade de comportamentos suspeitos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Requer uma combinação de minúsculas, maiúsculas, números e caracteres especiais</p> </td> 
   <td>✓ µ</td> 
   <td> <p>✓ µ </p> <p>Maior flexibilidade na escolha de requisitos específicos</p> </td> 
   <td> <p>✓ µ</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Definir um comprimento mínimo de senha </p> </td> 
   <td> Não disponível </td> 
   <td> ✓ µ </td> 
   <td> <p>✓ µ</p> </td> 
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
   <td colspan="3"> <p><strong>Suporte ao Single Sign-On Protocol</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Oferece suporte a integrações SSO compatíveis com o Ative Diretory e os protocolos LDAP</p> </td> 
   <td> ✓ µ </td> 
   <td> <p> Obsoleto</p> <p>Os sistemas Ative Diretory, Azure e LDAP devem usar o SAML 2.0</p> </td> 
   <td> <p>Obsoleto</p> <p>Os sistemas Ative Diretory, Azure e LDAP podem ser configurados com SAML 2.0 criptografado ou OpenID Connect.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Suporta protocolos SSO compatíveis com SAML 2.0 </p> </td> 
   <td>✓ µ</td> 
   <td> ✓ µ </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Suporta protocolos Open ID Connect</p> </td> 
   <td> <p>Não disponível</p> </td> 
   <td> <p>Não disponível</p> </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Configure a página de logon do Workfront para sempre redirecionar para a página de logon do provedor de identidade </p> </td> 
   <td> Ativado por padrão e não pode ser desativado</td> 
   <td> <p>✓ µ</p> <p>O administrador do Workfront pode configurar a página de logon para redirecionar para a página de logon do provedor de identidade ou pode configurar um ou mais botões de logon.</p> </td> 
   <td> <p>✓ µ</p> <p> Os administradores do Workfront podem configurar a página de logon para redirecionar para a página de logon do provedor de identidade ou podem configurar um ou mais botões de logon.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que cada instância habilite vários provedores de SSO</p> </td> 
   <td> <p>N/A</p> </td> 
   <td> <p>Não planejado</p> </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Suporte a ambiente</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Um único nome de usuário e senha para ambientes de Visualização</p> </td> 
   <td> <p>Não disponível</p> </td> 
   <td> <p>Não disponível</p> </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Um único nome de usuário e senha para ambientes de sandbox</p> </td> 
   <td> <p>Não disponível</p> </td> 
   <td> <p>Não disponível</p> </td> 
   <td> <p>✓ µ</p> </td> 
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
