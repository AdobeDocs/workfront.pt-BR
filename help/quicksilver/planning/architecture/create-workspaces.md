---
title: Criar espaços de trabalho
description: Um espaço de trabalho é uma coleção de tipos de registro usados por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning. Os tipos de registro são organizados por seções em um espaço de trabalho.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: c4716157a6fdf667f7e608d0c37399f57ec1bbfe
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 2%

---


# Criar espaços de trabalho

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

No Adobe Workfront Planning, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho.

Um espaço de trabalho é uma coleção de tipos de registro usados por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning.

Para obter informações gerais sobre espaços de trabalho, consulte [Visão geral sobre espaços de trabalho](/help/quicksilver/planning/architecture/workspaces-overview.md).

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
<p>Qualquer pacote do Workfront ou Workflow</p> 
<p>Qualquer pacote do Workfront Planning</p>
<p>Um pacote do Workfront Planning Prime ou superior <span class="preview">para criar vários espaços de trabalho de uma vez</span></p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p>
   <p><span class="preview">Administrador do sistema para criar vários espaços de trabalho de uma só vez usando o conjunto de modelos de práticas recomendadas</p>
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

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Criar um espaço de trabalho

Você pode criar um espaço de trabalho e adicionar tipos de registro a ele para organizar seus objetos no Workfront Planning.

Para obter mais informações sobre como editar um espaço de trabalho, consulte [Editar espaços de trabalho](/help/quicksilver/planning/architecture/edit-workspaces.md).

Você pode criar espaços de trabalho das seguintes maneiras:

* Criar um espaço de trabalho do zero ou de um modelo

  Para obter informações, consulte a seção [Criar um espaço de trabalho do zero ou de um modelo](#create-a-workspace-from-scratch-or-from-a-template) neste artigo.
* Crie um espaço de trabalho usando o Planning Designer habilitado por IA. No momento, esse recurso está disponível somente para um número limitado de clientes em um programa do Beta.

  Para obter informações, consulte [Introdução ao Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

<div class="preview">

* Criar vários espaços de trabalho usando um pacote de modelos de vários espaços de trabalho de prática recomendada

  Para obter informações, consulte a seção [Criar vários espaços de trabalho usando um conjunto de modelos de vários espaços de trabalho de práticas recomendadas](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle) neste artigo

  >[!TIP]
  >
  >Não é possível criar vários espaços de trabalho de uma vez, a menos que você use o conjunto de modelos de prática recomendada.


</div>

### Criar um espaço de trabalho do zero ou de um modelo

{{step1-to-planning}}

1. Clique em **Criar espaço de trabalho**

   A caixa Criar espaço de trabalho é exibida. Você pode criar um espaço de trabalho do zero ou criá-lo usando um dos modelos disponíveis.

1. (Opcional e condicional) Clique em **Visualizar** dentro de qualquer um dos seguintes modelos de espaço de trabalho predefinidos:

   * Básico: Gestão de Marketing
   * Avançado: Gestão de Marketing
   * Corporativo: Gestão de Marketing
   * Gerenciamento de vendas
   * Gerenciamento de produtos

   A caixa de pré-visualização do modelo é aberta.

   Há uma indicação de quais tipos de registro operacional, taxonomias e quantos campos estão associados a cada modelo.

   ![Visualizando um modelo de espaço de trabalho](assets/previewing-a-workspace-template.png)

   Para obter informações sobre modelos de espaço de trabalho do Workfront Planning, consulte [Lista de modelos de espaço de trabalho](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Na caixa de visualização do modelo, clique em **Usar modelo** para começar a criar o espaço de trabalho a partir do modelo selecionado

   Ou

   Clique em **Voltar** e em **Novo espaço de trabalho** para criar um espaço de trabalho do zero.

   Um para os seguintes tipos de espaços de trabalho é criado:

   * Um espaço de trabalho vazio chamado **Workspace sem título**, no qual você pode começar a adicionar tipos de registro manualmente ao criar um espaço de trabalho do zero.
   * Um espaço de trabalho nomeado com base no modelo selecionado que é preenchido com tipos de registro de amostra. É possível personalizar ainda mais os tipos de registro e o espaço de trabalho.

   Para administradores do Workfront, o novo espaço de trabalho é exibido na guia **Espaços de trabalho em que estou**.

   Para todos os outros usuários que podem criar espaços de trabalho, o novo espaço de trabalho é exibido na área **Espaços de Trabalho**.

1. Clique dentro do nome do espaço de trabalho no cabeçalho do novo espaço de trabalho para renomeá-lo e pressione Enter.

1. (Opcional e condicional) Se você criou o espaço de trabalho a partir de um modelo, clique dentro do nome das **seções Tipos de Registro Operacionais** ou **Taxonomias**

   Ou

   Passe o mouse sobre o nome de uma seção, em seguida, clique no menu **Mais** ![Mais menu](assets/more-menu.png), em seguida, clique em **Renomear** para renomear a seção.

   >[!TIP]
   >
   >É possível renomear qualquer seção de qualquer espaço de trabalho, mesmo que você não tenha criado a seção.

   Para obter mais informações sobre a edição de espaços de trabalho, incluindo a edição de seções de espaço de trabalho, consulte [Editar espaços de trabalho](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Opcional) Clique em **Adicionar tipo de registro** para adicionar tipos de registro ao espaço de trabalho em qualquer seção.

   Para obter informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   Para obter mais informações sobre edição e exclusão de tipos de registros em um espaço de trabalho, consulte [Editar espaços de trabalho](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Opcional) Clique na seta para trás à esquerda do novo espaço de trabalho para abrir a página principal do Planning. Um novo cartão de espaço de trabalho foi criado para o novo espaço de trabalho na guia **Espaços de trabalho nos quais estou**.

   O nome do usuário que criou o espaço de trabalho é salvo no cartão do espaço de trabalho como o Proprietário.

   >[!NOTE]
   >
   >Para usuários que estão sendo atualmente migrados para o Adobe Identity Management System (IMS), os espaços de trabalho criados apenas por usuários do Workfront que não são usuários do IMS são exibidos conforme criados pelo **Sistema**.
   >
   >Para obter informações sobre IMS, consulte [Experiência unificada do Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

<div class="preview">

### Criar vários espaços de trabalho usando um pacote de modelos de vários espaços de trabalho de prática recomendada

>[!IMPORTANT]
>
>A criação de vários espaços de trabalho de cada vez usando o pacote de modelos de práticas recomendadas estará disponível somente quando os seguintes pré-requisitos forem atendidos:
>
>* Sua organização adquiriu um pacote do Workfront Planning Prime ou Ultimate.
>* Você é um Administrador do sistema

Você pode usar um pacote de modelos de vários espaços de trabalho para criar 6 espaços de trabalho com um clique.

Os modelos incluídos no pacote contêm espaços de trabalho, tipos de registro, registros, exibições e campos para ajudar você a começar a implementação do Planning.

>[!IMPORTANT]
>
>Os nomes dos espaços de trabalho e registros incluídos no pacote são exemplos e não refletem seu próprio ambiente.
>
>Os nomes dos tipos de registro e dos campos podem ser usados em qualquer organização como padrão para implementação em qualquer setor, de acordo com nossa recomendação.
>

{{step1-to-planning}}

1. Clique em **Criar espaço de trabalho**

   A caixa Criar espaço de trabalho é exibida. Você pode criar um espaço de trabalho do zero ou criá-lo usando um dos modelos disponíveis.

1. Clique em **Revisar configuração do espaço de trabalho** na área **Iniciar aqui (Recomendado)**.
1. (Opcional) Clique em **Visualizar** dentro de qualquer um dos seguintes modelos de espaço de trabalho predefinidos para abrir a caixa Visualizar para cada modelo:

   * 1.Classificações e taxonomias globais

     O modelo de Classificações e Taxonomias Globais inclui todos os tipos de registro e campos recomendados que você crie em seu ambiente para uma implementação bem-sucedida do Workfront Planning.

     Posteriormente, você poderá vincular ou importar os tipos de registro nesse modelo em outros espaços de trabalho criados.
   * 2.Fréscopa Marketing Global
   * 3.Fréscopa Marketing Social
   * 4.Fréscopa Mídia e RP
   * 5.Eventos globais da Fréscopa
   * 6.Fréscopa Liderança da Empresa Executiva

1. Depois de abrir a caixa **Visualizar** para cada modelo de espaço de trabalho, clique em Voltar para voltar à caixa **Criar espaço de trabalho** ou clique em Usar modelos para usar os modelos, incluindo no pacote, e criar espaços de trabalho.

   Os espaços de trabalho são criados e exibidos nas guias **Espaços de trabalho em que estou** e **Todos os espaços de trabalho** para administradores do sistema. Todos os usuários com licenças Padrão verão os espaços de trabalho em sua área Espaços de trabalho depois que um Administrador do sistema criá-los e compartilhá-los com eles.

1. Comece a editar os espaços de trabalho criados e a adicionar tipos de registro, registros, exibições e campos pertinentes à sua organização.

   Para obter mais informações sobre as práticas recomendadas para implementar o Workfront, consulte os artigos na seção [Práticas recomendadas do Adobe Workfront Planning: índice do artigo](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md).

   Para obter informações sobre a edição de espaços de trabalho, consulte [Editar espaços de trabalho](/help/quicksilver/planning/architecture/edit-workspaces.md).

</div>



