---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Armazenamento de dados em [!DNL Adobe Workfront Fusion]
description: Um armazenamento de dados, semelhante a um banco de dados ou a uma tabela simples, pode armazenar dados de cenários, permitindo transferir dados entre cenários individuais ou execuções de cenário. Você pode usar um armazenamento de dados para armazenar novos dados de vários sistemas durante a sincronização.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Armazenamento de dados em [!DNL Adobe Workfront Fusion]

Um armazenamento de dados, semelhante a um banco de dados ou a uma tabela simples, pode armazenar dados de cenários, permitindo transferir dados entre cenários individuais ou execuções de cenário. Você pode usar um armazenamento de dados para armazenar novos dados de vários sistemas durante a sincronização.

Os módulos de armazenamento de dados permitem que você execute as seguintes ações em registros em seus [!DNL Adobe Workfront Fusion] armazenamento de dados:

* Adicionar
* Substituir
* Atualizar
* Recuperar
* Excluir
* Pesquisar
* Contagem

Para obter informações sobre o uso de módulos de armazenamento de dados, consulte [[!UICONTROL Armazenamento de dados] módulos](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

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
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Criar um armazenamento de dados em [!DNL Workfront Fusion]

* [Configurar o armazenamento de dados](#set-up-the-data-store)
* [Configurar a estrutura de dados](#set-up-the-data-structure)

### Configurar o armazenamento de dados

Antes de usar um armazenamento de dados em um módulo, você deve criar o armazenamento de dados em [!DNL Workfront Fusion].

>[!NOTE]
>
>Sua organização tem um número limitado de armazenamentos de dados disponíveis. Se você tentar criar mais armazenamentos de dados do que o disponível, [!DNL Workfront] retorna um [!UICONTROL Máximo de lojas atingido] erro.
>
>Para obter mais informações, consulte [Erro de máximo de lojas atingido](#maximum-stores-reached-error) neste artigo.

1. Faça logon no [!DNL Workfront Fusion] conta.
1. Clique em **[!UICONTROL Repositórios de dados]** no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Adicionar armazenamento de dados]** no canto superior direito da tela.
1. Insira as configurações para o novo armazenamento de dados.

   Um título em negrito em um campo em um [!DNL Workfront Fusion] indica uma configuração obrigatória.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nome do armazenamento de dados] </td> 
      <td> <p>Insira um nome para o armazenamento de dados. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Estrutura de dados]</p> </td> 
      <td> <p>Uma estrutura de dados é uma lista das colunas de uma tabela. Essa lista indica o nome da coluna e o tipo de dados.</p> <p>Siga um destes procedimentos:</p> 
       <ul> 
        <li style="font-weight: bold;">Selecione uma estrutura de dados que já foi criada</li> 
        <li> <p style="font-weight: bold;">Adicionar uma nova estrutura de dados</p> <p>Clique em <strong>[!UICONTROL Adicionar]</strong> para criar uma nova estrutura de dados.</p> <p>Para obter mais informações, consulte o <a href="#set-up-the-data-structure" class="MCXref xref">Configurar a estrutura de dados</a> neste artigo.</p> </li> 
        <li style="font-weight: bold;"> <p>Deixe o campo vazio</p> <p style="font-weight: normal;">Se você não selecionar ou adicionar uma estrutura de dados, o banco de dados conterá apenas a chave primária. Esse tipo de banco de dados é útil se você deseja salvar chaves somente e está interessado em saber apenas se uma chave específica existe ou não no banco de dados.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Tamanho do armazenamento de dados em MB]</p> </td> 
      <td> <p>Aloque o tamanho do armazenamento de dados do seu armazenamento de dados interno total.</p> <p>Observação: O valor reservado pode ser alterado a qualquer momento.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Configurar a estrutura de dados

1. Ao criar ou editar um armazenamento de dados, clique em **[!UICONTROL Adicionar]**.
1. No **[!UICONTROL Adicionar estrutura de dados]** for exibida, configure os seguintes campos:

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
      <td> <p>Siga um destes procedimentos para configurar as colunas do seu armazenamento de dados.</p> 
       <ul> 
        <li> <p>Clique em <strong>[!UICONTROL Adicionar item]</strong> para especificar as propriedades de uma coluna manualmente.</p> <p>Insira o <strong>[!UICONTROL Name]</strong> e <strong>[!UICONTROL Tipo]</strong> para a coluna de armazenamento de dados e defina as propriedades correspondentes.</p> </li> 
        <li> <p>Clique em <strong>[!UICONTROL Generator]</strong> para determinar as colunas dos dados de amostra fornecidos.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Exemplo: </b></span></span> 
          <p>Por exemplo, os seguintes dados de amostra JSON criam três colunas: nome, idade e número de telefone. Número de telefone é uma coleção de números de celular e telefone fixo.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>As colunas vazias na visualização do armazenamento de dados:</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>Em seguida, é possível adicionar valores ao armazenamento de dados manualmente ou usando a variável [!DNL Workfront Fusion] módulos de armazenamento de dados.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Strict] </td> 
      <td> <p>Ative essa opção para garantir que a carga corresponda às estruturas de dados. As cargas que contêm itens extras não especificados na estrutura de dados são rejeitadas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Editar um armazenamento de dados existente

É possível editar as propriedades e os conteúdos de um Data Store existente na [!UICONTROL Armazenamento de dados] área de [!DNL Workfront Fusion].

* [Editar as propriedades de um armazenamento de dados](#edit-the-properties-of-a-data-store)
* [Editar o conteúdo de um armazenamento de dados](#edit-the-contents-of-a-data-store)

### Editar as propriedades de um armazenamento de dados

As propriedades de um armazenamento de dados incluem a estrutura de dados que o armazenamento de dados usa, bem como o tamanho do armazenamento de dados.

1. Clique em **[!UICONTROL Armazenamento de dados]** ![](assets/data-store-icon.png) no painel de navegação esquerdo para abrir o [!UICONTROL Armazenamento de dados] área.
1. Clique em **[!UICONTROL Editar]** ![](assets/data-store-edit.png) ao lado do armazenamento de dados que deseja editar.
1. (Opcional) Se desejar alterar a estrutura de dados usada por esse armazenamento de dados para outra estrutura de dados existente, selecione-a no **[!UICONTROL Estrutura de dados]** lista suspensa.

   Ou

   (Opcional) Se desejar alterar a estrutura de dados usada por esse armazenamento de dados para uma estrutura de dados totalmente nova, consulte [Configurar a estrutura de dados](#set-up-the-data-structure) neste artigo.

1. (Opcional) Altere o tamanho do armazenamento de dados inserindo o novo tamanho na variável **[!UICONTROL Tamanho do armazenamento de dados em MB]** campo.
1. Clique em **[!UICONTROL Salvar]**.

### Editar o conteúdo de um armazenamento de dados

1. Clique no botão **[!UICONTROL Armazenamento de dados]** ícone ![](assets/data-store-icon.png) no painel de navegação esquerdo para abrir o [!UICONTROL Armazenamento de dados] área.
1. Clique em **[!UICONTROL Procurar]** ![](assets/browse-data-store.png) ao lado do armazenamento de dados que deseja editar.
1. (Opcional) Reorganize as colunas arrastando-as para o local desejado.
1. (Opcional) [!UICONTROL Editar] uma única célula clicando no botão **[!UICONTROL Editar]** ícone ![](assets/data-store-edit.png)nessa célula, em seguida, insira o valor desejado.
1. (Opcional) Adicione um novo item ao armazenamento de dados clicando em **[!UICONTROL Adicionar]**, em seguida, inserindo as informações do novo item.
1. Clique em **[!UICONTROL Salvar]**.

## Solução de problemas

* [Restauração de dados perdidos de um armazenamento de dados](#restoring-lost-data-from-a-data-store)
* [Erro de falta de espaço](#out-of-space-error)
* [Erro de máximo de lojas atingido](#maximum-stores-reached-error)

### Restauração de dados perdidos de um armazenamento de dados

No momento, não há nenhuma ferramenta que possa automatizar a restauração de dados perdidos.

#### Solução alternativa

1. Examine todos os logs de execução de cenários em que itens foram inseridos no armazenamento de dados.

   Para obter mais informações sobre a análise de logs de execução, consulte [Visualize o histórico de execução de um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copie os dados.
1. Insira os dados no armazenamento de dados novamente.

   Para obter informações sobre como inserir dados em um armazenamento de dados, consulte [Editar o conteúdo de um armazenamento de dados](#edit-the-contents-of-a-data-store) neste artigo.

### [!UICONTROL Sem espaço] erro

Um [!UICONTROL Sem espaço] ocorre porque seus armazenamentos de dados criados anteriormente já receberam o armazenamento de armazenamento de dados alocado.

#### Solução alternativa

1. Edite qualquer um dos armazenamentos de dados existentes para usar menos espaço. Isso libera espaço para o novo armazenamento de dados.

   Para obter mais informações, consulte [Editar as propriedades de um armazenamento de dados](#edit-the-properties-of-a-data-store) neste artigo.

>[!NOTE]
>
>Recomendamos que você não atribua todo o seu espaço a um único armazenamento de dados, a menos que tenha certeza de que não precisará de mais armazenamentos de dados.

### [!UICONTROL Máximo de lojas atingido] erro

A [!UICONTROL Máximo de lojas atingido] ocorre porque sua organização usou todos os armazenamentos de dados disponíveis. Uma organização tem vários armazenamentos de dados disponíveis iguais ao dobro do número de cenários disponíveis. Portanto, o número total de armazenamentos de dados disponíveis depende do plano que você comprou.

Por exemplo, se sua organização adquiriu um plano com 15 cenários, a organização pode ter até 30 armazenamentos de dados.

#### Solução alternativa

Para reduzir o número de armazenamentos de dados existentes, considere fazer o seguinte:

* Combinar armazenamentos de dados existentes
* Excluir armazenamentos de dados não utilizados
