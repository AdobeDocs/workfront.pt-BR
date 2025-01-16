---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adicionar um módulo de acionamento a um cenário básico
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: f4588063-024f-4520-986e-45342a6b6777
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# Use uma função para atualizar um projeto em um cenário simples no [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Usar uma função para atualizar um projeto em um cenário básico](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/use-function-to-build-practice-scenario.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Atualizar um item de trabalho do Workfront é um caso de uso comum para o Workfront Fusion. Neste exemplo, você usará uma função para alterar o nome de um projeto para ficar em letras maiúsculas.

O Fusion inclui muitos tipos de funções que permitem transformar e executar lógica condicional em seus dados. Para obter mais informações sobre como usar funções, consulte [Mapear informações de um módulo para outro no Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Este exemplo modifica o cenário criado em [Criar um cenário básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Pré-requisitos

Você deve criar o cenário descrito em [Criar um cenário básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimento.

## Usar uma função para atualizar um projeto

### Adicionar o módulo Atualizar Registro ao seu cenário

1. Abra o cenário no editor de cenários.
1. Passe o mouse sobre o círculo parcial à direita do do módulo e clique em **[!UICONTROL Adicionar outro módulo]**.
1. Selecione [!DNL Adobe Workfront] na lista de aplicativos e escolha o módulo **[!UICONTROL Atualizar Registro]**.
1. no campo ID, selecione o bloco ID que está sob o módulo Converter objeto. Esta é a ID do projeto emitido por esse módulo.

   ![ID do objeto Convert](assets/id-convert-object.png)

1. No campo Tipo de registro, selecione Projeto, pois o objeto a ser atualizado é um projeto.
1. Na área Selecionar campos a serem mapeados, selecione Nome.

   Um campo Nome será aberto.

### Mapear a função para a atualização de nome

Quando esse cenário converte uma solicitação em um projeto, o nome do projeto é igual ao da solicitação. A função aqui pega esse nome e coloca todas as letras em maiúsculas nele.

1. Clique no campo **Nome**.

   O painel de mapeamento é aberto.
1. No painel de mapeamento, clique no ícone **Funções binárias e de texto**. ![Ícone de funções de texto](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Selecione a função **upper**.

   A função aparece no campo Nome, incluindo a formatação da entrada esperada.

   A entrada para este exemplo é o nome do problema do qual o projeto foi convertido.

1. Mova o cursor entre os parênteses, porque é para onde a entrada irá.
1. No painel de mapeamento, clique no ícone **saída do módulo**. ![Ícone de saída do módulo](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Selecione o bloco de nome que foi emitido pelo primeiro módulo.

   O bloco de nome aparece na função.

   ![Bloco de nome na função](assets/map-name.png)

1. Clique em OK para salvar as configurações do módulo.

### Testar e ativar

1. Teste o cenário clicando em **Executar uma vez** no canto inferior esquerdo da tela.
1. Examine a saída para garantir que o cenário seja executado conforme esperado.
1. Quando estiver satisfeito com o funcionamento do cenário, clique no botão de alternância **Agendamento** no canto inferior esquerdo da tela para **Ativado**.

   Isso ativa o cenário. Cenários ativos são executados de acordo com o agendamento definido no módulo do acionador.
1. Em [!DNL Workfront Fusion], clique em **[!UICONTROL Salvar]** próximo ao canto inferior esquerdo para salvar seu progresso no cenário.

   >[!IMPORTANT]
   >
   >Salve com frequência à medida que você aprimora e testa um cenário.

## Recursos:

* [Mapear itens usando funções em  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
