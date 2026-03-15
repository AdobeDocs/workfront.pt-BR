---
product-area: reporting
keywords: alterar,proprietário,compartilhado,relatório,compartilhar,executar,usuário,acesso,direitos,inserido,última,visualizado,data,relatório,atividades
navigation-topic: report-usage
title: Criar um relatório sobre atividades de relatório
description: Ao criar um relatório sobre relatórios, você pode identificar informações específicas de relatório, que podem incluir se os relatórios são atribuídos a usuários desativados, se os relatórios são definidos para execução com direitos de acesso de um usuário desativado, se os usuários estão acessando um relatório que você planeja excluir e assim por diante.
author: Courtney
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 9%

---

# Criar um relatório sobre atividades de relatório

Ao criar um relatório sobre relatórios, você pode identificar informações específicas de relatório, que podem incluir se os relatórios são atribuídos a usuários desativados, se os relatórios são definidos para execução com direitos de acesso de um usuário desativado, se os usuários estão acessando um relatório que você planeja excluir e assim por diante.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Padrão</p>
   <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários</p> <p>Editar acesso a filtros, exibições e agrupamentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar o relatório sobre relatórios existentes {#create-the-report-about-existing-reports}

1. Clique no ícone **Menu Principal** ícone ![Menu Principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.
1. Clique em **Relatórios** e depois em **Novo Relatório**.
1. No menu suspenso **Novo Relatório**, selecione **Relatório** para criar um relatório sobre relatórios existentes.

1. Na guia **Colunas (Exibição)**, adicione as colunas desejadas no relatório.\
   Alguns dos seguintes campos podem ser úteis:

   | Campo | Descrição |
   |---|---|
   | **Executar Como Usuário: Nome** | Este é o usuário especificado no **Executar este relatório com o campo Direitos de Acesso de:** no relatório. Se este usuário estiver desativado, um relatório não será exibido para ninguém com quem o relatório está compartilhado. |
   | **Compartilhado com** | Estas são todas as entidades com as quais o relatório é compartilhado. |
   | **Inserido por** | Este é o proprietário do relatório. |
   | **Última Data Visualizada** | Esta é a data e a hora em que o relatório foi visualizado pela última vez por um usuário. |

   {style="table-layout:auto"}

1. (Opcional) Para limitar sua lista de relatórios a usuários desativados específicos:

   1. Selecione a guia **Filtros** e clique em **Adicionar uma Regra de Filtro**.

   1. Adicionar o filtro **Executar como ID de Usuário** > **Igual**.

   1. Digite o nome do usuário desativado que você deseja adicionar ao filtro e, em seguida, clique no nome quando ele for exibido na lista.
   1. Repita a Etapa C até ter selecionado todos os usuários desativados que você deseja incluir no relatório.

1. (Opcional) Para limitar sua lista de relatórios a relatórios agendados:

   1. Selecione a guia **Filtros** e clique em **Adicionar uma Regra de Filtro**.

   1. Adicione o filtro **ID do Relatório Agendado** > **Não Está em Branco**.

1. Clique em **Salvar + Fechar**, digite um nome para o relatório e clique em **Salvar Relatório**.

   As informações do seu relatório são exibidas.

1. (Opcional) Exporte esse relatório para o Excel e salve-o em seu computador.\
   Para obter informações sobre como exportar um relatório, consulte [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Atualizar informações sobre um relatório

Depois de criar o relatório, você pode atualizá-lo conforme necessário.

1. Vá para o relatório que deseja atualizar.
1. Dependendo da ação que você deseja executar, siga um destes procedimentos:

   * Atualize o **Executar este relatório com o campo Direitos de Acesso de:** para um usuário ativo: para obter mais informações, consulte [Executar e entregar um relatório com os direitos de acesso de outro usuário](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Criar uma cópia do relatório: Para obter mais informações, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Excluir um relatório: para obter mais informações, consulte a seção [Criar uma cópia exata de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) do artigo [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Compartilhar um relatório: para obter mais informações, consulte [Compartilhar um relatório no Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Condicional) Se você copiar os relatórios originais, use as informações do relatório criado em [Criar o relatório sobre relatórios existentes](#create-the-report-about-existing-reports) para compartilhar as novas cópias com as mesmas entidades dos relatórios originais.
