---
title: Ativar uma Workspace do Workfront Planning para o GenStudio for Performance Marketing
description: Você pode disponibilizar um espaço de trabalho do Adobe Workfront Planning no GenStudio for Performance Marketing quando tiver acesso a ambos os aplicativos.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 9dc53e749a61247529d67ce077856ea6bea8e494
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 4%
---
# Ativar um espaço de trabalho do Workfront Planning para o GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--Iskuhi said "ACPC projects" will be renamed when this will be released but not sure if it has been. Follow up with Syuzanna, Gurgen Mosesyan and possibly Himanshi Kumar - see slack threads -->

Quando sua empresa também compra o Adobe GenStudio for Performance Marketing e você é um cliente do Adobe Workfront Planning, o espaço de trabalho do GenStudio também está disponível no Workfront Planning.

Se você já tiver um espaço de trabalho do Planning no Workfront Planning, poderá habilitá-lo para o GenStudio for Performance Marketing em vez de recriar os mesmos dados a partir dele no GenStudio.

A habilitação de um espaço de trabalho o vincula a um projeto do Adobe Could Storage e mapeia seus tipos de registros e campos para o espaço de trabalho do GenStudio. Após concluir a configuração, você pode abrir os registros do espaço de trabalho no GenStudio.

Você deve ter o seguinte:

* Acesso ao Workfront Planning e ao GenStudio for Performance Marketing.
* Um projeto do Adobe Cloud Storage para vincular ao espaço de trabalho. Um administrador de organização pode criar um na Adobe Admin Console.

  Para obter informações, consulte [Gerenciar armazenamento do Adobe](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html). <!--ensure this site still works-->

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer Workfront ou Fluxo de trabalho e qualquer pacote do Planning</p> 
Ou
<p>Qualquer pacote do Planning quando adquirido como um produto independente</p>

</td> 
   <tr> 
<td> 
   <p> Produtos adicionais</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>

<tr> 
<td> 
   <p> Configurações do Adobe Admin Console</p> </td> 
   <td> 
   <p> Você deve criar projetos da Adobe Storage Cloud na Adobe Admin Console </p>

<p>Para obter informações, consulte <a href="https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/projects-in-business-storage.html#project-policies">Gerenciar projetos</a>

</td> 
  </tr>
  <tr>

<tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Planejamento padrão</p>
   </td> 
  </tr>
<tr> 
   <td role="rowheader"><p>Configuração do nível de acesso Adobe Workfront</p></td> 
   <td> <p>Você deve adicionar um Workflow e um tipo de licença do Planning ao nível de acesso do Workfront quando tiver um Workflow e um pacote do Planning</p>   
</td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Funções de usuário do Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Qualquer função de usuário do GenStudio se precisar acessar Campanhas, Produtos e Personalidades</li>
   <li>GenStudio System Manager se você precisar acessar Ativations <!--and Events--></li></ul>
   Para obter informações, consulte <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funções e permissões de usuário</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>  
   <p>No Workfront Planning: </p>
   <ul>
   <li><p>Gerenciar permissões no espaço de trabalho <!--to add new fields or record types to the GenStudio workspace--></p></li>
   <!--
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   -->
   </ul>
   <!--
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   -->
   <p>No Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <!--
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   -->
   <li><p> Criar permissões no Adobe GenStudio for Performance Marketing para criar itens</p></li></ul>
   </td>  
</tbody> 
</table>

Para obter informações sobre o acesso ao Adobe Workfront Planning, consulte [Visão geral do acesso ao Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Para obter mais informações sobre o Adobe GenStudio for Performance Marketing, consulte [Guia do Usuário do Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home).

+++ 

## Ativar um espaço de trabalho do Workfront Planning para o GenStudio

1. No Workfront Planning, abra o espaço de trabalho que deseja ativar.
1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do espaço de trabalho e clique em **Habilitar GenStudio**.

   A caixa **Criar espaço de trabalho habilitado para GenStudio** é aberta com as seguintes etapas:

   1. **Projeto ACPC**: selecione o **Projeto ACPC** (projeto do Adobe Cloud Storage) que deseja sincronizar com este espaço de trabalho e clique em **Avançar**. Os usuários acessam o espaço de trabalho no GenStudio por meio deste projeto.

      ![Habilitar o GenStudio do espaço de trabalho - etapa do projeto ACPC](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **Tipos de registro**: mapeie os tipos de registro do espaço de trabalho para os seis tipos de registro exigidos pela GenStudio:

      * Campanhas
      * Produtos
      * Personas
      * Canais
      * Regiões
      * Ativações

      Para cada um, abra a lista e selecione o tipo de registro correspondente do Planning ou selecione **Adicionar novo** para criá-lo e clique em **Avançar**.

      ![Habilitar o GenStudio do espaço de trabalho - Etapa de tipos de registro](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **Campos**: mapeie os campos para cada tipo de registro. Use as guias na parte superior da caixa de diálogo para se mover entre tipos de registro. Para cada campo, selecione o campo correspondente do Planning ou selecione **Adicionar novo** para criar um campo.

      Repita a configuração de campo para todos os tipos de registro.

      ![Habilitar o GenStudio do espaço de trabalho - Etapa de campos](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. Analise e resolva quaisquer avisos.

      Por exemplo, um novo campo pode se tornar o campo principal do tipo de registro ou um alias de campo que já está em uso é renomeado (se você já tiver um campo chamado &quot;Regiões&quot;, o campo importado pode se tornar &quot;Regiões 2&quot;).

      Mapear um campo **Status** adiciona as opções necessárias.

   1. Clique em **Publicar**.

      Uma mensagem de confirmação é exibida quando o espaço de trabalho é ativado. Os tipos de registro mapeados são marcados no espaço de trabalho.

      Os tipos de registro mapeados para serem acessíveis pelo GenStudio têm um novo ícone **Adobe** em seus cartões.

      ![Tipo de registro de campanhas com ícone do Adobe](assets/campaigns-record-type-card-with-adobe-icon.png)

1. Abra o GenStudio, selecione **Campanhas** e clique no **projeto ACPC** que você configurou originalmente para esta configuração no canto inferior esquerdo da tela. Revise os tipos e campos de registro importados.

   >[!TIP]
   >
   >Você verá apenas os registros permitidos pela associação ao projeto Adobe Cloud Storage.
