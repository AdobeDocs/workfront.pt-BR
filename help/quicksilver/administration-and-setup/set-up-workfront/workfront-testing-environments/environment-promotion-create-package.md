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
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 839b53afb9233ef0e36e981b243c8b2593b45f0f
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Criar ou editar um pacote de promoção de ambiente

Você deve criar um pacote no ambiente do qual deseja copiar os objetos **de**. Por exemplo, se você estiver configurando um projeto no ambiente Personalizar atualização da sandbox e promovendo-o para o ambiente Produção, será necessário criar o pacote no ambiente Personalizar atualização da sandbox.

>[!IMPORTANT]
>
>Se sua sandbox de atualização personalizada for atualizada enquanto você estiver configurando o objeto para promoção de ambiente, essa configuração será perdida na atualização. Recomendamos que você não atualize sua sandbox de atualização personalizada a menos que todos os objetos e pacotes de promoção de ambiente pendentes tenham sido promovidos com êxito.

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

## Criar um pacote

1. Vá para o ambiente em que deseja criar o pacote. Este é o ambiente do qual você está copiando objetos **de**.
1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. Selecione **Sistema** na navegação à esquerda e **Promoção do ambiente**.
1. Clique em **Criar Pacote**.

   A página Novo pacote de promoção é aberta.

1. No campo **Nome do pacote**, digite um nome para o pacote.
1. No campo **Descrição**, insira uma descrição para este pacote.
1. Para adicionar um objeto ao pacote, na navegação à esquerda, selecione o tipo de objeto que deseja adicionar.
1. Selecione um ou mais objetos na lista exibida ou digite o nome na barra de pesquisa e selecione o objeto quando ele aparecer na lista. Você pode selecionar mais de um objeto na lista.

   A lista inclui até 500 objetos do tipo selecionado. Para localizar um objeto que não esteja na lista, use a barra de pesquisa.
1. Clique em **Adicionar (X Objetos)** para adicionar os objetos selecionados ao pacote.

   >[!INFO]
   >
   >**Exemplo**
   >
   >Se você selecionou três projetos para adicionar ao projeto, o botão dirá **Adicionar 3 projetos**.

   Os objetos adicionados aparecerão na área Conteúdo do Package à direita da página.

1. Para adicionar outro tipo de objeto, repita as etapas 7 a 9.
1. (Opcional) Para remover um objeto do pacote, passe o mouse sobre o objeto na área Conteúdo do pacote, em seguida, clique no X ao lado do objeto.
1. Depois de ter adicionado todos os objetos desejados ao pacote, clique em **Salvar e Fechar** para salvar o pacote sem montá-lo.

   Ou

   Clique em **Salvar e reunir** para salvar e reunir o pacote.

   >[!NOTE]
   >
   >* Os botões Salvar e Fechar e Salvar e Reunir estarão disponíveis se um pacote tiver um nome com cinco ou mais caracteres e pelo menos um objeto adicionado a ele.
   >* Não é possível montar um pacote que esteja em um status instalável, como Teste ou Ativo.

## Editar ou reunir um pacote existente

Um pacote deve estar com o status `DRAFT` para ser editado.

1. Vá para o ambiente em que deseja editar o pacote. Este é o ambiente em que o pacote foi criado originalmente.
1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. Selecione **Sistema** na navegação à esquerda e **Promoção do ambiente**.
1. Selecione o pacote na lista exibida.
1. (Condicional) Para ver pacotes desabilitados, habilite a opção **Mostrar pacotes desabilitados**.
1. (Opcional) Para exibir o conteúdo, incluindo todos os objetos e seus subobjetos, clique na seta suspensa ao lado do tipo de objeto na seção **Conteúdo**.
1. (Opcional) Para exibir instalações anteriores e tentativas de instalação deste pacote, clique em **Implantações**.
1. (Opcional) Para editar o pacote, clique em **Editar Pacote** no canto superior direito da tela.
Um pacote deve estar com o status `DRAFT` para ser editado. Para mover o pacote para o status `DRAFT`, no campo **Status**, selecione `Draft`. Você pode continuar editando o pacote.
1. Para instalar o pacote, clique em **Instalar** no canto superior direito da tela.

   Para obter instruções sobre como instalar um pacote, consulte [Instalar um pacote de promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).

## Criar um pacote a partir de uma comparação de objetos

Você pode criar um pacote diretamente de uma comparação de objetos.

1. Crie uma comparação de objetos, conforme descrito em [Comparar objetos entre ambientes](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).
1. Na comparação gerada, selecione os objetos que deseja incluir no pacote.
1. Clique em **Criar pacote** no canto superior direito da tela.
1. Insira um nome e uma descrição para o pacote.
1. Clique em **Criar pacote** na janela Criar pacote.

   O pacote é gerado.
