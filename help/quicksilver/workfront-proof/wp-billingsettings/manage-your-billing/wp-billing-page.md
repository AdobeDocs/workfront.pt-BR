---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: A  [!DNL Workfront] Página de Cobrança da Prova
description: Para acessar a página [!UICONTROL Faturamento], abra o menu Configurações na parte superior direita da tela e escolha Faturamento no menu suspenso.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# A página de cobrança [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

## A página de faturamento

Para acessar a página [!UICONTROL Faturamento], abra o menu **[!UICONTROL Configurações]** na parte superior direita da tela e escolha **[!UICONTROL Faturamento]** no menu suspenso.

A página [!UICONTROL Faturamento] contém o seguinte:

* Nome da conta (1)
* Lista de contas (por exemplo, se você tiver contas satélite)(2)
* Plano de mudança (3)
* Alterar detalhes do pagamento (4)
* Nova conta satélite (5)
* Fechar conta (6)
* Informações sobre o plano atual (7)
* Contato e endereço para cobrança (8)
* Estatísticas de uso (9)
* Histórico de faturamento (10)
* Atividade de faturação (11)

  ![Página_de_Faturamento.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL Plano Atual]

Esta seção (7) mostra os detalhes do seu plano atual, incluindo o seguinte:

* O nome do plano
* Método de pagamento atual
* Datas de início e término atuais do plano
* Próximo tipo de plano
* Próximo método de pagamento do plano

  Para obter mais informações, consulte [Escolhendo seu método de pagamento [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL Contato e Endereço de Cobrança]

Esta seção (8) mostra os principais detalhes de contato e endereço para cobrança da sua conta.

O contato de Faturamento pode ser selecionado somente a partir dos usuários configurados como Administradores de Faturamento em sua conta. Nas contas satélite, somente os administradores de cobrança da conta principal podem ser definidos nesse campo.

![Contato_de_Faturamento.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> Você pode ter vários Administradores de Cobrança em sua conta, mas apenas um deles, selecionado no campo [!UICONTROL Contato de cobrança], receberá todas as notificações de cobrança e alertas de uso da conta.

Isso inclui os seguintes emails de notificação:

* Uso da prova
* Faturas
* Fazer downgrade
* Alerta de pagamento atrasado/suspensão de conta
* Falha de cartão de crédito

  ![Billin_CC.png](assets/billin-cc-350x103.png)

O campo [!UICONTROL CC] de Cobrança também permite que você adicione um endereço de email para ser copiado em todos os emails relacionados à cobrança. Clique no campo para ativar a edição inclinada e inserir um endereço de email de sua escolha (também pode ser o endereço de email de um usuário existente).

## [!UICONTROL Endereço de cobrança]

Esta seção usa edição em linha, portanto, basta clicar nos campos para inserir/editar o texto.

>[!NOTE]
>
> Incluímos esse endereço em suas faturas de assinatura para garantir que esses dados estejam sempre atualizados.

![Endereço_de_Faturamento.png](assets/billing-address-350x199.png)

## [!UICONTROL Estatísticas de uso]

Esta seção mostra as estatísticas de uso da sua conta dentro do período de faturamento atual, incluindo as seguintes:

* Armazenamento usado
* Provas usadas
* Limite de usuários usado

![Estatísticas_de_Uso.png](assets/usage-statistics-350x51.png)

### [!UICONTROL Avisos de Uso]

Os [[!UICONTROL Perfis de Permissões de Prova] em [!DNL Workfront] Prova](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) definidos como o Contato de Cobrança (1) da sua conta serão notificados por email quando a sua conta atingir:

* 75% e, em seguida, 98% de sua capacidade de armazenamento
* 75% e, em seguida, 100% do limite de prova

![Contato_de_Faturamento__1_.png](assets/billing-contact--1--350x74.png)

Depois que as provas ou os limites de armazenamento forem atingidos, você também verá os alertas na parte superior da página [!UICONTROL Faturamento]:

* Para o limite de provas atingido

  ![Proofs_limit_reached.png](assets/proofs-limit-reached-350x65.png)

* Para o limite de armazenamento atingido

![Limite_armazenamento_atingido.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>Sua contagem de prova é utilizada quando provas são criadas em sua conta e não pode ser restaurada removendo as provas.

O espaço de armazenamento pode ser liberado excluindo as provas e os arquivos e esvaziando a [!UICONTROL Lixeira] posteriormente.

Lembre-se de que, se você precisar de mais provas, armazenamento ou usuários, você pode atualizar sua conta a qualquer momento; e isso tem efeito imediato.

## [!UICONTROL Histórico de Cobrança]

Esta seção mostra a atividade de qualquer período de faturamento recente. Você também pode baixar suas faturas nesta seção.

Para obter mais informações, consulte &quot; [Baixando sua [!DNL Workfront Proof] Fatura](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md).&quot;

## [!UICONTROL Atividade de Cobrança]

Esta seção mostra as alterações recentes feitas na sua configuração de cobrança, por exemplo, assinaturas, atualizações, rebaixamentos e renovações do seu Plano [!DNL Workfront Proof].

Se você alterar seu plano para um com um limite de usuário mais baixo (1), os usuários que excederem o novo limite serão automaticamente desativados quando o novo plano for iniciado. Essa atividade também será capturada em seus logs de conta (2).

![Billing_Downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
