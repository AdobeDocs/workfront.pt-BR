---
product-area: reporting
keywords: alterar,proprietário,compartilhado,relatório,compartilhar,executar,usuário,acesso,direitos,inseridos,último,visualizado,data,relatórios,atividades
navigation-topic: report-usage
title: Criar um relatório sobre atividades de relatório
description: Ao criar um relatório sobre relatórios, você pode identificar informações específicas do relatório, que podem incluir se os relatórios forem atribuídos a usuários desativados, se os relatórios forem definidos para serem executados com direitos de acesso de um usuário desativado, se os usuários estiverem acessando um relatório que você planeja excluir, e assim por diante.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 2%

---

# Criar um relatório sobre atividades de relatório

Ao criar um relatório sobre relatórios, você pode identificar informações específicas do relatório, que podem incluir se os relatórios forem atribuídos a usuários desativados, se os relatórios forem definidos para serem executados com direitos de acesso de um usuário desativado, se os usuários estiverem acessando um relatório que você planeja excluir, e assim por diante.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar o relatório sobre relatórios existentes {#create-the-report-about-existing-reports}

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.
1. Clique em **Relatórios**, em seguida **Novo relatório**.
1. No **Novo relatório** menu suspenso, selecione **Relatório** para criar um relatório sobre relatórios existentes.

1. No **Colunas (Exibir)** , adicione as colunas desejadas em seu relatório.\
   Alguns dos seguintes campos podem ser úteis:

   | Campo | Descrição |
   |---|---|
   | **Executar como usuário: Nome** | Esse é o usuário especificado na variável **Execute este relatório com os Direitos de acesso de:** no relatório. Se esse usuário estiver desativado, um relatório não será exibido para ninguém com o qual o relatório é compartilhado. |
   | **Compartilhado com** | Estas são todas as entidades com as quais o relatório é compartilhado. |
   | **Cadastrado por** | Este é o proprietário do relatório. |
   | **Última data da visualização** | Esta é a data e a hora em que o relatório foi visualizado pela última vez por um usuário. |

   {style=&quot;table-layout:auto&quot;}

1. (Opcional) Para limitar sua lista de relatórios a usuários desativados específicos:

   1. Selecione o **Filtros** e, em seguida, clique em **Adicionar uma regra de filtro**.

   1. Adicionar o filtro **Executar como ID de usuário** > **Igual**.

   1. Digite o nome do usuário desativado que deseja adicionar ao filtro e clique no nome quando ele for exibido na lista.
   1. Repita a Etapa C até selecionar todos os usuários desativados que deseja incluir no relatório.

1. (Opcional) Para limitar sua lista de relatórios aos relatórios programados:

   1. Selecione o **Filtros** e, em seguida, clique em **Adicionar uma regra de filtro**.

   1. Adicionar o filtro **ID de relatório agendada** > **Não está em Branco**.

1. Clique em **Salvar + Fechar**, digite um nome para o relatório e clique em **Salvar relatório**.

   Suas informações de relatório são exibidas.

1. (Opcional) Exporte este relatório para o Excel e salve-o em seu computador.\
   Para obter informações sobre como exportar um relatório, consulte [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Atualizar informações sobre um relatório

Após criar seu relatório, você pode atualizar seus relatórios conforme necessário.

1. Vá para o relatório que deseja atualizar.
1. Dependendo da ação que deseja realizar, execute um dos seguintes procedimentos:

   * Atualize o **Execute este relatório com os Direitos de acesso de:** para um usuário ativo: Para obter mais informações, consulte [Executar e entregar um relatório com os direitos de acesso de outro usuário](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Crie uma cópia do relatório: Para obter mais informações, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Excluir um relatório: para obter mais informações, consulte o [Criar uma cópia exata de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) seção do artigo [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Compartilhar um relatório: para obter mais informações, consulte [Compartilhar um relatório no Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Condicional) Se você copiar os relatórios originais, use as informações do relatório que você criou em [Criar o relatório sobre relatórios existentes](#create-the-report-about-existing-reports) para compartilhar as novas cópias com as mesmas entidades dos relatórios originais.
