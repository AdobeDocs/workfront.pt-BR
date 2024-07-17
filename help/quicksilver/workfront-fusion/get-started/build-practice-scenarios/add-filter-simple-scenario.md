---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adicionar um filtro a um cenário básico
description: Os filtros permitem garantir que o cenário avance somente se determinadas condições forem atendidas.
author: Becky
feature: Workfront Fusion
exl-id: b43355ed-9329-4080-8e61-7177eb580994
source-git-commit: 1a405d38968922388589ddb3f2979b4e59cd50b8
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Adicionar um filtro a um cenário básico em [!DNL Adobe Workfront Fusion]

Os filtros permitem garantir que o cenário avance somente se determinadas condições forem atendidas.

Neste exemplo, você adicionará um filtro ao cenário que permite que um novo projeto seja criado a partir de uma solicitação somente se a solicitação tiver sido enviada para uma fila de solicitações específica.

Este exemplo modifica o cenário criado em [Criar um cenário básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Os módulos de acionamento do Workfront incluem filtros que permitem que um cenário seja iniciado somente se determinadas condições forem atendidas. No entanto, como os filtros entre módulos são usados para todos os casos de uso que não são de acionador ou que não são do Workfront, é importante saber como usar filtros entre módulos. Esse exemplo usa um filtro entre módulos para uma funcionalidade que pode ser atendida com um filtro no módulo.

## Pré-requisitos

Você deve criar o cenário descrito em [Criar um cenário básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimento.

## Adicionar um filtro

### Preparar para adicionar o filtro

1. Abra o primeiro cenário.
1. Na área **Saídas**, selecione `Project`.
Agora você deve ter `ID`, `Name` e `Project` selecionados.
1. Clique em OK para salvar as configurações do módulo.
1. Abra o Workfront.
1. No Workfront, localize o projeto que representa a fila de solicitações com a qual o cenário do Fusion funcionará.

   Esse projeto deve estar na mesma conta do Workfront para a qual a conexão do Fusion está configurada.

1. Anote a ID do projeto no URL.

   Exemplo: https://\&lt;MyDomain\>.my.workfront.com/project/\&lt;ProjectID\>/tasks

### Adicionar e configurar o filtro

1. Abra o cenário no editor de cenários.
1. Clique no ícone de chave inglesa ![Ícone de chave inglesa](assets/wrench-icon.png) entre o primeiro e o segundo módulo e selecione **Configurar um filtro**.
1. No campo Rótulo, digite um rótulo para esse filtro, como &quot;Filtro para fila de solicitações&quot;.
1. Na área **Condição**, no campo superior, mapeie o `projectID` do primeiro módulo.

   ![Mapear ID do projeto](assets/map-proj-id.png)
1. Deixe o operador **Condição** como Igual a.
1. No campo inferior da área **Condição**, cole a ID do projeto que você anotou da URL do projeto em [Preparar para adicionar o filtro](#prepare-to-add-the-filter).
1. Clique em **OK** para salvar as configurações de filtro.

### Testar e ativar

1. Vá para o ambiente do Workfront ao qual o Fusion está se conectando e adicione um problema ao projeto especificado no filtro. Adicione outro problema a um projeto diferente.
1. Clique em **[!UICONTROL Executar uma vez]** no canto inferior esquerdo do editor de cenários.
1. Examine a saída para garantir que o cenário seja executado conforme esperado.

   Ambos os problemas devem aparecer na saída do primeiro cenário, mas somente o problema no projeto especificado deve aparecer como entrada no segundo cenário,
1. Quando estiver satisfeito com o funcionamento do cenário, clique no botão de alternância **Agendamento** no canto inferior esquerdo da tela para **Ativado**.

   Isso ativa o cenário.
1. Em [!DNL Workfront Fusion], clique em **[!UICONTROL Salvar]** próximo ao canto inferior esquerdo para salvar seu progresso no cenário.

   >[!IMPORTANT]
   >
   >Salve com frequência à medida que você aprimora e testa um cenário.

## Recursos

* Para obter mais informações sobre filtros, consulte [Adicionar um filtro a um cenário](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
