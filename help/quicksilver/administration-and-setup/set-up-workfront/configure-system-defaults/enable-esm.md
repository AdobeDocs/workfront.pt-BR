---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Ativar o armazenamento corporativo da Adobe para sua organização
description: Você pode habilitar o armazenamento empresarial da Adobe para que sua organização use uma solução de armazenamento unificado para todos os produtos da Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 97c351ca38a8b6075634b2f755f2330562bc8b52
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 13%

---

# Habilitar o armazenamento corporativo da Adobe para sua organização

O armazenamento corporativo da Adobe é uma solução de armazenamento unificado para todos os produtos da Adobe. É uma solução de armazenamento em nuvem que serve como repositório central para ativos em produtos corporativos da Adobe.

o armazenamento corporativo da Adobe é ativado por padrão para novos clientes e pode ser ativado para clientes existentes mediante renovação de contrato.

Para obter mais informações sobre o Adobe enterprise storage, consulte [visão geral do Adobe enterprise storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão</p> <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador do Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Habilitar o armazenamento corporativo da Adobe para sua organização

Para habilitar o armazenamento corporativo da Adobe para sua organização:

{{step-1-to-setup}}

1. Selecione **Sistema** na navegação à esquerda e **Preferências**.
1. Role até a seção **Preferências de armazenamento**.
1. No menu suspenso Padrão, selecione **Adobe enterprise storage**.
1. (Opcional) Se quiser usar uma combinação de armazenamento corporativo Adobe e Armazenamento herdado do Workfront, marque a caixa de seleção **Permitir que o usuário selecione o provedor de armazenamento**.

   >[!NOTE]
   >
   >Habilitar essa opção permite que os usuários selecionem o provedor de armazenamento quando criarem um novo projeto. o armazenamento corporativo é rotulado como &quot;Novo projeto&quot;, pois é o provedor de armazenamento padrão. O armazenamento herdado do Workfront é rotulado como &quot;Projeto herdado&quot;.
   >
   >![opções de projeto novo e herdado](assets/new-esm-project.png)

1. Clique em **Salvar**.