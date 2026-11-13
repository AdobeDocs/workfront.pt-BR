---
title: Usar a promoção de ambiente para o Adobe Workfront Planning
description: Você pode copiar espaços de trabalho, tipos de registro, campos e exibições do Workfront Planning de um ambiente Workfront para outro usando os recursos de Promoção do Ambiente. Em vez de reconstruir tudo manualmente, você monta a configuração em um pacote no ambiente de origem e o instala no ambiente de destino.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 58aec1c9c7dc45c5ecb6ad5d070a4e34b29c458c
workflow-type: tm+mt
source-wordcount: '1433'
ht-degree: 2%
---

# Usar a promoção de ambiente para o Adobe Workfront Planning

<!--add to TOC-->
<!--add to miniTOC-->


<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente para clientes selecionados em seus ambientes de Produção e Sandbox desde 12 de novembro de 2026. Posteriormente, os mesmos recursos também estarão disponíveis nos ambientes de produção, pré-visualização e sandbox para todos os clientes. </span>

<span class="preview">Para obter informações sobre versões, consulte [Versões do produto](/help/quicksilver/product-announcements/product-releases/product-releases.md) . </span>


>[!IMPORTANT]
>
>As informações neste artigo se referem ao Adobe Workfront Planning. Sua empresa deve adquirir um pacote adicional do Planning para acessar o Workfront Planning.
>
>A funcionalidade descrita aqui não estará disponível se sua organização tiver adquirido o Workfront Planning como um produto independente.
>
>Para obter informações gerais sobre o Workfront Planning, consulte [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>

<!--
Future - when they make it available in Planning: replace the above with this OR ... insert the snippet:

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning which your organization can purchase either as an Adobe Workfront package or a standalone product. 
>
>Not all capabilities included in the Planning package are available to Workfront Planning when it is purchased as a standalone product. 
>
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>For information about Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 
>
-->

Você pode copiar espaços de trabalho do Workfront Planning e seus objetos adicionais de um ambiente do Workfront para outro usando os recursos de Promoção do ambiente do Adobe Workfront.

Em vez de reconstruir tudo manualmente, você monta a configuração em um pacote no ambiente de origem e o instala no ambiente de destino.

O uso da Promoção do ambiente com o Planning é semelhante ao uso dela para o Workfront. Para obter mais informações, consulte a seção &quot;Promoção do ambiente&quot; no artigo [Ambientes de teste do Adobe Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md).

## Considerações sobre o uso da Promoção do ambiente com o Planning

* Você deve ser um administrador do Workfront para usar a Promoção do ambiente.
* Quando você copia um espaço de trabalho para outro ambiente, os seguintes objetos associados a esse espaço de trabalho também são importados por meio da promoção do ambiente:

  * Espaços de trabalho
  * Seções do Workspace
  * Tipos de registro
  * Campos
  * Exibições
  * Hierarquias
  * Configurações de compartilhamento para todos os objetos
  * Formulários de solicitação
  * Regras de negócios
  * Objetos conectados
  * Objetos dos quais o espaço de trabalho depende ou com os quais outros objetos são compartilhados, como grupos, equipes, funções de trabalho, empresas e usuários.

    Existem os seguintes cenários:

    * Se um objeto com o mesmo nome já existir no ambiente de destino, o Workfront sinalizará um conflito e você decidirá como tratá-lo.
    * Se uma equipe ou grupo com o qual um objeto é compartilhado não existir no ambiente de destino, a promoção o criará.
  <!--* Automations -- this is not promoted, for now, per Lilit -->
* Para cada objeto, você pode fazer o seguinte:

  * Criar como um novo objeto
  * Usar o objeto existente, mas criar com um novo nome
  * Substituir um objeto existente. A substituição substitui a configuração no público-alvo.
* Não é possível exportar os seguintes objetos:

  * Automações que pertencem ao espaço de trabalho que você está copiando
  * Registros
  * Campos que não pertencem aos espaços de trabalho exportados

* Os tipos de registro conectados entre espaços de trabalho não podem ser promovidos, a menos que já existam no ambiente de destino.

  Primeiro, recomendamos promover os espaços de trabalho que contêm os tipos de registro conectáveis entre espaços de trabalho e, somente depois disso, promover os espaços de trabalho que fazem referência a esses tipos de registro.

* A instalação pode levar alguns minutos. Você pode reverter uma instalação da página de resultados, se necessário.
* Recomendamos testar o processo antes de prosseguir, quando possível. Você pode instalar em uma sandbox ou ambiente de Pré-visualização antes de promovê-lo para produção.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Pacote de fluxo de trabalho do Prime ou Ultimate com um pacote do Prime ou Ultimate Planning</p>
<!--This might come later: <p>Prime or Ultimate Planning package when purchased as a standalone product</p>-->
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Planning</p></td> 
   <td><p>Planejamento padrão</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Você precisa ser um Administrador do sistema</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para espaços de trabalho</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Importar configuração do Planning usando a Promoção do Ambiente

Estas são as principais etapas para promover a configuração do Planning para outro ambiente:

* [Criar um pacote no ambiente de origem](#create-a-package-in-the-source-environment)
* [Prepare o pacote para a instalação](#make-the-package-ready-to-install)
* [Instalar o pacote no ambiente de destino](#install-the-package-in-the-target-environment)
* [Verifique os resultados](#verify-the-results)

Siga as instruções nas seções a seguir para copiar uma configuração do Planning entre dois ambientes do Workfront.

### Criar um pacote no ambiente de origem

1. Vá para um ambiente de origem em que a configuração desejada esteja estabelecida.
1. No ambiente de origem, clique no **Menu Principal** ![Menu Principal](assets/main-menu-shell.png) e vá para **Instalação** > **Sistema** > **Promoção do Ambiente**.
A lista **Pacotes de Configuração** mostra pacotes existentes com seu status, ambiente de origem e onde eles foram implantados.
1. Clique em **Criar pacote**.

   >[!TIP]
   >
   >Um pacote precisa de pelo menos um objeto para ser montado e instalado.
1. Na guia **Detalhes do Pacote**, digite um **Nome** e uma **Descrição** para o pacote. O ambiente de origem já está preenchido com o ambiente atual (origem).
1. Na lista de tipos de objetos à esquerda, selecione **espaço de trabalho do Planning**.
1. Procure o espaço de trabalho que deseja promover, marque a caixa de seleção correspondente e clique em **Adicionar espaço de trabalho do Planning**. O espaço de trabalho aparece em **Conteúdo do Pacote**.

   ![Workspace selecionado para promoção de ambiente](assets/workspace-selected-for-environment-promotion.png)
1. Clique em **Salvar e reunir**.

   A Workfront monta o pacote e adiciona uma entrada na guia **Atualizações** do pacote. É possível revisar o que o pacote inclui na guia Contents.
1. (Condicional e opcional) Clique em **Salvar e fechar** se desejar terminar mais tarde.
1. (Opcional) Clique em **Conteúdo** para examinar o conteúdo do pacote ou clique em **Implantações** para ver se este pacote foi implantado várias vezes.

   Continue a preparar o pacote para instalação.

### Prepare o pacote para a instalação

Antes de instalar o pacote no ambiente de destino, recomendamos testá-lo em um ambiente de teste.

1. Depois que o pacote terminar a compilação conforme descrito na seção anterior, clique em **Detalhes do Pacote** e em **Editar**, defina o **Status** como **Testes** e clique em **Salvar e fechar**.

   >[!TIP]
   >
   >Após a compilação do pacote, seu status é definido como **Rascunho**. O status **Ativo** não estará disponível até que você tenha testado o pacote primeiro.
1. (Recomendado) Clique em **Instalar** e escolha um dos ambientes de teste disponíveis para implantá-lo e testar a configuração.

   >[!TIP]
   >
   >O ambiente de Produção não está disponível como uma das opções quando o status é definido como **Testing**.

1. Depois de instalá-lo em um ambiente de teste, clique novamente em **Editar** e defina o **Status** como **Ativo**. Em seguida, clique em **Salvar e fechar**.

   >[!TIP]
   >
   >A instalação do pacote em um ambiente de teste é semelhante à instalação dele na Produção, conforme descrito na seção a seguir.

   Prossiga com a seção a seguir para instalar o pacote no ambiente de destino.


### Instalar o pacote no ambiente de destino

1. Na página do pacote, depois de verificá-lo, clique em **Instalar**.
1. Na lista **Ambiente de destino**, selecione o ambiente no qual implantar (por exemplo, seu ambiente de Produção) e clique em **Continuar**. O destino padrão é o ambiente atual.
1. Na página **Informações do pacote**, confirme o ambiente de origem e o ambiente no qual você está implantando.
1. Na seção **Mapeamento de objeto**, expanda cada agrupamento de objeto, como um **espaço de trabalho do Planning**, para examinar os objetos.

   >[!TIP]
   >
   >Grupos, equipes, funções, empresas e usuários podem ser exibidos aqui, se qualquer um dos objetos do espaço de trabalho for compartilhado com eles.

1. Para cada objeto, revise as colunas **Colisão** e **Status** e escolha uma **Ação de implantação** na lista. Escolha entre as seguintes opções:


   * **Criar novo**: adiciona o objeto ao destino. Use isto quando nenhuma colisão for detectada.
   * **Usar existente**: mapeia o objeto para um que já existe no destino, como um espaço de trabalho com o mesmo nome.
   * **Criar com novo nome**: adiciona o objeto com um nome especificado por você.
   * **Substituir**: substitui o objeto existente no destino pelo do pacote.

   >[!TIP]
   >
   >Se o sistema não encontrar um espaço de trabalho com a mesma ID, ele tentará encontrar uma correspondência com base no nome do espaço de trabalho.

1. (Opcional) Para alterar vários objetos de uma só vez, marque suas caixas de seleção, escolha uma ação na lista Ação de implantação na parte superior do grupo e clique em Aplicar à selecionada. Use os filtros acima da lista, como Mostrar apenas erros, para focalizar objetos específicos.
1. Resolva qualquer indicador de erro. Se você selecionar **Usar existente** para um objeto, também deverá selecionar o objeto para o qual ele é mapeado.  Caso contrário, o status mostrará um erro e **Implantar** permanecerá indisponível.
1. Clique em **Implantar** e depois em **Implantar** para confirmar.


   O Workfront mostra uma página de instalação com a mensagem **Este pacote está sendo instalado**. Isso pode levar alguns minutos.

   Quando a instalação for concluída, a página mostrará uma mensagem de sucesso, o ambiente no qual o pacote foi instalado e uma lista dos objetos instalados, com status para cada um, como **Usado existente** ou **Instalado (Criar novo)**.
1. (Opcional) Clique em **Reverter instalação**, se necessário, para reverter a instalação e remover a configuração do ambiente de destino.

   Continue a verificar os resultados da instalação.

### Verifique os resultados

1. Vá para o ambiente de destino > **Menu Principal** > **Planning** e localize o espaço de trabalho importado.
1. Abra os tipos e as exibições de registro para confirmar se os campos e o layout correspondem à origem. Os registros não são incluídos, portanto, as tabelas ficam vazias.


