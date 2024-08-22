---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Erro: o usuário autoprovisionado não consegue fazer logon"
description: Se um usuário provisionado automaticamente tentar fazer logon pela primeira vez e receber um erro informando que o sistema não está atribuindo a ele um nível de acesso, talvez isso ocorra porque seu sistema não tem níveis de acesso associados à licença de solicitação.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 2%

---

# Erro: o usuário autoprovisionado não consegue fazer logon

Quando um usuário provisionado automaticamente tenta fazer logon pela primeira vez, ele recebe o seguinte erro:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problema

O sistema não está atribuindo um nível de acesso ao novo usuário.

Por padrão, o provisionamento automático usa o tipo Solicitar licença. Quando não existem níveis de acesso com uma licença de solicitação, o sistema não pode atribuir um nível de acesso ao usuário.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solução

Criar um nível de acesso básico com uma licença de Solicitação:

1. Vá para **[!UICONTROL Configuração]** > **[!UICONTROL Níveis de Acesso]**.

1. Clique em **[!UICONTROL Novo Nível de Acesso]**.
1. Insira um **[!UICONTROL Nome]**.
1. No menu suspenso **[!UICONTROL Tipo de licença]**, selecione Solicitar.
1. Clique em **[!UICONTROL Salvar alterações]**.

Depois de criar um nível de acesso com uma licença de Solicitação, peça ao usuário para fazer logon com suas credenciais de SSO.


