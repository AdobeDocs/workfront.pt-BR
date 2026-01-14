---
title: Criar hierarquias do Workspace
description: Como um gerenciador de espaço de trabalho, você pode criar várias hierarquias de espaço de trabalho entre os tipos de registro no Adobe Workfront Planning. Depois de conectar tipos de registro em um espaço de trabalho e criar uma hierarquia, os tipos de registro são conectados uns aos outros, com um tipo de registro designado como pai e até três outros tipos de registro configurados como filhos.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 9a7ab1928bfd25c197fca65eddfba1bc01977ea7
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 1%

---


# Criar hierarquias do espaço de trabalho

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Como um gerenciador de espaço de trabalho, você pode criar várias hierarquias de espaço de trabalho entre tipos de registro no Adobe Workfront Planning.

Depois que os tipos de registro forem conectados em um espaço de trabalho, você poderá criar uma hierarquia que organiza essas conexões. As hierarquias organizam tipos de registro e objeto em relacionamentos pai-filho e podem conter até quatro níveis de tipos de objeto.

Se uma conexão entre dois tipos de registro ainda não existir, ela poderá ser criada conforme você configura a hierarquia. Uma vez definida, a hierarquia estabelece um caminho estruturado entre tipos de registro relacionados no espaço de trabalho.

As hierarquias geram navegações estruturais para seus respectivos registros que são exibidos em seus cabeçalhos. Dessa forma, os usuários sabem onde estão na hierarquia em qualquer estágio do fluxo de trabalho.

Para obter informações gerais sobre hierarquias e navegações estruturais, consulte [Visão geral sobre hierarquia e navegação estrutural](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para executar as etapas deste artigo:  

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
<ul> 
<li><p>Qualquer Workfront e qualquer pacote do Planning</p></li>
Ou
<li><p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p></li></ul>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões em um espaço de trabalho</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma hierarquia de espaço de trabalho

Você pode criar até 5 hierarquias em um espaço de trabalho.

{#step1-to-planning}

1. Clique em um cartão de espaço de trabalho.
1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do espaço de trabalho e clique em **Configurações**.
A seção **Hierarquias** é aberta por padrão.
1. Clique em **Nova hierarquia** no canto superior direito da página **Hierarquias**.
1. Clique em **Adicionar objeto** e selecione um tipo de objeto no menu suspenso. Este será o primeiro tipo de objeto na sua hierarquia. <!--logged bug to correct to "Add object type"-->

   O primeiro tipo de objeto só pode ser um tipo de registro do Planning.

   Os projetos Workfront não podem ser selecionados como pais de outros tipos de objeto em uma hierarquia.

1. Clique em **Adicionar objeto** para adicionar um segundo tipo de objeto que seja o primeiro filho na hierarquia e, em seguida, selecione outro tipo de objeto no menu suspenso.
Cada tipo de objeto adicional se torna filho dos tipos de objeto anteriores.

   ![Nova caixa de hierarquia sem campo selecionado](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. Clique em **Selecionar campo conectado** para indicar qual campo conecta os dois objetos.
1. (Condicional) Se houver vários campos de conexão, selecione um na lista,

   Ou

   Clique em **Adicionar nova conexão** para adicionar um novo campo de conexão.

   Isso cria um campo de conexão do tipo de registro que você está usando como pai e um campo de conexão correspondente a ele a partir do tipo de registro que você está usando como filho.

   Se você estiver criando uma conexão com projetos Workfront, nenhum campo será criado no projeto.

1. (Condicional) Se não houver campos conectados disponíveis, clique em **Criar conexão** e adicione uma nova conexão, depois clique em **Salvar**.

1. (Condicional) Se você estiver adicionando uma nova conexão, faça o seguinte:

   1. Adicione um nome para o campo conectado na caixa **Nome**.
   1. Selecione um dos seguintes tipos de conexão:

      * **De muitos para muitos**
      * **De um para muitos**
      * **De muitos para um**
      * **Um para um**

   1. Selecione um dos seguintes tipos de aparências de registro:

      * **Nome e imagem**
      * **Nome**
      * **Imagem**

      Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).

   1. Clique em **Salvar**.

1. (Condicional) Se o **Criar campo correspondente no tipo de registro vinculado** não foi selecionado quando o campo conectado foi criado, você receberá um erro e deverá fazer o seguinte primeiro: <!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. Clique em **Cancelar** na caixa **Nova hierarquia**.
   1. Clique na seta para trás à esquerda do nome do espaço de trabalho e, em seguida, clique no cartão do tipo de registro que você deseja escolher como pai.
   1. Abra a exibição de tabela do tipo de registro selecionado na etapa acima e vá para o campo de conexão com o tipo de objeto que deseja usar como filho, passe o mouse sobre o cabeçalho da coluna e clique no campo **Editar**.
   1. Ative a configuração **Criar campo correspondente no tipo de registro vinculado** e clique em **Salvar**.
   1. Retorne à área **Configurações** do espaço de trabalho, clique novamente em **Nova hierarquia** e siga as etapas para criar uma hierarquia.

1. (Opcional) Continue adicionando até quatro tipos de objeto às suas hierarquias seguindo as etapas acima. Você pode adicionar todos os seus tipos de objetos primeiro e, em seguida, adicionar os campos de conexão entre eles.
1. (Opcional) Clique no ícone **Remover** ![Remover ícone](assets/minus-icon.png) para remover uma conexão.
1. Clique em **Salvar** para salvar sua hierarquia.

   >[!TIP]
   >
   >O botão **Salvar** ficará esmaecido se não houver todos os campos conectados.

   As seguintes situações ocorrem:

   * A hierarquia é adicionada à seção **Hierarquias** do espaço de trabalho.
   * Os registros que preenchem os campos de conexão exibem todas as conexões em suas navegações estruturais, quando você acessa a página de um registro.

   >[!NOTE]
   >
   >Você pode conectar um registro de um tipo de registro filho a até 10 registros de um tipo de registro pai.
   >
   >Para obter mais informações, consulte [Visão geral sobre hierarquia e navegação estrutural](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

1. (Opcional) Passe o mouse sobre uma hierarquia e clique no menu **Mais**.

   ![Menu Mais de Hierarquia expandido](assets/hierarchy-more-menu-expanded.png)

1. Clique em uma das opções a seguir:

   * **Editar**: abre a caixa **Editar hierarquia**, na qual você pode fazer alterações.
   * **Excluir**: exclui a hierarquia permanentemente. As hierarquias excluídas não podem ser recuperadas. Os campos de conexão não são excluídos.





