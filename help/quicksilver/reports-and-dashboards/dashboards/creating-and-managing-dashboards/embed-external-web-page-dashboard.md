---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incorporar uma página da Web externa em um painel
description: Você pode incorporar uma página da Web externa em um painel para fornecer acesso a informações relacionadas de outros sistemas no Adobe Workfront ou a outras páginas do Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: a8a3aec50b5538de5867ce3ba7723d92c046b50d
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Incorporar uma página da Web externa em um painel

Você pode incorporar uma página da Web externa em um painel para fornecer acesso a informações relacionadas de outros sistemas no Adobe Workfront ou a outras páginas do Workfront.

Por exemplo, se sua organização tiver um repositório de documentos baseado na Web, wiki ou outro sistema de gerenciamento de conteúdo que contenha informações do projeto acessadas regularmente por meio de um URL, você poderá exibir essas informações no Workfront criando uma página externa em um painel.

>[!IMPORTANT]
>
>Por motivos de segurança, alguns sites não permitem que você incorpore páginas da Web como um iframe. Se a página da Web que você deseja incorporar em um painel não permitir isso, a página não será exibida no painel. No entanto, ainda é possível acessar a página externa clicando no nome do painel.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Para permitir a incorporação de um site que você possui, trabalhe com o administrador da Web para ajustar a variável **X-Frame-Options** configuração. Para obter mais informações, consulte [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).


>[!IMPORTANT]
>
>Páginas de painel não são mais suportadas como páginas externas incorporadas em Painéis. Especificamente, os seguintes subdomínios Workfront.com não são mais compatíveis:
>
>* /painéis &#x200B;
>* /dashboard/:ID &#x200B;
>* /portfólio/:ID/content-dashboard_:dashboardID &#x200B;
>* /program/:ID/content-dashboard_:dashboardID &#x200B;
>* /project/:ID/content-dashboard_:dashboardID &#x200B;
>* /task/:ID/content-dashboard_:dashboardID &#x200B;
>* /template/:ID/content-dashboard_:dashboardID &#x200B;
>* /templatetask/:ID/content-dashboard_:dashboardID &#x200B;
>* /resourcemanagement/:ID/content-dashboard_:dashboardID &#x200B;
>* /equipe/:ID/content-dashboard_:dashboardID &#x200B;
>* /iteração/:ID/content-dashboard_:dashboardID &#x200B;
>* /requests/:ID/content-dashboard_:dashboardID &#x200B;
>* /group/:ID/content-dashboard_:dashboardID &#x200B;
>* /billingrecord/:ID/content-dashboard__:dashboardID


## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a Relatórios, Painéis e Calendários</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões no painel</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve criar um painel antes de poder incorporar uma página externa a ele.

Para obter informações sobre como criar painéis, consulte [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Incorporar uma página externa em um painel

>[!IMPORTANT]
>
>Você pode remover uma Página externa de um painel se ela não for mais necessária. No entanto, não é possível excluir uma página externa após sua criação no Workfront. Você pode excluir uma página externa somente usando a API . Para obter mais informações, consulte [Remover uma página externa de um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Localize o URL da página a ser exibida no Workfront e copie o URL localizado na barra de endereços.

   >[!NOTE]
   >
   >Se você estiver compartilhando URLs em objetos Workfront, lembre-se de que alguns URLs expiram ao longo do tempo. Por exemplo, os URLs do documento expiram depois de terem sido abertos. Isso é configurado como uma medida de segurança e, por design, são considerados URLs não estáticos e não devem ser compartilhados.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png), depois clique em **Painéis**.

1. Para editar um painel existente, selecione o painel no qual deseja incorporar a página do site e clique em **Ações do painel** e selecione **Editar** no menu .\
   Ou\
   Para criar um novo painel, clique em **Novo painel**.\
   Para obter mais informações sobre como criar um painel, consulte [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Clique em **Adicionar página externa**.

   ![](assets/qs-add-external-page-350x239.png)

1. Especifique um **Nome** para a página externa.
1. Especifique um **Descrição**.
1. Cole o URL copiado anteriormente no **URL** campo.\
   Você pode especificar os seguintes tipos de URLs:

   * Um URL https (criptografado) para uma página da Web.\
      Somente as páginas https (criptografadas) são carregadas com o URL.\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * Um URL de modelo que contém informações de sessão para um site específico.\
      Por exemplo: *https://localhost/?session={!$$SESSION}*
Você deve estar conectado ao site especificado para exibir a Página externa.\
      Para obter informações sobre como obter uma SessionID do Workfront, consulte [Noções básicas da API](../../../wf-api/general/api-basics.md).\
      O administrador do Workfront pode configurar as preferências do sistema de uma maneira que não permita o uso de informações da sessão em suas páginas externas, por motivos de segurança. Nesse caso, a página externa não é carregada no painel.\
      Para obter mais informações sobre preferências de segurança do sistema, consulte [Configurar preferências de segurança do sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. Clique em **Salvar**.\
   A página é adicionada automaticamente ao painel. Se os painéis futuros forem criados, a página externa poderá ser adicionada. A página externa será encontrada entre os Relatórios disponíveis.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## Atualizar uma página externa em um painel

Para atualizar as informações de uma página externa usada em um painel:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png), depois clique em **Painéis**.
1. Selecione o painel que deseja atualizar e clique em **Editar** ![](assets/edit-icon.png).

   ![Selecione o ícone Edit .](assets/nwe-editdashboard2021-350x188.png)

1. No lado direito da tela, localize a página externa que deseja atualizar e clique no botão **Editar** ícone .\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. No **Editar página externa** , atualize os campos que deseja alterar e clique em **Salvar**.
1. (Opcional) Clique no botão **Excluir** ícone ![](assets/delete.png) para remover a página externa do painel. Para obter mais informações, consulte [Remover uma página externa de um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. No canto inferior esquerdo, clique em **Salvar + Fechar**.

## Exibir páginas externas em um relatório

Você pode exibir todas as páginas externas no Workfront em um relatório de Página externa.

1. Vá para o **Menu principal** ícone ![](assets/main-menu-icon.png) > **Relatórios**.
1. Clique em **Novo relatório** > selecionar **Página Externa**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Opcional) Atualize as guias Exibir, Filtros ou Agrupamentos do relatório.

   Para obter mais informações, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Clique em **Salvar+Fechar**.

   Você pode exibir o nome e o URL associados às páginas externas em seu sistema no novo relatório.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
