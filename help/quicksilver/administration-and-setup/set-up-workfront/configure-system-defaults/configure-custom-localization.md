---
user-type: administrator
product-area: system-administration;setup
title: Configurar localização personalizada
description: A localização personalizada permite definir termos e frases personalizados em diferentes idiomas. O Workfront exibe esses termos no conjunto de idiomas nas configurações do navegador.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: b077c95d8bb795fcd7c0983c78b7533cb8167270
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 5%
---
# Configurar localização personalizada

{{highlighted-preview}}

A localização personalizada permite que você <span class="preview"> use a IA</span> para definir termos e frases personalizados em diferentes idiomas. O Workfront exibe esses termos no conjunto de idiomas nas configurações do Adobe Identity Management (IMS) do usuário.

Por exemplo, o rótulo &quot;Público-alvo&quot; pode ser localizado para a palavra alemã &quot;Zielgruppe&quot;. Qualquer usuário com o alemão selecionado como idioma principal do navegador verá a palavra &quot;Zielgruppe&quot; como um rótulo para qualquer campo rotulado como &quot;Público-alvo&quot; em inglês.

Você pode configurar traduções para vários idiomas. Os idiomas disponíveis no momento incluem:

* Chinês (tradicional)
* Chinês (simplificado)
* Francês
* Alemão
* Italiano
* Japonês
* Coreano
* Português (Brasil)
* espanhol

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Fluxo de trabalho Prime ou superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront para configurar traduções.</p>  </td> 
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações ao definir a localização

Considere o seguinte ao configurar a localização:

* Você pode configurar um termo para traduzir em vários idiomas.
* A localização se aplica a rótulos de campo personalizados (incluindo quando usados como um cabeçalho de coluna) e dicas de ferramentas.
* A localização personalizada pode se aplicar a mensagens geradas pelas Regras de Negócios, mas deve ser habilitada na Regra de Negócios.

  Para obter instruções, consulte [Habilitar localização em uma Regra de Negócios](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules) no artigo Criar e editar regras de negócios.

## Configurar traduções

As traduções são configuradas na área Configuração.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. Na área Configuração, clique em **Localização** no painel de navegação esquerdo.
1. Para adicionar uma nova tradução, clique em **Nova linha**.
1. Na coluna **Inglês**, digite o termo em inglês que deve ser traduzido.
1. Na coluna do idioma em que você deseja que o termo seja traduzido, insira o termo no idioma de destino.
1. (Opcional) Para traduzir a palavra em idiomas adicionais, adicione a tradução na coluna de idioma apropriada.
1. (Opcional) Para reordenar colunas de idioma, clique no cabeçalho de uma coluna que você deseja mover e arraste-a para o local desejado.
1. (Opcional) Para excluir as traduções de um termo, clique na caixa de seleção ao lado do termo e em **Excluir** na barra azul na parte inferior da página.

<div class="preview">

## Localizar texto personalizado não traduzido usando traduções de IA

Você pode usar a IA para localizar texto personalizado. Você seleciona o termo e os idiomas e pode aprovar as traduções antes de serem aplicadas.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. Na área Configuração, clique em **Localização** no painel de navegação esquerdo.
1. Na área Localização, selecione a guia **Texto personalizado não traduzido**.

   Uma lista de texto personalizado não traduzido é exibida. Isso inclui texto como rótulos de campo e mensagens de regras personalizadas.

1. Selecione um ou mais termos que deseja traduzir.
1. Na barra azul na parte inferior da tela, selecione **Traduzir com IA**.

   A janela Gerar traduções é aberta.

1. Clique nos idiomas para os quais você deseja traduzir o termo ou termos. Para selecionar rapidamente todos os idiomas, clique em **Selecionar tudo**.
1. (Opcional) Para fornecer orientações mais específicas para a tradução, insira instruções no campo &quot;Instruções para IA&quot;.
1. Clique em **Gerar**.

   A IA começa a gerar traduções.

   A janela Revisar traduções é aberta.

1. (Opcional) Para ajustar as traduções ou adicionar sua própria tradução, clique no quadrado apropriado da tabela e digite a tradução desejada.
1. Clique em **Salvar**.

## Traduzir um termo localizado para idiomas adicionais

Você pode traduzir um termo localizado anteriormente para novos idiomas usando IA ou fornecer sua própria tradução.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. Na área Configuração, clique em **Localização** no painel de navegação esquerdo.
1. Na área Localização, selecione a guia **Traduções**.

   Uma lista de termos traduzidos anteriormente e suas traduções são exibidas.

1. (Opcional) Para editar ou inserir diretamente uma tradução, clique na caixa apropriada na tabela e digite a tradução desejada.
1. Selecione os termos para os quais você deseja gerar traduções adicionais clicando nas caixas de seleção ao lado desses termos.
1. Na barra azul na parte inferior da página, clique em **Preencher com IA**.


   A janela Gerar traduções é aberta.

1. Clique nos idiomas para os quais você deseja traduzir o termo ou termos. Para selecionar rapidamente todos os idiomas, clique em **Selecionar tudo**.
1. (Opcional) Para fornecer orientações mais específicas para a tradução, insira instruções no campo &quot;Instruções para IA&quot;.
1. Clique em **Gerar**.

   A IA começa a gerar traduções.

   A janela Revisar traduções é aberta.

1. (Opcional) Para ajustar as traduções ou adicionar sua própria tradução, clique no quadrado apropriado da tabela e digite a tradução desejada.
1. Clique em **Salvar**.
1. (Opcional) Para excluir todas as traduções de um termo, clique na caixa de seleção ao lado do termo e em **Excluir** na barra azul na parte inferior da página.


</div>
