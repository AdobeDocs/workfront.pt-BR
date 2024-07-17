---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: A Dropzone
description: Se você tiver o plano Enterprise, poderá usar a Área de lançamento para submeter novas provas e novas versões de provas para sua conta sem precisar efetuar login em sua conta.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# A Dropzone

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Se você tiver o plano Enterprise, poderá usar a Área de lançamento para submeter novas provas e novas versões de provas para sua conta sem precisar efetuar login em sua conta.

Quando você envia uma prova por meio do Dropzone, ela aparece na página Dropzone na sua conta [!DNL Workfront Proof]. A partir daí, você pode direcioná-lo para o seu workflow.

## Envio de uma nova prova através do URL da Dropzone

1. No seu navegador, vá para a URL exclusiva do Dropzone, conforme descrito em [Configurar o dropzone em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Insira seu endereço de email.
1. Clique em **[!UICONTROL Selecionar um arquivo]** ou **[!UICONTROL Capturar uma página da Web]** e escolha o arquivo ou a página da Web que deseja carregar.

1. Digite o código de segurança e clique em **[!UICONTROL Avançar]**.\
   Uma barra de progresso mostra o progresso do upload.\
   Na próxima tela, será possível adicionar detalhes da Prova.\
   Observe que esta seção só será exibida se tiver sido ativada nas configurações da Zona suspensa.

1. Depois de preencher os detalhes, clique em **[!UICONTROL Avançar]**.
1. Os revisores adicionados à prova só receberão o email de notificação após a ativação da prova (veja abaixo).
1. Sua prova passa pelos seguintes estados depois de enviá-la para a Área de lançamento:

   * Ao fazer upload de um arquivo para a Zona de lançamento pela primeira vez, a prova é exibida como um Rascunho.
   * Depois de concluir o envio, a prova será exibida no Dropzone como Enviado.
   * Depois que a prova for ativada e desbloqueada, ela será exibida no Dropzone como Ativo.
   * Se a prova estiver bloqueada, ela será exibida no Dropzone como Bloqueado.

## Envio de uma nova versão de uma prova existente por meio do URL da zona de lançamento

1. No seu navegador, vá para a URL exclusiva do Dropzone, conforme descrito em [Configurar o dropzone em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Insira seu endereço de email.
1. Marque a caixa de seleção para indicar que você está fazendo upload de uma nova versão de uma prova existente.\
   Para obter informações sobre como criar uma nova versão de uma prova, consulte.
1. Clique em **[!UICONTROL Selecionar um arquivo]** ou **[!UICONTROL Capturar uma página da Web]** e escolha o arquivo ou a página da Web que deseja carregar.

1. Digite o código de segurança e clique em **[!UICONTROL Avançar]**.\
   Uma barra de progresso mostra o progresso do upload.\
   O Workfront Proof envia um email de validação.

1. Clique no link do email.\
   O email abre a janela Dropzone no navegador. O link na notificação por email é válido por 24 horas.
1. Selecione a versão anterior da prova (somente as provas que você criou/enviou serão exibidas).\
   Na próxima tela, você poderá adicionar detalhes da prova.\
   Esta seção só será exibida se tiver sido ativada nas configurações da Zona suspensa.

1. Digite os detalhes, clique em **[!UICONTROL Avançar]**.

   >[!NOTE]
   >
   >Os revisores adicionados à prova só receberão o email de notificação após a ativação da prova (veja abaixo).

   Sua prova passa pelos seguintes estados depois de enviá-la para a Área de lançamento:

   * Ao fazer upload de um arquivo para a Zona de lançamento pela primeira vez, a prova é exibida como um Rascunho.
   * Depois de concluir o envio, a prova será exibida no Dropzone como Enviado.
   * Depois que a prova for ativada e desbloqueada, ela será exibida no Dropzone como Ativo.
   * Se a prova estiver bloqueada, ela será exibida no Dropzone como Bloqueado.

## Enviar uma prova por email para a área de lançamento

>[!NOTE]
>
>Enviar uma prova por email para a zona de destino não é mais suportado.


## Concluindo seu envio

O Workfront envia a você (o remetente) um email Concluir o envio solicitando que você confirme se o arquivo era uma nova prova ou uma nova versão. O link na notificação por email é válido por 24 horas.

1. Clique no link e siga as etapas acima, dependendo se é uma nova prova ou uma nova versão de uma prova existente.

## Ativação da prova

O proprietário do Dropzone recebe um email de notificação para avisar que uma nova prova foi enviada para o Dropzone:

* A prova é exibida na página Área de lançamento em sua conta (para acessar a página Zona de lançamento, clique no link na barra lateral de navegação esquerda).
* A prova pode ser acessada pelo proprietário do Dropzone (ou por um usuário que tenha pelo menos um perfil Supervisor ). O proprietário pode ser alterado nas configurações da zona de destino (somente um administrador de cobrança ou um administrador pode fazer isso).
* Antes que a prova possa ser trabalhada, ela deve ser ativada/desbloqueada pelo proprietário do Dropzone (um usuário com pelo menos um perfil Supervisor também pode fazer isso). O status da prova é exibido como Enviado até que tenha sido ativado/desbloqueado.

Para ativar a prova:

1. Vá para o menu suspenso à direita da prova e clique em **[!UICONTROL Ativar]**.
1. Depois que a prova for ativada/desbloqueada:

   * O status da prova muda para Ativo.
   * Qualquer pessoa adicionada à prova receberá um email de notificação para avisar que tem uma nova prova para revisar. (Nenhum email é enviado até que a prova tenha sido ativada/desbloqueada.)
   * A prova pode ser trabalhada normalmente
   * Se o remetente também se adicionar explicitamente à prova, ele não receberá um email de nova prova. Para obter mais informações, consulte [Novo email de prova](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

## Gerenciamento da área de lançamento

A página do Dropzone facilita o gerenciamento dos envios para o seu Dropzone. Sua página Dropzone inclui as seguintes opções e funcionalidades:

* Layout da página (1)
* Opte por incluir/excluir provas arquivadas na visualização (2)
* Botões de ação (3)
* Ordenar (4)
* Filtro (5)
* Menu de ações de prova (6)
* Desarquivar a prova (7)
* Expandir/recolher o resumo da prova (8)
* Selecione uma prova (9)

O layout da página e as opções de classificação e filtragem são iguais nas listas [!DNL Views]. Consulte [Gerenciar Itens na Página Exibições [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) para obter mais informações.

![Novo_Dropzone_design_Feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
