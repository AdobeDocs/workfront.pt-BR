---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Criar e gerenciar campos personalizados em [!DNL Workfront Proof]
description: Um Select ou Premium [!DNL Workfront] O plano é necessário para usar esse recurso. Para obter mais informações sobre os vários planos disponíveis, consulte Planos do Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 0%

---

# Criar e gerenciar campos personalizados em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Um Select ou Premium [!DNL Workfront] O plano é necessário para usar esse recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos da Workfront](https://www.workfront.com/plans).

Campos personalizados permitem capturar dados adicionais ao criar uma nova prova, um novo usuário ou um novo convidado.

Por exemplo, os usuários que criam uma nova prova podem querer incluir uma seção adicional que permita capturar um Número da Ordem de Produção, Código do Departamento ou Referência do Fornecedor.

>[!NOTE]
>
>* Capturar esse tipo de informação na página Nova prova por meio de campos Personalizados também permitirá reduzir o comprimento do nome da prova, pois esses detalhes não precisarão ser incluídos no nome. Para obter informações sobre a página Nova prova, consulte &quot;Criação de provas em [!DNL Workfront Proof].&quot;
>
>Depois que um campo Personalizado for usado em uma prova, usuário ou contato, você não poderá excluí-lo ou editar o tipo de campo. No entanto, é possível ocultá-lo (por meio da variável [!UICONTROL Configurações de campo personalizado] para que não seja usada para novos itens.
>
>Se você tornar uma Seção de campo personalizada oculta, todos os campos dentro da seção também estarão ocultos, mesmo que os campos individuais estejam definidos como visíveis.

Este artigo explica como fazer o seguinte:

## Criar campos personalizados

Primeiro, é necessário configurar a seção Campo personalizado à qual você adicionará campos personalizados.

1. Clique em **[!UICONTROL Configurações]** >**[!UICONTROL Configurações da conta]**, em seguida, abra o **[!UICONTROL Campos personalizados]** guia .

1. Clique em **[!UICONTROL Adicionar seção de campo personalizado]** no módulo relevante (Prova, Usuários ou Contatos).
1. Digite um **Nome** para seção de campo personalizado, clique em **[!UICONTROL Salvar]**.

   Agora é possível configurar campos personalizados na seção :

1. Clique no botão **[!UICONTROL Configurações de campos personalizados]** para atualizar a página.
1. Clique no nome da nova seção de campo personalizado para abrir o **[!UICONTROL Campo personalizado] seção** para a nova seção.
1. Clique no botão **[!UICONTROL Novo campo personalizado]** próximo ao canto superior direito.
1. No **[!UICONTROL Novo campo personalizado]** página exibida, especifique os detalhes do campo personalizado:

   | **Obrigatório** | O Workfront exige que os usuários preencham o campo. |
   |---|---|
   | **Pesquisável** | Permite que os usuários encontrem itens pesquisando nos dados do campo Personalizado. |
   | **Oculto** | Oculta o campo personalizado no [!UICONTROL Nova prova], Novo convidado e [!UICONTROL Novo usuário] páginas |

   {style="table-layout:auto"}

1. Clique em **[!UICONTROL Salvar]**.
1. No **Campo personalizado** página exibida, clique no botão **[!UICONTROL Configurações de campos personalizados]** para atualizar a página.

1. Faça mais alterações nas configurações do campo:

   * Oculte ou exiba a seção do campo personalizado clicando no botão **[!UICONTROL Mais]** menu (três pontos) à direita do nome da seção do campo personalizado e, em seguida, clique em **[!UICONTROL Ocultar seção]** ou **[!UICONTROL Mostrar seção]**.

   * Oculte ou exiba o campo personalizado clicando no botão **[!UICONTROL Mais]** menu (três pontos) à direita do nome da seção do campo personalizado e, em seguida, clique em **[!UICONTROL Ocultar campo personalizado]** ou **[!UICONTROL Mostrar campo personalizado]**.

   * Altere a ordem dos campos usando as setas para cima/para baixo exibidas à direita de seus nomes (se você tiver adicionado vários campos em uma seção).

1. Abra o **[!UICONTROL Regras de visibilidade]** guia .\
   As regras de visibilidade permitem determinar quais campos adicionais serão mostrados, com base na conclusão do campo Personalizado inicial. Por exemplo, se o campo dependente for A e o campo Controle for X, isso significa que o Campo A só estará visível se o campo X for concluído.

   Você pode usar valores de controle para determinar os valores no campo de controle que, se selecionado, resultarão na visibilidade do campo dependente. Por exemplo, imagine que o campo dependente é A e o campo de controle é X e você define os valores de controle em X para serem apenas as opções 1 e 2. Isso significa que o campo A estará visível somente se a opção 1 ou 2 do campo X estiver selecionada. Isso significa que, se o campo X opções 3 ou 4 estiver selecionado, o campo A não será exibido. Abra o **[!UICONTROL Regras de visibilidade]** guia .

   Para adicionar uma regra de visibilidade:

   1. Clique em **[!UICONTROL Nova regra de visibilidade]** para o módulo no qual você deseja adicionar a regra.
   1. Selecione as configurações desejadas para a regra e clique em **[!UICONTROL Salvar]**.

1. Abra o **[!UICONTROL Regras de dependência]** guia .

   As regras de dependência permitem determinar as opções disponíveis no campo dependente quando determinadas opções são selecionadas no campo de controle. Por exemplo, se o campo dependente for &quot;B&quot; e o campo de controle for &quot;Y&quot;, você poderá configurá-lo da seguinte maneira:

   Se a opção 1 no campo Y for escolhida, apenas as opções 1 e 2 no campo B serão mostradas.

   Se a opção 2 no campo Y for escolhida, apenas serão mostradas as opções 3 e 4 no campo B.

   Para adicionar uma regra de dependência:

   1. Clique em **[!UICONTROL Nova regra de dependência]** para o módulo que você deseja adicionar a regra.
   1. Selecione as configurações desejadas para a dependência e clique em **[!UICONTROL Salvar]**.

## Gerenciar seus campos personalizados

Você pode exibir e editar os detalhes da seção Campo personalizado ou campos personalizados individuais.

1. Clique em **[!UICONTROL Configurações]** >**[!UICONTROL Configurações da conta]**, em seguida, abra o **[!UICONTROL Campos personalizados]** guia .

1. Clique no nome da seção de campo personalizado ou do campo personalizado individual.
1. (Condicional) Se você estiver gerenciando uma seção de campo personalizado , faça qualquer uma das seguintes alterações no **[!UICONTROL Seção de campo personalizado]** página:

   * Edite o nome da seção .
   * Mova-o para um módulo diferente.
   * Ocultar/mostrar a seção.

1. (Condicional) Se você estiver gerenciando um campo personalizado, faça qualquer uma das seguintes alterações no **[!UICONTROL Campo personalizado]** página:

   * Mova o campo para uma seção diferente.
   * Edite o nome do campo.
   * Texto de ajuda de entrada (um ícone de ponto de interrogação será exibido ao lado da seção do campo e o texto será exibido ao passar o mouse sobre ele).
   * Ative/desative o **[!UICONTROL Obrigatório]** no campo .
   * Ative/desative o **[!UICONTROL Pesquisável]** no campo .
   * Ocultar/mostrar o campo.
   * Edite o tipo de campo .
   * Defina/edite um valor padrão para o campo .
   * Configure as regras de visibilidade e dependência (conforme descrito acima nas etapas 11 e 12).
