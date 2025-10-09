---
title: Introdução à Integração do Workfront Planning e do GenStudio for Performance Marketing
description: O espaço de trabalho do GenStudio for Performance Marketing estará disponível no Adobe Workfront Planning quando sua empresa tiver comprado ambos os produtos. Saiba mais sobre as noções básicas sobre como você pode simplificar seus fluxos de trabalho usando essa integração.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: e717e095f1995dbed0232789616d42492156d843
workflow-type: tm+mt
source-wordcount: '1906'
ht-degree: 0%

---

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->


# Introdução à integração do Adobe Workfront Planning e do Adobe GenStudio for Performance Marketing

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

As organizações que usam o Adobe Workfront Planning e o Adobe GenStudio for Performance Marketing geralmente definem conceitos de marketing como Campanhas, Produtos, Ativações e Personalidades com mais detalhes do que o GenStudio suporta por padrão.

Há uma integração nativa entre o GenStudio for Performance Marketing e o Workfront Planning. Essa integração permite que os usuários no Workfront Planning gerenciem Campanhas, Produtos, Personalidades, Ativações, Canais e Regiões usados no GenStudio. Ela também permite configurar o GenStudio para fazer referência aos tipos de registro existentes do Workfront Planning, criando um fluxo de trabalho de marketing mais conectado e consistente.

O espaço de trabalho do GenStudio for Performance Marketing estará disponível no Adobe Workfront Planning quando sua empresa tiver comprado ambos os produtos.

## Benefícios da integração

Com a integração entre o Workfront Planning e o GenStudio for Performance Marketing, você pode:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Exiba o espaço de trabalho do GenStudio no Workfront Planning.
* Modifique suas campanhas, produtos, personalidades e ativações no GenStudio for Performance Marketing e atualize em tempo real as mesmas informações no Workfront Planning.
* Modifique suas campanhas, produtos, personalidades e ativações no Workfront Planning e atualize em tempo real as mesmas informações no GenStudio for Performance Marketing.
* Evite a entrada de dados duplicados.
* Mantenha o alinhamento entre os esforços de planejamento e ativação.

## Requisitos de integração

Sua organização deve atender aos seguintes requisitos para que a integração entre o Workfront Planning e o GenStudio for Performance Marketing exista:

* O Workfront e o GenStudio for Performance Marketing devem ser habilitados para a mesma organização.

  Para obter mais informações sobre o GenStudio, consulte [Guia do Usuário do Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home).

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* Sua instância do Workfront faz parte da Experiência unificada da Adobe, incluindo o uso do Identity Management System (IMS).

  Para obter informações, consulte [Experiência unificada da Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Os usuários que usam o Workfront Planning e o GenStudio for Performance Marketing devem pertencer a apenas uma instância do Workfront na organização IMS.

  Usuários somente do Workfront podem exibir o espaço de trabalho do GenStudio, mesmo que não sejam usuários do GenStudio for Performance Marketing.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Requisitos de acesso

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront</p>
<p>Qualquer pacote do Planning</p>

</td> </tr>
   <tr> 
<td> 
   <p> Produtos adicionais</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Funções de usuário do Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Qualquer função de usuário do GenStudio para acessar Campanhas, Produtos e Personalidades</li>
   <li>GenStudio System Manager para acessar Ativações <!--and Events--></li></ul>
   Para obter informações, consulte <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funções e permissões de usuário</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>  
   <p>No Workfront Planning: </p>
   <ul>
   <li><p>Gerenciar permissões no espaço de trabalho do GenStudio para adicionar novos campos ou tipos de registro ao espaço de trabalho do GenStudio</p></li>
   <li><p>Contribuir com permissões para o espaço de trabalho do GenStudio para adicionar, atualizar ou excluir registros no espaço de trabalho do GenStudio</p> </li>  
   </ul>
   <p>Nenhum usuário pode remover tipos de registro ou campos do GenStudio for Performance Marketing do espaço de trabalho do GenStudio no Workfront Planning</p>
   <p>No Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Quaisquer permissões no Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Criar permissões no Adobe GenStudio for Performance Marketing para criar itens</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

Para obter informações sobre o acesso ao Adobe Workfront Planning, consulte [Visão geral do acesso ao Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Para obter mais informações sobre o Adobe GenStudio for Performance Marketing, consulte [Guia do Usuário do Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home).


## Visão geral dos recursos de integração do Workfront Planning e do GenStudio for Performance Marketing

Dependendo de quantas instâncias do Workfront sua organização tiver, você terá automaticamente as seguintes permissões para o espaço de trabalho do GenStudio no Planning:

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Uma instância do Workfront</p></td> 
   <td> 
<p>O espaço de trabalho do GenStudio está visível na sua instância do Workfront Planning</p>
<p>Todos os usuários, incluindo administradores do Workfront, têm acesso ao espaço de trabalho do GenStudio no Planning por padrão</p>
<p>Os administradores do Workfront podem modificar e conceder permissões de gerenciamento no espaço de trabalho do GenStudio a qualquer pessoa</p>
</td> </tr>
   <tr> 
<td> 
   <p> Várias instâncias do Workfront</p> </td> 
   <td>

<p>O espaço de trabalho do GenStudio está visível em todas as instâncias do Workfront</p>
<p>Todos os usuários com acesso ao GenStudio for Performance Marketing e ao Workfront Planning têm permissões do Contribute no GenStudio no Planning por padrão</p> 
<p>Os administradores do Workfront não podem conceder permissões de gerenciamento ao espaço de trabalho do GenStudio a ninguém</p>
</td> 
  </tr>
   </tbody> 
</table>

<!--If Iskuhi confirms, add this or a corrected version to the second row of the table above:
<p>The following are the scenarios for when your organization has more than one instance of Workfront with Workfront Planning:</p>
   <ul><li>If your company has multiple instances of Workfront at the moment when they purchase Adobe GenStudio for Performance Marketing, the GenStudio workspace is visible from all Workfront instances.</li>
   <li>If your company adds more Workfront instances after their original instance has already been integrated with Adobe GenStudio for Performance Marketing, the GenStudio workspace is visible only from the original Workfront instance. For information about connecting additional instance of Workfront to Adobe GenStudio, contact your account representative. </li></ul>  
   
   -->

Para obter informações sobre permissões do Workfront Planning, consulte [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

As seções abaixo descrevem o seguinte:

* Recursos para atualizar informações do Workfront Planning no GenStudio for Performance Marketing
* Recursos para atualização de informações do GenStudio for Performance Marketing no Workfront Planning
* Limitações para o que você pode ou não gerenciar em um espaço de trabalho do GenStudio no Workfront Planning.

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### O espaço de trabalho do GenStudio no Workfront Planning

* O espaço de trabalho do GenStudio exibe um indicador visual no Workfront Planning para identificá-lo como representando o espaço de trabalho do GenStudio for Performance Marketing.

  ![cartão GenStudio no Planning](assets/genstudio-card-with-tag-highlighted.png)

  Para obter informações, consulte [Gerenciar o espaço de trabalho do GenStudio no Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Quando você tem a opção Gerenciar permissões para o espaço de trabalho do GenStudio no Planning, é possível:

   * Atualizar o espaço de trabalho do GenStudio no Planning (nome, descrição, ícone)
   * Criar seções
   * Adicionar tipos de registro
   * Compartilhar com outras pessoas

     Você pode compartilhar o espaço de trabalho do GenStudio com outras pessoas que não têm uma conta do GenStudio. Você pode compartilhá-lo somente com usuários disponíveis no Sistema Identity Management (IMS) de sua organização. <!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* Quando você tem permissões do Contribute para o espaço de trabalho do GenStudio no Planning, não é possível modificar o espaço de trabalho do Workfront Planning.

### Tipos de registro no espaço de trabalho do GenStudio

* Os tipos de registro visíveis no GenStudio for Performance Marketing e no Planning têm um indicador GenStudio no Workfront Planning.

  ![Cartão de tipo de registro do GenStudio no Workfront Planning](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* Quando você tem permissões para Gerenciar o espaço de trabalho do GenStudio no Planning, é possível fazer o seguinte no Workfront Planning:
   * Editar informações de tipos de registros do GenStudio (sua aparência, configurações avançadas).
   * Compartilhar tipos de registros do GenStudio com outras pessoas.
   * Criar tipos de registro. Esses tipos de registro permanecem somente no Workfront Planning. Eles não são exibidos no GenStudio.
   * Habilite registros do espaço de trabalho do GenStudio para se conectar a outros espaços de trabalho.
   * Habilite registros do espaço de trabalho do GenStudio para serem adicionados a outros espaços de trabalho.
* Quando você tem permissões do Contribute para o espaço de trabalho do GenStudio no Planning, não é possível modificar os tipos de registro do GenStudio no Planning.

### Registros no espaço de trabalho do GenStudio

* Ao editar registros do GenStudio no GenStudio for Performance Marketing, as alterações ficam visíveis no espaço de trabalho do GenStudio em todas as instâncias do Workfront.
* Não é possível criar ou excluir registros de Ativação do espaço de trabalho do GenStudio no Workfront Planning.
* Quando você tem permissões Gerenciar ou Contribute para o espaço de trabalho do GenStudio no Planning, é possível fazer o seguinte no Workfront Planning:
   * Adicione ou exclua registros e eles se tornarão visíveis no (ou serão removidos do) GenStudio for Performance Marketing.

     Os registros excluídos do Workfront Planning ou do GenStudio for Performance Marketing são colocados no compartimento do Workfront Planning Recentemente excluídos por 30 dias. O GenStudio for Performance Marketing não tem um compartimento excluído recentemente.
   * Restaure um registro do compartimento Excluído recentemente. A restauração de registros excluídos os coloca de volta no Workfront Planning e no GenStudio for Performance Marketing.
   * Adicione registros das seguintes maneiras:

      * Manualmente, do zero, de qualquer exibição usando o botão Novo registro
      * Importando-os usando um arquivo CSV ou do Excel na exibição de tabela
      * Manualmente, em qualquer exibição no Workfront Planning
      * Ao enviar uma solicitação para um formulário de solicitação de tipo de registro no Workfront.

  Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).
* É possível editar informações de registro em todos os registros no espaço de trabalho do GenStudio no Workfront Planning.

  Para obter informações, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

### Campos de tipo de registro no espaço de trabalho do GenStudio

* Os campos de tipo de registro são importados do GenStudio for Performance Marketing para o Workfront Planning por padrão.
* Não é possível adicionar campos a tipos de registro do GenStudio for Performance Marketing.
<!--Iskuhi said this is not possible but I can add fields: * You cannot create or delete Activation records' fields from the GenStudio workspace in Workfront Planning. -->
* Quando você tem permissões para Gerenciar o espaço de trabalho do GenStudio no Planning, é possível fazer o seguinte no Workfront Planning:

   * Editar configurações de campo do GenStudio.
   * Crie campos para tipos de registro do GenStudio, caso tenha acesso de Gerenciamento no espaço de trabalho do Gen Studio.

     Quando você cria campos para tipos de registro do GenStudio no Planning, eles ficam visíveis nas seguintes áreas:

      * Exibições do Workfront Planning
      * Páginas de detalhes do registro do Workfront Planning
      * Páginas de detalhes do registro do GenStudio

     >[!TIP]
     >
     >Os campos criados no Workfront Planning não estão visíveis na exibição de lista do GenStudio.

   * Ocultar campos na exibição de tabela de um tipo de registro do GenStudio no Workfront Planning.
&lt;!—* Exclua os campos criados no Workfront Planning para tipos de registro do GenStudio do Workfront Planning. — isso não é possível, de acordo com Iskuhi; o link está lá, mas gerará um erro —>

  <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* Quando você tem permissões do Contribute para o espaço de trabalho do GenStudio no Planning:

   * Não é possível editar configurações de campo, excluir ou adicionar campos do espaço de trabalho do GenStudio no Workfront Planning.
   * Você pode ocultar campos da exibição de tabela no Workfront Planning.

#### Os campos Criado por e Aprovado por

* Você pode adicionar os campos Criado por e Aprovado por para os tipos de registro do GenStudio no Workfront Planning do Workfront Planning.
* Os registros exibidos nos tipos de registro Canal e Região exibirão &quot;Sistema&quot; como Criado pelo usuário. Esses registros são criados automaticamente quando o espaço de trabalho do GenStudio é criado no Workfront Planning.
* Os registros criados no GenStudio após a disponibilização do espaço de trabalho no Workfront Planning exibirão o nome do usuário IMS que criou o registro no campo Criado por, mesmo que o usuário tenha criado os registros no GenStudio e não seja um usuário do Workfront.
* O campo Aprovado por exibe o nome do aprovador quando um formulário de solicitação é enviado para criar um registro no tipo de registro do GenStudio no Workfront Planning.
* Os campos Criado por e Aprovado por são exibidos nos detalhes dos registros no GenStudio for Performance Marketing. Elas não são exibidas na exibição de lista.

### Exibições de registro no espaço de trabalho do GenStudio

>[!NOTE]
>
>Os tipos de registro do GenStudio são exibidos na exibição de tabela padrão importada da exibição de lista do GenStudio for Performance Marketing.
>
>Não é possível excluir a exibição de tabela original que foi importada por padrão do GenStudio for Performance Marketing.

* Não é possível criar várias exibições no GenStudio for Performance Marketing.

* Quando você tem permissões para Gerenciar o espaço de trabalho do GenStudio no Planning, é possível fazer o seguinte no Workfront Planning:

   * Criar exibições para tipos de registro do GenStudio.

     Para obter informações, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

   * Renomeie, compartilhe, exporte, duplique ou exclua exibições personalizadas dos tipos de registro do GenStudio.

* Quando você tem permissões do Contribute para o espaço de trabalho do GenStudio no Planning, é possível fazer o seguinte no Workfront Planning:

   * Criar exibições para tipos de registro do GenStudio.

     Para obter informações, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

   * Renomeie, exporte, duplique ou exclua exibições personalizadas dos tipos de registro do GenStudio.

     Não é possível compartilhar exibições do espaço de trabalho do GenStudio no Workfront Planning

### Registrar conexões no espaço de trabalho do GenStudio

Você pode criar conexões entre tipos de registro em espaços de trabalho do GenStudio nos quais tem permissões de gerenciamento.

Você pode fazer as seguintes conexões entre tipos de registro do GenStudio e outros tipos de registro ou objeto no Workfront Planning:

* Dois tipos de registro do GenStudio
* Um tipo de registro GenStudio e um tipo de registro Planning do mesmo espaço de trabalho
* Um tipo de registro do GenStudio e um tipo de registro do Planning de outro espaço de trabalho, se os tipos de registro estiverem configurados para se conectar de outro espaço de trabalho.
* Um tipo de registro GenStudio e um tipo de objeto Workfront (projetos, portfólios, programas, empresas, grupos)
* Um tipo de registro GenStudio e um tipo de objeto AEM Assets.

### Formulários de solicitação e automações no tipo de registro do GenStudio

* Você pode adicionar formulários de solicitação a um tipo de registro do GenStudio no Workfront Planning.

  Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* Você pode configurar automações para um tipo de registro do GenStudio no Workfront Planning.

  Para obter informações, consulte [Configurar automações do Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

## O ambiente de Pré-visualização

* O espaço de trabalho do GenStudio acessível no ambiente de Produção também é exibido no ambiente de Pré-visualização da mesma instância do Workfront.
* Você pode executar todas as atividades descritas neste artigo no espaço de trabalho do GenStudio no Workfront Planning no seu ambiente de Pré-visualização, mas essas alterações não estarão visíveis no GenStudio.

  Somente as alterações feitas nos itens no ambiente de Produção são sincronizadas entre o Workfront Planning e o GenStudio.

  O GenStudio não tem um ambiente de Pré-visualização.

