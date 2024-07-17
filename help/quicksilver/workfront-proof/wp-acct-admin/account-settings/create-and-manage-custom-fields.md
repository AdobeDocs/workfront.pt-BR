---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Criar e gerenciar campos personalizados em  [!DNL Workfront Proof]
description: Um Plano Select ou Premium [!DNL Workfront] é necessário para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte Planos do Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 6e6cc1db8f89b76d9903905e6ee4cf9014727ba1
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 0%

---

# Criar e gerenciar campos personalizados em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

É necessário um Plano Select ou Premium [!DNL Workfront] para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos do Workfront](https://www.workfront.com/plans).

Campos personalizados permitem capturar dados adicionais ao criar uma nova prova, um novo usuário ou um novo convidado.

Por exemplo, os usuários que criam uma nova prova podem querer incluir uma seção adicional que lhes permita capturar um Número da Ordem de Produção, Código do Departamento ou Referência do Fornecedor.

>[!NOTE]
>
>* A captura desse tipo de informação na página Nova prova por meio de Campos personalizados também permitirá que você reduza o comprimento do nome da prova, pois esses detalhes não precisarão ser incluídos no nome. Para obter informações sobre a página Nova prova, consulte &quot;Criando Provas em [!DNL Workfront Proof]&quot;.
>
>Depois que um campo personalizado for usado em uma prova, usuário ou contato, você não poderá excluí-lo nem editar o tipo de campo. No entanto, você poderá ocultá-lo (por meio da página [!UICONTROL Configurações de campo personalizado]) para que ele não seja usado para novos itens.
>
>Se você tornar oculta uma Seção de campo personalizado, todos os campos dentro da seção também serão ocultados, mesmo que os campos individuais estejam definidos como visíveis.

Este artigo explica como fazer o seguinte:

## Criar campos personalizados

Primeiro, é necessário configurar a seção Campo personalizado à qual você adicionará campos personalizados.

1. Clique em **[!UICONTROL Configurações]** >**[!UICONTROL Configurações da conta]** e abra a guia **[!UICONTROL Campos personalizados]**.

1. Clique em **[!UICONTROL Adicionar seção de campo personalizado]** no módulo relevante (Prova, Usuários ou Contatos).
1. Digite um **Nome** para a seção de campo personalizado e clique em **[!UICONTROL Salvar]**.

   Agora é possível configurar campos personalizados na seção:

1. Clique na guia **[!UICONTROL Configurações de campos personalizados]** para atualizar a página.
1. Clique no nome da nova seção de campo personalizado para abrir a página **[!UICONTROL Seção de campo personalizado]** da nova seção.
1. Clique no **[!UICONTROL Novo campo personalizado]** próximo ao canto superior direito.
1. Na página **[!UICONTROL Novo campo personalizado]** que é exibida, especifique os detalhes do campo personalizado:

   | **Obrigatório** | O Workfront exige que os usuários preencham o campo. |
   |---|---|
   | **Pesquisável** | Permite que os usuários localizem itens pesquisando nos dados do campo Personalizado. |
   | **Oculto** | Oculta o campo personalizado nas páginas [!UICONTROL Nova prova], Novo convidado e [!UICONTROL Novo usuário] |

   {style="table-layout:auto"}

1. Clique em **[!UICONTROL Salvar]**.
1. Na página **Campo personalizado** exibida, clique na guia **[!UICONTROL Configurações de campos personalizados]** para atualizar a página.

1. Faça mais alterações nas configurações do campo:

   * Oculte ou reexiba a seção de campo personalizado clicando no menu **[!UICONTROL Mais]** (três pontos) à direita do nome da seção de campo personalizado e clicando em **[!UICONTROL Ocultar seção]** ou **[!UICONTROL Reexibir seção]**.

   * Oculte ou reexiba o campo personalizado clicando no menu **[!UICONTROL Mais]** (três pontos) à direita do nome da seção de campo personalizado e clicando em **[!UICONTROL Ocultar campo personalizado]** ou **[!UICONTROL Reexibir campo personalizado]**.

   * Altere a ordem dos campos usando as setas para cima/para baixo exibidas à direita de seus nomes (se você tiver adicionado vários campos em uma seção).

1. Abra a guia **[!UICONTROL Regras de visibilidade]**.\
   As regras de visibilidade permitem determinar quais campos adicionais são mostrados, com base no preenchimento do campo Personalizado inicial. Por exemplo, se o campo dependente for A e o campo Controlando for X, isso significa que o Campo A só estará visível se o campo X estiver preenchido.

   Você pode usar valores de controle para determinar os valores no campo de controle que, se separados, resultarão na visibilidade do campo dependente. Por exemplo, imagine que o campo dependente é A e o campo de controle é X e você define os valores de controle em X para serem somente as opções 1 e 2. Isso significa que o campo A estará visível somente se a opção 1 ou 2 do campo X estiver selecionada. Isso significa que se as opções 3 ou 4 do campo X forem selecionadas, o campo A não será exibido. Abra a guia **[!UICONTROL Regras de visibilidade]**.

   >[!NOTE]
   >
   >Somente os tipos de campo personalizado Lista e Rádio podem ser usados para o campo de controle em uma regra de visibilidade, enquanto o campo dependente pode ser qualquer tipo de campo.

   Para adicionar uma regra de visibilidade:

   1. Clique em **[!UICONTROL Nova regra de visibilidade]** para o módulo ao qual você deseja adicionar a regra.
   1. Selecione as configurações desejadas para a regra e clique em **[!UICONTROL Salvar]**.

1. Abra a guia **[!UICONTROL Regras de dependência]**.

   As regras de dependência permitem determinar as opções disponíveis no campo dependente quando determinadas opções são selecionadas no campo de controle. Por exemplo, se o campo dependente for &quot;B&quot; e o campo de controle for &quot;Y&quot;, você poderá configurá-lo da seguinte maneira:

   Se a opção 1 no campo Y for escolhida, somente as opções 1 e 2 no campo B serão exibidas.

   Se a opção 2 no campo Y for escolhida, somente as opções 3 e 4 no campo B serão exibidas.

   >[!NOTE]
   >
   >Somente os tipos de campo personalizado Lista e Rádio podem ser usados para os campos dependentes e de controle em uma regra de dependência.

   Para adicionar uma regra de dependência:

   1. Clique em **[!UICONTROL Nova regra de dependência]** para o módulo que deseja adicionar à regra.
   1. Selecione as configurações desejadas para a dependência e clique em **[!UICONTROL Salvar]**.

## Gerenciar campos personalizados

Você pode exibir e editar os detalhes da sua seção Campo personalizado ou de campos personalizados individuais.

1. Clique em **[!UICONTROL Configurações]** >**[!UICONTROL Configurações da conta]** e abra a guia **[!UICONTROL Campos personalizados]**.

1. Clique no nome da seção de campo personalizado ou no campo personalizado individual.
1. (Condicional) Se você estiver gerenciando uma seção de campo personalizado, faça qualquer uma das seguintes alterações na página **[!UICONTROL Seção de campo personalizado]**:

   * Edite o nome da seção.
   * Mova-o para um módulo diferente.
   * Ocultar/mostrar a seção.

1. (Condicional) Se estiver gerenciando um campo personalizado, faça qualquer uma das seguintes alterações na página **[!UICONTROL Campo personalizado]**:

   * Mova o campo para uma seção diferente.
   * Edite o nome do campo.
   * Insira o texto de ajuda (um ícone de ponto de interrogação será exibido ao lado da seção do campo e o texto será exibido ao passar o mouse sobre ele).
   * Habilite/desabilite a configuração **[!UICONTROL Obrigatório]** no campo.
   * Habilite/desabilite a configuração **[!UICONTROL Pesquisável]** no campo.
   * Ocultar/reexibir o campo.
   * Edite o tipo de campo.
   * Definir/editar um valor padrão para o campo.
   * Configure as regras de visibilidade e dependência (conforme descrito acima nas etapas 11 e 12).
