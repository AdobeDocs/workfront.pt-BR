---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Armazenamentos de dados no [!DNL Adobe Workfront Fusion]
description: Um armazenamento de dados, semelhante a um banco de dados ou a uma tabela simples, pode armazenar dados de cenários, possibilitando a transferência de dados entre cenários individuais ou execuções de cenário. Você pode usar um armazenamento de dados para armazenar novos dados de vários sistemas durante a sincronização.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 1%

---

# Armazenamentos de dados no [!DNL Adobe Workfront Fusion]

Um armazenamento de dados, semelhante a um banco de dados ou a uma tabela simples, pode armazenar dados de cenários, possibilitando a transferência de dados entre cenários individuais ou execuções de cenário. Você pode usar um armazenamento de dados para armazenar novos dados de vários sistemas durante a sincronização.

Os módulos de armazenamento de dados permitem que você execute as seguintes ações nos registros em seu [!DNL Adobe Workfront Fusion] armazenamento de dados:

* Adicionar
* Substituir
* Atualizar
* Recuperar
* Excluir
* Pesquisar
* Contagem

Para obter informações sobre o uso de módulos de armazenamento de dados, consulte [[!UICONTROL Armazenamento de dados] módulos](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

Para obter uma introdução em vídeo aos armazenamentos de dados no Workfront Fusion, consulte:

* [Armazenamentos de dados](https://video.tv.adobe.com/v/3427029/){target=_blank}

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Criar um armazenamento de dados no [!DNL Workfront Fusion]

* [Configurar o armazenamento de dados](#set-up-the-data-store)
* [Configurar a estrutura de dados](#set-up-the-data-structure)

### Configurar o armazenamento de dados

Antes de usar um armazenamento de dados em um módulo, você deve criar o armazenamento de dados no [!DNL Workfront Fusion].

>[!NOTE]
>
>Sua organização tem um número limitado de armazenamentos de dados disponíveis. Se você tentar criar mais armazenamentos de dados do que os disponíveis, [!DNL Workfront] retorna um [!UICONTROL Máximo de armazenamentos atingido] erro.
>
>Para obter mais informações, consulte [Erro de máximo de armazenamentos atingido](#maximum-stores-reached-error) neste artigo.

1. Faça logon no [!DNL Workfront Fusion] conta.
1. Clique em **[!UICONTROL Armazenamentos de dados]** no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Adicionar armazenamento de dados]** no canto superior direito da tela.
1. Insira as configurações para o novo armazenamento de dados.

   Um título em negrito em um campo em uma [!DNL Workfront Fusion] O módulo indica uma configuração necessária.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nome do armazenamento de dados] </td> 
      <td> <p>Insira um nome para o armazenamento de dados. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Estrutura de Dados]</p> </td> 
      <td> <p>Uma estrutura de dados é uma lista das colunas de uma tabela. Essa lista indica o nome da coluna e o tipo de dados.</p> <p>Siga um destes procedimentos:</p> 
       <ul> 
        <li style="font-weight: bold;">Selecionar uma estrutura de dados que já foi criada</li> 
        <li> <p style="font-weight: bold;">Adicionar uma nova estrutura de dados</p> <p>Clique em <strong>[!UICONTROL Adicionar]</strong> para criar uma nova estrutura de dados.</p> <p>Para obter mais informações, consulte <a href="#set-up-the-data-structure" class="MCXref xref">Configurar a estrutura de dados</a> neste artigo.</p> </li> 
        <li style="font-weight: bold;"> <p>Deixe o campo vazio</p> <p style="font-weight: normal;">Se você não selecionar ou adicionar uma estrutura de dados, o banco de dados conterá apenas a chave primária. Esse tipo de banco de dados é útil se você quiser salvar somente as chaves e estiver interessado em saber apenas se uma chave específica existe ou não no banco de dados.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Tamanho do armazenamento de dados em MB]</p> </td> 
      <td> <p>Aloque o tamanho do armazenamento de dados do armazenamento de dados interno total.</p> <p> O valor padrão é 10 MB. Se você tiver menos de 10 MB de espaço não alocado do Armazenamento de dados em sua alocação de 500 MB, o tamanho padrão será a quantidade de armazenamento não alocado.  <p>Nota: A quantia reservada pode ser alterada a qualquer momento.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Configurar a estrutura de dados

1. Ao criar ou editar um armazenamento de dados, clique em **[!UICONTROL Adicionar]**.
1. No **[!UICONTROL Adicionar estrutura de dados]** que for exibida, configure os seguintes campos:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nome da estrutura de dados]</td> 
      <td> <p> Insira um nome para a nova estrutura de dados.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Especificação]</p> </td> 
      <td> <p>Siga um destes procedimentos para configurar as colunas do armazenamento de dados.</p> 
       <ul> 
        <li> <p>Clique em <strong>[!UICONTROL Adicionar item]</strong> para especificar as propriedades de uma coluna manualmente.</p> <p>Insira o <strong>[!UICONTROL Nome]</strong> e <strong>[!UICONTROL Tipo]</strong> para a coluna armazenamento de dados e defina as propriedades correspondentes.</p> </li> 
        <li> <p>Clique em <strong>[!UICONTROL Gerador]</strong> para determinar as colunas com base nos dados de amostra fornecidos.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Exemplo: </b></span></span> 
          <p>Por exemplo, os seguintes dados de amostra JSON criam três colunas: nome, idade e número de telefone. O número de telefone é uma coleção de números de telefone celular e fixo.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>As colunas vazias na exibição do armazenamento de dados:</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>Em seguida, é possível adicionar valores ao armazenamento de dados manualmente ou usando o [!DNL Workfront Fusion] módulos de armazenamento de dados.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Estrito] </td> 
      <td> <p>Habilite essa opção para garantir que a carga corresponda às estruturas de dados. Cargas que contêm itens extras não especificados na estrutura de dados são rejeitadas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Editar um armazenamento de dados existente

É possível editar as propriedades e o conteúdo de um Armazenamento de dados existente na [!UICONTROL Armazenamento de dados] área de [!DNL Workfront Fusion].

* [Editar as propriedades de um armazenamento de dados](#edit-the-properties-of-a-data-store)
* [Editar o conteúdo de um armazenamento de dados](#edit-the-contents-of-a-data-store)

### Editar as propriedades de um armazenamento de dados

As propriedades de um armazenamento de dados incluem a estrutura de dados que o armazenamento de dados usa, bem como o tamanho do armazenamento de dados.

1. Clique em **[!UICONTROL Armazenamento de dados]** ![](assets/data-store-icon.png) no painel de navegação esquerdo, para abrir a janela [!UICONTROL Armazenamento de dados] área.
1. Clique em **[!UICONTROL Editar]** ![](assets/data-store-edit.png) ao lado do armazenamento de dados que você deseja editar.
1. (Opcional) Se desejar alterar a estrutura de dados usada por esse armazenamento de dados para outra estrutura de dados existente, selecione-a na **[!UICONTROL Estrutura de dados]** menu suspenso.

   Ou

   (Opcional) Se quiser alterar a estrutura de dados usada por esse armazenamento de dados para uma estrutura de dados totalmente nova, consulte [Configurar a estrutura de dados](#set-up-the-data-structure) neste artigo.

1. (Opcional) Altere o tamanho do armazenamento de dados inserindo o novo tamanho na variável **[!UICONTROL Tamanho do armazenamento de dados em MB]** campo.
1. Clique em **[!UICONTROL Salvar]**.

### Editar o conteúdo de um armazenamento de dados

1. Clique em **[!UICONTROL Armazenamento de dados]** ícone ![](assets/data-store-icon.png) no painel de navegação esquerdo, para abrir a janela [!UICONTROL Armazenamento de dados] área.
1. Clique em **[!UICONTROL Procurar]**  ao lado do armazenamento de dados que você deseja editar.
1. (Opcional) Reordene as colunas arrastando-as para o local desejado.
1. (Opcional) [!UICONTROL Editar] uma única célula clicando no ícone **[!UICONTROL Editar]** nessa célula e, em seguida, inserindo o valor desejado.
1. (Opcional) Adicione um novo item ao armazenamento de dados clicando em **[!UICONTROL Adicionar]** e, em seguida, especificando as informações do novo item.
1. Clique em **[!UICONTROL Salvar]**.

## Solução de problemas

* [Restauração de dados perdidos de um armazenamento de dados](#restoring-lost-data-from-a-data-store)
* [Erro de falta de espaço](#out-of-space-error)
* [Erro de máximo de armazenamentos atingido](#maximum-stores-reached-error)

### Restauração de dados perdidos de um armazenamento de dados

No momento, não há nenhuma ferramenta que possa automatizar a restauração de dados perdidos.

#### Solução alternativa

1. Examine todos os logs de execução de cenários em que os itens foram inseridos no armazenamento de dados.

   Para obter mais informações sobre o exame de logs de execução, consulte [Exibir o histórico de execução de um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copie os dados.
1. Insira os dados no armazenamento de dados novamente.

   Para obter informações sobre como inserir dados em um armazenamento de dados, consulte [Editar o conteúdo de um armazenamento de dados](#edit-the-contents-of-a-data-store) neste artigo.

### [!UICONTROL Sem espaço] erro

Um [!UICONTROL Sem espaço] erro porque os armazenamentos de dados criados anteriormente já receberam o armazenamento de armazenamento de dados alocado.

#### Solução alternativa

1. Edite qualquer um dos armazenamentos de dados existentes para usar menos espaço. Isso libera espaço para o novo armazenamento de dados.

   Para obter mais informações, consulte [Editar as propriedades de um armazenamento de dados](#edit-the-properties-of-a-data-store) neste artigo.

>[!NOTE]
>
>Recomendamos que você não atribua todo o seu espaço a um único armazenamento de dados, a menos que tenha certeza de que não exigirá mais armazenamentos de dados.

### [!UICONTROL Máximo de armazenamentos atingido] erro

A [!UICONTROL Máximo de armazenamentos atingido] erro porque sua organização usou todos os armazenamentos de dados disponíveis. Uma organização tem um número de armazenamentos de dados disponíveis igual ao dobro do número de cenários disponíveis. Portanto, o número total de armazenamentos de dados disponíveis depende do plano adquirido.

Por exemplo, se sua organização tiver adquirido um plano com 15 cenários, ela poderá ter até 30 armazenamentos de dados.

#### Solução alternativa

Para reduzir o número de armazenamentos de dados existentes, considere seguir um destes procedimentos:

* Combinar armazenamentos de dados existentes
* Excluir armazenamentos de dados não utilizados
