---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configurar opções de decisão de aprovação em  [!DNL Workfront Proof]
description: Você pode configurar as opções de decisão de aprovação para todas as provas criadas por  [!DNL Workfront Proof]  usuários em sua organização.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Configurar opções de decisão de aprovação em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Como administrador do [!DNL Workfront Proof] usando um plano de edição Select ou Premium, você pode configurar as opções de decisão de aprovação das seguintes maneiras para todas as provas criadas por usuários do [!DNL Workfront Proof] em sua organização:

* Alterar o nome da decisão
* Alterar a ordem das decisões mostradas no visualizador de provas
* Decidir quais decisões devem ser exibidas

Este artigo explica o seguinte:

## Definindo configurações de decisão

1. Clique em **[!UICONTROL Configurações da conta]**.
1. Abra a guia **[!UICONTROL Decisões]**.
1. Faça qualquer uma das seguintes alterações:

   * Para ocultar uma decisão, clique em **[!UICONTROL Ocultar]** à direita da decisão desnecessária.
   * Para renomear uma decisão, clique no nome da decisão, edite-a e clique fora da caixa (ou pressione Enter). [!DNL Workfront Proof] atualiza o nome da decisão em todas as provas existentes no sistema.

     >[!IMPORTANT]
     >
     >Mantenha a lógica de uma decisão ao renomeá-la. Por exemplo, a decisão padrão &quot;Rejeitada&quot; pode ser alterada para &quot;Nova versão necessária&quot;, mas não deve ser alterada para &quot;Enviar para impressoras&quot;).

     Se quiser voltar aos padrões de [!DNL Workfront Proof], você pode clicar em Restaurar decisões padrão.

>[!NOTE]
>
>* A lógica por trás das decisões é usada para calcular o status geral de um fluxo de trabalho de prova se houver várias decisões de vários níveis.
>* As decisões &quot;Aprovado&quot; e &quot;Aprovado com alterações&quot; acionam o próximo estágio em um fluxo de trabalho automático.
>* Se você renomear uma decisão e quiser verificar a lógica, clique em **[!UICONTROL Atividade]** no painel de navegação esquerdo e verifique seu Log de atividades onde as decisões originais são exibidas entre parênteses.
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## Criação de motivos de decisão

Os motivos de decisão são uma boa maneira de capturar informações adicionais de decisão sobre uma prova.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]**.

1. Abra a guia **[!UICONTROL Decisões]**.
Por padrão, os motivos estão disponíveis para todos os tomadores de decisão em suas provas, mas você pode restringi-los somente aos tomadores de decisão principais.
Dependendo das suas necessidades, você pode permitir que vários motivos sejam selecionados ou pode transformá-los em uma lista de opções únicas. Também é possível tornar os motivos obrigatórios, o que significa que os revisores terão que escolher um motivo antes de terem permissão para salvar sua decisão em uma prova.
   ![Reasons_setup.png](assets/reasons-setup-350x121.png)

1. Na seção **[!UICONTROL Motivos]**, clique em **[!UICONTROL Novo motivo]**.
   ![Novo_motivo.png](assets/new-reason-350x135.png)

1. Digite um título para a seção de motivos na caixa que aparece em **[!UICONTROL Motivo]**.
1. Para incluir uma caixa de texto, selecione **[!UICONTROL Incluir caixa de texto]**.
1. Clique em **[!UICONTROL Salvar]**.
   ![reason_setup_2.png](assets/reasons-setup-2-350x146.png)
A etapa mais importante é selecionar as decisões nas quais os motivos devem ser exibidos. Se você esquecer de fazer isso, os motivos não aparecerão em suas provas.

1. Marque as caixas na coluna **[!UICONTROL Exibir motivos]** na lista de decisões na parte superior da página. Você pode selecionar uma ou mais decisões por seus motivos.
   ![reason_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## Criação de uma mensagem de decisão do Post

Você pode criar uma mensagem de decisão de publicação para exibir depois que um revisor salvar sua decisão sobre a prova.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]**.

1. Abra a guia **[!UICONTROL Decisões]**.
1. Na seção **[!UICONTROL Mensagem de decisão do Post]**, clique em **[!UICONTROL Editar]** no final da linha **[!UICONTROL Mensagem]**.
Você também pode decidir se deseja que a mensagem seja exibida para todos os tomadores de decisão ou se deseja limitá-la ao Tomador de decisão principal.
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. Na coluna **[!UICONTROL Exibir mensagem]**, especifique as decisões nas quais essa mensagem deve ser exibida.
Se você não selecionar pelo menos uma decisão, a mensagem não será exibida em suas provas. Certifique-se de marcar pelo menos uma caixa nesta coluna.
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
