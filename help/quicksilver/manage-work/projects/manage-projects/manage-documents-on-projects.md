---
product-area: projects
navigation-topic: manage-projects
title: Visão geral do gerenciamento de documentos para projetos e objetos relacionados
description: Dependendo de o administrador do Workfront escolher o padrão de sua preferência de armazenamento, você poderá armazenar documentos no armazenamento herdado do Workfront ou no armazenamento em nuvem do Adobe. Este artigo descreve como você pode gerenciar documentos de projetos, portfólios, programas, modelos, tarefas e problemas.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 9a35246858141a3b69ec85be3372c7a8d9497d6e
workflow-type: tm+mt
source-wordcount: '1920'
ht-degree: 0%

---

# Visão geral do gerenciamento de documentos para projetos e objetos relacionados

O administrador do Adobe Workfront pode definir o padrão para a preferência de armazenamento de sua organização para indicar onde os documentos devem ser armazenados no Workfront.

O administrador do Workfront pode escolher uma das seguintes opções:

* armazenamento Workfront
* armazenamento em nuvem Adobe

Essa preferência permite armazenar automaticamente documentos anexados a objetos do Workfront em um dos locais de armazenamento disponíveis.

>[!IMPORTANT]
>
>Sua instância do Workfront pode não ter acesso ao armazenamento do Workfront e do Adobe. Algumas instâncias do Workfront têm acesso somente ao Workfront, enquanto outras têm acesso somente ao armazenamento em nuvem do Adobe por padrão. Nenhuma configuração é necessária para clientes com acesso a apenas um tipo de armazenamento.

O administrador do Workfront pode executar um dos seguintes procedimentos:

* Escolha uma das duas opções de armazenamento como padrão para sua organização
* Permite escolher qual armazenamento você prefere usar ao criar um dos seguintes objetos:

   * Projetos
   * Portfólios
   * Modelos

Para obter informações sobre como definir preferências de armazenamento para o Workfront, consulte [Habilitar o Adobe Cloud Storage para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

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
* Somente armazenamento em nuvem Adobe. A área Preferências de Armazenamento em Preferências do Sistema não existe.
* O Workfront Storage e o Adobe Cloud Storage. O administrador do Workfront pode escolher entre o seguinte:

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


Os documentos armazenados em objetos no armazenamento do Workfront são gerenciados de forma diferente daqueles armazenados no armazenamento em nuvem do Adobe.

Para obter mais informações, consulte [visão geral do armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

As seções a seguir documentam como o armazenamento de documentos funciona para objetos do Workfront quando as opções de armazenamento na nuvem do Workfront e do Adobe existem no mesmo ambiente.

### Gerenciamento de documentos para projetos

Leve em consideração o seguinte ao trabalhar com projetos:

* Ao criar um projeto de armazenamento na nuvem do Adobe, o Workfront cria uma pasta na seção Documentos do projeto em que os documentos são salvos. O nome da pasta é igual ao do projeto. Não é possível excluir ou renomear manualmente a pasta. A pasta será renomeada se você alterar o nome do projeto para corresponder ao novo nome do projeto.
* Ao criar ou mover um projeto do Adobe Cloud Storage para um portfólio ou programa herdado do Workfront Storage, o portfólio ou programa é convertido automaticamente em um objeto do Adobe Cloud Storage se o portfólio ou programa não tiver documentos anexados antes de o projeto ser adicionado.
* Não é possível criar um projeto herdado do Workfront Storage para um portfólio ou programa do Adobe Cloud Storage.
* Quando você importa um projeto do MS Project, o Workfront cria um projeto de armazenamento herdado do Workfront, mesmo quando o administrador do Workfront tornou o armazenamento em nuvem do Adobe padrão para o seu sistema.
* Quando você cria projetos usando uma automação do Workfront Planning, o Workfront usa a preferência de armazenamento padrão do sistema para o projeto. Você deve adquirir o pacote do Planning para ter acesso ao Workfront Planning.

### Gerenciamento de documentos para portfólios

Considere o seguinte ao trabalhar com portfólios:

* Ao criar um portfólio de armazenamento em nuvem do Adobe, o Workfront cria uma pasta na seção Documentos do portfólio em que os documentos são salvos. O nome da pasta é igual ao do portfólio. Não é possível excluir ou renomear manualmente a pasta. A pasta será renomeada se você alterar o nome do portfólio para corresponder ao novo nome dele.

* Quando você adiciona um projeto de armazenamento em nuvem do Adobe a um portfólio de armazenamento Workfront herdado e o portfólio não tem documentos anexados a ele, o portfólio é convertido em um portfólio de armazenamento em nuvem do Adobe.
* Quando você adiciona um projeto de armazenamento em nuvem do Adobe a um portfólio de armazenamento Workfront herdado e o portfólio tem documentos anexados a ele, o armazenamento de documentos do portfólio permanece no armazenamento do Workfront. No entanto, o ícone de armazenamento herdado do Workfront para o portfólio ![ícone de armazenamento herdado do portfólio](assets/legacy-storage-project-icon.png) é removido do portfólio.
* Não é possível adicionar um projeto herdado do Workfront Storage a um portfólio Adobe de armazenamento na nuvem.

* Ao criar portfólios usando uma automação do Workfront Planning, a Workfront usa a preferência de armazenamento padrão do sistema para o portfólio. Você deve adquirir o pacote do Planning para ter acesso ao Workfront Planning.

### Gerenciamento de documentos para programas

Leve em consideração o seguinte ao trabalhar com programas:

* Ao criar um programa de armazenamento na nuvem do Adobe, o Workfront cria uma pasta na seção Documentos do programa em que os documentos são salvos. O nome da pasta é igual ao nome do programa. Não é possível excluir ou renomear manualmente a pasta. A pasta será renomeada se você alterar o nome do programa para corresponder ao novo nome do programa.

* Quando você adiciona um projeto do Adobe Cloud Storage a um programa herdado do Workfront Storage e o programa não tem documentos anexados a ele, o programa é convertido em um programa do Adobe Cloud Storage. O portfólio do programa também é convertido.
* Quando você adiciona um projeto de armazenamento em nuvem do Adobe a um programa de armazenamento Workfront herdado e o programa tem documentos anexados a ele, o armazenamento de documentos do programa permanece no armazenamento do Workfront. Se o portfólio também tiver documentos, seu armazenamento de documentos também permanecerá no armazenamento do Workfront; caso contrário, o portfólio será convertido no armazenamento em nuvem do Adobe.

  O ícone de armazenamento herdado do Workfront para o programa ![Ícone de armazenamento herdado do portfólio](assets/legacy-storage-project-icon.png) foi removido do programa.
* Não é possível adicionar um projeto herdado do Workfront Storage a um programa do Adobe Cloud Storage.

* Quando você cria programas usando uma automação do Workfront Planning, a Workfront usa a preferência de armazenamento padrão do sistema para o programa. Você deve adquirir o pacote do Planning para ter acesso ao Workfront Planning.

### Gerenciamento de documentos para tarefas

Considere o seguinte ao trabalhar com tarefas:

* As tarefas herdam o tipo de armazenamento dos projetos.
* Quando você faz upload de um documento para uma tarefa em um projeto de armazenamento na nuvem do Adobe, o Workfront cria automaticamente uma pasta na seção Documentos da tarefa. O nome da pasta é igual ao da tarefa.
* É possível renomear e excluir a pasta de documentos da tarefa de armazenamento na nuvem do Adobe, que também exclui os documentos na pasta. Depois de adicionar novos documentos à tarefa, a pasta é automaticamente recriada. Os documentos excluídos não são colocados de volta na pasta.
* Para projetos do Adobe Cloud Storage, a pasta de documentos em uma tarefa é exibida como uma subpasta na pasta de documentos criada automaticamente para o projeto.
* Não é possível copiar ou mover uma tarefa de um projeto herdado do Workfront Storage para um projeto do Adobe Cloud Storage. O inverso também não é possível.
* Os seguintes cenários existem ao converter uma tarefa em um projeto: <!--this info also duplicated in Convert tasks to projects-->
   * Uma tarefa herdada de armazenamento do Workfront cria um projeto herdado de armazenamento do Workfront.
   * Uma tarefa de armazenamento na nuvem do Adobe cria um projeto de armazenamento na nuvem do Adobe.
   * Usar um modelo de armazenamento herdado do Workfront para converter uma tarefa de armazenamento em nuvem do Adobe cria um projeto de armazenamento em nuvem do Adobe.
   * Usar um modelo de armazenamento em nuvem do Adobe para converter uma tarefa herdada de armazenamento do Workfront cria um projeto herdado de armazenamento do Workfront.
* Não é possível adicionar documentos a tarefas de armazenamento na nuvem do Adobe no painel Resumo.

### Gerenciamento de documentos para problemas

Leve em consideração o seguinte ao trabalhar com problemas:

* Problemas herdam o tipo de armazenamento de projetos.
* Ao fazer upload de um documento para um problema em um projeto de armazenamento em nuvem do Adobe, o Workfront cria automaticamente uma pasta na seção Documentos do problema. O nome da pasta é igual ao nome do problema.
* Você pode renomear e excluir a pasta de documentos do problema de armazenamento na nuvem do Adobe, que também exclui os documentos na pasta. Depois de adicionar novos documentos ao problema, a pasta é recriada automaticamente. Os documentos excluídos não são colocados de volta na pasta.
* Para projetos do Adobe Cloud Storage, a pasta de documentos sobre um problema é exibida como uma subpasta na pasta de documentos criada automaticamente para o projeto.
* Não é possível copiar ou mover um problema de um projeto herdado do Workfront Storage para um projeto do Adobe Cloud Storage. O inverso também não é possível.
* Quando você envia uma solicitação com um documento anexado a um projeto herdado de armazenamento do Workfront, a área Documentos da solicitação exibe o documento usando o tipo de armazenamento do projeto, mesmo quando a preferência padrão de armazenamento do sistema é Armazenamento em nuvem do Adobe.
* Os seguintes cenários existem ao converter um problema em um projeto: <!--this info also duplicated in Convert an issue to a project-->
   * Um problema de armazenamento herdado do Workfront cria um projeto de armazenamento herdado do Workfront.
   * Um problema de armazenamento em nuvem do Adobe cria um projeto de armazenamento em nuvem do Adobe.
   * Usar um modelo de armazenamento herdado do Workfront para converter um problema do Adobe Cloud Storage cria um projeto do Adobe Cloud Storage.
   * Usar um modelo de armazenamento em nuvem do Adobe para converter um problema de armazenamento herdado do Workfront cria um projeto de armazenamento herdado do Workfront.
* Não é possível adicionar documentos a problemas de armazenamento na nuvem do Adobe no painel Resumo.

### Gerenciamento de documentos para modelos de projeto

Considere o seguinte ao trabalhar com modelos:

* Ao criar um modelo de armazenamento na nuvem do Adobe, o Workfront cria uma pasta na seção Documentos do modelo em que os documentos são salvos. O nome da pasta é igual ao do programa. Não é possível excluir ou renomear manualmente a pasta. A pasta será renomeada se você alterar o nome do modelo para corresponder ao novo nome do modelo.
* Você pode usar um modelo herdado do Workfront Storage para criar projetos herdados do Workfront Storage; pode usar um modelo do Adobe Cloud Storage para criar um projeto do Adobe Cloud Storage.
* Você pode anexar um modelo de armazenamento herdado do Workfront a um projeto do Adobe Cloud Storage e isso não altera o local de armazenamento dos documentos no projeto.
* Você pode anexar um modelo de armazenamento na nuvem do Adobe a um projeto de armazenamento Workfront herdado e isso não altera o local de armazenamento dos documentos no projeto. Os documentos na pasta de armazenamento na nuvem do Adobe para o modelo são adicionados ao projeto diretamente, sem a pasta, enquanto os documentos nas pastas de tarefa do modelo são adicionados às pastas anexadas às tarefas do projeto na seção Documentos das tarefas.

### Gerenciamento de documentos para tarefas de modelo

Considere o seguinte ao trabalhar com tarefas de modelo:

* Tarefas de modelo herdam o tipo de armazenamento dos modelos.
* Quando você faz upload de um documento para uma tarefa de modelo em um modelo de armazenamento na nuvem do Adobe, o Workfront cria automaticamente uma pasta na seção Documentos da tarefa de modelo. O nome da pasta é igual ao da tarefa de modelo.
* Você pode renomear e excluir a pasta de documentos da tarefa de modelo de armazenamento na nuvem do Adobe, que também exclui os documentos na pasta. Após adicionar novos documentos à tarefa de modelo, a pasta será automaticamente recriada. Os documentos excluídos não são colocados de volta na pasta.
* Para modelos de armazenamento na nuvem do Adobe, a pasta de documentos em uma tarefa de modelo é exibida como uma subpasta na pasta de documentos criada automaticamente para o modelo.
* Não é possível copiar ou mover uma tarefa de modelo de um modelo de armazenamento herdado do Workfront para um modelo de armazenamento na nuvem do Adobe. O inverso também não é possível.
* Ao anexar um documento a um problema enviado a uma fila de solicitações associada ao armazenamento do Adobe, uma pasta é criada para cada problema enviado em que os documentos são armazenados. A pasta também é adicionada como uma subpasta à pasta de projeto criada automaticamente na fila de solicitações.
