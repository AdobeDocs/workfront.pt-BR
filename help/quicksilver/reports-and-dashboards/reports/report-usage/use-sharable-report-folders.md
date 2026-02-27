---
product-area: reporting
navigation-topic: report-usage
title: Usar pastas de relatórios compartilháveis
description: Use pastas de relatórios compartilháveis para organizar os relatórios criados e compartilhe essas pastas com outros usuários no Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 65831f2e-9092-4e99-a86b-40df42c713bf
source-git-commit: 650d24c36c3ccee810b8918ccdf456f607b055e9
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 5%

---

# Usar pastas de relatórios compartilháveis

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

<!-- This article is linked in the UI -->

Você pode usar pastas de relatórios compartilháveis para organizar relatórios e compartilhá-las com outros usuários. Esse recurso foi projetado para equipes que gerenciam grandes volumes de relatórios e precisam de controle de acesso escalável e consistente.

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
   <p>qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Entender as permissões de pasta

As pastas de relatório compartilháveis usam dois níveis de permissão:

* **Exibir**: os usuários podem abrir relatórios na pasta, mas não podem editar detalhes da pasta, adicionar ou remover itens, nem excluir a pasta. Você pode permitir que usuários com acesso de Visualização compartilhem a pasta ao habilitar a configuração **Compartilhar** ao conceder acesso.
* **Gerenciar**: os usuários podem editar detalhes da pasta e adicionar ou mover itens de relatório. Também recebem acesso de Gerenciar aos relatórios na pasta. Você pode permitir que usuários com acesso de Gerenciar compartilhem ou excluam pastas, habilitando as configurações de **Compartilhar** e **Excluir** ao conceder o acesso.

Comportamento adicional:

* Os administradores de sistema podem visualizar todas as pastas.
* Outros usuários veem somente as pastas às quais têm acesso.
* As permissões concedidas a uma pasta principal se aplicam a todas as subpastas e relatórios dentro dessa árvore de pastas.
* Os usuários com acesso a uma subpasta podem ver suas pastas principais para navegação, mas não pastas irmãs, a menos que o acesso seja concedido.

## Criar uma pasta de relatório compartilhável

Somente administradores do sistema podem criar pastas no nível superior. Depois que uma pasta compartilhável é criada, os usuários com acesso Gerenciar podem criar subpastas dentro dela.

{{step1-to-reports}}

1. Ative a opção **Pastas de relatório compartilháveis**.
1. Clique em **Criar pasta**.
1. Insira um nome para a pasta.
1. Clique em **Criar**.

![criar uma pasta compartilhável](assets/add-sharable-folder.png)

## Criar uma subpasta em uma pasta de relatórios compartilháveis

Você pode criar até três níveis de subpastas em uma pasta de relatórios compartilháveis. As subpastas herdam permissões da pasta principal, mas você também pode definir permissões exclusivas para cada subpasta.

{{step1-to-reports}}

1. Localize a pasta na qual deseja criar uma subpasta.
1. Clique em **Mais** > **Adicionar subpasta**.
1. Insira um nome para a subpasta.
1. Clique em **Criar**.

## Compartilhar uma pasta de relatório com outros usuários

Quando você compartilha uma pasta com usuários, eles herdam acesso a todas as subpastas nessa árvore de pastas. Os usuários também devem ter acesso a cada relatório, por meio de permissões de pasta ou compartilhamento direto de relatório.

{{step1-to-reports}}

1. Localize a pasta que deseja compartilhar.
1. Clique em **Mais** > **Compartilhar**.
1. Adicione usuários, equipes, funções, grupos ou empresas.
1. Escolha o acesso **Exibir** ou **Gerenciar**:
   * O acesso de Visualização permite que os usuários abram relatórios na pasta. Você também pode permitir que usuários com acesso de Visualização compartilhem a pasta novamente selecionando **Compartilhar** nas configurações adicionais.
   * O acesso Gerenciar permite que os usuários editem detalhes da pasta e adicionem ou removam itens. Você também pode permitir que usuários com acesso de Gerenciamento excluam pastas ou compartilhem a pasta ao selecionar **Excluir** e **Compartilhar** nas configurações adicionais.
1. Clique em **Salvar**.

   ![compartilhar uma pasta e ajustar o acesso](assets/share-settings-sharable-folders.png)

## Mover um relatório para uma pasta compartilhável

Para mover um relatório para uma pasta, você deve ter direitos de **Gerenciar** para o relatório e para a pasta compartilhável.

{{step1-to-reports}}

1. Marque a caixa de seleção ao lado do relatório que você deseja mover.
1. Clique em **Mover para a pasta** na barra de ações na parte inferior da tela.
1. Localize a pasta para a qual deseja mover o relatório e clique em **Mover**. A árvore de relatório está recolhida por padrão, portanto, talvez seja necessário expandir as pastas para encontrar a pasta de destino.

   ![mover um relatório para uma pasta compartilhável](assets/move-to-folder.png)

## Excluir uma pasta de relatório compartilhável

Quando você exclui uma pasta, todas as subpastas dentro dessa pasta também são excluídas. Você deve ter acesso de **Gerenciar** à pasta para excluí-la. Os relatórios na pasta não são excluídos e ainda podem ser encontrados na lista de relatórios principal.

As permissões de relatório concedidas por meio das permissões de pasta são removidas quando a pasta é excluída. As permissões de relatório concedidas diretamente do relatório ou herdadas de um painel permanecem em vigor.


{{step1-to-reports}}

1. Clique em **Mais** > **Excluir**.
1. Clique em **Sim, exclua-o** para confirmar.


## Nova experiência de lista para pastas compartilháveis

Ao acessar pastas compartilháveis na área Relatórios, você verá uma nova experiência de lista que permite visualizar e gerenciar facilmente suas pastas e relatórios. Para obter mais informações sobre a nova experiência de lista, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).