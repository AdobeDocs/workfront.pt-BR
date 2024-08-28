---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Reverter um pacote de promoção de ambiente
description: O recurso de promoção de ambiente tem como objetivo fornecer a capacidade de mover objetos relacionados à configuração de um ambiente para outro. Saiba como reverter um pacote de promoção instalado de um ambiente de destino.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 84a72ab4547a582707351948052fdd59cc57a9d5
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Reverter um pacote de promoção de ambiente

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Depois de instalar um pacote, você pode revertê-lo. Isso remove as alterações feitas pelo pacote no ambiente de destino e restaura os objetos afetados às configurações anteriores.

Você pode reverter um pacote promocional em 24 horas após sua instalação. Após 24 horas, a funcionalidade de reversão não estará mais disponível para essa instalação.

## Requisitos de acesso

Você deve ter o seguinte:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plano</strong>
   </td>
   <td> <p>Novo: Prime ou Ultimate</p><p>Ou</p><p>Atual: não disponível</p>
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenças</strong>
   </td>
   <td> <p>[!UICONTROL Padrão]</p><p>Ou</p><p>Atual: não disponível</p>
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

* Um pacote de promoção de ambiente deve ser instalado antes de ser revertido.

  Para obter instruções, consulte [Instalar um pacote de promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


## Determinar se a implantação de um pacote específico pode ser revertida

Para saber se uma implantação de pacote específica pode ser revertida, considere o seguinte:

* Devem ter passado menos de 24 horas desde a instalação do pacote.
* Somente a implantação de pacote mais recente pode ser revertida.
* Uma implantação com falha pode ser revertida.
* Não é possível reverter reversões.


## Reverter um pacote de promoção de ambiente instalado

1. Vá para o ambiente em que o pacote foi instalado.
1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. Selecione **Promoção do ambiente** na navegação à esquerda.
1. Selecione o pacote que você deseja reverter e clique em **Implantações**.
1. Passe o mouse sobre a implantação (instalação) que você deseja reverter e clique em Reverter quando ela aparecer à direita da linha dessa implantação.

   Ou

   Clique na implantação que você deseja reverter e em **Reverter pacote**, no canto superior direito da tela.

   >[!IMPORTANT]
   >
   >A implantação deve ter ocorrido menos de 24 horas antes de ser revertida. Instalações com mais de 24 horas não podem ser revertidas.

1. (Opcional) Na área Visualização da reversão, visualize as alterações que ocorrerão quando a implantação for revertida.
1. Clique em **Reverter** no canto superior direito da tela.







