---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Tipo de licença de usuário externo ausente nos níveis de acesso
description: Não consigo mais ver o tipo de licença de Usuário Externo em Níveis de Acesso em Configuração.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 2%

---

# Tipo de licença de usuário externo ausente nos níveis de acesso

## Problema

Não consigo mais ver o tipo de licença de Usuário Externo em Níveis de Acesso em Configuração.

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

## Solução

1. Vá para **[!UICONTROL Configuração]** > **[!UICONTROL Sistema]** > **[!UICONTROL Preferências]**.

1. Na seção **[!UICONTROL Segurança]**, verifique se a opção **[!UICONTROL Colaborar com pessoas sem contas do Workfront usando seus endereços de email]** está habilitada.

   Se essa opção não estiver ativada, o usuário externo não aparecerá na Configuração do nível de acesso.
