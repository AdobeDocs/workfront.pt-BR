---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: O [!DNL Workfront] Página de Faturamento da Prova
description: Para acessar o [!UICONTROL Faturamento] abra o menu Configurações no canto superior direito da tela e escolha Faturamento no menu suspenso.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# O [!DNL Workfront Proof] Página de Faturamento

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

## A página Faturamento

Para acessar o [!UICONTROL Faturamento] , abra o **[!UICONTROL Configurações]** no canto superior direito do ecrã e escolha **[!UICONTROL Faturamento]** no menu suspenso.

O [!UICONTROL Faturamento] contém o seguinte:

* Nome da conta (1)
* Lista de contas (por exemplo, se você tiver contas satélite)(2)
* Plano de alteração (3)
* Alterar detalhes do pagamento (4)
* Nova conta satélite (5)
* Fechar conta (6)
* Informações sobre o plano atual (7)
* Contato e endereço para faturação (8)
* Estatísticas de utilização (9)
* Histórico de cobrança (10)
* Atividade de faturamento (11)

   ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL Plano Atual]

Esta seção (7) mostra os detalhes do seu plano atual, incluindo o seguinte:

* O nome do plano
* Método de pagamento atual
* Datas de início e término do plano atual
* Próximo tipo de plano
* Método de pagamento do próximo plano

   Para obter mais informações, consulte [Escolha do Método de Pagamento em [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL Contato e Endereço de Faturamento]

Esta seção (8) mostra o contato de faturamento principal e os detalhes de endereço de sua conta.

O contato de Faturamento pode ser selecionado somente a partir dos usuários configurados como Administradores de Faturamento em sua conta. Nas contas Satélite, somente os Administradores de Faturamento da conta principal podem ser definidos neste campo.

![Billing_Contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> Você pode ter vários Administradores de faturamento em sua conta, mas apenas um deles, selecionado no [!UICONTROL Contato de faturamento] , receberá todas as notificações de faturamento e alertas de uso de conta.

Isso inclui os seguintes emails de notificação:

* Uso da prova
* Faturas
* Fazer downgrade
* Alerta de suspensão de conta/pagamento atrasado
* Falha no cartão de crédito

   ![Billin_CC.png](assets/billin-cc-350x103.png)

O [!UICONTROL Faturamento CC] O campo também permite adicionar um endereço de email a ser copiado em todos os emails relacionados a cobrança. Clique no campo para ativar a edição de inclusão e insira um endereço de email de sua escolha (também pode ser um endereço de email de um usuário existente).

## [!UICONTROL Endereço de cobrança]

Esta seção usa a edição em linha, então simplesmente clique nos campos para inserir/editar o texto.

>[!NOTE]
>
> Incluímos esse endereço em suas faturas de assinatura para garantir que esses dados estejam sempre atualizados.

![Billing_Address.png](assets/billing-address-350x199.png)

## [!UICONTROL Estatísticas de uso]

Esta seção mostra as estatísticas de uso da sua conta dentro do período de faturamento atual, incluindo o seguinte:

* Armazenamento usado
* Provas usadas
* Limite de usuários usado

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL Avisos de uso]

O [[!UICONTROL Perfis de permissões de prova] em [!DNL Workfront] Prova](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) definido como Contato de Faturamento (1) em sua conta será notificado por email quando sua conta atingir:

* 75% e depois 98% da capacidade de armazenamento
* 75% e, em seguida, 100% do seu limite de prova

![Billing_Contact_1_.png](assets/billing-contact--1--350x74.png)

Quando as provas ou os limites de armazenamento forem atingidos, você também verá os alertas na parte superior do [!UICONTROL Faturamento] página:

* Para o limite de provas alcançado

   ![Proofs_limit_reached.png](assets/proofs-limit-reached-350x65.png)

* Para o limite de armazenamento atingido

![Storage_limit_reached.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>Sua contagem de prova é usada quando as provas são criadas em sua conta e não podem ser restauradas removendo as provas.

O espaço de armazenamento pode ser liberado excluindo provas e arquivos e esvaziando o [!UICONTROL Lixeira] depois.

Lembre-se de que, se você precisar de mais provas, armazenamento ou usuários, poderá atualizar sua conta a qualquer momento; e produz efeito imediato.

## [!UICONTROL Histórico de Faturamento]

Esta seção mostra a atividade para qualquer período de faturamento recente. Também é possível baixar faturas nesta seção.

Para obter mais informações, consulte &quot; [Download do [!DNL Workfront Proof] Fatura](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md).&quot;

## [!UICONTROL Atividade de faturamento]

Esta seção mostra as alterações recentes na configuração de faturamento, por exemplo, assinaturas, atualizações, downloads e renovações de seu [!DNL Workfront Proof] Plano.

Se você alterar seu plano para um com um limite de usuário inferior (1), os usuários que excederem o novo limite serão automaticamente desativados quando o novo plano começar. Essa atividade também será capturada em seus registros de conta (2).

![Billing_Download_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
