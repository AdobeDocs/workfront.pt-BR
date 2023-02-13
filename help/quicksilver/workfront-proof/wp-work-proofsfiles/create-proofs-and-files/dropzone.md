---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: Dropzone
description: Se você tiver o plano Enterprise , poderá usar o Dropzone para enviar novas provas e novas versões de provas para sua conta sem ter que fazer logon em sua conta.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Dropzone

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Se você tiver o plano Enterprise , poderá usar o Dropzone para enviar novas provas e novas versões de provas para sua conta sem ter que fazer logon em sua conta.

Ao enviar uma prova pelo Dropzone, ela é exibida na página Dropzone em sua [!DNL Workfront Proof] conta. A partir daí, você pode roteá-lo para o seu fluxo de trabalho.

## Envio de uma nova prova pelo URL do Dropzone

1. No seu navegador, vá para o URL exclusivo do Dropzone, conforme descrito em [Configure a área suspensa em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Entre com seu endereço de email.
1. Clique em **[!UICONTROL Selecionar um arquivo]** ou **[!UICONTROL Capturar uma página da Web]** e escolha o arquivo ou a página da Web que deseja fazer upload.

1. Insira o código de segurança e clique em **[!UICONTROL Próximo]**.\
   Uma barra de progresso mostra o progresso do seu upload.\
   Na próxima tela, você poderá adicionar Proof details.\
   Observe que esta seção aparece somente se foi ativada nas configurações do Dropzone.

1. Depois de preencher os detalhes, clique em **[!UICONTROL Próximo]**.
1. Qualquer revisor adicionado à prova receberá apenas o email de notificação após a ativação da prova (veja abaixo).
1. Sua prova passa pelos seguintes estados depois de enviá-la para o Dropzone:

   * Ao fazer upload de um arquivo pela primeira vez no Dropzone, a prova é exibida como um Rascunho.
   * Depois de concluir o envio, a prova é exibida no Dropzone como Submetido.
   * Depois que a prova for ativada e desbloqueada, ela será exibida no Dropzone como Ativa.
   * Se a prova estiver bloqueada, ela será exibida no Dropzone como Bloqueada.

## Envio de uma nova versão de uma prova existente por meio do URL do Dropzone

1. No seu navegador, vá para o URL exclusivo do Dropzone, conforme descrito em [Configure a área suspensa em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Entre com seu endereço de email.
1. Marque a caixa de seleção para indicar que você está fazendo upload de uma nova versão de uma prova existente.\
   Para obter informações sobre como criar uma nova versão de uma prova, consulte .
1. Clique em **[!UICONTROL Selecionar um arquivo]** ou **[!UICONTROL Capturar uma página da Web]** e escolha o arquivo ou a página da Web que deseja fazer upload.

1. Insira o código de segurança e clique em **[!UICONTROL Próximo]**.\
   Uma barra de progresso mostra o progresso do seu upload.\
   A Workfront Proof envia um email de validação para você.

1. Clique no link no email.\
   O email abre a janela Dropzone no seu navegador. O link na notificação por email é válido por 24 horas.
1. Selecione a versão anterior da prova (somente as provas que você criou/enviou serão mostradas).\
   Na próxima tela, você poderá adicionar detalhes de prova.\
   Esta seção aparece somente se foi ativada nas configurações do Dropzone.

1. Digite os detalhes, clique em **[!UICONTROL Próximo]**.

   >[!NOTE]
   >
   >Qualquer revisor adicionado à prova receberá apenas o email de notificação após a ativação da prova (veja abaixo).

   Sua prova passa pelos seguintes estados depois de enviá-la para o Dropzone:

   * Ao fazer upload de um arquivo pela primeira vez no Dropzone, a prova é exibida como um Rascunho.
   * Depois de concluir o envio, a prova é exibida no Dropzone como Submetido.
   * Depois que a prova for ativada e desbloqueada, ela será exibida no Dropzone como Ativa.
   * Se a prova estiver bloqueada, ela será exibida no Dropzone como Bloqueada.

## Envio de uma Prova ao Dropzone

>[!NOTE]
>
>Não há mais suporte para enviar uma prova por email para a área de soltar.


## Concluir seu envio

A Workfront envia a você (o remetente) um email de envio Complete solicitando que você confirme se o arquivo é uma nova prova ou uma nova versão. O link na notificação por email é válido por 24 horas.

1. Clique no link e siga as etapas acima, dependendo se é uma nova prova ou uma nova versão de uma prova existente.

## Ativar a prova

O proprietário do Dropzone recebe um email de notificação para avisar que uma nova prova foi enviada para o Dropzone:

* A prova aparece na página Dropzone na sua conta (para acessar a página Dropzone, clique no link na barra lateral de navegação esquerda).
* A prova é acessível pelo proprietário do Dropzone (ou por um usuário que tenha pelo menos um perfil de Supervisor). O proprietário pode ser alterado nas configurações do Dropzone (somente um Administrador de Faturamento ou um Administrador pode fazer isso).
* Antes que a prova possa ser trabalhada, ela deve ser ativada/desbloqueada pelo proprietário do Dropzone (um usuário com pelo menos um perfil supervisor também pode fazer isso). O status da prova é exibido como Enviado até que tenha sido ativado/desbloqueado.

Para ativar a prova:

1. Vá para o menu suspenso à direita da prova e clique em **[!UICONTROL Ativar]**.
1. Depois que a prova for ativada/desbloqueada:

   * O status da prova é alterado para Ativo.
   * Qualquer pessoa que foi adicionada à prova receberá um email de notificação para avisar que tem uma nova prova para revisar. (Nenhum email será enviado até que a prova tenha sido ativada/desbloqueada.)
   * A prova pode ser trabalhada normalmente
   * Se o remetente também se adicionar explicitamente à prova, ele não receberá um email New proof . Para obter mais informações, consulte [Novo email de prova](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

## Gerenciando Sua Zona Do Dropzone

A página Dropzone facilita o gerenciamento dos envios para seu Dropzone. A página Dropzone inclui as seguintes opções e funcionalidades:

* Layout da página (1)
* Escolha incluir/excluir provas arquivadas na exibição (2)
* Botões de ação (3)
* Ordenar (4)
* Filtro (5)
* Menu de ações de prova (6)
* Desarquivar a prova (7)
* Expandir/recolher resumo de prova (8)
* Selecionar uma prova (9)

As opções de layout, classificação e filtragem da página são as mesmas do cenário [!DNL Views] listas. Consulte [Gerenciar itens na página de exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) para obter mais informações.

![New_Dropzone_design_Feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
