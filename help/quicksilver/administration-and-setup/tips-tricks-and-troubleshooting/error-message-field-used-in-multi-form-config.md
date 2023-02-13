---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensagem de erro: Há um pequeno problema. Esse campo é usado em uma configuração de vários formulários'
description: Ao alterar um cálculo em um campo personalizado calculado em um formulário personalizado e uma mensagem de erro informar que o campo é usado em uma configuração de vários formulários, é necessário substituir o campo por um novo campo contendo o cálculo que deseja usar.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# Mensagem de erro: Há um pequeno problema. Esse campo é usado em uma configuração de vários formulários

## Problema

Ao alterar um cálculo em um campo personalizado calculado em um formulário personalizado, [!DNL Adobe Workfront] pode exibir o seguinte aviso:

Há um pequeno problema

[O campo] for usada em uma configuração de vários formulários, se quiser alterar essa fórmula, será necessário remover esse campo e substituí-lo por um novo contendo o cálculo desejado.

## Causa

Pelo menos dois formulários personalizados contendo o campo personalizado calculado que você está tentando alterar são anexados a um único objeto em seu [!DNL Workfront] instância.

**Exemplo:** Os formulários personalizados A e B são anexados à mesma tarefa. Ambos os formulários contêm um campo personalizado calculado chamado Lucro. Você encontra o erro ao tentar editar o cálculo no campo Lucro no formulário personalizado A.

Não é possível alterar o cálculo do campo personalizado em um dos formulários, pois isso entraria em conflito com a fórmula no mesmo campo do outro formulário.
Para resolver esse conflito, você deve encontrar o objeto no qual os vários formulários com o mesmo campo personalizado calculado são anexados e, em seguida, realizar um dos seguintes procedimentos:

* Remova um dos formulários do objeto.
* Altere o cálculo conforme necessário, mas faça isso em todos os formulários personalizados anexados ao objeto.
* Em todos os formulários personalizados anexados ao objeto, adicione um novo campo personalizado calculado contendo o cálculo necessário e marque o campo personalizado calculado antigo como obsoleto.

Este artigo explica como encontrar o objeto e depois resolver o problema de uma dessas três maneiras.

## Encontre o objeto ao qual os formulários personalizados estão anexados {#find-the-object-where-the-custom-forms-are-attached}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Usuários]** ![](assets/users-icon-in-main-menu.png).

1. Clique em **[!UICONTROL Forms personalizada]** > **[!UICONTROL Campos]**.
1. Aplique o **[!UICONTROL Lista de campos]** exibir para localizar o campo calculado que você está tentando modificar e anotar todos os formulários personalizados nos quais ele é usado (por exemplo, Formulário 1, Formulário 2, Formulário 3) .
1. Clique em **[!UICONTROL Forms]**, em seguida, aplique a variável **[!UICONTROL Lista de formulários]** exibir.
1. Clique no botão **[!UICONTROL Filtro]** lista suspensa e **[!UICONTROL Novo filtro]**.

1. Clique em **[!UICONTROL Adicionar uma regra de filtro]**, comece digitando &quot;nome de formulário personalizado&quot; e selecione esse valor quando ele for exibido na lista.
1. Selecionar **[!UICONTROL Igual]** para o modificador de filtro, comece a digitar o nome de cada formulário do qual você fez uma observação na Etapa 1 e, em seguida, selecione-o quando for exibido.

   **Exemplo:** O Nome Do Formulário Personalizado É Igual Ao Formulário 1, Formulário 2, Formulário 3.

1. Clique em **[!UICONTROL Salvar filtro]**, nomeie o novo filtro e clique em **[!UICONTROL Salvar filtro]**.

1. Na lista de formulários, anote o tipo de objeto do filtro, como Tarefa ou Problema, que é exibido na **[!UICONTROL Tipo]** coluna.
1. Em cada formulário personalizado encontrado na Etapa 1, crie um novo campo personalizado Caixa de seleção com um único valor padrão, Sim.

   **Exemplo:** Campo 1 no Formulário 1 = Sim, Campo 2 no Formulário 2 = Sim, Campo 3 no Formulário 3 = Sim. Isso significa que &quot;O campo personalizado calculado existe no formulário 1&quot; ou &quot;O campo personalizado calculado existe no formulário 2&quot; e assim por diante.

1. No **[!UICONTROL Ícone de Pesquisa]** ![](assets/search-icon.png) no canto superior direito da tela, clique em **[!UICONTROL Pesquisa avançada]**.
1. Clique no objeto do formulário personalizado (como Problema) e clique em **[!UICONTROL Filtrar os resultados]**, depois clique em **[!UICONTROL Adicionar um filtro]**.
1. Comece digitando o nome de um campo de Caixa de seleção no **[!UICONTROL Iniciar a digitação do nome do campo]** e selecione-o quando for exibido na lista, em seguida, selecione **[!UICONTROL Igual]** e tipo **[!UICONTROL Sim]** (sem aspas) na caixa seguinte.

   **Exemplo:** Campo 1 igual (diferencia maiúsculas de minúsculas) Sim.

1. Clique em **[!UICONTROL Adicionar um filtro]** e adicione todos os campos de Caixa de seleção à Pesquisa avançada.

   Procure todas as combinações possíveis.

   **Exemplo:** Crie vários filtros com as combinações que encontrar, conforme listado abaixo. Você deve encontrar objetos com vários formulários personalizados anexados que contenham os mesmos campos calculados. Você pode encontrar os seguintes cenários:

   * Campo 1= Sim + Campo 2 = Sim + Campo 3 = Sim (sem objetos, por exemplo)
   * Campo 1= Sim + Campo 2 = Sim (sem objetos, por exemplo)
   * Campo 1= Sim + Campo 3 = Sim (dois objetos, por exemplo)

   Isso significa que o campo calculado existe no Formulário 1 e no Formulário 3, pois os campos Caixa de seleção correspondentes (Campo 1 e Campo 3) existem nesses objetos.

   Campo 2 = Sim + Campo 3 = Sim (sem objetos, por exemplo)

1. Continue para uma das seguintes seções neste artigo:

   * [Remova um dos formulários personalizados do objeto e edite o cálculo lá](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Faça edições idênticas no cálculo em todos os formulários personalizados anexados](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Adicione um novo campo calculado contendo o cálculo editado a um ou todos os formulários personalizados anexados](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Remova um dos formulários personalizados do objeto e edite o cálculo lá {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Localize o objeto ao qual os formulários personalizados são anexados, conforme explicado em [Encontre o objeto ao qual os formulários personalizados estão anexados](#find-the-object-where-the-custom-forms-are-attached) neste artigo, abra o objeto .
1. Remova um dos formulários personalizados do objeto e salve o objeto.

   >[!NOTE]
   >
   >Para adicionar os campos do formulário removido do objeto, talvez seja necessário editar o formulário personalizado que permanece anexado ao objeto. Dessa forma, é possível preservar as informações de dados personalizadas no objeto.

1. No formulário personalizado que você removeu, edite o cálculo do campo personalizado que você estava tentando atualizar originalmente e clique em **[!UICONTROL Salvar]**.

   Desta vez, [!DNL Workfront] não deve encontrar um conflito.

1. (Opcional) Remova os campos da caixa de seleção dos formulários personalizados ou exclua-os de [!DNL Workfront].

## Faça edições idênticas no cálculo em todos os formulários personalizados anexados {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>Os dados são perdidos nos objetos em que o formulário personalizado já está anexado ao seguir essas etapas. No entanto, se o campo calculado fizer referência a campos estáticos, não calculados, você poderá usar [!UICONTROL Recalcular expressões personalizadas] no objeto para restaurar os dados perdidos

1. Localize o objeto ao qual os formulários personalizados são anexados, conforme explicado em [Encontre o objeto ao qual os formulários personalizados estão anexados](#find-the-object-where-the-custom-forms-are-attached) neste artigo.
1. Remova o campo de todos os formulários personalizados anexados ao objeto e salve os formulários.

1. Adicione o campo personalizado que contém o novo cálculo de volta aos formulários personalizados.

   >[!IMPORTANT]
   >
   >Os cálculos devem ser idênticos em todos os formulários personalizados anexados.

1. (Opcional) Remova os campos da caixa de seleção dos formulários ou exclua-os de [!DNL Workfront].

## Adicione um novo campo calculado contendo o cálculo editado a um ou todos os formulários personalizados anexados {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

Para evitar a perda de dados no campo personalizado calculado existente, ou se precisar usar o cálculo editado em apenas um dos formulários personalizados anexados ao objeto encontrado:

1. Localize o objeto ao qual os formulários personalizados são anexados, conforme explicado em [Encontre o objeto ao qual os formulários personalizados estão anexados](#find-the-object-where-the-custom-forms-are-attached) neste artigo.
1. Adicione um novo campo personalizado calculado contendo o cálculo necessário para um ou todos os formulários.
1. Renomear o campo personalizado calculado antigo **Obsoleto**.

   Em todos os formulários anexados ao objeto, esse formulário personalizado calculado mais antigo preserva seus dados históricos, mas os usuários param de usá-lo.

   >[!IMPORTANT]
   >
   >O campo mais antigo pode ser referenciado em outros campos personalizados calculados, portanto, é necessário atualizar esses cálculos depois de alterar seu nome.

1. (Opcional) Remova os campos da caixa de seleção dos formulários ou exclua-os do Workfront.

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->
