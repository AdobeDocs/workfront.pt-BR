---
title: Organizar e visualizar um formulário
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode organizar um formulário personalizado com o Form Designer.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '1330'
ht-degree: 0%

---

# Organizar e pré-visualização um formulário

É possível organizar um formulário personalizado com o designer de formulários e pré-visualização-lo para verificar se ele foi configurado corretamente.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar uma quebra de seção

É possível grupo os campos e widgets personalizados em um formulário personalizado em seções com cabeçalhos. Isso é útil para apresentar uma experiência organizada a usuários que preencherão o formulário. Além disso, se você precisar limitar o acesso a determinados campos e widgets personalizados a determinados usuários, poderá colocá-los em uma seção e conceder acesso à seção somente a esses usuários.

Por exemplo, se você precisar rastrear informações confidenciais que somente administradores do sistema devem poder exibir ou editar, poderá criar uma quebra de seção com permissões Somente de administrador e colocar os campos confidenciais nessa seção.

As configurações de acesso selecionadas para uma seção são vinculadas diretamente às permissões que os usuários têm no objeto do Workfront ao qual o formulário personalizado está anexado. Você pode ocultar ou mostrar uma seção com base no fato de o usuário ter acesso para exibir, contribuir ou gerenciar esse objeto. Ou você pode definir uma seção como Somente administrador para que somente usuários com um nível de acesso de administrador do sistema possam acessá-la.

Para obter informações sobre permissões em objetos, consulte [Visão geral das permissões de compartilhamento em objetos](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Criar um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) personalizado.

### Criar e configurar o acesso para uma seção em um formulário personalizado

1. Comece a criar ou editar um formulário personalizado e adicionar campos, conforme descrito Criar [um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) personalizado.

1. Clique **em Quebrar seção** e arraste-a para a posição desejada na tela.

1. No painel direito, configure as opções desejadas para a seção:

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
      <td>Digite texto se quiser explicar aos usuários para que serve a seção. É exibido abaixo do rótulo da seção no formulário personalizado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Conceder acesso</p> </td> 
      <td> <p> Selecione as permissões que os usuários precisam em um objeto ao qual o formulário personalizado está anexado para exibir esta seção e editar seus valores de campo. 
       <p>As seguintes permissões estão disponíveis em <b>Os usuários com este acesso ao objeto podem exibir os valores do campo</b>:</p> 
         <ul>
          <li><strong></strong>Exibir: permissões Exibir para o objeto</li>
          <li><p><b>Editar</b> limitada: (disponível apenas se o objeto for um projeto, tarefa, problema ou usuário):</p> 
          <p>Permite que os usuários contribuam com o objeto se ele for um projeto, tarefa ou problema.</p>
          <p>Permite que os usuários editem o perfil ou sejam proprietários da permissão de perfil para o objeto, se for um usuário.</p></li> 
          <li><b>Editar</b>: gerenciar permissões para o objeto </li> 
          <li><b>Somente administrador</b>: nível de acesso de Administrador do Sistema</li> 
         </ul> </li> 
        <p>As seguintes permissões estão disponíveis em <b>Os usuários com este acesso ao objeto podem editar os valores dos campos</b>: </p> 
         <ul> 
          <li> <p><b>Editar</b> limitada: (disponível apenas se o objeto for um projeto, tarefa, problema ou usuário):</p> 
           <p>Se o objeto for um projeto, tarefa ou um problema, esse permissão permitirá que os usuários contribuam para o objeto</p>
          <p>Se o objeto for um usuário, esse permissão permite que os usuários editem os perfil ou possuam os perfil permissão ao objeto.</p> 
          <li><b></b>Editar: gerenciar permissões para o objeto </li> 
          <li><b>Somente administrador</b>: nível de acesso de Administrador do Sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Para obter informações sobre permissões em objetos, consulte <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral das permissões de compartilhamento em objetos</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Os usuários sem as permissões especificadas aqui não podem ver os campos e widgets personalizados na seção. </p> <p>Isso também é verdadeiro se você exibir os valores dos campos nos relatórios ou usá-los em campos calculados nos relatórios do modo de texto.</p> </li> 
       <li><p>Para formulários personalizados de solicitação/ocorrência: se o acesso de Exibição for necessário para ver os campos na quebra de seção, mas o acesso de Administrador for necessário para editar os campos, a seção e todos os seus campos não estarão visíveis para não administradores quando eles preencherem o formulário. Depois que o solicitação é criado, os usuários com acesso Exibir podem visualização os campos na seção.</p></li>
       <li> <p>A associação de vários tipos de objetos ao formulário pode alterar as permissões de visualização e edição disponíveis nessas etapas. Para obter mais informações, consulte <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Como vários tipos de objetos podem afetar as permissões de quebra de seção em um formulário</a> personalizado neste artigo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Adicionar Lógica</p></td> 
      <td><p>Use a lógica de exibição para especificar se a seção deve ser exibida no formulário, com base nas seleções que os usuários fazem em campos personalizados de múltipla escolha quando preenchem o formulário.</p><p><strong>OBSERVAÇÃO:</strong> se todos os campos individuais em uma quebra de seção tiverem uma lógica de exibição aplicada a eles e todos estiverem ocultos como resultado da lógica, a seção inteira será ocultada no formulário personalizado. Isso ocorrerá mesmo se a lógica de exibição não for aplicada à quebra de seção.</p><p>Para obter mais informações, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">Adicionar lógica de exibição e lógica de salto com o designer de formulário</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Arraste ou adicione pelo menos um campo ou widget personalizado à nova seção. Isso é necessário antes de salvar a seção.

1. Clique **Concluído**.

   >[!TIP]
   >
   >Você pode clicar **Aplicar** a qualquer momento ao criar um formulário personalizado para salvar as alterações e manter o formulário aberto.

### Como vários tipos de objetos podem afetar as permissões de interrupção de seção {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

A permissão Edição limitada para quebras de seção de formulário personalizado está disponível somente para os tipos de objeto Projeto, Tarefa, Problema e Usuário.

Em um formulário personalizado com uma quebra de seção configurada com a permissão Edição limitada, se você adicionar um dos outros tipos de objeto ao formulário (Portfolio, Programa, Documento, Empresa, Registro de faturamento, Iteração, Despesa ou Grupo), será solicitado que você alterne para a permissão Editar, que é compatível com esse tipo de objeto e com os tipos de objeto existentes no formulário.

>[!INFO]
>
>**Exemplo:** em um formulário personalizado associado ao tipo de objeto Projeto, uma quebra de seção é configurada com a permissão Edição Limitada.
>
>Adicione o tipo de objeto Portfolio ao formulário, o que significa que a opção de permissão Edição limitada não está mais disponível para a quebra de seção no formulário.
>
>Uma mensagem na tela solicita que você alterne para a permissão Editar, que é o nível mínimo de permissões compatíveis com o tipo de objeto Projeto e o tipo de objeto Portfolio.


## Posicionar campos e widgets personalizados em um formulário personalizado


1. Comece a criar ou editar um formulário personalizado, conforme descrito em [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Para posicionar campos e widgets personalizados na mesma linha, arraste um ao lado do outro até que uma linha apareça entre eles.

   >[!NOTE]
   >
   >* Você pode usar o botão **Visualizar** no canto superior direito para ter uma ideia de como os campos e widgets personalizados serão exibidos no formulário.
   >* Campos e widgets personalizados nem sempre podem ser exibidos da mesma maneira no formulário, dependendo de quanto espaço na tela está disponível quando um usuário o está visualizando. Por exemplo, o terceiro campo em uma linha de campos pode passar para a próxima linha de campos se o espaço horizontal for limitado.

1. (Opcional) Para posicionar um campo personalizado ou um widget acima ou abaixo de outro, arraste-o para cima ou para baixo até que uma linha azul horizontal apareça entre os itens.

1. Para mover um campo personalizado para outra seção no formulário, arraste-o e solte-o no local ou clique no **ícone Mover para** o campo e selecione a seção para movê-lo.

   ![Mover campo para uma seção](assets/move-field-to-section.png)

1. Para salvar as alterações, clique em **Aplicar**

   ou

   Clique em **Salvar e fechar**.

## Pré-visualizar um formulário personalizado

1. Comece a criar ou editar um formulário personalizado e adicionar campos, conforme descrito em [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Clique **Visualização** no canto superior direito para ver como o formulário ficará ao ser usado e clique **em End Visualização** para voltar a editar o formulário.

