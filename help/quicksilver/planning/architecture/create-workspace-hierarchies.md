---
title: Criar hierarquias do Workspace
description: Como um gerenciador de espaço de trabalho, você pode criar várias hierarquias de espaço de trabalho entre os tipos de registro no Adobe Workfront Planning. Depois de conectar tipos de registro em um espaço de trabalho e criar uma hierarquia, os tipos de registro são conectados uns aos outros, com um tipo de registro designado como pai e até seis outros tipos de registro configurados como filhos.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# Criar hierarquias do espaço de trabalho

Como um gerenciador de espaço de trabalho, você pode criar várias hierarquias de espaço de trabalho entre os tipos de registro no Adobe Workfront Planning.

Depois de conectar tipos de registro em um espaço de trabalho e criar uma hierarquia, os tipos de registro são conectados uns aos outros, com um tipo de registro designado como pai e até seis outros tipos de registro configurados como filhos. <!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

As hierarquias gerarão navegações estruturais para os tipos de registros e registros <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> exibidos em seus cabeçalhos. Dessa forma, os usuários sabem onde estão na hierarquia em qualquer estágio do fluxo de trabalho.

Para obter informações gerais sobre hierarquias e navegações estruturais, consulte [Visão geral sobre hierarquia e navegação estrutural](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Requisitos de acesso

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

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

{#step1-to-planning}

1. Clique em um cartão de espaço de trabalho.
1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do espaço de trabalho e clique em **Configurações**.
A seção **Hierarquias** é aberta por padrão.
1. Clique em **Nova hierarquia** no canto superior direito da página **Hierarquias**.
1. Clique em **Adicionar objeto** e selecione um objeto no menu suspenso. Este será o objeto pai na sua hierarquia.
Você pode selecionar um tipo de registro no espaço de trabalho atual ou um projeto do Workfront.
1. Clique em **Adicionar objeto** para adicionar um segundo objeto que é o primeiro filho na hierarquia e, em seguida, selecione outro objeto no menu suspenso.
   ![Nova caixa de hierarquia sem campo selecionado](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. Clique em **Selecionar campo conectado** para indicar qual campo conecta os dois objetos.
1. (Condicional) Se um campo conectado existir entre os dois tipos de objeto, selecione-o na lista. Ou clique em **Adicionar nova conexão**.

   >[!WARNING]
   >
   >Se o **Criar campo correspondente no tipo de registro vinculado** não foi selecionado quando o campo conectado foi criado, edite o campo primeiro para poder continuar.

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
1. (Opcional) Continue adicionando até quatro tipos de objeto às suas hierarquias seguindo as etapas acima. Você pode adicionar todos os seus tipos de objetos primeiro e, em seguida, adicionar os campos de conexão entre eles.
1. (Opcional) Clique no ícone **Remover** ![Remover ícone](assets/minus-icon.png) para remover uma conexão.
1. Clique em **Salvar** para salvar sua hierarquia.

   >[!TIP]
   >
   >O botão **Salvar** ficará esmaecido se não houver todos os campos conectados.

   As seguintes situações ocorrem:

   * A hierarquia é adicionada à seção **Hierarquias** do espaço de trabalho.
   * Os registros que preenchem os campos de conexão exibem todas as conexões em suas navegações estruturais, quando você acessa a página de um registro.
1. (Opcional) Passe o mouse sobre uma hierarquia, clique no menu **Mais** e, em seguida, clique em uma das seguintes opções:

   * **Editar**: abre a caixa **Editar hierarquia**, na qual você pode fazer alterações.
   * **Excluir**: exclui a hierarquia permanentemente. As hierarquias excluídas não podem ser recuperadas. Os campos de conexão não são excluídos.





