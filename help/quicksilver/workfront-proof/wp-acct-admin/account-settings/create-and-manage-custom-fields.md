---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Criar e gerenciar campos personalizados em  [!DNL Workfront Proof]
description: Um Plano Select ou Premium [!DNL Workfront] é necessário para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte Planos do Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 7f24186c8803237a6f5116293b3c6a5fd1ea90f6
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Criar e gerenciar campos personalizados em [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

É necessário um Plano Select ou Premium [!DNL Workfront] para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos do Workfront](https://business.adobe.com/products/workfront/pricing.html).

Campos personalizados permitem capturar dados adicionais ao criar uma nova prova, usuário ou convidado. Por exemplo, os usuários que criam uma nova prova podem querer incluir uma seção adicional que lhes permita capturar um Número da Ordem de Produção, Código do Departamento ou Referência do Fornecedor.

>[!NOTE]
>
>* A captura desse tipo de informação na página Nova prova por meio de campos personalizados também permite reduzir o comprimento do nome da prova, pois esses detalhes não precisarão ser incluídos no nome.
>
>* Depois que um campo personalizado é usado em uma prova, usuário ou contato, não é possível excluí-lo ou editar o tipo de campo. No entanto, você poderá ocultá-lo por meio da página Configurações do campo personalizado para que ele não seja usado para novos itens.
>
>* Se você ocultar uma seção de campo personalizado, todos os campos na seção também serão ocultos, mesmo que os campos individuais estejam definidos como visíveis.

## Criar campos personalizados

{{step1-to-proofing}}

1. No canto superior direito da página, clique em **Configurações da conta**.

1. Na página **Configurações de conta**, selecione a guia **Campos personalizados**.

1. Clique em **[!UICONTROL Adicionar seção de campo personalizado]** no lado direito do módulo (**Prova**, **Usuários** ou **Contatos**) ao qual deseja adicionar o campo personalizado. A guia **Detalhes da seção** é aberta.

1. Digite um **Nome** para a seção de campo personalizado e clique em **[!UICONTROL Salvar]**.

1. Clique na guia **[!UICONTROL Configurações de campos personalizados]** para atualizar a página. A nova seção de campo personalizado é exibida em seu módulo atribuído.

   ![Guia de configurações de campos personalizados](assets/custom-field-settings-tab.png)

1. Clique no nome da nova seção de campo personalizado para abrir a guia **Seção de campos personalizados**.

1. No lado superior direito da página, clique no botão **[!UICONTROL Novo campo personalizado]**. A página **Novo campo personalizado** é exibida.

1. Especifique os **Detalhes do campo**:

   * **Nome**: insira o nome do campo personalizado.
   * **Ajuda**: insira o texto de ajuda que será exibido em uma dica de ferramenta.
   * **Obrigatório**: marque esta caixa para exigir que o usuário preencha o campo.
   * **Pesquisável** (Condicional): marque esta caixa para tornar o campo personalizado pesquisável.
   * **Oculto**: marque esta caixa para ocultar o campo personalizado nas páginas **Nova prova**, **Novo convidado** e **Novo usuário**.

1. Especifique o **Tipo de campo** e os detalhes:

   * **Tipo**: selecione o tipo de campo personalizado.
   * **Listar itens**: (Condicional) Adicione os itens da lista que aparecerão no campo personalizado.
   * **Valor padrão**: selecione o valor padrão para este campo personalizado. Essa opção varia de acordo com o tipo de campo personalizado selecionado.

1. Clique em **[!UICONTROL Salvar]**.

1. Faça mais alterações nas configurações do campo:

   * Oculte ou reexiba a seção de campo personalizado clicando no menu **Mais** ![Mais botão](assets/more-button-small.png) à direita do nome da seção de campo personalizado e clicando em **[!UICONTROL Ocultar seção]** ou **[!UICONTROL Reexibir seção]**.
   * Oculte ou reexiba o campo personalizado clicando no menu **Mais** ![Mais botão](assets/more-button-small.png) à direita do nome da seção de campo personalizado e clicando em **[!UICONTROL Ocultar campo personalizado]** ou **[!UICONTROL Reexibir campo personalizado]**.
   * Altere a ordem dos campos usando as setas para cima/para baixo exibidas à direita de seus nomes (se você tiver adicionado vários campos em uma seção).

1. Clique na guia **[!UICONTROL Regras de visibilidade]**.

   As regras de visibilidade permitem determinar quais campos adicionais são mostrados com base no preenchimento do campo personalizado inicial. Por exemplo, se o campo dependente for A e o campo Controlando for X, isso significa que o Campo A só estará visível se o campo X estiver preenchido.

   Você pode usar valores de controle para determinar os valores no campo de controle que, se separados, resultarão na visibilidade do campo dependente. Por exemplo, imagine que o campo dependente é A e o campo de controle é X e você define os valores de controle em X para serem somente as opções 1 e 2. Isso significa que o campo A estará visível somente se a opção 1 ou 2 do campo X estiver selecionada. Além disso, se as opções 3 ou 4 do campo X forem selecionadas, o campo A não será exibido.

   >[!NOTE]
   >
   >Somente os tipos de campo personalizado Lista e Rádio podem ser usados para o campo de controle em uma regra de visibilidade, enquanto o campo dependente pode ser qualquer tipo de campo.

   Para adicionar uma regra de visibilidade:

   1. Clique em **[!UICONTROL Nova regra de visibilidade]** para o módulo ao qual deseja adicionar a regra.

   1. Selecione as configurações desejadas para a regra e clique em **[!UICONTROL Salvar]**.

1. Abra a guia **[!UICONTROL Regras de dependência]**.

   As regras de dependência permitem determinar as opções disponíveis no campo dependente quando determinadas opções são selecionadas no campo de controle. Por exemplo, se o campo dependente for &quot;B&quot; e o campo de controle for &quot;Y&quot;, você poderá configurá-lo da seguinte maneira:

   * Se a opção 1 no campo Y for escolhida, somente as opções 1 e 2 no campo B serão exibidas.

   * Se a opção 2 no campo Y for escolhida, somente as opções 3 e 4 no campo B serão exibidas.

   >[!NOTE]
   >
   >Somente os tipos de campo personalizado Lista e Rádio podem ser usados para os campos dependentes e de controle em uma regra de dependência.

   Para adicionar uma regra de dependência:

   1. Clique em **[!UICONTROL Nova regra de dependência]** para o módulo ao qual deseja adicionar a regra.

   1. Selecione as configurações desejadas para a dependência e clique em **[!UICONTROL Salvar]**.

## Gerenciar campos personalizados

É possível exibir e editar os detalhes da seção Campo personalizado ou de campos personalizados individuais.

{{step1-to-proofing}}

1. No canto superior direito da página, clique em **Configurações da conta**.

1. Na página **Configurações de conta**, selecione a guia **Campos personalizados**.

1. Clique no nome da seção de campo personalizado ou no campo personalizado individual.

1. (Condicional) Se você estiver gerenciando uma seção de campo personalizado, faça qualquer uma das seguintes alterações na página **[!UICONTROL Seção de campo personalizado]**:

   * Edite o nome da seção.
   * Mova-o para um módulo diferente.
   * Ocultar/mostrar a seção.

1. (Condicional) Se estiver gerenciando um campo personalizado, faça qualquer uma das seguintes alterações na página **[!UICONTROL Campo personalizado]**:

   * Mova o campo para uma seção diferente.
   * Edite o nome do campo.
   * Editar texto de ajuda.
   * Habilite/desabilite a configuração **[!UICONTROL Obrigatório]** no campo.
   * (Condicional) Habilite/desabilite a configuração **[!UICONTROL Pesquisável]** no campo.
   * Ocultar/reexibir o campo.
   * Edite o tipo de campo.
   * Definir/editar um valor padrão para o campo.
   * Configurar regras de visibilidade e dependência.
