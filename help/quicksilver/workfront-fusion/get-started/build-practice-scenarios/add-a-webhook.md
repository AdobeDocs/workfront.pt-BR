---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adicionar um webhook a um cenário básico
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Adicionar um webhook a um cenário básico em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Adicionar um webhook a um cenário básico](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-a-webhook-to-basic-scenario.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Webhooks, também conhecidos como acionadores instantâneos, são um tipo específico de módulo de acionador que pode iniciar um cenário sempre que uma alteração for feita, em vez de em um determinado agendamento.

Neste exemplo, você adicionará um webhook para iniciar um cenário assim que qualquer solicitação for enviada para uma fila específica. O cenário converte essas solicitações em um projeto.

Este exemplo modifica o cenário criado em [Criar um cenário básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Pré-requisitos

Você deve criar o cenário descrito em [Criar um cenário básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimento.

## Adicionar e configurar o webhook

1. Abra o módulo Converter objeto.
1. No campo ID do problema, exclua o bloco de ID preto. O bloco está preto porque o módulo do qual foi mapeado não está mais disponível.
1. Selecione o bloco de ID no primeiro módulo (Eventos de observação) para mapeá-lo para o segundo módulo.
1. Clique em **OK**.

### Adicionar o módulo de webhook

1. Abra o cenário no editor de cenários.
1. Clique com o botão direito no primeiro módulo e selecione **Excluir módulo**.

   O módulo é excluído, deixando um espaço reservado em branco.

1. Clique no módulo em branco e selecione **Adobe Workfront** na lista de aplicativos.
1. Selecione **Assistir Eventos**.
1. Clique em **Adicionar** ao lado do campo Webhook.
1. no campo Tipo de Registro, selecione **Problema**, para que o módulo acione alterações nos problemas.
1. No campo Estado, selecione **Novo estado**. Este é um campo obrigatório usado para o filtro, que este exemplo não cobre.
1. No campo Origem do Registro, selecione **Somente Novo Registro**. Isso permite que o cenário seja acionado quando um problema for adicionado, não quando um for atualizado ou excluído.
1. Clique em **Salvar** para salvar a configuração do módulo.
