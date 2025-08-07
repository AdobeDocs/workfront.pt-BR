---
title: Introdução à Integração do Workfront Planning e do GenStudio for Performance Marketing
description: O espaço de trabalho do GenStudio for Performance Marketing estará disponível no Adobe Workfront Planning quando sua empresa tiver comprado ambos os produtos. Saiba mais sobre as noções básicas sobre como você pode simplificar seus fluxos de trabalho usando essa integração.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 36cd1c23dfb6e01dc1016a6a12ae47e4f9172d20
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 1%

---

# Introdução à integração do Workfront Planning e do GenStudio for Performance Marketing

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

Organizações que usam o Adobe Workfront Planning e o Adobe GenStudio for Performance Marketing geralmente definem conceitos de marketing como Campanhas, Produtos e Personalidades com mais detalhes do que o GenStudio suporta por padrão.

Há uma integração nativa entre o GenStudio for Performance Marketing e o Workfront Planning. Essa integração permite que os usuários no Workfront Planning gerenciem Campanhas, Produtos, Personalidades, Ativações, Canais e Regiões usados no GenStudio. Ela também permite configurar o GenStudio para fazer referência aos tipos de registro existentes do Workfront Planning, criando um fluxo de trabalho de marketing mais conectado e consistente.

Essa integração ajuda a evitar a entrada de dados duplicados, manter o alinhamento entre os esforços de planejamento e ativação e oferece suporte ao sistema de marketing de registro.

O espaço de trabalho do GenStudio for Performance Marketing estará disponível no Adobe Workfront Planning quando sua empresa tiver comprado ambos os produtos.

Com a integração entre o Workfront Planning e o GenStudio for Performance Marketing, você pode:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Exiba o espaço de trabalho do GenStudio no Workfront Planning.
* Modifique suas campanhas no GenStudio e atualize em tempo real as mesmas informações no Workfront Planning.
* Modifique suas campanhas no Workfront Planning e atualize em tempo real as mesmas informações no GenStudio.

## Requisitos de integração

* O Workfront e o GenStudio for Performance Marketing devem ser habilitados para a mesma organização.

  Para obter mais informações sobre o GenStudio, consulte [Guia do Usuário do Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home).

* O GenStudio não estará disponível no Workfront Planning quando sua empresa tiver várias instâncias do Workfront. <!--this will change-->

* A instância do Workfront faz parte da Experiência unificada do Adobe, incluindo o uso do Identity Management System (IMS).

  Para obter informações, consulte [Experiência unificada da Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Os usuários que usam o Planning e o GenStudio podem pertencer a apenas uma instância do Workfront na organização IMS.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Requisitos de acesso

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar o Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p> Administrador do sistema</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Contribuir com ou mais permissões para um espaço de trabalho e tipo de registro  </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Visão geral da integração do Workfront Planning e do GenStudio

As seções a seguir descrevem o seguinte:

* Recursos para atualizar informações do Workfront Planning no GenStudio
* Recursos para atualização de informações do GenStudio no Workfront Planning
* Limitações para o que você pode ou não gerenciar em um espaço de trabalho do GenStudio no Workfront Planning.

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### O espaço de trabalho do GenStudio no Workfront Planning

* Se sua organização tiver várias instâncias do Workfront, o espaço de trabalho do GenStudio não estará visível em nenhuma das instâncias do Workfront. <!-- this might change-->
* O espaço de trabalho do GenStudio exibe um indicador visual que deixa claro que ele é importado do GenStudio. Para obter informações, consulte [Gerenciar o espaço de trabalho do GenStudio no Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Todos os usuários com acesso ao GenStudio e ao Workfront Planning também podem ver o espaço de trabalho do GenStudio no Workfront Planning.
* Os usuários do Workfront Planning devem ser gerenciados por meio do Adobe Identity Management System (IMS) para exibir e usar o espaço de trabalho do GenStudio no Workfront.

  Usuários somente do Workfront não podem ver o espaço de trabalho do GenStudio, mesmo quando ele está disponível no Workfront.

  Para obter informações, consulte [Experiência unificada da Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


### Tipos de registro

* Você pode editar informações de tipos de registro (por exemplo, sua aparência) no GenStudio no Workfront Planning.
* Você pode compartilhar tipos de registros do GenStudio com outras pessoas no Planning.  <!--checking with Ani H.-->
* Você pode criar tipos de registro no Planning no espaço de trabalho do GenStudio. <!-- checking with Ani where these show up in GenS-->
* Os tipos de registro sincronizados com o GenStudio exibem um indicador visual que deixa claro que os tipos de registro são importados do GenStudio.

### Registros

* É possível adicionar ou excluir registros no GenStudio e eles se tornam visíveis no (ou são removidos do) Workfront Planning.
É possível adicionar ou excluir registros no Workfront Planning e eles se tornam visíveis no (ou são removidos do) GenStudio.
* Você pode adicionar registros do Workfront Planning das seguintes maneiras:

   * Manualmente, do zero, de qualquer exibição usando o botão Novo registro
   * Importando-os usando um arquivo CSV ou do Excel
   * Manualmente, embutido, na exibição de tabela
   * Manualmente, diretamente na exibição de linha do tempo

  Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).
* Não é possível criar ou excluir registros de Ativação do Workfront Planning.
* É possível editar informações de registro em todos os registros no espaço de trabalho do GenStudio no Planning em qualquer um dos campos visíveis do Workfront Planning.

  Para obter informações, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Campos

* Os campos de registro são importados do GenStudio. É possível editar as configurações de campo no Workfront Planning.
* Você poderá criar mais campos para tipos de registro do GenStudio no Workfront Planning se tiver acesso de Gerenciamento no Gen Studio.
* Quando você cria campos para tipos de registro do GenStudio no Planning, eles ficam visíveis nas seguintes áreas:
   * Exibições do Planning
   * Páginas de detalhes do registro de planejamento
   * Páginas de detalhes do registro do GenStudio

  >[!TIP]
  >
  >Os campos criados no Workfront Planning não estão visíveis na exibição de lista do GenStudio.

* Você pode ocultar campos na exibição de tabela de um tipo de registro do GenStudio no Planning, mas não pode excluir campos do Workfront Planning.


<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### Visualizações

* É possível criar exibições para tipos de registro do GenStudio.

  Para obter informações, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

* Você pode compartilhar a exibição de um tipo de registro do GenStudio como compartilharia uma exibição para um tipo de registro do Planning.

### Conexões

* Você pode fazer as seguintes conexões entre tipos de registro do GenStudio e outros tipos de registro ou objeto no Workfront Planning:

   * Dois tipos de registro GenStudio e
   * Um tipo de registro GenStudio e um tipo de registro Planning do mesmo espaço de trabalho
   * Um tipo de registro do GenStudio e um tipo de registro do Planning de outro espaço de trabalho, se os tipos de registro estiverem configurados para se conectar de outro espaço de trabalho.
   * Um tipo de registro GenStudio e um tipo de objeto Workfront (projetos, portfólios, programas, empresas, grupos)