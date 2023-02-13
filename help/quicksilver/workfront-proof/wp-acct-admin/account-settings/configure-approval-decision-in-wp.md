---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configure as opções de decisão de aprovação em [!DNL Workfront Proof]
description: Como um [!DNL Workfront Proof] administrador usando um plano de edição Select ou Premium, você pode configurar as opções de decisão de aprovação das seguintes maneiras para todas as provas criadas por [!DNL Workfront Proof] usuários em sua organização - EDITE-ME.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Configure as opções de decisão de aprovação em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Como um [!DNL Workfront Proof] administrador usando um plano de edição Select ou Premium, você pode configurar as opções de decisão de aprovação das seguintes maneiras para todas as provas criadas por [!DNL Workfront Proof] usuários em sua organização:

* Alterar o nome da decisão
* Alterar a ordem das decisões mostradas no visualizador de prova
* Decida quais decisões devem ser exibidas

Este artigo explica o seguinte:

## Definição das configurações de decisão

1. Clique em **[!UICONTROL Configurações da conta]**.
1. Abra o **[!UICONTROL Decisões]** guia .
1. Faça qualquer uma das seguintes alterações:

   * Para ocultar uma decisão, clique em **[!UICONTROL Ocultar]** à direita da decisão que você não precisa.
   * Para renomear uma decisão, clique no nome da decisão, edite-a e clique fora da caixa (ou pressione Enter). [!DNL Workfront Proof] O atualiza o nome da decisão em todas as provas existentes no sistema.

      >[!IMPORTANT]
      >
      >Mantenha a lógica de uma decisão ao renomeá-la. Por exemplo, a decisão padrão &quot;Rejected&quot; (Rejeitado) pode ser alterada para &quot;New version required&quot;, mas não deve ser alterada para &quot;Send to Printers&quot;).

      Se você quiser voltar para a [!DNL Workfront Proof] padrões, você pode clicar em Restaurar decisões padrão.

>[!NOTE]
>
>* A lógica por trás das decisões é usada para calcular o status geral de um workflow de prova se houver várias decisões de vários níveis.
>* As decisões &quot;Aprovado&quot; e &quot;Aprovado com alterações&quot; acionam a próxima etapa em um fluxo de trabalho automático.
>* Se você renomear uma decisão e quiser verificar a lógica, clique em **[!UICONTROL Atividade]** no painel de navegação esquerdo e verifique seu registro de atividades, onde as decisões originais são exibidas entre colchetes.
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## Criação de motivos de decisão

Os motivos de decisão são uma boa maneira de capturar informações de decisão adicionais sobre uma prova.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]**.

1. Abra o **[!UICONTROL Decisões]** guia .
Por padrão, os motivos estão disponíveis para todos os tomadores de decisão em suas provas, mas você pode restringir isso somente aos tomadores de decisão primários.
Dependendo dos seus requisitos, você pode permitir que vários motivos sejam selecionados ou pode torná-la uma lista de escolha única. Você também pode tornar os motivos obrigatórios, o que significa que os revisores terão que escolher um motivo antes que possam salvar sua decisão em uma prova.
   ![Motivos_setup.png](assets/reasons-setup-350x121.png)

1. No **[!UICONTROL Motivos]** seção , clique em **[!UICONTROL Novo motivo]**.
   ![New_reason.png](assets/new-reason-350x135.png)

1. Digite um título para a seção motivos na caixa que aparece em **[!UICONTROL Motivo]**.
1. Se desejar incluir uma caixa de texto, selecione **[!UICONTROL Incluir caixa de texto]**.
1. Clique em **[!UICONTROL Salvar]**.
   ![reasons_setup_2.png](assets/reasons-setup-2-350x146.png)
O passo mais importante é selecionar as decisões nas quais os motivos devem ser exibidos. Se você se esquecer de fazer isso, as razões não serão mostradas em suas provas.

1. Marque as caixas no **[!UICONTROL Exibir motivos]** na lista de decisões na parte superior da página. É possível selecionar uma ou mais decisões pelos motivos.
   ![reasons_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## Criação de uma mensagem de pós decisão

Você pode criar uma mensagem de decisão de publicação para exibir depois que um revisor salvar sua decisão na prova.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]**.

1. Abra o **[!UICONTROL Decisões]** guia .
1. No **[!UICONTROL Mensagem pós-decisão]** seção , clique em **[!UICONTROL Editar]** no final do **[!UICONTROL Mensagem]** linha.
Você também pode decidir se deseja que a mensagem seja exibida para todos os tomadores de decisão ou se deseja limitá-la ao principal responsável pela tomada de decisão.
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. No **[!UICONTROL Exibir mensagem]** , especifique as decisões nas quais essa mensagem deve ser exibida.
Se você não selecionar pelo menos uma decisão, a mensagem não será exibida em suas provas. Certifique-se de marcar pelo menos uma caixa nessa coluna.
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
