---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Instalar um Blueprint
description: Você pode instalar um esquema no ambiente de produção ou em um ambiente de sandbox.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 9%

---

# Instalar um blueprint

<!-- Audited: 5/2025 -->

Você pode instalar um esquema no ambiente de produção ou em um ambiente de sandbox.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <p>Padrão</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Administrador do Workfront</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Onde devo instalar um esquema? {#where-should-i-install-a-blueprint}

Você pode instalar o pacote em qualquer um dos seguintes ambientes:

<table style="table-layout:auto">
        <tr>
        <td><strong>Produção</strong></td>
        <td>A produção é o seu ambiente ativo.</td>
    </tr>
    <tr>
        <td><strong>Visualização da sandbox</strong></td>
        <td>A visualização da sandbox é um ambiente de teste que serve como uma réplica do seu ambiente ativo e é atualizado todos os finais de semana pelo Adobe Workfront. Todos os pacotes de suporte têm acesso à Visualização da sandbox. Para obter mais informações, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">O [!DNL Adobe Workfront] Ambiente de Sandbox de Visualização</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 e 2</strong></td>
        <td>A Sandbox de atualização personalizada é um ambiente de teste separado que é atualizado manualmente por você. Há um custo adicional para obter a Sandbox de Atualização Personalizada. Para obter mais informações, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">O [!DNL Adobe Workfront] ambiente da Sandbox de Atualização Personalizada</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Recomendamos primeiro instalar o blueprint em um ambiente de sandbox. Dessa forma, você pode testar o conteúdo do projeto e garantir que ele seja adequado à sua organização sem fazer alterações nos dados dinâmicos.

>[!NOTE]
>
>Alguns blueprints estão disponíveis apenas para instalação no ambiente de visualização para fins de teste. Se você acessar somente a Visualização no ambiente de produção, Sandbox 1 ou Sandbox 2, o botão de instalação não estará ativo e uma mensagem de aviso poderá ser exibida.\
>Além disso, o recurso de alternância de ambiente é limitado ao acessar conteúdo somente visualização, mesmo quando você está no ambiente de visualização.

## Instalar o esquema

{{step1-to-blueprints}}

1. Encontre o esquema que deseja instalar. Você pode filtrar por caso de uso, nível de maturidade, status de instalação e tipo no lado direito da página.
1. (Opcional) Clique em **[!UICONTROL Detalhes]** para saber como o esquema funciona.
1. Clique em **[!UICONTROL Instalar]**.
1. Escolha instalar em seu ambiente de produção ou em um ambiente de sandbox.\
   Para obter mais informações, consulte [Onde devo instalar um blueprint?Seção &#x200B;](#where-should-i-install-a-blueprint) neste artigo.
1. Na página **Configurar**, você pode optar por fazer o seguinte:

   * Instale o esquema como está. Para tipos de blueprint que não requerem nenhuma configuração, esta é a única opção. Para tipos de blueprint que precisam de configuração, você também pode optar por instalar o blueprint agora e configurá-lo mais tarde. Clique em **[!UICONTROL Instalar como está]**.
   * Configure o blueprint antes da instalação do para blueprints que requerem configuração. Faça suas seleções de configuração e clique em **[!UICONTROL Instalar o blueprint]**.

     Para obter mais informações, consulte [Configurar um esquema](../../administration-and-setup/blueprints/configure-template-package.md).

   A instalação é concluída e uma mensagem exibe uma lista de objetos específicos (como funções, equipes ou grupos) que foram instalados com êxito com o esquema e todos os objetos que não foram instalados.

Depois de instalar o blueprint, algumas ações adicionais podem ser necessárias para implantá-lo totalmente. Para obter mais informações, consulte [Ações a serem executadas após a instalação de um esquema](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
