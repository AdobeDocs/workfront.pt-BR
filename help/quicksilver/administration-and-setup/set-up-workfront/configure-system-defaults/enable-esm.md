---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Ativar o armazenamento corporativo da Adobe para sua organização
description: Você pode habilitar o armazenamento empresarial da Adobe para que sua organização use uma solução de armazenamento unificado para todos os produtos da Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 10%

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

1. No menu suspenso Aplica-se a, escolha uma das seguintes opções:

   - **Organização inteira**: essa opção aplica o provedor de armazenamento padrão a todo o ambiente do Workfront. Sempre que um usuário criar um novo projeto, o provedor de armazenamento padrão será usado.
   - **Grupos específicos**: essa opção aplica o provedor de armazenamento padrão somente a grupos específicos dentro da organização. Sempre que um usuário nos grupos especificados criar um novo projeto, o provedor de armazenamento padrão será usado

1. Clique em **Salvar**.
