---
title: Adicionar Lógica de exibição e Lógica de salto para um formulário
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode decidir quais seções de um formulário personalizado devem ser exibidas ou ignoradas com base nas escolhas que um usuário faz ao preenchê-lo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 75aaa531dba8037ed75c0d6baa6d7c69ec4cfefd
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 0%

---

# Adicionar lógica de exibição e lógica de salto a um formulário

Você pode decidir quais seções de um formulário personalizado devem ser exibidas ou ignoradas com base nas escolhas que um usuário faz ao preenchê-lo.

>[!NOTE]
>
>A lógica se aplica somente a um formulário e não pode ser baseada em seleções de um formulário diferente.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">plano do Adobe Workfront </td> 
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
   <td>Acesso administrativo a formulários personalizados </td> 
  </tr>  
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir e ignorar ícones lógicos

Os formulários personalizados exibem ícones para indicar qual lógica é aplicada a determinados campos. Os ícones em um campo no designer do formulário indicam que a lógica é aplicada ao campo.

| Ícone | Localização no campo no designer do formulário | Definição |
|--- |--- |--- |
| ![Lógica de exibição para o campo de destino](assets/display-logic-bottom-left.png) | Inferior esquerdo | O campo é o campo de destino da lógica de exibição. Se uma seleção específica for feita no formulário, esse campo será exibido. |
| ![Definir ícone da lógica de exibição](assets/display-logic-bottom-right.png) | Inferior direito | O campo define a lógica de exibição. Uma seleção ou um valor específico nesse campo exibe o campo de destino. |
| ![Lógica de salto para o campo de destino](assets/skip-logic-bottom-left.png) | Inferior esquerdo | O campo é o campo de destino para lógica de salto. Se uma seleção específica for feita no formulário, ele pulará adiante para esse campo e os campos intermediários estarão ocultos. |
| ![Definir ícone de lógica de salto](assets/skip-logic-bottom-right.png) | Inferior direito | O campo define a lógica de salto. Uma seleção ou um valor específico nesse campo ignora outros campos e vai diretamente para o campo de destino. |

![Ícones de lógica](assets/logic-icons-3.png)

Selecione um campo com lógica aplicada para exibir as regras de lógica existentes nas configurações do campo.

![Regras de lógica](assets/form-designer-view-only-logic.png)

## Considerações sobre o uso da lógica de exibição e da lógica de salto

* Para adicionar lógica de exibição em um campo personalizado, widget ou quebra de seção, pelo menos um campo de múltipla escolha (botões de opção, lista suspensa ou caixas de seleção) deve ser posicionado antes dele no formulário.
Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Não é possível adicionar lógica de salto a um widget ou quebra de seção. Você pode adicioná-lo somente a um campo de múltipla escolha (botões de opção, lista suspensa ou caixas de seleção).
* Não é possível aplicar a exibição ou a lógica de salto para mostrar ou ocultar as opções de um campo de várias opções. Por exemplo, você não pode restringir as opções exibidas para um campo Suspenso, Grupo de caixas de seleção ou Botão de opção, com base na exibição ou na lógica de ignorar outro campo.
* Você pode adicionar a lógica de exibição e a lógica de salto a um campo personalizado se todos os itens a seguir forem verdadeiros sobre o campo personalizado:

   * É um campo de múltipla escolha (botões de opção, lista suspensa ou caixas de seleção)
   * É precedido por um campo de múltipla escolha
   * Ele é seguido por outro campo personalizado

* Ao copiar formulários com lógica de exibição ou lógica de salto, a lógica é copiada para o novo formulário personalizado.
* Ao editar objetos em massa, todos os campos personalizados são exibidos na caixa Editar objetos, incluindo os campos que são ignorados ou ocultos.
* Lembre-se do seguinte ao criar uma regra de lógica de exibição para um formulário personalizado:

   * Campos personalizados não incluídos em uma instrução lógica de exibição são exibidos em um formulário personalizado por padrão.
   * Você pode criar instruções lógicas de exibição de vários campos.
   * Se todos os campos em uma quebra de seção tiverem lógica de exibição aplicada a eles e todos estiverem ocultos como resultado da lógica, a seção inteira será ocultada no formulário personalizado.

## Adicionar lógica de exibição a um formulário personalizado

A lógica de exibição define quais campos personalizados aparecem no formulário quando o usuário seleciona um valor específico em um campo de múltipla escolha. A lógica é adicionada ao campo de destino, que é exibido somente quando o valor é selecionado.

{{step-1-to-setup}}

1. Clique em **Forms Personalizado**.
1. Crie um novo formulário personalizado ou abra um formulário existente. Consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) para obter detalhes.
1. Adicione campos ao formulário conforme necessário. Pelo menos um campo de múltipla escolha (botão de opção, lista suspensa ou caixa de seleção) deve ser posicionado antes do campo de destino que será exibido.
1. Selecione o campo de destino e clique em **Adicionar lógica** no canto inferior esquerdo da tela.
1. Selecione a guia **Exibir Lógica**.
1. Clique em **Adicionar regra de exibição** no construtor de lógica.

   ![Exibir construtor de lógica](assets/custom-form-logic-builder-display-blank.png)

1. Siga as etapas abaixo no construtor para criar a instrução lógica.

   1. A primeira opção é escolher o campo de definição. Este é o campo com o valor de seleção que exibe o target. Deve ser um campo de múltipla escolha.
   1. A segunda opção é escolher o valor de seleção. Somente os valores já definidos para esse campo estão disponíveis.
   1. A terceira opção é **Selecionado** ou **Não Selecionado**. Escolher **Selecionado** significa que, quando o valor for selecionado, o campo de destino será exibido. Escolher **Não selecionado** significa que quando qualquer outro valor é selecionado no campo de definição, o campo de destino é exibido.
   1. Para adicionar uma regra **And** à instrução lógica, clique em **Adicionar Regra** diretamente abaixo da regra que você acabou de criar. Siga os mesmos prompts para criar a regra. Todas as regras And devem ser atendidas para que o campo de público alvo seja exibido.

      ![Exibir construtor de lógica](assets/custom-form-logic-builder-display1.png)

   1. Para adicionar uma regra **Or** à instrução lógica, clique em **Adicionar regra** próximo à parte inferior do construtor de lógica. Em seguida, clique em **Adicionar regra** dentro da área Ou e siga os mesmos prompts para criar a regra. Quando uma regra Ou é atendida, o campo de destino é exibido.

1. Clique em **Salvar** quando terminar de criar a instrução lógica.

   Os ícones de lógica de exibição são adicionados ao campo de destino e ao campo de definição no designer do formulário.

## Adicionar lógica de salto a um formulário personalizado

A lógica de salto define campos de formulário personalizados que são ignorados quando o usuário seleciona um valor específico em um campo de múltipla escolha. Os campos ignorados estão ocultos no formulário. A lógica é aplicada ao campo de definição onde a seleção é feita, não aos campos que são ignorados.

{{step-1-to-setup}}

1. Clique em **Forms Personalizado**.
1. Crie um novo formulário personalizado ou abra um formulário existente. Consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) para obter detalhes.
1. Adicione campos ao formulário conforme necessário. O campo de definição para a lógica de salto deve ser um campo de múltipla escolha (botão de opção, lista suspensa ou caixa de seleção).
1. Selecione o campo de definição e clique em **Adicionar lógica** no canto inferior esquerdo da tela.
1. Selecione a guia **Ignorar lógica**.
1. Clique em **Adicionar Regra de salto** no construtor de lógica.

   ![Ignorar construtor de lógica](assets/custom-form-logic-builder-skip-blank.png)

1. Siga as etapas abaixo no construtor para criar a instrução lógica.

   1. O campo de definição é mostrado no construtor. É o campo que você selecionou para aplicar a lógica de salto.
   1. A primeira opção é escolher o valor da seleção. Somente os valores já definidos para o campo estão disponíveis.
   1. A segunda opção é **Selecionada** ou **Não Selecionada**. Escolher **Selecionado** significa que quando o valor é selecionado, o campo de destino é exibido e os campos intermediários são ignorados. Escolher **Não selecionado** significa que quando qualquer outro valor é selecionado no campo de definição, o campo de destino é exibido e os campos intermediários são ignorados.
   1. A terceira opção é o campo de destino ou para onde pular. Selecione um nome de campo ou **Fim do formulário**. Talvez seja necessário clicar na palavra &quot;vazio&quot; primeiro antes de selecionar uma opção.

      ![Ignorar construtor de lógica](assets/custom-form-logic-builder-skip1.png)

   1. Para adicionar uma regra **Or** à instrução lógica, clique em **Adicionar regra** próximo à parte inferior do construtor de lógica. Em seguida, selecione as opções seguindo os mesmos prompts para criar a regra. Quando uma regra **Or** é atendida, o campo de destino é exibido.

1. Clique em **Salvar** quando terminar de criar a instrução lógica.

   Os ícones de lógica de salto são adicionados ao campo de destino e ao campo de definição no designer do formulário.


