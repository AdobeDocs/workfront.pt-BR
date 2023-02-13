---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Instalar um blueprint
description: Você pode instalar um blueprint no seu ambiente de Produção ou em um ambiente de sandbox.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Instalar um blueprint

Você pode instalar um blueprint no seu ambiente de Produção ou em um ambiente de sandbox.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano</strong></td> 
   <td> <p> Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licença</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Administrador do sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Onde devo instalar um blueprint? {#where-should-i-install-a-blueprint}

Você pode instalar seu pacote em qualquer um dos seguintes ambientes:

<table style="table-layout:auto">
        <tr>
        <td><strong>Produção</strong></td>
        <td>A produção é o seu ambiente ativo.</td>
    </tr>
    <tr>
        <td><strong>Visualização da sandbox</strong></td>
        <td>A Visualização de sandbox é um ambiente de teste que serve como réplica do ambiente ativo e é atualizado a cada fim de semana pela Workfront. Todos os pacotes de suporte têm acesso à Visualização da sandbox. Para obter mais informações, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">O [!DNL Adobe Workfront] Visualizar ambiente do Sandbox</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 e 2</strong></td>
        <td>A Sandbox de atualização personalizada é um ambiente de teste separado, que é atualizado manualmente por você. Há um custo adicional para obter a Caixa de proteção de atualização personalizada. Para obter mais informações, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">O [!DNL Adobe Workfront] Ambiente de sandbox de atualização personalizada</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Recomendamos primeiro instalar o blueprint em um ambiente de sandbox. Dessa forma, você pode testar o conteúdo do blueprint e certificar-se de que ele é adequado para sua organização sem fazer alterações nos dados ao vivo.

>[!NOTE]
>
>Determinados blueprints só estão disponíveis para instalação no ambiente Preview para fins de teste. Se você acessar o conteúdo Somente visualização no ambiente de Produção, Sandbox 1 ou Sandbox 2, o botão de instalação não estará ativo e poderá ver uma mensagem de aviso.\
>Além disso, o recurso de alternância de ambiente é limitado ao acessar conteúdo somente visualização, mesmo quando você está no ambiente de Visualização.

## Instalar o blueprint

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront, em seguida, clique em **[!UICONTROL Blueprints]**.
1. Encontre o blueprint que deseja instalar. Você pode filtrar por caso de uso, nível de maturidade, status de instalação e digitar no lado direito.
1. (Opcional) Clique em **[!UICONTROL Detalhes]** para saber como funciona o blueprint.
1. Clique em **[!UICONTROL Instalar]**.
1. Escolha instalar no ambiente de produção ou em um ambiente sandbox.\
   Para obter mais informações, consulte o [Onde devo instalar um blueprint?](#where-should-i-install-a-blueprint) neste artigo.
1. No [!UICONTROL Configurar] é possível optar por fazer uma das seguintes opções:

   * Instale o blueprint como está. Para tipos de blueprint que não exigem configuração, essa é a única opção. Para tipos de blueprint que precisam de configuração, opcionalmente, você pode optar por instalar o blueprint agora e configurá-lo mais tarde. Clique em **[!UICONTROL Instalar como está]**.
   * Configure o blueprint antes da instalação, para blueprints que exigem configuração. Faça suas seleções de configuração e clique em **[!UICONTROL Instalar blueprint]**.\

      Para obter mais informações, consulte [Configurar um blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
Quando a instalação estiver concluída, uma mensagem exibirá uma lista dos objetos específicos (como funções, equipes ou grupos) que foram instalados com êxito com o blueprint e quaisquer objetos que não foram instalados.

Depois de instalar o blueprint, algumas ações adicionais podem ser necessárias para implantá-lo totalmente. Para obter mais informações, consulte [Ações a serem tomadas após a instalação de um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
