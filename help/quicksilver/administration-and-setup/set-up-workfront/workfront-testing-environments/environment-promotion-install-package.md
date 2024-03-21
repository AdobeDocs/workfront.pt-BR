---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Instalar um pacote de promoção de ambiente
description: O recurso de promoção de ambiente tem como objetivo fornecer a capacidade de mover objetos relacionados à configuração de um ambiente para outro. Saiba como instalar um pacote de promoção de ambiente em um ambiente de destino.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 610469811a937fde70a938af829b156e69cca391
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# Instalar um pacote de promoção de ambiente


1. Vá para o ambiente em que deseja instalar o pacote. Este é o ambiente no qual você está copiando objetos **para**.
1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Configuração]** ![Ícone de Configuração](/help/_includes/assets/gear-icon-setup.png).
1. Selecionar **Sistema** na navegação à esquerda, selecione **Promoção do ambiente**.
1. Selecione o pacote na lista exibida.
1. Para instalar o pacote, clique em **Instalar** no canto superior direito da tela.
1. Mapeie cada objeto no pacote para o objeto correspondente no ambiente de destino.

   Para obter mais informações, consulte [Mapeamento](#mapping) neste artigo


## Mapeamento

Cada tipo de objeto é listado na navegação à esquerda e em um cartão. O cartão exibe objetos desse tipo e se esses objetos existem no ambiente de destino. Você pode determinar como esses objetos serão movidos para o ambiente de destino.

* Criar novo: crie um novo objeto no ambiente de destino. Se o objeto existir no ambiente de destino, você poderá criar um novo objeto com um novo nome. Se não existir no ambiente de destino, você poderá criar o objeto com um novo nome ou com o nome que o objeto tem no pacote.
* Usar existente: o objeto no pacote não está instalado e o objeto que já existia no ambiente de destino não é alterado.
* Substituir existente: (não disponível no momento) o objeto no pacote substitui o objeto existente no ambiente de destino.
* Não usar: o objeto no pacote não está instalado no ambiente de destino. Se você selecionar Do not use (Não usar), uma mensagem de erro será exibida detalhando como essa escolha afetará outros objetos ou campos.

Os valores padrão são `Create new` se o objeto não existir no ambiente de destino e `Use existing` se o objeto não existir no ambiente de destino. Você pode reverter para o mapeamento padrão clicando em **Redefinir para mapeamento padrão**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
