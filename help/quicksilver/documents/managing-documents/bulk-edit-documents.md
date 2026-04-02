---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Editar documentos em massa
description: É possível editar vários documentos de uma só vez na área Documentos.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 84%

---

# Editar documentos em massa

Você pode editar a descrição, adicionar formulários personalizados e editar formulários personalizados em vários documentos ao mesmo tempo.

## Considerações ao editar formulários personalizados

Considere o seguinte ao editar formulários personalizados de documentos em massa:

* As informações que você está alterando em todos os documentos selecionados substituem as informações existentes nos documentos individuais.
* Quando você seleciona documentos que têm valores diferentes para o mesmo campo, o campo exibe um indicador “Múltiplos valores”. Os campos que são caixas de seleção, botões de opção e botões de alternância têm um indicador “Múltiplos valores” ao lado deles.
* Quando você atualiza uma opção em um campo com várias opções (como um campo que exibe um conjunto de botões ou caixas de seleção), todas as outras opções devem corresponder entre os documentos selecionados.

>[!BEGINSHADEBOX]

**Exemplo**
Você pode ter um formulário personalizado com um campo de caixa de seleção e três caixas de seleção (Opção 1, Opção 2 e Opção 3), no qual a Opção 1 está desmarcada para todos os documentos selecionados e as Opções 2 e 3 estão marcadas para alguns documentos e desmarcadas para outros documentos selecionados. Se você deseja marcar a Opção 1 para todos os documentos, também deve fazer com que as Opções 2 e 3 correspondam a todos os projetos selecionados antes de salvar suas alterações. Portanto, você deve selecioná-las ou desmarcá-las para que correspondam em todos os projetos selecionados. Se você não alterar nenhuma das opções, poderá salvar o campo como está, e os documentos manterão a seleção atual para todas as opções.

>[!ENDSHADEBOX]

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront*</td> 
   <td><p>Colaborador ou posterior</p> 
   <p>Solicitação ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar o acesso ao documento</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar documentos em massa na área de documentos herdados

Se sua organização utiliza o Workfront Storage herdado, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o Workfront Storage, consulte [Diferenças entre o Adobe Enterprise Storage e o Workfront Storage herdado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

Para editar documentos em massa:

1. Navegue até a guia Documentos de um projeto ou até a área Documentos no menu principal.
1. Pressione Ctrl ou Cmd no teclado e selecione os documentos que deseja editar.
1. Clique no ícone Editar ![Ícone Editar](assets/edit-icon.png).
   ![Local do ícone Editar na página](assets/edit-multiple-documents.png)
1. (Opcional) Adicione ou edite a **Descrição**. Se a descrição de cada documento for diferente, você verá _Múltiplos valores_ na caixa de descrição. Você pode adicionar a mesma descrição para todos os documentos, mas não pode editar descrições individuais de documentos ao editar em massa.
1. Faça as seguintes alterações com formulários personalizados:

   <table>
    <tr>
    <td><strong>Adicionar formulários</strong></td>
    <td>Na <strong>caixa Adicionar formulário personalizado</strong>, você pode escolher entre formulários anexados e formulários a serem adicionados. Os formulários anexados estão em alguns dos documentos selecionados, mas não em todos. Um formulário anexado a todos os documentos selecionados é exibido automaticamente na janela de edição.  </td>
    </tr>
    <tr>
    <td><strong>Editar formulários</strong></td>
    <td>Edite quaisquer formulários personalizados anexados. As informações que você alterar substituirão as informações existentes nos documentos individuais. Os campos com valores diferentes nos documentos são exibidos como “Múltiplos valores”. </td>
    </tr>
    <tr>
    <td><strong>Reorganizar formulários</strong></td>
    <td>Clique e arraste o formulário personalizado para reorganizá-lo.</td>
    </tr>
    </table>
1. Clique em **Salvar**.

## Editar documentos em massa na nova área de documentos


Se sua organização usar armazenamento corporativo, você verá a nova área de documentos ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento corporativo, consulte [visão geral sobre o armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para editar documentos em massa:

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Pressione Ctrl ou Cmd no teclado e selecione os documentos que deseja editar.
1. Clique em Editar na parte inferior da página.
   ![editar vários documentos](assets/bulk-edit-documents.png)
1. (Opcional) Adicione ou edite a **Descrição**. Se a descrição de cada documento for diferente, você verá _Múltiplos valores_ na caixa de descrição. Você pode adicionar a mesma descrição para todos os documentos, mas não pode editar descrições individuais de documentos ao editar em massa.
1. Faça as seguintes alterações com formulários personalizados:

   <table>
    <tr>
    <td><strong>Adicionar formulários</strong></td>
    <td>Na seção <strong>Formulário personalizado</strong>, você pode adicionar um novo formulário personalizado aos documentos selecionados. Formulários personalizados anexados a todos os documentos selecionados são exibidos na seção <strong>Formulários personalizados em comum</strong>.  </td>
    </tr>
    <tr>
    <td><strong>Editar formulários</strong></td>
    <td>Edite quaisquer formulários personalizados anexados. As informações que você alterar substituirão as informações existentes nos documentos individuais. Os campos com valores diferentes nos documentos são exibidos como “Múltiplos valores”. </td>
    </tr>
    </table>
1. Clique em **Salvar**.

## Editar documentos em massa em um relatório de documentos

1. Navegue até um relatório de documento existente.
ou
Crie um relatório de documento conforme descrito em [Criar um relatório personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Selecione os documentos que deseja editar.
1. Clique no ícone Editar ![Ícone Editar](assets/edit-icon.png).
1. (Opcional) Adicione ou edite a **Descrição**. Se a descrição de cada documento for diferente, você verá _Múltiplos valores_ na caixa de descrição. Você pode adicionar a mesma descrição para todos os documentos, mas não pode editar descrições individuais de documentos ao editar em massa.
1. Faça as seguintes alterações com formulários personalizados:

   <table>
    <tr>
    <td><strong>Adicionar formulários</strong></td>
    <td>Na <strong>caixa Adicionar formulário personalizado</strong>, você pode escolher entre formulários anexados e formulários a serem adicionados. Os formulários anexados estão em alguns dos documentos selecionados, mas não em todos. Um formulário anexado a todos os documentos selecionados é exibido automaticamente na janela de edição.  </td>
    </tr>
    <tr>
    <td><strong>Editar formulários</strong></td>
    <td>Edite quaisquer formulários personalizados anexados. As informações que você alterar substituirão as informações existentes nos documentos individuais. Os campos com valores diferentes nos documentos são exibidos como “Múltiplos valores”. </td>
    </tr>
    <tr>
    <td><strong>Reorganizar formulários</strong></td>
    <td>Clique e arraste o formulário personalizado para reorganizá-lo.</td>
    </tr>
    </table>
1. Clique em **Salvar**.
