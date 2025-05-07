---
title: Criar tipos de registro importando informações de um arquivo CSV ou do Excel
description: Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, é possível criar tipos de registro personalizados que ilustrem os itens de trabalho necessários no ciclo de vida da organização importando informações de um arquivo CSV ou do Excel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 3dfac5ada17248f5c67380b56b9a0969b10b73e6
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 1%

---

# Criar tipos de registro importando informações de um arquivo CSV ou do Excel

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, é possível criar tipos de registro personalizados que ilustrem os itens de trabalho necessários no ciclo de vida da organização importando informações de um arquivo CSV ou do Excel.

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
   <td><p> Padrão</p>
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
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>No ambiente de Produção, todos os usuários, inclusive os Administradores do Sistema, devem ser atribuídos a um modelo de layout que inclua o Planning.</p>
<p><span class="preview">No ambiente de Pré-visualização, os usuários do Standard e os administradores do sistema têm o Planning habilitado por padrão.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerações sobre a importação de tipos de registro usando um arquivo Excel ou CSV

* Cada folha do arquivo do Excel se torna um tipo de registro. O nome da planilha se tornará o nome do tipo de registro.
* Se houver apenas uma planilha ou se você importar um arquivo CSV, o nome do arquivo se tornará o nome do tipo de registro.
* Os cabeçalhos de colunas em cada planilha se tornam os campos associados a cada tipo de registro.
* Os campos são exclusivos para seus respectivos tipos de registro.
* Cada linha em cada planilha se torna um registro exclusivo associado ao respectivo tipo de registro.
* Cada folha do arquivo Excel não deve exceder o seguinte:
   * 25.000 linhas
   * 500 colunas
* O arquivo não deve ter mais de 5 MB.
* Planilhas vazias não são suportadas.
* Os campos dos seguintes tipos não são suportados e não podem ser mapeados para campos na planilha de importação:

   * &#x200B;<!--In the Production environment,--> Campos de conexão para registros do Planning ou objetos do Workfront e AEM Assets

     <!--<span class="preview">In the Preview environment, you can map and import connection fields to Planning records. </span>-->

   * Campos de pesquisa de registros conectados do Planning ou objetos do Workfront e AEM Assets
   * Campos de fórmula
   * Data de criação, Criado por
   * Última data de modificação, Última modificação por
   * Pessoas

Para importar tipos de registro usando um arquivo Excel ou CSV:

{{step1-to-planning}}

1. Clique no espaço de trabalho onde deseja criar tipos de registro,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.
1. Clique em **Adicionar tipo de registro**.
1. Clique em **Do arquivo**.
1. Arraste e solte um arquivo Excel ou CSV salvo anteriormente no computador ou clique em **Selecionar um arquivo CSV ou Excel** para procurar um.
1. Clique em **Visualizar e editar**.

   A caixa **Visualizar e editar** é exibida com as seguintes informações:

   * Os nomes das planilhas ou dos futuros tipos de registros são exibidos no painel esquerdo. Por padrão, o Workfront Planning seleciona um ícone e uma cor para cada novo tipo de registro.
   * A primeira folha ou tipo de registro é selecionado e os nomes dos campos associados a ela são exibidos como cabeçalhos de coluna. O tipo de cada campo é selecionado por padrão.
   * Cada linha representa um novo registro. Somente os primeiros 10 registros são exibidos na caixa Preview and edit.

   ![Visualizar e editar caixa](assets/preview-and-edit-box.png)

1. (Opcional) Clique no nome de cada planilha no painel esquerdo para revisar as informações que ela contém.

   >[!NOTE]
   >
   >Planilhas vazias não são suportadas e estão esmaecidas.

1. (Opcional) Desmarque as planilhas que você não deseja importar do painel esquerdo.

   ![Selecione as planilhas a serem importadas com o menu suspenso não selecionado](assets/select-sheets-to-import-drop-down-with-unselected.png)

   As planilhas desmarcadas são exibidas com um plano de fundo cinza.

1. (Opcional) Clique na seta para baixo à direita do cabeçalho da coluna para executar um dos seguintes procedimentos:

   * Renomear um dos campos
   * Alterar o **Tipo de campo**
   * Atualizar o campo **Descrição**

1. (Condicional) Depois de atualizar as informações sobre o campo, clique em **Salvar**.

1. Clique em **Importar** quando estiver pronto para importar o arquivo.

   As seguintes informações são importadas para o Workfront Planning:

   * Novos tipos de registro
   * Novos campos associados a cada tipo de registro
   * Novos registros associados a cada tipo de registro

   Você pode começar a gerenciar campos e registros nas páginas de tipos de registro.

   Todos os usuários com acesso ao Workfront Planning e ao espaço de trabalho agora podem exibir e editar os tipos de registros importados e suas informações.
