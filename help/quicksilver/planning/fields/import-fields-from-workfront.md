---
title: Importar campos do Adobe Workfront
description: No Adobe Workfront Planning, é possível criar campos personalizados para cada tipo de tipo de registro. Em seguida, é possível associar o campo aos registros do Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 8%

---

<!--add to TOC-->

# Importar campos do Adobe Workfront

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->


{{planning-important-intro}}

É possível importar cópias de campos existentes do Workfront. A importação de campos do Workfront cria uma cópia de cada campo para um tipo de registro do Workfront Planning.


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
<p>Qualquer Workfront e qualquer pacote do Planning</p> <p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
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

<!--Old:

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
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p> </td> 
  </tr> 
</tbody> 
</table> -->


## Considerações sobre a importação de campos do Workfront

* Você pode importar campos nativos ou personalizados do Workfront para um tipo de registro no Workfront Planning.
* A importação de campos do Workfront cria cópias dos mesmos campos e preserva o nome do campo no Workfront Planning. Depois de copiados para o Workfront Planning, os campos são independentes dos campos originais do Workfront e não compartilham informações.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* Você pode adicionar campos nativos ou personalizados a partir dos seguintes objetos do Workfront:
   * Portfólio
   * Programa
   * Projeto
   * Tarefa
   * Problema
   * Documento
   * Empresa
   * Grupo
   * Usuário
   * Função no trabalho
   * Atribuição
   * Hora
   * Registro de cobrança
     <!--Available only to Preview, but might not come to Prod:* Rate card - visible in Production but asking PM if it should be hidden-->
   * Despesa
   * Iteração
     <!--* Non-labor resource - - visible in Production but asking PM if it should be hidden-->
     <!--* Non-labour resource category - - visible in Production but asking PM if it should be hidden-->
* Os campos do Workfront podem não preservar seu tipo de campo, após serem importados no Workfront Planning.

  A tabela abaixo mostra os tipos de campo do Workfront e seus tipos de campo correspondentes do Workfront Planning.

  | Tipo de campo do Workfront | Tipo de campo do Workfront Planning |
  |------------------------------------------|-------------------------------|
  | Texto em linha única formatado com texto | Texto de linha única |
  | Texto de linha única formatado por número | Número |
  | Texto de linha única formatado por moeda | Moeda |
  | Parágrafo | Parágrafo |
  | Texto com formatação | Parágrafo |
  | Lista suspensa de seleção única | Seleção única |
  | Lista suspensa com seleção múltipla | Seleção múltipla |
  | Não há suporte para filtros de digitação antecipada de usuário | People |
  | Calculado* | Fórmula |
  | Data | Data |
  | Grupo de caixas de seleção | Seleção múltipla |
  | Botão de opção | Seleção múltipla |

  *Os campos calculados estarão disponíveis em uma data posterior.
Todos os outros tipos de campo do Workfront não são suportados no Workfront Planning.


## Importar campos do Workfront

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja criar campos.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.

1. Clique no cartão de um tipo de registro.

   Todos os registros existentes associados ao tipo de registro são exibidos nas linhas da exibição de tabela.

   >[!TIP]
   >
   >    Alguns campos podem estar ocultos. Clique em **Campos** e habilite a alternância para os campos que deseja exibir como colunas na exibição de tabela.

1. Clique no ícone **+** no canto superior direito da exibição de tabela

   Ou

   Passe o mouse sobre o cabeçalho de qualquer coluna, clique na seta para baixo após o nome do campo e clique em **Inserir à esquerda** ou **Inserir à direita** para adicionar o novo campo.
1. Clique em **Adicionar existente** no canto inferior direito da guia **Novo campo**. <!--check UI - did they change this??-->

   ![Adicionar campos existentes do modal do Workfront](assets/add-existing-fields-from-workfront-modal.png)

1. Comece a digitar o nome de um campo do Workfront existente na área de pesquisa e clique em **+** quando ele for exibido na lista.
1. (Opcional) Digite outro campo e clique em **+** quando ele for exibido na lista.
1. (Opcional) Clique no ícone **Filtros** ![Filtros no ícone de importar campos](assets/filters-in-import-fields-icon.png) e atualize um ou ambos os campos a seguir:

   * Tipo de objeto: selecione um tipo de objeto do Workfront cujos campos você deseja importar.
   * Formulário personalizado: selecione um ou vários formulários personalizados no Workfront. Você pode selecionar um formulário personalizado sem primeiro selecionar um tipo de objeto.
1. Clique em **+** e depois em **Adicionar campos**.
Os campos são adicionados à exibição de tabela e às páginas de detalhes dos registros.

   >[!IMPORTANT]
   >
   >    Há um limite de 500 campos para qualquer tipo de registro. Os campos existentes junto com os campos importados contribuem para esse limite.

   Os campos adicionados são cópias dos campos do Workfront e não se conectam mais aos campos originais no Workfront.
