---
product-area: reporting
keywords: alterar,proprietário,compartilhado,relatório,compartilhar,executar,usuário,acesso,direitos,inserido,último,exibido,data,relatórios,atividades
navigation-topic: report-usage
title: Criar um relatório sobre atividades de relatório
description: Ao criar um relatório sobre relatórios, você pode identificar informações específicas do relatório, que podem incluir se os relatórios são atribuídos a usuários desativados, se os relatórios são definidos para serem executados com direitos de acesso de um usuário desativado, se os usuários estão acessando um relatório que você planeja excluir e assim por diante.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# Criar um relatório sobre atividades de relatório

Ao criar um relatório sobre relatórios, você pode identificar informações específicas do relatório, que podem incluir se os relatórios são atribuídos a usuários desativados, se os relatórios são definidos para serem executados com direitos de acesso de um usuário desativado, se os usuários estão acessando um relatório que você planeja excluir e assim por diante.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Criar o relatório sobre relatórios existentes {#create-the-report-about-existing-reports}

1. Clique no ícone **Menu Principal** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.
1. Clique em **Relatórios** e depois em **Novo Relatório**.
1. No menu suspenso **Novo Relatório**, selecione **Relatório** para criar um relatório sobre relatórios existentes.

1. Na guia **Colunas (Modo de Exibição)**, adicione as colunas desejadas no relatório.\
   Alguns dos seguintes campos podem ser úteis:

   | Campo | Descrição |
   |---|---|
   | **Executar como Usuário: Nome** | Este é o usuário especificado no **Executar este relatório com o campo Direitos de Acesso de:** no relatório. Se esse usuário estiver desativado, um relatório não será exibido para ninguém com quem o relatório é compartilhado. |
   | **Compartilhado com** | Essas são todas as entidades com as quais o relatório é compartilhado. |
   | **Cadastrado por** | Este é o proprietário do relatório. |
   | **Data da Última Visualização** | Esta é a data e hora em que o relatório foi visualizado pela última vez por um usuário. |

   {style="table-layout:auto"}

1. (Opcional) Para limitar sua lista de relatórios a usuários desativados específicos:

   1. Selecione a guia **Filtros** e clique em **Adicionar uma Regra de Filtro**.

   1. Adicionar o filtro **Executar como ID de Usuário** > **Igual**.

   1. Digite o nome do usuário desativado que deseja adicionar ao filtro e clique no nome quando ele for exibido na lista.
   1. Repita a Etapa C até selecionar todos os usuários desativados que deseja incluir no relatório.

1. (Opcional) Para limitar sua lista de relatórios a relatórios agendados:

   1. Selecione a guia **Filtros** e clique em **Adicionar uma Regra de Filtro**.

   1. Adicionar o filtro **ID do Relatório Agendado** > **Não Está em Branco**.

1. Clique em **Salvar + Fechar**, digite um nome para o relatório e clique em **Salvar Relatório**.

   As informações do relatório são exibidas.

1. (Opcional) Exporte este relatório para o Excel e salve-o em seu computador.\
   Para obter informações sobre como exportar um relatório, consulte [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Atualizar informações sobre um relatório

Depois de criar o relatório, você pode atualizá-los conforme necessário.

1. Vá para o relatório que deseja atualizar.
1. Dependendo da ação que deseja executar, execute um dos procedimentos a seguir:

   * Atualizar o **Executar este relatório com o campo Direitos de Acesso de:** para um usuário ativo: Para obter mais informações, consulte [Executar e entregar um relatório com os direitos de acesso de outro usuário](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Criar uma cópia do relatório: Para obter mais informações, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Excluir um relatório: Para obter mais informações, consulte a seção [Criar uma cópia exata de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) do artigo [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Compartilhar um relatório: para obter mais informações, consulte [Compartilhar um relatório no Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Condicional) Se você copiar os relatórios originais, use as informações do relatório que você criou em [Criar o relatório sobre relatórios existentes](#create-the-report-about-existing-reports) para compartilhar as novas cópias com as mesmas entidades dos relatórios originais.
