---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Criar ou editar um pacote de promoção de ambiente
description: O recurso de promoção de ambiente tem como objetivo fornecer a capacidade de mover objetos relacionados à configuração de um ambiente para outro. Saiba como criar um pacote de promoção de ambiente que você pode instalar em um ambiente diferente.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 6497bfa1bf8236baaf4beee38078426b754e1241
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Criar ou editar um pacote de promoção de ambiente

## Criar um pacote

1. Vá para o ambiente em que deseja criar o pacote. Este é o ambiente no qual você está copiando objetos **de**.
1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Configuração]** ![Ícone de Configuração](/help/_includes/assets/gear-icon-setup.png).
1. Selecionar **Sistema** na navegação à esquerda, selecione **Promoção do ambiente**.
1. Clique em **Criar pacote**.

   A página Novo pacote de promoção é aberta.

1. No **Nome do pacote** insira um nome para o pacote.
1. No **Descrição** insira uma descrição para este pacote.
1. Para adicionar um objeto ao pacote, clique em **Adicionar objetos** no painel de navegação esquerdo e selecione o tipo de objeto que deseja adicionar.
1. Selecione um ou mais objetos na lista ou digite o nome na barra de pesquisa e selecione o objeto quando ele aparecer na lista. Você pode selecionar mais de um objeto na lista.
1. Clique em **Adicionar (X Objetos)** para adicionar os objetos selecionados ao pacote.

   >[!INFO]
   >
   >**Exemplo**
   >
   >Se você selecionou três projetos para adicionar ao projeto, o botão diz **Adicionar 3 projetos**.

   Os objetos adicionados aparecerão na área Conteúdo do Package à direita da página.

1. Para adicionar outro tipo de objeto, repita as etapas 7 a 9.
1. (Opcional) Para remover um objeto do pacote, passe o mouse sobre o objeto na área Conteúdo do pacote, em seguida, clique no X ao lado do objeto.
1. Depois de ter adicionado todos os objetos desejados ao pacote, clique em **Salvar e fechar** para salvar o pacote sem montá-lo.

   Ou

   Clique em **Salvar e reunir** para salvar e montar o pacote.

   >[!NOTE]
   >
   >* Os botões Salvar e Fechar e Salvar e Reunir estarão disponíveis se um pacote tiver um nome com cinco ou mais caracteres e pelo menos um objeto adicionado a ele.
   >* Não é possível montar um pacote que esteja em um status instalável, como Teste ou Ativo.

## Editar ou reunir um pacote existente

1. Vá para o ambiente em que deseja criar o pacote. Este é o ambiente no qual você está copiando objetos **de**.
1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Configuração]** ![Ícone de Configuração](/help/_includes/assets/gear-icon-setup.png).
1. Selecionar **Sistema** na navegação à esquerda, selecione **Promoção do ambiente**.
1. Selecione o pacote na lista exibida.
1. (Condicional) Para ver pacotes desativados, ative a variável **Mostrar pacotes retirados** opção.
1. (Opcional) Para exibir o conteúdo, incluindo todos os objetos e seus subobjetos, clique na seta suspensa ao lado do tipo de objeto na **Conteúdo** seção.
1. (Opcional) Para exibir instalações anteriores e tentativas de instalação deste pacote, clique em **Implantações**.
1. (Opcional) Para editar o pacote, clique em **Editar pacote** no canto superior direito da tela.
1. Para instalar o pacote, clique em **Instalar** no canto superior direito da tela.

   Para obter instruções sobre como instalar um pacote, consulte [Instalar um pacote de promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
