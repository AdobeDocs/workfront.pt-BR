---
product-area: projects
navigation-topic: manage-projects
title: Visão geral do gerenciamento de documentos para projetos e objetos relacionados
description: Dependendo de o administrador do Workfront escolher o padrão de sua preferência de armazenamento, você poderá armazenar documentos no armazenamento Workfront herdado ou no armazenamento corporativo Adobe. Este artigo descreve como você pode gerenciar documentos de projetos, portfólios, programas, modelos, tarefas e problemas.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 2b0fdb3c74882b566a397872e1cc8007728b770c
workflow-type: tm+mt
source-wordcount: '1755'
ht-degree: 0%

---

# Visão geral do gerenciamento de documentos para projetos e objetos relacionados

O administrador do Adobe Workfront pode definir o padrão para a preferência de armazenamento de sua organização para indicar onde os documentos devem ser armazenados no Workfront.

O administrador do Workfront pode escolher uma das seguintes opções:

* armazenamento Workfront
* Armazenamento corporativo Adobe

Essa preferência permite armazenar automaticamente documentos anexados a objetos do Workfront em um dos locais de armazenamento disponíveis.

>[!IMPORTANT]
>
>Sua instância do Workfront pode não ter acesso ao armazenamento do Workfront e do Adobe. Algumas instâncias do Workfront têm acesso somente ao Workfront, enquanto outras têm acesso somente ao armazenamento Adobe Enterprise por padrão. Nenhuma configuração é necessária para clientes com acesso a apenas um tipo de armazenamento.

O administrador do Workfront pode executar um dos seguintes procedimentos:

* Escolha uma das duas opções de armazenamento como padrão para sua organização
* Permite escolher qual armazenamento você prefere usar ao criar um dos seguintes objetos:

   * Projetos
   * Portfólios
   * Modelos

Para obter informações sobre como definir preferências de armazenamento para o Workfront, consulte [Habilitar o armazenamento corporativo do Adobe para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

Este artigo descreve como você pode gerenciar documentos de projetos, portfólios, programas, tarefas, problemas, modelos e tarefas de modelo.

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## Visão geral do armazenamento de documentos

Os clientes podem ter acesso a um dos seguintes recursos de armazenamento de documentos:

* Somente armazenamento Workfront. A área Preferências de Armazenamento em Preferências do Sistema não existe.
* Somente armazenamento Adobe Enterprise. A área Preferências de Armazenamento em Preferências do Sistema não existe.
* Tanto o armazenamento da Workfront quanto o armazenamento corporativo da Adobe. O administrador do Workfront pode escolher entre o seguinte:

   * Seleciona um ambiente de armazenamento padrão para o modo como os documentos serão tratados no futuro.
   * Permite que os usuários escolham qual armazenamento escolher quando criam os seguintes objetos:

      * Projetos
      * Portfólios
      * Modelos

  >[!NOTE]
  >
  >* Tarefas e problemas herdam o tipo de armazenamento do projeto.
  >* Tarefas de modelo herdam o tipo de armazenamento do modelo
  >* Os programas herdam o tipo de armazenamento do portfólio.


Os documentos armazenados em objetos no armazenamento Workfront são gerenciados de forma diferente daqueles armazenados no armazenamento corporativo Adobe.

Para obter mais informações, consulte [visão geral do armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

As seções a seguir documentam como o armazenamento de documentos funciona para objetos do Workfront quando existem opções de armazenamento corporativo Workfront e Adobe no mesmo ambiente.

### Gerenciamento de documentos para projetos

Leve em consideração o seguinte ao trabalhar com projetos:

* Quando você cria um projeto de armazenamento corporativo do Adobe, o Workfront cria uma pasta na seção Documentos do projeto em que os documentos são salvos. O nome da pasta é igual ao do projeto. Não é possível excluir ou renomear manualmente a pasta. A pasta será renomeada se você alterar o nome do projeto para corresponder ao novo nome do projeto.
* Quando você cria ou move um projeto de armazenamento corporativo da Adobe para um portfólio ou programa herdado de armazenamento da Workfront, o portfólio ou programa é convertido automaticamente em um objeto de armazenamento corporativo da Adobe.
* Não é possível criar um projeto de armazenamento da Workfront para um portfólio ou programa de armazenamento corporativo da Adobe.
* Quando você importa um projeto do MS Project, a Workfront cria um projeto de armazenamento Workfront, mesmo quando o administrador do Workfront tornou o armazenamento Adobe Enterprise padrão para o seu sistema.
* Quando você cria projetos usando uma automação do Workfront Planning, o Workfront usa a preferência de armazenamento padrão do sistema para o projeto. Você deve adquirir o pacote do Planning para ter acesso ao Workfront Planning.

### Gerenciamento de documentos para portfólios

Considere o seguinte ao trabalhar com portfólios:

* Quando você cria um portfólio de armazenamento corporativo da Adobe, a Workfront cria uma pasta na seção Documentos do portfólio em que os documentos são salvos. O nome da pasta é igual ao do portfólio. Não é possível excluir ou renomear manualmente a pasta. A pasta será renomeada se você alterar o nome do portfólio para corresponder ao novo nome dele.
* Quando você cria ou move um projeto de armazenamento corporativo da Adobe para um portfólio de armazenamento corporativo herdado da Workfront, o portfólio é convertido automaticamente em um objeto de armazenamento corporativo da Adobe.
* Se o portfólio convertido anteriormente tinha documentos anexados, eles continuam armazenados no armazenamento da Workfront. Novos documentos também são armazenados no armazenamento do Workfront.
* Se o portfólio convertido não tiver documentos anexados ao armazenamento da Workfront, os novos documentos serão armazenados no armazenamento corporativo da Adobe.
* Ao criar portfólios usando uma automação do Workfront Planning, a Workfront usa a preferência de armazenamento padrão do sistema para o portfólio. Você deve adquirir o pacote do Planning para ter acesso ao Workfront Planning.

### Gerenciamento de documentos para programas

Leve em consideração o seguinte ao trabalhar com programas:

* Quando você cria um programa de armazenamento corporativo Adobe, a Workfront cria uma pasta na seção Documentos do programa em que os documentos são salvos. O nome da pasta é igual ao nome do programa. Não é possível excluir ou renomear manualmente a pasta. A pasta será renomeada se você alterar o nome do programa para corresponder ao novo nome do programa.
* Quando você cria ou move um projeto de armazenamento corporativo da Adobe para um portfólio de armazenamento corporativo herdado da Workfront, o portfólio é convertido automaticamente em um objeto de armazenamento corporativo da Adobe.
* Se o programa convertido anteriormente tinha documentos anexados, eles continuam armazenados no armazenamento do Workfront. Novos documentos também são armazenados no armazenamento do Workfront.
* Se o programa convertido não tiver documentos anexados ao armazenamento do Workfront, novos documentos serão armazenados no armazenamento corporativo da Adobe.
* Quando você cria programas usando uma automação do Workfront Planning, a Workfront usa a preferência de armazenamento padrão do sistema para o programa. Você deve adquirir o pacote do Planning para ter acesso ao Workfront Planning.

### Gerenciamento de documentos para tarefas

Considere o seguinte ao trabalhar com tarefas:

* As tarefas herdam o tipo de armazenamento dos projetos.
* Quando você faz upload de um documento para uma tarefa em um projeto de armazenamento Adobe, o Workfront cria automaticamente uma pasta na seção Documentos da tarefa. O nome da pasta é igual ao da tarefa.
* Você pode renomear e excluir a pasta de documentos da tarefa de armazenamento corporativo do Adobe que também exclui os documentos da pasta. Depois de adicionar novos documentos à tarefa, a pasta é automaticamente recriada. Os documentos excluídos não são colocados de volta na pasta.
* Para projetos de armazenamento corporativo do Adobe, a pasta de documentos em uma tarefa é exibida como uma subpasta na pasta de documentos criada automaticamente para o projeto.
* Não é possível copiar ou mover uma tarefa de um projeto de armazenamento da Workfront para um projeto de armazenamento da Adobe. O inverso também não é possível.
* Os seguintes cenários existem ao converter uma tarefa em um projeto: <!--this info also duplicated in Convert tasks to projects-->
   * Uma tarefa de armazenamento Workfront cria um projeto de armazenamento Workfront.
   * Uma tarefa de armazenamento corporativo da Adobe cria um projeto de armazenamento Adobe.
   * Usar um modelo de armazenamento Workfront para converter uma tarefa de armazenamento Adobe cria um projeto de armazenamento Adobe.
   * O uso de um modelo de armazenamento Adobe para converter uma tarefa de armazenamento Workfront cria um projeto de armazenamento Workfront.

### Gerenciamento de documentos para problemas

Leve em consideração o seguinte ao trabalhar com problemas:

* Problemas herdam o tipo de armazenamento de projetos.
* Quando você faz upload de um documento para um problema em um projeto de armazenamento Adobe, o Workfront cria automaticamente uma pasta na seção Documentos do problema. O nome da pasta é igual ao nome do problema.
* Você pode renomear e excluir a pasta de documentos do problema de armazenamento corporativo do Adobe que também exclui os documentos da pasta. Depois de adicionar novos documentos ao problema, a pasta é recriada automaticamente. Os documentos excluídos não são colocados de volta na pasta.
* Para projetos de armazenamento corporativo do Adobe, a pasta de documentos referente a um problema é exibida como uma subpasta na pasta de documentos criada automaticamente para o projeto.
* Não é possível copiar ou mover um problema de um projeto de armazenamento da Workfront para um projeto de armazenamento da Adobe. O inverso também não é possível.
* Quando você envia uma solicitação com um documento anexado a um projeto de armazenamento Workfront, a área Documentos da solicitação exibe o documento usando o tipo de armazenamento do projeto, mesmo quando a preferência padrão de armazenamento do sistema é Adobe Enterprise.
* Os seguintes cenários existem ao converter um problema em um projeto: <!--this info also duplicated in Convert an issue to a project-->
   * Um problema de armazenamento Workfront cria um projeto de armazenamento Workfront.
   * Um problema de armazenamento corporativo da Adobe cria um projeto de armazenamento Adobe.
   * Usar um modelo de armazenamento Workfront para converter um problema de armazenamento Adobe cria um projeto de armazenamento Adobe.
   * Usar um modelo de armazenamento Adobe para converter um problema de armazenamento Workfront cria um projeto de armazenamento Workfront.

### Gerenciamento de documentos para modelos de projeto

Considere o seguinte ao trabalhar com modelos:

* Quando você cria um modelo de armazenamento corporativo do Adobe, o Workfront cria uma pasta na seção Documentos do modelo em que os documentos são salvos. O nome da pasta é igual ao do programa. Não é possível excluir ou renomear manualmente a pasta. A pasta será renomeada se você alterar o nome do modelo para corresponder ao novo nome do modelo.
* Você pode usar um modelo de armazenamento Workfront para criar projetos de armazenamento Workfront; você pode usar um modelo de armazenamento Adobe para criar um projeto de armazenamento Adobe.
* Você pode anexar um modelo de armazenamento Workfront a um projeto de armazenamento Adobe e isso não altera o local de armazenamento do projeto.
* Você pode anexar um modelo de armazenamento Adobe a um projeto de armazenamento Workfront e isso não altera o local de armazenamento do projeto. Os documentos na pasta de armazenamento Adobe do modelo são adicionados diretamente ao projeto, sem a pasta, enquanto os documentos nas pastas de tarefas do modelo são adicionados às pastas anexadas às tarefas do projeto na seção Documentos das tarefas.

### Gerenciamento de documentos para tarefas de modelo

Considere o seguinte ao trabalhar com tarefas de modelo:

* Tarefas de modelo herdam o tipo de armazenamento dos modelos.
* Quando você faz upload de um documento para uma tarefa de modelo em um modelo de armazenamento Adobe, o Workfront cria automaticamente uma pasta na seção Documentos da tarefa de modelo. O nome da pasta é igual ao da tarefa de modelo.
* Você pode renomear e excluir a pasta de documentos da tarefa de modelo de armazenamento corporativo do Adobe que também exclui os documentos da pasta. Após adicionar novos documentos à tarefa de modelo, a pasta será automaticamente recriada. Os documentos excluídos não são colocados de volta na pasta.
* Para modelos de armazenamento corporativo do Adobe, a pasta de documentos em uma tarefa de modelo é exibida como uma subpasta na pasta de documentos criada automaticamente para o modelo.
* Não é possível copiar ou mover uma tarefa de modelo de um modelo de armazenamento Workfront para um modelo de armazenamento Adobe. O inverso também não é possível.
* Ao anexar um documento a um problema enviado a uma fila de solicitações associada ao armazenamento do Adobe, uma pasta é criada para cada problema enviado em que os documentos são armazenados. A pasta também é adicionada como uma subpasta à pasta de projeto criada automaticamente na fila de solicitações.
