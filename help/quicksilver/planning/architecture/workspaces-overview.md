---
title: Visão geral dos espaços de trabalho
description: Um espaço de trabalho é uma coleção de tipos de registro usados por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning para corresponder aos fluxos de trabalho de suas unidades organizacionais.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
TQID: https://experienceleague.adobe.com/Hh1Gh4ex1dLrPhsmqiLv3x5NAU0yKzIwcsV4hEogXTo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: bd1c8dfc4b03b4b8d9948da278406addf801d226
workflow-type: tm+mt
source-wordcount: 516
ht-degree: 3%

---

# Visão geral dos espaços de trabalho

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Um espaço de trabalho é uma coleção de tipos de registro usados por uma unidade organizacional e representa o ciclo de vida e os processos de trabalho da unidade. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning.

<!--update screenshot with production, it was broken at Preview-->

![Conta de administrador da página de aterrissagem do Workspaces](assets/workspaces-landing-page-admin-account.png)

## Considerações sobre espaços de trabalho

* Você pode criar espaços de trabalho para unidades organizacionais específicas na sua organização, para corresponder à maneira exclusiva como cada unidade funciona.
* O Workfront Planning não vem com nenhum espaço de trabalho pré-configurado. Você deve criá-los de acordo com as necessidades de sua organização.
* Você pode criar espaços de trabalho das seguintes maneiras:

   * Do zero
   * Uso de um template. Os modelos contêm um número pré-configurado de tipos de registro e seus campos.
   * Uso da Designer do Planning habilitada por IA. Este recurso atualmente está no Beta.
   * Uso de um pacote de modelo de vários espaços de trabalho.

  Para obter informações, consulte [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

* Os espaços de trabalho são estruturas nas quais suas unidades organizacionais (uma equipe, grupo, departamento ou divisão) trabalham. Elas não podem ser associadas a campos. Somente os tipos de registro em um espaço de trabalho podem ser associados a campos.

  Para obter informações, consulte [Visão geral dos tipos de registro](/help/quicksilver/planning/architecture/overview-of-record-types.md).
* Os espaços de trabalho são exibidos nas seguintes guias na área Planejamento:

   * **Espaços de trabalho em que estou**: exibe os espaços de trabalho que você criou ou os espaços de trabalho que são compartilhados com você.
   * **Outros espaços de trabalho**: exibe todos os outros espaços de trabalho no sistema. Isso só está disponível para Administradores do sistema.

  <div class="preview">

   * **Espaços de trabalho de exemplo**: exibe exemplos internos de espaços de trabalho de práticas recomendadas. Não é possível editar os espaços de trabalho, os tipos de registro ou adicionar registros ou campos, mas você pode adicionar, editar e compartilhar exibições com outras pessoas.

  </div>

  >[!NOTE]
  >
  ><span class="preview">Recomendamos não editar os espaços de trabalho de exemplo, mas usá-los como uma referência para criar os seus próprios. Use o pacote de modelos de vários espaços de trabalho para criar espaços de trabalho idênticos aos listados na guia Espaços de trabalho de amostra. Para obter informações, consulte a seção &quot;Criar vários espaços de trabalho usando um conjunto de modelos de vários espaços de trabalho de práticas recomendadas&quot; no artigo [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md). </span>

<!--
No longer the case - they match now: 

* For all other users:

* **Workspaces I'm on**: Workspaces they created (for Standard-license users) and workspaces others shared with them display in the Workspaces area.

<div class="preview"> 

* **Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.

</div>
-->



* Os tipos de registro que um espaço de trabalho contém devem refletir o ciclo de vida do trabalho e os conceitos de uma unidade organizacional.

  Por exemplo, se os objetos de trabalho de uma unidade forem campanhas, produtos e regiões, o espaço de trabalho dessa unidade deverá conter os tipos de registro Campanha, Produto e Região.
* Ao criar um espaço de trabalho, somente você tem permissão para acessar e gerenciar seu espaço de trabalho. Você deve compartilhá-lo com outros usuários para que eles colaborem com você no mesmo espaço.

  Para obter informações, consulte [Compartilhar um espaço de trabalho](/help/quicksilver/planning/access/share-workspaces.md).

  Os administradores do sistema podem gerenciar todos os espaços de trabalho, mesmo aqueles que não criaram.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Há limites para a quantidade de objetos do espaço de trabalho que você pode criar na instância do Workfront Planning. Para obter informações, consulte [visão geral das limitações de objetos do Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).
