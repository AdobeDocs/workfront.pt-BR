---
title: Adicionar ou editar uma imagem ou outro widget de ativo em um formulário personalizado
description: É possível adicionar ou editar as propriedades de qualquer um dos seguintes widgets de ativo, como imagens, vídeos, arquivos PDF e arquivos Adobe XD, em um formulário personalizado. Isso é útil quando você precisa incluir conteúdo visual, como imagens de marca, um vídeo de instrução ou um protótipo interativo para um aplicativo que você está criando.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: eeff0c8a3f7cbccd942c978d771d24f4cf9c425d
workflow-type: tm+mt
source-wordcount: '1325'
ht-degree: 1%

---

# Adicionar ou editar uma imagem ou outro widget de ativo em um formulário personalizado

É possível adicionar ou editar as propriedades de qualquer um dos seguintes widgets de ativo em um formulário personalizado:

* Imagem
* Vídeo
* Arquivo PDF
* Arquivo Adobe XD

Isso é útil quando você precisa incluir conteúdo visual, como imagens de marca, um vídeo de instrução ou um protótipo interativo para um aplicativo que você está criando.

Quando um formulário personalizado contendo um widget é anexado a um objeto, os usuários que trabalham com ele podem vê-lo nas seguintes áreas:

* A área Detalhes do objeto (por exemplo, para um projeto, a área Detalhes do projeto)
* A caixa Editar do objeto, se ele tiver a nova aparência da experiência do Adobe Workfront (por exemplo, as caixas Editar projeto e Editar tarefa)

Atualmente, os usuários não podem ver o widget nas seguintes áreas: &#x200B;

* Listas e relatórios
* Início e resumo
* A caixa Editar do objeto, se ele não tiver a nova aparência da experiência do Adobe Workfront (por exemplo, a caixa Editar Despesa)
* O aplicativo móvel do Workfront


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
   <td>Plano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você possui, entre em contato com o administrador da Workfront.

## Adicionar ou editar um widget de ativo em um formulário personalizado

1. Comece a trabalhar em um formulário personalizado, conforme descrito em [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Com o **Adicionar um campo** abra a guia , siga um destes procedimentos:

   * Se estiver adicionando um novo widget, selecione **Imagem**, **PDF** ou **Vídeo** para adicioná-lo à parte inferior do formulário ou arraste-o onde deseja no formulário.

      ![](assets/add-widget.png)


   * Se desejar adicionar um widget que já foi adicionado a outro formulário personalizado, clique em **Biblioteca de campos**, em seguida, clique no nome do widget na lista exibida. Para obter mais informações, consulte [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * Se você estiver editando um widget já adicionado ao formulário personalizado, selecione-o.

1. Digite ou edite qualquer uma das seguintes propriedades do widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima do widget. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obrigatório) Este nome é como o sistema identifica o widget.</p> <p>Ao configurar o widget pela primeira vez e digitar o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Rótulo e Nome não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p> <p><b>IMPORTANTE</b>: Embora seja possível fazer isso, recomendamos que você não altere esse nome depois que você ou outros usuários começarem a usar o formulário personalizado no widget. Caso sim, o sistema não reconhecerá mais o widget, onde ele pode ser referenciado em outras áreas do Workfront. </p> <p>Cada nome de widget deve ser exclusivo na instância do Workfront de sua organização. Dessa forma, é possível reutilizar um que já foi criado para outro formulário personalizado. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obrigatório) Digite ou cole o URL do widget onde ele está armazenado na Internet.</p> 
      <p>Se você estiver adicionando um widget de vídeo, no momento, é possível fazê-lo adicionando o seguinte na caixa URL:</p> 
      <ul> 
      <li> <p>Link YouTube ou Vimeo</p> </li> 
      <li> <p>Link de vídeo da unidade Google</p> </li> 
      <li> <p>Link para vídeo com extensão MP4 e MOV</p> </li> 
      <li> <p>Link para o vídeo já carregado na área Documents na instância do Workfront. Para obter instruções, consulte <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Adicionar um widget de vídeo a um formulário personalizado na área Documentos</a> neste artigo.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruções</td> 
      <td> <p>Digite quaisquer informações adicionais sobre o widget. Quando os usuários preenchem o formulário personalizado, eles podem passar o mouse sobre o ícone de ponto de interrogação para visualizar uma dica de ferramenta com as informações digitadas aqui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamanho</td> 
      <td>Altere o tamanho de exibição do widget, conforme necessário.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Aplicar**.
1. Se quiser continuar criando seu formulário personalizado de outras maneiras, continue com um dos seguintes artigos:

   * [Posicionar campos e widgets personalizados em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Reutilizar um campo personalizado calculado existente em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Adicionar lógica de exibição e ignorar lógica a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Visualizar e preencher um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## Adicionar um arquivo XD a um formulário personalizado

1. Comece a trabalhar em um formulário personalizado, conforme descrito em [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Com o **Adicionar um campo** abrir guia, selecionar **Adobe XD**.
1. Digite ou edite qualquer uma das seguintes propriedades do widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima do widget. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obrigatório) Este nome é como o sistema identifica o widget.</p> <p>Ao configurar o widget pela primeira vez e digitar o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Rótulo e Nome não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p> <p><b>IMPORTANTE</b>: Embora seja possível fazer isso, recomendamos que você não altere esse nome depois que você ou outros usuários começarem a usar o formulário personalizado no widget. Caso sim, o sistema não reconhecerá mais o widget, onde ele pode ser referenciado em outras áreas do Workfront. </p> <p>Cada nome de widget deve ser exclusivo na instância do Workfront de sua organização. Dessa forma, é possível reutilizar um que já foi criado para outro formulário personalizado. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obrigatório) Digite ou cole um link de protótipo de XD válido.</p> 
      <p>Observação: A configuração Acesso a link na guia Compartilhar no Adobe XD deve ser definida como Qualquer pessoa com o link . Caso contrário, os usuários não poderão visualizar o protótipo. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruções</td> 
      <td> <p>(Opcional) Digite quaisquer informações adicionais sobre o widget. Quando os usuários preenchem o formulário personalizado, eles podem passar o mouse sobre o ícone de ponto de interrogação para visualizar uma dica de ferramenta com as informações digitadas aqui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamanho</td> 
      <td>(Opcional) Altere o tamanho de exibição do widget, conforme necessário.</td> 
     </tr> 
    </tbody> 
   </table>

1. Se quiser continuar criando seu formulário personalizado de outras maneiras, continue com um dos seguintes artigos:

   * [Posicionar campos e widgets personalizados em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Reutilizar um campo personalizado calculado existente em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Adicionar lógica de exibição e ignorar lógica a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Visualizar e preencher um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Adicionar um widget de vídeo a um formulário personalizado na área Documentos {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Ao adicionar um vídeo a um formulário personalizado dessa forma, somente as permissões definidas para o formulário personalizado se aplicam ao vídeo quando os usuários acessam o formulário em um objeto, não as permissões definidas para o vídeo na área Documentos.

1. Vá para o vídeo na área Documents e gere uma prova para ele, conforme descrito em [Criar uma prova interativa para um site ou outro conteúdo da Web](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Abra a prova.
1. Clique com o botão direito do mouse em qualquer lugar do vídeo e selecione **Copiar endereço de vídeo**.
1. No formulário personalizado, onde você está adicionando o widget de vídeo, cole o endereço copiado no **URL** caixa.
