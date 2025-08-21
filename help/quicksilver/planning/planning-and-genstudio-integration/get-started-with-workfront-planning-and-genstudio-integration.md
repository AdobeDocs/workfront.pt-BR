---
title: Introdução à Integração do Workfront Planning e do GenStudio for Performance Marketing
description: O espaço de trabalho do GenStudio for Performance Marketing estará disponível no Adobe Workfront Planning quando sua empresa tiver comprado ambos os produtos. Saiba mais sobre as noções básicas sobre como você pode simplificar seus fluxos de trabalho usando essa integração.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '1475'
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

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Organizações que usam o Adobe Workfront Planning e o Adobe GenStudio for Performance Marketing geralmente definem conceitos de marketing como Campanhas, Produtos e Personalidades com mais detalhes do que o GenStudio suporta por padrão.

Há uma integração nativa entre o GenStudio for Performance Marketing e o Workfront Planning. Essa integração permite que os usuários no Workfront Planning gerenciem Campanhas, Produtos, Personalidades, Ativações, Canais e Regiões usados no GenStudio. Ela também permite configurar o GenStudio para fazer referência aos tipos de registro existentes do Workfront Planning, criando um fluxo de trabalho de marketing mais conectado e consistente.

O espaço de trabalho do GenStudio for Performance Marketing estará disponível no Adobe Workfront Planning quando sua empresa tiver comprado ambos os produtos.

## Benefícios da integração

Com a integração entre o Workfront Planning e o GenStudio for Performance Marketing, você pode:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Exiba o espaço de trabalho do GenStudio no Workfront Planning.
* Modifique suas campanhas no GenStudio e atualize em tempo real as mesmas informações no Workfront Planning.
* Modifique suas campanhas no Workfront Planning e atualize em tempo real as mesmas informações no GenStudio.
* Evite a entrada de dados duplicados.
* Mantenha o alinhamento entre os esforços de planejamento e ativação.

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
    <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote de fluxo de trabalho do Adobe Workfront</p>
<p>Qualquer pacote do Adobe Workfront Planning</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Pacote do Adobe GenStudio</p></td> 
   <td> 
<p>??? O GEN STUDIO TEM UM PACOTE COMPATÍVEL COM ISSO??</p>

</td> </tr>

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
   <td><p> Standard</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe GenStudio</p></td> 
   <td><p> ??? O GEN STUDIO EXIGE UMA LICENÇA ESPECÍFICA QUE O SUPORTE??</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> Produtos adicionais</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>  
   <p>Configuração do GenStudio: ???WHAT IS THE ACCESS LEVEL NEED FOR GENS???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto*</p></td> 
   <td>  
   <p>No Workfront Planning: </p>
   <ul>
   <li><p>Contribuir com ou mais permissões para um espaço de trabalho e tipo de registro  </p> </li> 
   <li><p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p></li>
   </ul>
   <p>No Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Quaisquer permissões no Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Criar permissões no Adobe GenStudio for Performance Marketing para criar itens</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
*Para obter mais informações sobre o Adobe GenStudio for Performance Marketing, consulte [Guia do Usuário do Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home).


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

* É possível editar informações de tipos de registros do GenStudio (por exemplo, sua aparência) no Workfront Planning.
* Você pode compartilhar tipos de registros do GenStudio com outras pessoas no Planning.
* Você pode criar tipos de registro no Planning no espaço de trabalho do GenStudio. Esses tipos de registro permanecem somente no Planning. Eles não são exibidos no GenStudio.
* Os tipos de registro sincronizados com o GenStudio exibem um indicador visual no Workfront Planning que deixa claro que os tipos de registro são importados do GenStudio.

### Registros

Os itens a seguir são possíveis para registros que pertencem a tipos de registro do GenStudio exibidos no GenStudio e no Workfront Planning:

* É possível adicionar ou excluir registros no GenStudio e eles se tornam visíveis no (ou são removidos do) Workfront Planning.
* É possível adicionar ou excluir registros no Workfront Planning e eles se tornam visíveis no (ou são removidos do) GenStudio.
* Quando você exclui registros do Workfront Planning ou do GenStudio, eles são colocados no compartimento Excluído recentemente do Workfront Planning por 30 dias. O GenStudio não tem um compartimento excluído recentemente.
* A restauração de um registro do compartimento Excluído recentemente os coloca de volta no Workfront Planning e no GenStudio.
* Você pode adicionar registros do Workfront Planning das seguintes maneiras:

   * Manualmente, do zero, de qualquer exibição usando o botão Novo registro
   * Importando-os usando um arquivo CSV ou do Excel
   * Manualmente, embutido, na exibição de tabela
   * Manualmente, diretamente na linha do tempo ou na exibição de calendário <!--ensure the calendar is released when this releases-->

  Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).
* Não é possível criar ou excluir registros de Ativação do Workfront Planning.
* É possível editar informações de registro em todos os registros no espaço de trabalho do GenStudio no Planning em qualquer um dos campos visíveis do Workfront Planning.

  Para obter informações, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Campos

* Os campos de registro são importados do GenStudio. É possível editar as configurações de campo do GenStudio no Workfront Planning.
* Você poderá criar campos para tipos de registro do GenStudio no Workfront Planning se tiver acesso de Gerenciamento no Gen Studio.
* Quando você cria campos para tipos de registro do GenStudio no Planning, eles ficam visíveis nas seguintes áreas:
   * Exibições do Planning
   * Páginas de detalhes do registro de planejamento
   * Páginas de detalhes do registro do GenStudio

  >[!TIP]
  >
  >Os campos criados no Workfront Planning não estão visíveis na exibição de lista do GenStudio.

* Você pode ocultar campos na exibição de tabela de um tipo de registro GenStudio no Planning.
* Não é possível excluir campos importados do GenStudio do Workfront Planning.
* Você pode excluir campos criados no Workfront Planning para tipos de registro do GenStudio do Workfront Planning.

### Os campos Criado por e Aprovado por

* Você pode adicionar os campos Criado por e Aprovado por para os tipos de registro do GenStudio no Workfront Planning do Workfront Planning.
* Os registros exibidos nos tipos de registro Canal e Região exibirão &quot;Sistema&quot; como Criado pelo usuário. Esses registros são criados automaticamente quando o espaço de trabalho do GenStudio é criado no Workfront Planning.
* Os registros criados no GenStudio após a disponibilização do espaço de trabalho no Workfront Planning exibirão o nome do usuário IMS que criou o registro no campo Criado por, mesmo que o usuário tenha criado os registros no GenStudio e não seja um usuário do Workfront.
* O campo Aprovado por exibe o nome do aprovador quando um formulário de solicitação é enviado para criar um registro no tipo de registro do GenStudio no Workfront Planning.

### Exibições

* É possível criar exibições para tipos de registro do GenStudio.

  Para obter informações, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

* O compartilhamento da exibição de um tipo de registro do GenStudio é idêntico ao compartilhamento de uma exibição para um tipo de registro do Planning.
* Não é possível criar várias exibições no GenStudio.

### Conexões

* Você pode fazer as seguintes conexões entre tipos de registro do GenStudio e outros tipos de registro ou objeto no Workfront Planning:

   * Dois tipos de registro do GenStudio
   * Um tipo de registro GenStudio e um tipo de registro Planning do mesmo espaço de trabalho
   * Um tipo de registro do GenStudio e um tipo de registro do Planning de outro espaço de trabalho, se os tipos de registro estiverem configurados para se conectar de outro espaço de trabalho.
   * Um tipo de registro GenStudio e um tipo de objeto Workfront (projetos, portfólios, programas, empresas, grupos)
   * Um tipo de registro GenStudio e um tipo de objeto AEM Assets.

### Formulários de solicitação e automações

* Você pode adicionar formulários de solicitação a um tipo de registro do GenStudio no Workfront Planning.
* Você pode configurar automações para um tipo de registro do GenStudio no Workfront Planning.

### O ambiente de Pré-visualização

* O espaço de trabalho do GenStudio acessível no ambiente de produção também é exibido no ambiente de Pré-visualização.
* Você pode executar todas as atividades descritas neste artigo no espaço de trabalho do GenStudio no Workfront Planning no seu ambiente de Pré-visualização, mas essas alterações não serão transferidas para o GenStudio.
Somente as alterações feitas nos itens no ambiente de Produção são sincronizadas entre o Workfront Planning e o GenStudio.
O GenStudio não tem um ambiente de Pré-visualização.

