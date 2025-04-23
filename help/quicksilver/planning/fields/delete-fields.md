---
title: Excluir campos
description: No Adobe Workfront Planning, é possível excluir campos personalizados que não são mais relevantes.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---



# Excluir campos

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

No Adobe Workfront Planning, é possível criar campos personalizados para armazenar informações sobre registros.

Para obter informações sobre como criar campos personalizados no Workfront Planning, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

É possível excluir campos do Workfront Planning que não são mais relevantes.

## Considerações sobre a exclusão de campos do Workfront Planning:

* É possível excluir um campo somente na exibição de tabela do tipo de registro.
* Não é possível excluir o campo principal de um registro.
* As informações armazenadas no campo são excluídas e não podem ser recuperadas.
* Quando você exclui um campo de registro conectado, todos os campos de pesquisa conectados também são excluídos do tipo de registro ao qual você se conecta. Os campos de registro conectados dos tipos de registro aos quais você se conecta também são excluídos do registro ao qual você se conecta.

  Por exemplo, ao conectar campanhas a outro tipo de registro chamado produto e excluir o campo conectado Produto e o campo de pesquisa Status do Produto da campanha, as seguintes opções são excluídas:

   * O campo Produto conectado da campanha
   * O campo de pesquisa Status do produto da campanha
   * O campo conectado do Campaign do produto.

  Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
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
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão </p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho <span class="preview">e tipo de registro</span> </a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Excluir campos

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos campos de registro você deseja deletar.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.

1. Clique no cartão de um tipo de registro.

1. (Condicional) Se ainda não estiver selecionada, clique na guia de uma **exibição de Tabela** na página de tipo de registro.

   Todos os registros existentes associados ao tipo de registro são exibidos nas linhas da exibição de tabela.

1. Localize o campo que deseja excluir nos cabeçalhos da coluna, passe o mouse sobre o cabeçalho da coluna e clique na seta para baixo após o nome do campo.

   ![Menu de seta após o nome do campo no cabeçalho da tabela realçado](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Clique em **Excluir**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Clique em **Excluir** para confirmar.

   O campo é excluído, não pode ser recuperado e não pode mais ser associado a nenhum registro.
