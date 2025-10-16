---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Instalar um blueprint
description: Você pode instalar um blueprint no seu ambiente de produção ou um ambiente de sandbox.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: 5fd855bec596926a4361fd07a1a763c7956e5e61
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# Instalar um blueprint

<!-- Audited: 5/2025 -->

Você pode instalar um blueprint no seu ambiente de produção ou um ambiente de sandbox.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>administrador do Workfront</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Onde devo instalar um blueprint? {#where-should-i-install-a-blueprint}

Você pode instalar seu pacote em qualquer um dos seguintes ambientes:

<table style="table-layout:auto">
        <tr>
        <td><strong>Produção</strong></td>
        <td>A produção é o seu ambiente ativo.</td>
    </tr>
    <tr>
        <td><strong>Visualização da sandbox</strong></td>
        <td>A visualização da sandbox é um ambiente de teste que serve como uma réplica do seu ambiente ativo e é atualizado todos os finais de semana pela Adobe Workfront. Todos os pacotes de suporte têm acesso à Visualização da sandbox. Para obter mais informações, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">O [!DNL Adobe Workfront] Ambiente de pré-visualização da sandbox</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 e 2</strong></td>
        <td>A sandbox de atualização personalizada é um ambiente de teste separado que é atualizado manualmente por você. Há um custo adicional para obter a sandbox de atualização personalizada. Para obter mais informações, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">O [!DNL Adobe Workfront] ambiente da Sandbox de Atualização Personalizada</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Recomendamos instalar primeiro o blueprint em um ambiente de sandbox. Dessa forma, você pode testar o conteúdo do blueprint e garantir que ele se ajuste bem à sua organização sem fazer alterações nos dados em tempo real.

>[!NOTE]
>
>Determinados blueprints só estão disponíveis para instalação no ambiente de Pré-visualização para fins de teste. Se você acessar somente o conteúdo de Visualização no seu ambiente de Produção, Sandbox 1 ou Sandbox 2, o botão Instalar não estará ativo e você poderá ver uma mensagem de aviso.\
>Além disso, o recurso de alternância de ambiente é limitado ao acessar conteúdo somente visualização, mesmo quando você está no ambiente de Visualização.

## Instalar o blueprint

{{step1-to-blueprints}}

1. Encontre o blueprint que deseja instalar. Você pode filtrar por caso de uso, nível de maturidade, status de instalação e tipo no lado direito da página.
1. (Opcional) Clique em **[!UICONTROL Detalhes]** para saber como o blueprint funciona.
1. Clique em **[!UICONTROL Instalar]**.
1. Escolha instalar no ambiente de produção ou em um ambiente de sandbox.\
   Para obter mais informações, consulte o [Onde devo instalar um blueprint?seção ](#where-should-i-install-a-blueprint) neste artigo.
1. Na página **Configurar**, você pode optar por executar um dos seguintes procedimentos:

   * Instale o blueprint como está. Para tipos de blueprint que não exigem configuração, essa é a única opção. Para tipos de blueprint que precisam de configuração, você pode optar por instalar o blueprint agora e configurá-lo posteriormente. Clique em **[!UICONTROL Instalar como está]**.
   * Configure o blueprint antes da instalação do para blueprints que exigem configuração. Faça suas seleções de configuração e clique em **[!UICONTROL Instalar blueprint]**.

     Para obter mais informações, consulte [Configurar um blueprint](../../administration-and-setup/blueprints/configure-template-package.md).

   A instalação é concluída e uma mensagem exibe uma lista dos objetos específicos (como funções, equipes ou grupos) que foram instalados com êxito com o blueprint e todos os objetos que falharam na instalação.

Depois de instalar o blueprint, algumas ações adicionais podem ser necessárias para implantá-lo totalmente. Para obter informações, consulte [Ações a serem executadas após a instalação de um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
