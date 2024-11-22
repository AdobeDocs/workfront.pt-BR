---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Editar documentos em massa
description: É possível editar vários documentos de uma só vez na área Documentos.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: 8c1f829eb29d8cd13524814d98ed353add15e881
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---


# Editar documentos em massa

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Você pode editar a descrição, adicionar formulários personalizados e editar formulários personalizados em vários documentos de uma só vez.

## Considerações ao editar formulários personalizados

Considere o seguinte ao editar formulários personalizados de documento em massa:

* As informações que você está alterando em todos os documentos selecionados substituem as informações existentes em documentos individuais.
* Quando você seleciona documentos com valores diferentes para o mesmo campo, o campo exibe um indicador &quot;Vários valores&quot;. Os campos que são caixas de seleção, botões de opção e alternadores têm um indicador de &quot;Vários valores&quot; ao lado deles.
* Ao atualizar uma opção em um campo de várias opções (como um campo exibido como um conjunto de alternâncias ou caixas de seleção), todas as outras opções devem corresponder entre os documentos selecionados.

>[!BEGINSHADEBOX]

**Exemplo**
Talvez você tenha um formulário personalizado com um campo de caixa de seleção com três caixas de seleção (Opção 1, Opção 2 e Opção 3) e a Opção 1 esteja desmarcada para todos os documentos selecionados, e as Opções 2 e 3 estejam marcadas para alguns e desmarcadas para outros documentos selecionados. Se você quiser marcar a Opção 1 para todos os documentos, também deverá fazer com que as Opções 2 e 3 correspondam a todos os projetos selecionados antes de salvar suas alterações. Portanto, você deve selecioná-los ou desmarcá-los para que possam corresponder a todos os projetos selecionados. Se você não alterar nenhuma das opções, poderá salvar o campo como está e os documentos manterão sua seleção atual para todas as opções.

>[!ENDSHADEBOX]

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças da Adobe Workfront*</td> 
   <td><p> Novo: Colaborador ou superior</p> 
   <p> Atual: solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar acesso ao documento</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Editar documentos em massa

Para editar documentos em massa:

1. Navegue até a guia Documentos de um projeto ou até a área Documentos no menu principal.
1. Pressione ctrl ou cmd no teclado e selecione os documentos que deseja editar.
1. Clique no ícone Editar ![ícone editar](assets/edit-icon.png).
   ![editar local do ícone na página](assets/edit-multiple-documents.png)
1. (Opcional) Adicione ou edite a **Descrição**. Se a descrição de cada documento for diferente, você verá _Vários valores_ na caixa de descrição. Você pode adicionar a mesma descrição para todos os documentos, mas não pode editar descrições de documentos individuais ao editar em massa.
1. Faça as seguintes alterações com formulários personalizados:

   <table>
    <tr>
    <td><strong>Adicionar formulários</strong></td>
    <td>Na <strong>caixa Adicionar formulário personalizado</strong>, você pode escolher entre formulários anexados e formulários a serem adicionados. Os formulários anexados estão em alguns dos documentos selecionados, mas não em todos. Um formulário anexado a todos os documentos selecionados é exibido automaticamente na janela de edição.  </td>
    </tr>
    <tr>
    <td><strong>Editar formulários</strong></td>
    <td>Edite quaisquer formulários personalizados anexados. As informações alteradas substituem as informações existentes em documentos individuais. Campos com valores diferentes em documentos são exibidos como "Vários valores". </td>
    </tr>
    <tr>
    <td><strong>Reorganizar formulários</strong></td>
    <td>Clique e arraste o formulário personalizado para reorganizar.</td>
    </tr>
    </table>
1. Clique em **Salvar**.


