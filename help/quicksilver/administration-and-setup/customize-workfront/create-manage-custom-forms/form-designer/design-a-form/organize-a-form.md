---
title: Organizar e visualizar um formulário com o Designer de Formulários
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode organizar um formulário personalizado com o Designer de formulário.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Organizar e visualizar um formulário com o designer de formulário

Você pode organizar um formulário personalizado com o designer de formulário.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Plano Adobe Workfront*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>
   <p>Plano atual: Padrão</p>
   <p>ou</p>
   <p>Plano herdado: Plano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## Adicionar uma quebra de seção

É possível agrupar os campos e widgets personalizados em um formulário personalizado em seções com cabeçalhos. Isso é útil para apresentar uma experiência organizada aos usuários que preencherão o formulário. Além disso, se for necessário limitar o acesso a determinados campos e widgets personalizados a determinados usuários, coloque-os em uma seção e conceda acesso à seção somente para esses usuários.

Por exemplo, se você precisar rastrear informações confidenciais que somente administradores de sistema devem poder exibir ou editar, poderá criar uma quebra de seção com permissões Somente administrador e colocar os campos confidenciais nessa seção.

As configurações de acesso selecionadas para uma seção estão diretamente vinculadas às permissões que os usuários têm no objeto do Workfront, onde o formulário personalizado está anexado. Você pode ocultar ou mostrar uma seção com base no acesso do usuário para exibir, contribuir ou gerenciar esse objeto. Ou você pode definir uma seção como Somente administrador para que somente usuários com um nível de acesso de administrador do sistema possam acessá-la.

Para obter informações sobre permissões em objetos, consulte [Visão geral do compartilhamento de permissões em objetos](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Criar um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Criar e configurar o acesso de uma seção em um formulário personalizado

1. Comece a criar ou editar um formulário personalizado e a adicionar campos, conforme descrito em [Criar um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Clique em **Quebra de seção** e arraste-o para a posição desejada na tela.

1. No painel direito, configure as opções desejadas para a seção :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima da seção. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite o texto se desejar explicar aos usuários para que serve a seção. Isso é exibido abaixo do rótulo da seção no formulário personalizado.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>Conceder acesso</p> </td> 
      <td> <p> Selecione as permissões que os usuários precisam em um objeto ao qual o formulário personalizado está anexado para exibir esta seção e editar seus valores de campo. 
       <p>As seguintes permissões estão disponíveis em <b>Os usuários com esse acesso ao objeto podem exibir valores de campo</b>:</p> 
         <ul>  
          <li><p><b>Edição limitada</b>: (Disponível somente se o objeto for um projeto, tarefa, problema ou usuário):</p> 
          <p>Permite que os usuários contribuam com o objeto se for um projeto, tarefa ou problema.</p>
          <p>Permite que os usuários editem o perfil ou sejam proprietários da permissão de perfil para o objeto se for um usuário.</p></li> 
          <li><b>Editar</b>: Gerenciar permissões para o objeto </li> 
          <li><b>Somente administrador</b>: Nível de acesso do Administrador do sistema</li> 
         </ul> </li> 
        <p>As seguintes permissões estão disponíveis em <b>Os usuários com esse acesso ao objeto podem editar valores de campo</b>: </p> 
         <ul> 
          <li> <p><b>Edição limitada</b>: (Disponível somente se o objeto for um projeto, tarefa, problema ou usuário):</p> 
           <p>Se o objeto for um projeto, tarefa ou problema, essa permissão permitirá que os usuários contribuam para o objeto</p>
          <p>Se o objeto for um usuário, essa permissão permitirá que os usuários editem o perfil ou sejam proprietários da permissão de perfil para o objeto.</p> 
          <li><b>Editar</b>: Gerenciar permissões para o objeto </li> 
          <li><b>Somente administrador</b>: Nível de acesso do Administrador do sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Para obter informações sobre permissões em objetos, consulte <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral do compartilhamento de permissões em objetos</a>.</p> 
       <p><b>Nota</b>:  
       <ul> 
       <li> <p>Os usuários sem as permissões que você especificar aqui não podem ver os campos e widgets personalizados na seção . </p> <p>Isso também é verdadeiro se você exibir os valores dos campos nos relatórios ou usá-los em campos calculados no relatório do modo de texto.</p> </li> 
       <li> <p>Associar vários tipos de objetos ao formulário pode alterar as permissões de visualização e edição disponíveis nessas etapas. Para obter mais informações, consulte <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Como vários tipos de objetos podem afetar as permissões de quebra de seção em um formulário personalizado</a> neste artigo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Arraste ou adicione pelo menos um campo ou widget personalizado à nova seção. Isso é necessário antes de salvar a seção .

1. Clique em **Concluído**.

   >[!TIP]
   >
   >Você pode clicar em **Aplicar** em qualquer momento durante a criação de um formulário personalizado para salvar suas alterações e manter o formulário aberto.

### Como vários tipos de objetos podem afetar as permissões de quebra de seção {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

A permissão de Edição limitada para quebras de seção de formulário personalizado está disponível apenas para os tipos de objeto Projeto, Tarefa, Problema e Usuário.

Em um formulário personalizado com uma quebra de seção configurada com a permissão Edição limitada, se você adicionar um dos outros tipos de objeto ao formulário (Portfolio, Programa, Documento, Empresa, Registro de faturamento, Iteração, Despesa ou Grupo), será solicitado a alternar para a permissão Editar, que é compatível com esse tipo de objeto e com os tipos de objeto existentes no formulário.

>[!INFO]
>
>**Exemplo:** Em um formulário personalizado associado ao tipo de objeto Projeto , uma quebra de seção é configurada com a permissão Edição limitada.
>
>Você adiciona o tipo de objeto Portfolio ao formulário, o que significa que a opção de permissão Edição limitada não está mais disponível para a quebra de seção no formulário.
>
>Uma mensagem na tela solicita que você alterne para a permissão Editar , que é o menor nível de permissões compatível com o tipo de objeto Projeto e o tipo de objeto Portfolio.


## Posicionar campos e widgets personalizados em um formulário personalizado


1. Comece a criar ou editar um formulário personalizado, conforme descrito em [Criar um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Para posicionar campos e widgets personalizados na mesma linha, arraste um ao lado do outro até que uma linha apareça entre eles.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* Você pode usar o **Visualizar** no canto superior direito para ter uma ideia de como os campos e widgets personalizados serão exibidos no formulário.
>* Os campos e widgets personalizados nem sempre são exibidos da mesma maneira no formulário, dependendo da quantidade de espaço de tela disponível quando o usuário o visualiza. Por exemplo, o terceiro campo em uma linha de campos pode vincular à próxima linha de campos se o espaço horizontal for limitado.


1. (Opcional)Para posicionar um campo ou widget personalizado acima ou abaixo de outro, arraste-o para cima ou para baixo até que uma linha azul horizontal apareça entre os itens.

1. Para salvar as alterações, clique em **Aplicar**

   ou

   Clique em **Salvar e fechar**.

## Visualizar um formulário personalizado

1. Comece a criar ou editar um formulário personalizado e a adicionar campos, conforme descrito em [Criar um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Clique em **Visualizar** no canto superior esquerdo para ver como o formulário será exibido durante o uso, em seguida, clique em **Visualização final** para retornar à edição do formulário.