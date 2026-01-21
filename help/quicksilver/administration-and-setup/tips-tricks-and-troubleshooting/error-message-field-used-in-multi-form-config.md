---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensagem de erro: Há um pequeno problema. Esse campo é usado em uma configuração de vários formulários'
description: Quando você altera um cálculo em um campo personalizado calculado em um formulário personalizado e uma mensagem de erro informa que o campo é usado em uma configuração de vários formulários, é necessário substituir o campo por um novo campo que contenha o cálculo que você deseja usar.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: 8b93842d7ce61c7c84b07639b6329bedf4254ffd
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 0%

---

# Mensagem de erro: Há um pequeno problema. Esse campo é usado em uma configuração de vários formulários

## Problema

Quando você altera um cálculo em um campo personalizado calculado em um formulário personalizado, [!DNL Adobe Workfront] pode exibir o seguinte aviso:

Há um pequeno problema

[O campo] é usado em uma configuração de vários formulários. Se você quiser alterar essa fórmula, será necessário remover esse campo e substituí-lo por um novo campo que contenha o cálculo desejado.

## Causa

Pelo menos dois formulários personalizados contendo o campo personalizado calculado que você está tentando alterar estão anexados a um único objeto na sua instância [!DNL Workfront].

**Exemplo:** os formulários A e B personalizados estão anexados à mesma tarefa. Ambos os formulários contêm um campo personalizado calculado chamado Lucro. Você encontra o erro ao tentar editar o cálculo no campo Lucro no formulário A personalizado.

Você não pode alterar o cálculo do campo personalizado em um dos formulários porque isso entraria em conflito com a fórmula no mesmo campo do outro formulário.
Para resolver esse conflito, é necessário localizar o objeto ao qual os vários formulários com o mesmo campo personalizado calculado estão anexados e, em seguida, executar um dos seguintes procedimentos:

* Remova um dos formulários do objeto.
* Altere o cálculo conforme necessário, mas faça isso em todos os formulários personalizados anexados ao objeto.
* Em todos os formulários personalizados anexados ao objeto, adicione um novo campo personalizado calculado contendo o cálculo necessário e marque o campo personalizado calculado antigo como obsoleto.

Este artigo explica como localizar o objeto e, em seguida, resolver o problema de uma dessas três maneiras.

>[!NOTE]
>
>Se você vir o erro, mas não puder localizar mais de um objeto contendo o campo personalizado, verifique a Lixeira. É possível que um objeto na Lixeira contenha o campo. Como os objetos na Lixeira podem ser restaurados a qualquer momento, o erro de conflito multiformulário continuará ocorrendo até que o conflito seja resolvido.
>
>Para adicionar um campo com uma expressão diferente, você deve resolver esse conflito seguindo um destes procedimentos:
>
>* Remover o campo do formulário personalizado conflitante
>* Restaure o objeto excluído, desanexe um dos formulários personalizados conflitantes e exclua o objeto novamente, se necessário.

## Localizar o objeto ao qual os formulários personalizados estão anexados {#find-the-object-where-the-custom-forms-are-attached}

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Forms Personalizado]** > **[!UICONTROL Campos]**.
1. Aplique o modo de exibição **[!UICONTROL Lista de campos]** para localizar o campo calculado que você está tentando modificar e anote todos os formulários personalizados em que ele é usado (por exemplo, Formulário 1, Formulário 2, Formulário 3).
1. Clique em **[!UICONTROL Forms]** e aplique a exibição **[!UICONTROL Lista de Formulários]**.
1. Clique na lista suspensa **[!UICONTROL Filtro]** e depois em **[!UICONTROL Novo Filtro]**.

1. Clique em **[!UICONTROL Adicionar uma regra de filtro]**, comece a digitar &quot;nome de formulário personalizado&quot; e selecione esse valor quando ele for exibido na lista.
1. Selecione **[!UICONTROL Igual]** para o modificador de filtro, comece digitando o nome de cada formulário do qual você fez uma observação na Etapa 1, em seguida, selecione-o quando ele for exibido.

   **Exemplo:** O Nome Do Formulário Personalizado É Igual Ao Formulário 1, Formulário 2, Formulário 3.

1. Clique em **[!UICONTROL Salvar filtro]**, nomeie o novo filtro e clique em **[!UICONTROL Salvar filtro]**.

1. Na lista de formulários, anote o tipo de objeto do filtro, como Tarefa ou Problema, exibido na coluna **[!UICONTROL Tipo]**.
1. Em cada formulário personalizado encontrado na Etapa 1, crie um novo campo personalizado Caixa de seleção com um único valor padrão de Sim.

   **Exemplo:** Campo 1 no formulário 1 = Sim, Campo 2 no formulário 2 = Sim, Campo 3 no formulário 3 = Sim. Isso significa que &quot;O Campo personalizado calculado existe no Formulário 1&quot;, ou &quot;O Campo personalizado calculado existe no Formulário 2&quot; e assim por diante.

1. No **[!UICONTROL ícone de Pesquisa]** ![ícone de Pesquisa](assets/search-icon.png), no canto superior direito da tela, clique em **[!UICONTROL Pesquisa Avançada]**.
1. Clique no objeto do formulário personalizado (como Problema), clique em **[!UICONTROL Filtrar resultados]** e em **[!UICONTROL Adicionar um filtro]**.
1. Comece a digitar o nome de um campo Caixa de seleção no campo **[!UICONTROL Comece a digitar o nome do campo]** e selecione-o quando ele for exibido na lista, selecione **[!UICONTROL Igual]** e digite **[!UICONTROL Sim]** (sem aspas) na caixa a seguir.

   **Exemplo:** Campo 1 Igual (Diferencia Maiúsculas De Minúsculas) Sim.

1. Clique em **[!UICONTROL Adicionar um Filtro]** e adicione todos os campos da Caixa de Seleção à Pesquisa Avançada.

   Procure todas as combinações possíveis.

   **Exemplo:** Crie vários filtros com as combinações encontradas, conforme listado abaixo. Você deve encontrar objetos com vários formulários personalizados anexados que contêm os mesmos campos calculados. Você pode encontrar os seguintes cenários:

   * Campo 1= Sim + Campo 2 = Sim + Campo 3 = Sim (sem objetos, por exemplo)
   * Campo 1= Sim + Campo 2 = Sim (sem objetos, por exemplo)
   * Campo 1= Sim + Campo 3 = Sim (dois objetos, por exemplo)

   Isso significa que o campo calculado existe no Formulário 1 e no Formulário 3, pois os campos da Caixa de seleção correspondentes (Campo 1 e Campo 3) existem nesses objetos.

   Campo 2 = Sim + Campo 3 = Sim (sem objetos, por exemplo)

1. Prossiga para uma das seguintes seções neste artigo:

   * [Remova um dos formulários personalizados do objeto e edite o cálculo nele](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Fazer edições idênticas no cálculo em todos os formulários personalizados anexados](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Adicionar um novo campo calculado contendo o cálculo editado a um ou todos os formulários personalizados anexados](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Remova um dos formulários personalizados do objeto e edite o cálculo nele {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Localize o objeto ao qual os formulários personalizados estão anexados, conforme explicado em [Localize o objeto ao qual os formulários personalizados estão anexados](#find-the-object-where-the-custom-forms-are-attached) neste artigo e, em seguida, abra o objeto.
1. Remova um dos formulários personalizados do objeto e salve o objeto.

   >[!NOTE]
   >
   >Para adicionar os campos do formulário removido do objeto, talvez seja necessário editar o formulário personalizado que permanece anexado ao objeto. Dessa forma, você pode preservar as informações de dados personalizados no objeto.

1. No formulário personalizado removido, edite o cálculo do campo personalizado que você estava tentando atualizar originalmente e clique em **[!UICONTROL Salvar]**.

   Desta vez, [!DNL Workfront] não deve encontrar um conflito.

1. (Opcional) Remova os campos da Caixa de seleção dos formulários personalizados ou exclua-os de [!DNL Workfront].

## Fazer edições idênticas no cálculo em todos os formulários personalizados anexados {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>Os dados são perdidos nos objetos nos quais o formulário personalizado já está anexado quando você segue essas etapas. No entanto, se o campo calculado referenciar campos estáticos, não campos calculados, você poderá usar a opção [!UICONTROL Recalcular Expressões Personalizadas] no objeto para restaurar os dados perdidos

1. Localize o objeto ao qual os formulários personalizados estão anexados, conforme explicado em [Localize o objeto ao qual os formulários personalizados estão anexados](#find-the-object-where-the-custom-forms-are-attached) neste artigo.
1. Remova o campo de todos os formulários personalizados anexados ao objeto e salve os formulários.

1. Adicione novamente o campo personalizado que contém o novo cálculo aos formulários personalizados.

   >[!IMPORTANT]
   >
   >Os cálculos devem ser idênticos em todos os formulários personalizados anexados.

1. (Opcional) Remova os campos da Caixa de seleção dos formulários ou exclua-os de [!DNL Workfront].

## Adicionar um novo campo calculado contendo o cálculo editado a um ou todos os formulários personalizados anexados {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

Para evitar a perda de dados no campo personalizado calculado existente ou se precisar editar o cálculo em apenas um dos formulários personalizados anexados ao objeto encontrado:

1. Localize o objeto ao qual os formulários personalizados estão anexados, conforme explicado em [Localize o objeto ao qual os formulários personalizados estão anexados](#find-the-object-where-the-custom-forms-are-attached) neste artigo.
1. Adicione um novo campo personalizado calculado contendo o cálculo necessário a um ou todos os formulários.
1. Renomeie o antigo campo personalizado calculado **Obsoleto**.

   Em todos os formulários anexados ao objeto, esse formulário personalizado calculado mais antigo preserva seus dados históricos, mas os usuários param de usá-lo.

   >[!IMPORTANT]
   >
   >O campo mais antigo pode ser referenciado em outros campos personalizados calculados, portanto, é necessário atualizar esses cálculos depois de alterar seu nome.

1. (Opcional) Remova os campos Caixa de seleção dos formulários ou exclua-os do Workfront.

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
</blockquote>
-->
