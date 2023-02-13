---
content-type: reference
navigation-topic: search
title: Usar o número de referência de objetos
description: Em [!DNL Adobe Workfront], os itens são identificados como objetos. Os objetos correspondem ao banco de dados e são usados para correlacionar os dados com um item. Os números de referência são úteis na distinção entre dois objetos similares (como tarefas com o mesmo nome). Você pode pesquisar números de referência e incluí-los em relatórios.
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Usar o número de referência de objetos

Em [!DNL Adobe Workfront], os itens são identificados como objetos. Os objetos correspondem ao banco de dados e são usados para correlacionar os dados com um item.

O Workfront atribui automaticamente a cada um dos seguintes objetos um número de referência exclusivo quando o objeto é criado:

* Projetos
* Tarefas
* Problemas
* Documentos

Os números de referência são úteis na distinção entre dois objetos similares (como tarefas com o mesmo nome). Você pode pesquisar números de referência e incluí-los em relatórios.

>[!IMPORTANT]
>
>* [!DNL Workfront] atribui números de referência continuamente em todos os clientes e em todos os objetos. Por exemplo, ao criar uma tarefa, [!DNL Workfront] pode atribuir a ele um número de referência de 00005. Se outro cliente criar um projeto em seguida, seu projeto poderá receber o próximo número de referência disponível, por exemplo, 00006. Se você criar um problema em seguida, seu problema poderá receber o número de referência 00007 e assim por diante.
>* Não é possível controlar a sequência de números de referência para nenhum objeto em [!DNL Workfront]. A sequência é sempre controlada pelo nosso banco de dados.
>




## Exibir o número de referência de um objeto

Os números de referência são exibidos por padrão para tarefas e problemas. Você também pode configurar facilmente [!DNL Workfront] para exibir números de referência para outros tipos de objetos.

* [Exibir números de referência para tarefas e problemas](#view-reference-numbers-for-tasks-and-issues)
* [Exibir números de referência para outros objetos](#view-reference-numbers-for-other-objects)
* [Exibir números de referência em relatórios](#view-reference-numbers-in-reports)

### Exibir números de referência para tarefas e problemas

Os números de referência são exibidos por padrão ao visualizar uma tarefa ou problema.  Para ver o número de referência, clique em **[!UICONTROL Detalhes da tarefa]** ou **[!UICONTROL Detalhes do problema]** no painel esquerdo, em seguida, localize a variável **[!UICONTROL Informações básicas]** na seção Visão geral .

![](assets/reference-number-nwe-350x184.png)

### Exibir números de referência para outros objetos

Para exibir números de referência para objetos, é possível criar uma exibição personalizada ou modificar uma exibição existente e adicionar o [!UICONTROL Número de referência] para uma coluna na exibição. Por exemplo, você pode modificar o [!UICONTROL Projetos] exibir para exibir o número de referência de todos os seus projetos.

Para obter informações sobre como criar ou modificar uma Exibição, consulte [Visão geral das exibições em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Exibir números de referência em relatórios

É possível exibir o número de referência de objetos em relatórios ao adicionar a variável [!UICONTROL Número de referência] para o relatório.

Para obter informações sobre como adicionar uma coluna a um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Procurar um objeto por número de referência

[!DNL Workfront] permite procurar um objeto por número de referência.

Digite o número de referência de um objeto no **[!UICONTROL Pesquisar]** e pressione **[!UICONTROL Enter]**.

Para obter mais informações sobre como pesquisar no Workfront, consulte [Pesquisar [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
