---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Comparar objetos entre ambientes
description: Você pode comparar objetos entre ambientes para garantir que seus pacotes de promoção de ambiente contenham os objetos necessários.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 2ff7a8b0ae3cc1f641c0d7c0b1384548c9603423
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Comparar objetos entre ambientes

Você pode comparar objetos entre ambientes para garantir que seus pacotes de promoção de ambiente contenham os objetos necessários.

Você seleciona os ambientes e tipos de objetos a serem comparados. O Workfront compara todos os objetos dos tipos selecionados em ambos os ambientes e apresenta dados relativos às diferenças entre objetos.

## Requisitos de acesso

Você deve ter o seguinte:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plano</strong>
   </td>
   <td> Prime ou Ultimate (somente novos planos)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenças</strong>
   </td>
   <td> [!UICONTROL Padrão]
   </td>
  </tr>
   <tr>
   <td>Configurações de nível de acesso
   </td>
   <td>Você deve ser um administrador [!DNL Workfront].
   </td>
  </tr>
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

Sua organização deve estar na Plataforma de negócios Adobe para comparar objetos entre ambientes.

## Gerar uma comparação de objetos

1. Vá para um ambiente no qual você deseja comparar um objeto.
1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. Selecione **Sistema** na navegação à esquerda e **Promoção do ambiente**.
1. Clique em **Comparar ambientes** próximo ao canto superior direito da tela.
1. No campo **Ambiente Source**, selecione o ambiente no qual deseja criar o pacote. Este é o ambiente do qual você está copiando objetos **de**.
1. No campo **Ambiente de destino**, selecione o ambiente no qual deseja instalar o pacote. Este é o ambiente no qual você está copiando os objetos **para**.
1. Na área **Objetos a serem comparados**, selecione os tipos de objetos que você deseja comparar entre ambientes.
1. Clique em **Gerar comparação** próximo ao canto superior direito da tela.

   A comparação pode levar algum tempo para ser gerada, dependendo do número e do tamanho dos objetos comparados.

## Exibir comparação de objetos

Após a conclusão da geração da comparação, a comparação é exibida.

A lista inclui objetos dos tipos selecionados que existem no ambiente de origem, se esses objetos estão ausentes no ambiente de destino e se há diferenças de campo entre os dois.

>[!BEGINSHADEBOX]

![Exemplo de comparação](assets/environment-promotion-comparison.png)

Neste exemplo:

* A primeira linha mostra um objeto que está presente no ambiente de destino, mas é diferente do ambiente de origem.
* A segunda linha mostra um objeto que está presente no ambiente de destino e é igual ao ambiente de origem.
* A terceira linha mostra um objeto que não está presente no ambiente de destino.

>[!ENDSHADEBOX]

Para exibir diferenças específicas de objetos:

1. Clique no ícone de lupa ![](assets/compare-icon.png) na linha desse objeto.

   Uma janela é aberta com todos os campos desse objeto. as diferenças são marcadas em vermelho.

## Criar um pacote a partir de uma comparação de objetos

Você pode criar um pacote diretamente de uma comparação de objetos.

Para obter instruções, consulte [Criar um pacote a partir de uma comparação de objeto](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison) no artigo Criar ou editar um pacote de promoção de ambiente.
