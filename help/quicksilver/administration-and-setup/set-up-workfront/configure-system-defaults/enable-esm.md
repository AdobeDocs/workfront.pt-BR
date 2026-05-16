---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Habilitar o armazenamento em nuvem do Adobe para sua organização
description: Você pode habilitar o armazenamento em nuvem da Adobe para que sua organização use uma solução de armazenamento unificado para todos os produtos da Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 7%

---

# Habilitar o armazenamento em nuvem do Adobe para sua organização

O Adobe Cloud Storage é uma solução de armazenamento unificado para todos os produtos da Adobe. É uma solução de armazenamento em nuvem que serve como repositório central para ativos em produtos corporativos da Adobe.

O armazenamento na nuvem do Adobe é ativado por padrão para novos clientes e pode ser ativado para clientes existentes após a renovação do contrato.

Para obter mais informações sobre o Adobe Cloud Storage, consulte [Visão geral do Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer pacote de fluxo de trabalho</p></td> 
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

## Habilitar o armazenamento em nuvem do Adobe para sua organização

Para habilitar o Adobe Cloud Storage para sua organização:

{{step-1-to-setup}}

1. Selecione **Sistema** na navegação à esquerda e **Preferências**.
1. Role até a seção **Preferências de armazenamento**.
1. No menu suspenso Padrão, selecione **Adobe cloud storage**.
1. (Opcional) Se quiser usar uma combinação de armazenamento em nuvem do Adobe e Armazenamento herdado do Workfront, marque a caixa de seleção **Permitir que o usuário selecione o provedor de armazenamento**.

   >[!NOTE]
   >
   >Habilitar essa opção permite que os usuários selecionem o provedor de armazenamento quando criarem um novo projeto. O armazenamento na nuvem do Adobe é rotulado como &quot;Novo projeto&quot;, pois é o provedor de armazenamento padrão. O armazenamento herdado do Workfront é rotulado como &quot;Projeto herdado&quot;.
   >
   >![opções de projeto novo e herdado](assets/new-esm-project.png)

1. No menu suspenso Aplica-se a, escolha uma das seguintes opções:

   - **Organização inteira**: essa opção aplica o provedor de armazenamento padrão a todo o ambiente do Workfront. Sempre que um usuário criar um novo projeto, o provedor de armazenamento padrão será usado.
   - **Grupos específicos**: essa opção aplica o provedor de armazenamento padrão somente a grupos específicos dentro da organização. Sempre que um usuário nos grupos especificados criar um novo projeto, o provedor de armazenamento padrão será usado

1. Clique em **Salvar**.

   >[!NOTE]
   >
   >Os projetos existentes mantêm o modelo de armazenamento com o qual foram criados. Por exemplo, os projetos que usam o Adobe Cloud Storage continuam a usar o Adobe Cloud Storage após alterar a preferência de armazenamento padrão.

## Armazenamento em nuvem do Adobe em ambientes de sandbox

O armazenamento na nuvem do Adobe está disponível em ambientes de sandbox [!DNL Workfront], permitindo testar a funcionalidade descrita neste artigo antes de implantá-lo na produção. No entanto, o visualizador Frame.io não está disponível na sandbox, portanto, a experiência de revisão e aprovação unificada completa deve ser validada na produção.

Se você tiver uma sandbox de atualização personalizada, atualize-a depois de atualizar para uma versão do Workfront compatível com o armazenamento em nuvem da Adobe. A atualização fornece à sandbox acesso à funcionalidade de armazenamento em nuvem do Adobe para que você possa começar a testá-la. Para obter mais informações, consulte [O [!DNL Adobe Workfront] ambiente de Sandbox de Atualização Personalizada](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).
