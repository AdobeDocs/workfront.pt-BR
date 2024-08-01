---
title: Registros duplicados
description: Você pode duplicar um registro existente na exibição de tabela. Uma cópia idêntica do registro existente é adicionada à página de tipo de registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---


# Registros duplicados

<!--update the metadata after GA-->

{{planning-important-intro}}

No Adobe Workfront Planning, um registro é uma instância de um tipo de registro.

Você pode duplicar um registro existente na exibição de tabela. Uma cópia idêntica do registro existente é adicionada à página de tipo de registro.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no estágio de acesso antecipado do Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Novo: Padrão</p>
   <p>Atual: Plano</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de acesso para o Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Contribute ou permissões superiores para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral sobre acesso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso para a documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Duplicar um registro <!--in a record type table (I don't think you can create them elsewhere right now)-->

Você pode criar registros na exibição de tabela de uma página de tipo de registro duplicando uma existente. Um registro idêntico ao existente é criado e adicionado ao registro original.


{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.
Todos os registros do tipo selecionado são exibidos na visualização.

1. (Condicional) Selecione uma exibição de tabela.

1. Siga um destes procedimentos:

   * Passe o mouse sobre o nome de um registro, em seguida, clique no menu **Mais** incorporado com o nome do registro e, em seguida, clique no ícone **Duplicar** ![](assets/duplicate-icon-gray.png).

     ![](assets/more-menu-from-record-in-table-view.png)

   * Selecione um registro e clique no ícone ![](assets/duplicate-icon-white-and-blue.png) de **Duplicar**, na barra de ferramentas, na parte inferior da página.

     ![](assets/duplicate-icon-in-toolbar-in-table-view.png)

   Um registro idêntico com um nome idêntico é criado abaixo do registro original. Todos os campos do novo registro são preenchidos com as mesmas informações do registro original.

1. (Opcional) Comece a atualizar as informações sobre o novo registro nos campos disponíveis na exibição de tabela ou clique no registro e atualize as informações na visualização ou página do registro.

   >[!NOTE]
   >
   >  * Não há campos obrigatórios para registros. No entanto, recomendamos adicionar informações para o campo principal de um registro, pois é útil identificar registros ao vincular registros uns aos outros. Para obter mais informações sobre campos primários, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md) e [Visão geral do campo primário](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Os campos que se referem a outros tipos de registro ou campos calculados são campos somente leitura.

   Para obter mais informações sobre como editar registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

1. (Opcional) Use os seguintes atalhos de teclado para desfazer ou refazer a adição de novos registros ou suas informações ao adicioná-los na exibição de tabela:

   * CTRL + Z (⌘ + Z para Mac) para desfazer uma alteração
   * CTRL + Shift + Z (⌘ + Shift + Z para Mac) para refazer uma alteração.