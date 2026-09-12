---
title: Compartilhar um espaço de ideação com outros
description: O Adobe Workfront Planning agora oferece um recurso adicional para identificar antes de você iniciar suas campanhas. Aproveite o potencial da IA para criar e colaborar com ideias antes que elas se tornem registros de planejamento.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 2%

---


# Compartilhar um espaço de ideação com outras pessoas

<!--add to TOC and miniTOC-->

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente como parte do programa **Espaço de ideação Beta**. </span>

<span class="preview">Para obter mais informações, consulte [Introdução ao Espaço de ideação do Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

<!--ome of this information is also duplicated in the section for Ideation space permissions in the Access needed to use Ideation space article-->

As permissões de registro do Workfront Planning são transferidas para o espaço de ideação de um registro.

Além disso, você pode conceder permissões a outros usuários para usar o espaço de ideação e adicionar ideias a ele.

Considere o seguinte:

* Os criadores de ideações sempre têm permissões de Editor em suas próprias ideações.

* Você deve ter permissões de Editor em um espaço de ideação para criar resumos e exportá-los para outros aplicativos.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

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
<li><p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p></li>
Ou
<li><p>Qualquer pacote do Planning quando adquirido como um produto independente</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Produtos adicionais</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workflow</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> 
   <ul>
   <li><p>Você deve adicionar um Workflow e um tipo de licença do Planning ao nível de acesso quando tiver um Workflow e um pacote do Planning</p>   </li>
   <li><p>A configuração Desativar espaço de ideação no seu nível de acesso deve ser desmarcada</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Permissões do Contribute ou superior para o espaço de trabalho e tipo de registro ao qual você deseja adicionar registros </p>
      <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
      <p>Exibir permissões para objetos do Workfront para adicioná-los a resumos <!--not sure if this is available--></p>
      <p>Permissões do editor no espaço de ideação para criar resumos</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Funções de usuário do Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Qualquer função de usuário do GenStudio para acessar Campanhas, Produtos e Personalidades</li>
   <li>GenStudio System Manager para acessar as Ativações <!--and Events--></li></ul>
   Para obter informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funções e permissões de usuário</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Compartilhar um espaço de ideação

1. Acesse o espaço Ideação de um registro de Planejamento.

   Para obter informações, consulte um dos seguintes artigos:

   * [Criar registros do Planning a partir de resumos de espaço de ideação](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
   * [Criar resumos no espaço de ideação](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

1. Clique em **Compartilhar** no canto superior direito e no ícone **Configurações** ícone ![Configurações](assets/setting-icon.png) no canto superior direito da caixa **Compartilhar documento**.
1. Na lista Quem tem acesso, escolha uma das seguintes opções:

   * **Somente pessoas convidadas podem acessar**

     Você deve adicionar usuários individuais ao espaço de ideação e fornecer a eles um nível de permissão.
   * **Todos no &lt; ambiente Workfront da sua empresa > podem fazer comentários**

     Todas as pessoas na organização que tenham um Fluxo de trabalho e uma licença do Planning em seu nível de acesso podem encontrar e comentar a ideação.
   * **Qualquer pessoa com o link pode fazer um comentário**

     Qualquer pessoa com quem você compartilhar um link para a ideação pode comentá-la, incluindo pessoas externas à sua organização.

1. Clique em **Copiar link** para gerar um link para a ideação e compartilhá-lo com outras pessoas. O link é adicionado à área de transferência.
1. Clique na seta para trás na caixa Configurações para voltar para o compartilhamento.
1. (Condicional) Se você optou por compartilhar o espaço de ideação com pessoas específicas, comece digitando seu nome ou endereço de email e, em seguida, selecione um dos seguintes níveis de permissão:

   | Permissão de espaço de ideação | Recursos |
   |---|---|
   | **Editor** | Pode editar, baixar e compartilhar o espaço de ideação |
   | **Comentário** | Pode exibir e comentar no espaço de ideação |
   | **Visualizador** | Pode visualizar o espaço de ideação |

1. (Opcional) Inclua uma mensagem com sua atribuição e clique em **Convidar**.

   Os usuários convidados recebem uma notificação por email sobre sua atribuição de permissão.

1. Clique no ícone **X** para fechar a caixa **Compartilhar documento**.











