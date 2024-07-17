---
content-type: reference
navigation-topic: search
title: Usar o número de referência de objetos
description: Em  [!DNL Adobe Workfront], os itens são identificados como objetos. Os objetos correspondem ao banco de dados e são usados para correlacionar dados com um item. Números de referência são úteis na distinção entre dois objetos semelhantes (como tarefas com o mesmo nome). Você pode pesquisar números de referência e incluí-los nos relatórios.
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Usar o número de referência de objetos

Em [!DNL Adobe Workfront], os itens são identificados como objetos. Os objetos correspondem ao banco de dados e são usados para correlacionar dados com um item.

O Workfront atribui automaticamente a cada um dos seguintes objetos um número de referência exclusivo quando o objeto é criado:

* Projetos
* Tarefas
* Problemas
* Documentos

Números de referência são úteis na distinção entre dois objetos semelhantes (como tarefas com o mesmo nome). Você pode pesquisar números de referência e incluí-los nos relatórios.

>[!IMPORTANT]
>
>* O [!DNL Workfront] atribui números de referência continuamente em todos os clientes e objetos. Por exemplo, quando você cria uma tarefa, [!DNL Workfront] pode atribuir a ela um número de referência 00005. Se outro cliente criar um projeto em seguida, seu projeto poderá receber o próximo número de referência disponível, por exemplo, 00006. Se você criar um problema em seguida, ele receberá o número de referência 00007 e assim por diante.
>* Você não pode controlar a sequência de números de referência de nenhum objeto em [!DNL Workfront]. A sequência é sempre controlada pelo nosso banco de dados.
>



## Exibir o número de referência de um objeto

Os números de referência são exibidos por padrão para tarefas e problemas. Você também pode configurar facilmente o [!DNL Workfront] para exibir números de referência para outros tipos de objetos.

* [Exibir números de referência para tarefas e problemas](#view-reference-numbers-for-tasks-and-issues)
* [Exibir números de referência para outros objetos](#view-reference-numbers-for-other-objects)
* [Exibir números de referência em relatórios](#view-reference-numbers-in-reports)

### Exibir números de referência para tarefas e problemas

Os números de referência são exibidos por padrão ao visualizar uma tarefa ou problema.  Para ver o número de referência, clique em **[!UICONTROL Detalhes da tarefa]** ou **[!UICONTROL Detalhes do problema]** no painel esquerdo e localize a seção **[!UICONTROL Informações básicas]** na Visão geral.

![](assets/reference-number-nwe-350x184.png)

### Exibir números de referência para outros objetos

Para exibir números de referência para objetos, você pode criar um modo de exibição personalizado ou modificar um modo de exibição existente e adicionar o campo [!UICONTROL Número de Referência] a uma coluna no modo de exibição. Por exemplo, você pode modificar o modo de exibição [!UICONTROL Projetos] para exibir o número de referência de todos os seus projetos.

Para obter informações sobre como criar ou modificar uma Exibição, consulte [Visão geral das exibições em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Exibir números de referência em relatórios

Você pode exibir o número de referência para objetos em relatórios adicionando a coluna [!UICONTROL Número de Referência] ao relatório.

Para obter informações sobre como adicionar uma coluna a um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Procurar um objeto por número de referência

[!DNL Workfront] permite procurar um objeto por número de referência.

Digite o número de referência de um objeto no campo **[!UICONTROL Pesquisa]** e pressione **[!UICONTROL Enter]**.

Para obter mais informações sobre como pesquisar no Workfront, consulte [Pesquisar [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
