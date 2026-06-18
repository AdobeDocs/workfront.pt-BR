---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Converter portfólios herdados em armazenamento em nuvem do Adobe
description: Converta portfólios herdados existentes de armazenamento do Workfront para o armazenamento em nuvem do Adobe na área Preferências de armazenamento, em Preferências do sistema.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 9%

---

# Converter portfólios herdados em armazenamento em nuvem do Adobe

Como administrador do Workfront, você pode converter portfólios herdados do armazenamento Workfront em armazenamento em nuvem do Adobe na área Preferências de armazenamento, em Preferências do sistema. Depois que um portfólio é convertido, ele se comporta como qualquer outro portfólio de armazenamento em nuvem da Adobe.

Para obter mais informações sobre como os portfólios convertidos se comportam e como seus objetos filho são afetados, consulte [Portabilidade de objetos](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability) em [Mover para o Workfront no Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).

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

## Antes de converter um portfólio

Antes de converter um portfólio de armazenamento Workfront herdado, considere o seguinte:

* A conversão afeta apenas o próprio portfólio. Os projetos e programas secundários que usam o armazenamento herdado do Workfront permanecem no armazenamento herdado.

  >[!NOTE]
  >
  >Um programa herdado secundário converte automaticamente para o Adobe Cloud Storage somente quando alguém adiciona manualmente um projeto do Adobe Cloud Storage a ele.
* Os documentos e as pastas de documentos no portfólio permanecem no armazenamento herdado do Workfront após a conversão.
* Após a conversão, não é possível adicionar projetos de armazenamento herdados do Workfront ao portfólio.

## Converter portfólios herdados em armazenamento em nuvem do Adobe

Para converter um ou mais portfólios de armazenamento herdados do Workfront em armazenamento em nuvem do Adobe:

{{step-1-to-setup}}

1. Selecione **Sistema** na navegação à esquerda e **Preferências**.

1. Role para baixo até a seção **Preferências de Armazenamento**.

1. No campo **Selecionar portfólios para conversão em armazenamento na nuvem do Adobe**, selecione um ou mais portfólios de armazenamento herdados do Workfront.

1. Clique em **Salvar**.

   Uma mensagem de confirmação é exibida descrevendo o que acontece quando um portfólio é convertido:

   * Não é mais possível mover projetos de armazenamento herdados do Workfront para o portfólio.
   * Todos os novos projetos criados no portfólio usam o Adobe Cloud Storage.
   * O Frame.io é o visualizador de documentos nos projetos de armazenamento em nuvem do Adobe do portfólio.
   * Os projetos secundários que usam o armazenamento Workfront herdado permanecem no armazenamento herdado.
   * Os programas secundários permanecem no armazenamento herdado.

1. Clique em **Converter** para confirmar.

   Os portfólios selecionados são convertidos para o Adobe Cloud Storage.
