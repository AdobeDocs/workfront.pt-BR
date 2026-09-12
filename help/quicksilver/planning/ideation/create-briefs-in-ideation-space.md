---
title: Criar resumos no espaço de ideação
description: Este artigo descreve como você pode fazer um brainstorming e criar estratégias no espaço de ideação para criar resumos. É possível exportar resumos de ideação concluídos para um arquivo ou para o Workfront Planning para criar ou atualizar registros.
feature: Workfront Planning
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 1%

---


# Criar resumos no espaço de ideação

<!-- add to TOC and miniTOC-->

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente como parte do programa **Espaço de ideação Beta**. </span>

<span class="preview">Para obter mais informações, consulte [Introdução ao Espaço de ideação do Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Usando o Espaço de ideação, um novo recurso do Adobe Workfront Planning, você pode transformar resumos em registros do Planning. Os resumos exportados criam novos registros ou atualizam os existentes.

Este artigo descreve como você pode fazer um brainstorming e criar estratégias no espaço de ideação para criar resumos. Para criar ou atualizar registros, exporte os resumos de ideação concluídos para um arquivo ou para o Workfront Planning.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p></li>
Ou
<li><p>Qualquer pacote do Planning quando adquirido como um produto independente</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Produtos adicionais</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workflow</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> 
   <ul>
   <li><p>Você deve adicionar um Workflow e um tipo de licença do Planning ao nível de acesso quando tiver um Workflow e um pacote do Planning</p>   </li>
   <li><p>A configuração Desativar espaço de ideação no seu nível de acesso deve ser desmarcada</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Permissões do Contribute ou superior para o espaço de trabalho e tipo de registro ao qual você deseja adicionar registros </p>
      <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
      <p>Exibir permissões para objetos do Workfront para adicioná-los a resumos <!--not sure if this is available--></p>
      <p>Permissões do editor no espaço de ideação para criar resumos</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Funções de usuário do Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Qualquer função de usuário do GenStudio para acessar Campanhas, Produtos e Personalidades</li>
   <li>GenStudio System Manager para acessar as Ativações <!--and Events--></li></ul>
   Para obter informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funções e permissões de usuário</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Criar resumos do espaço de ideação

1. Comece no Workfront Planning e crie ou edite um registro usando o espaço Ideação.

   Para obter mais informações, consulte [Criar registros de Planejamento a partir de resumos de espaço de ideação](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).
1. Quando o **Espaço de ideação** for aberto, use o prompt fornecido para descrever o tipo de resumo que você deseja criar.

   Por exemplo, digite &quot;Create a back-to-school campaign for K-12 student to run through the month of ago, for parent and professors in the US&quot; (Crie uma campanha de volta às aulas para os alunos do ensino fundamental que durará o mês de agosto para os pais e os professores nos EUA).  Para tornar o resumo o mais completo possível, indique quantas informações você tem disponíveis para que tipo de campanha, a linha do tempo, as partes interessadas e outros detalhes.

1. Clique em **Iniciar idealização**.

   Depois de aberto, o agente do espaço de ideação passa pelas seguintes etapas:

   1. **Assimilação e síntese de dados**: extrai informações relevantes de fontes conectadas. Por exemplo:

      * Tipos de registro existentes ou o tipo de registro existente a partir do qual você iniciou.
      * Documentos recentes carregados no espaço de ideação.
      * Informações da Web que correspondem aos critérios de solicitação.

        >[!TIP]
        >
        >A configuração de pesquisa na Web deve estar ativada para que a IA possa procurar informações na Web.\
        >Para obter informações, consulte a seção [Configurar o espaço de ideação](#configure-the-ideation-space)neste artigo.
        >
   1. **Definição de público-alvo**: identifica ou recomenda parâmetros de público-alvo com base em padrões históricos
   1. **Enquadramento da estratégia**: estrutura a narrativa estratégica da campanha
   1. **Ideação de mensagens e conceito**: gera opções de mensagem iniciais e direções de conceito criativas
   1. **Breve geração e entrega do planejamento**: produz um resumo estruturado que é alimentado no espaço de trabalho do Workfront Planning

      Quando o agente de ideação finaliza o processo de coleta de todas as informações, as seguintes coisas ocorrem:

      * Cinco cartões são criados e organizados por informações relevantes e semelhantes.

        Os cartões são intitulados usando várias etapas na criação do registro solicitado, para facilitar o reconhecimento.

        Por exemplo, eles podem ser nomeados como:

        * Plano
        * Linha do tempo
        * Segmentos
        * Mecânica
        * Mensagens

      Os títulos dos cartões são personalizados para cada cartão na ideação.

      * As placas são colocadas dentro do mesmo quadro, indicando que este é o resultado de uma ideação.

      * Um resumo é criado e exibido em uma imagem de pré-visualização no canto inferior esquerdo do espaço de ideação. <!--add screen shot??-->

      O resumo contém campos sugeridos que o sistema considera pertinentes às ideias que você está explorando.

1. (Opcional) Clique no ícone ![](assets/more-information-icon.png) da **Ajuda** no canto superior direito para obter uma lista de atalhos de teclado para ajudá-lo a navegar pelo espaço de ideação.

1. (Opcional) Clique em **Fontes** na parte inferior de cada cartão para entender de onde as informações foram coletadas.

   As informações podem ser importadas do Workfront Planning ou da Web.
1. (Opcional) Use os ícones com miniatura para cima ou com miniatura para baixo em um cartão para fornecer feedback.<!--is this still available??-->
1. Clique em um cartão ou no quadro que contém todos os cartões e, em seguida, clique em **Adicionar ao resumo** para adicionar suas informações ao resumo.

   O Workfront corresponde cada informação ao campo que encontra com maior probabilidade de armazená-la.

   Por exemplo, linhas do tempo são adicionadas a campos do tipo data, descrições a campos do tipo parágrafo.
   1. (Condicional) Clique em um cartão e em **Pedir IA para ...** para obter ideias sobre a próxima etapa antes de adicionar as informações ao resumo. As respostas estão no contexto das informações de cada cartão.
   1. Clique no ícone **Adicionar documentos** ![Ícone Adicionar documentos](assets/add-documents-in-ideation-space.png) no canto superior esquerdo do espaço de ideação para carregar documentos para o espaço. É possível adicionar novos documentos ou documentos que já foram adicionados ao espaço anterior.

      >[!TIP]
      >
      >A configuração Documentos deve estar ativada para poder acessar documentos e carregá-los no espaço.
      >Para obter informações, consulte a seção [Configurar o espaço de ideação](#configure-the-ideation-space) neste artigo.
      > 
   1. Clique no ícone **Adicionar cartão de Taxonomia WF** ![Adicionar do Workfront Planning](assets/add-from-wf-planning-on-ideations-space.png) <!--send this tooltip to be revised--> e selecione um tipo de registro conectado e, em seguida, um registro de cada tipo para adicionar as informações desse registro ao tipo de registro selecionado.

      Um cartão é criado para o registro selecionado para ser adicionado ao espaço. O tipo de registro é exibido no canto superior esquerdo do cartão do registro.
   1. (Opcional) Clique no menu **Mais** ![Mais menus](assets/more-menu.png) e clique em **Exibir no Workfront**.

      A página de detalhes do registro é aberta em outra guia do navegador no Workfront Planning.
   1. (Opcional) Selecione o quadro de ideação ou um cartão, clique no ícone Excluir e clique em Excluir para confirmar. A placa é removida do espaço de ideação.

      Ao excluir cartões correspondentes a um documento armazenado ou a um registro, os itens são removidos do espaço de ideação, mas permanecem em seus respectivos aplicativos.

1. (Opcional) Use a caixa **Pergunte qualquer coisa** no canto inferior direito a qualquer momento para refinar sua ideia.

   Por exemplo, digite `regenerate` para que um cartão específico faça com que a IA o refaça usando o contexto atualizado. O espaço de ideação reexecuta suas etapas de raciocínio (pesquisa, síntese, citação) e atualiza os cartões afetados.

1. (Opcional) Na caixa **Pergunte qualquer coisa**, faça uma nova pergunta para iniciar uma nova ideação.

   Um novo conjunto de cartões é gerado, depois que o espaço executa novamente seus passos de raciocínio.

1. (Opcional) Clique em um dos conectores roxos de qualquer conjunto de cartões de ideação e clique no ícone **Copiar para barra de prompt** para executar novamente o raciocínio da ideação.

   ![Ícone Copiar para a barra de prompts](assets/copy-to-prompt-bar-icon-highlighted.png)

1. (Opcional) Clique nos ícones **Desfazer** ou **Refazer** ![Desfazer e refazer ícones](assets/undo-redo-icons.png) na parte superior da página para cancelar ou reverter uma ação.
1. Reduza o zoom para ver a imagem completa: seu objetivo original de campanha, todos os cartões de conceito gerados por IA com citações, documentos adicionais, os registros reais do Workfront Planning que você obteve (produtos, personas etc.). O cartão de resumo **Brief** no canto inferior esquerdo puxa tudo junto.

1. Clique na imagem de visualização breve no canto inferior esquerdo, revise o resumo e clique em uma das seguintes opções:

   * **Exportar para arquivo**. Você pode exportar o resumo para os seguintes tipos de arquivo:

     * PDF
     * Palavra
     * PowerPoint (com ou sem um modelo)
   * **Exportar para o Workfront Planning**. A exportação substitui todos os dados de campo existentes no registro no Workfront Planning.

   Isso finaliza a criação do registro com as informações adicionais e o adiciona ao tipo de registro selecionado originalmente.

   Para obter mais informações sobre a atualização de registros do Planning usando resumos, consulte a seção &quot;Considerações sobre o uso do espaço de ideação para criar registros&quot; no artigo [Criar registros do Planning a partir de resumos do espaço de ideação](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).


## Configurar o espaço de ideação

Existem controles para o espaço de ideação que configuram o que você vê na tela, bem como ajudam a navegar pelo espaço.

1. Clique no ícone **Configurações** ![Configurações](assets/setting-icon.png) para controlar de onde a IA extrai informações e escolha um dos **Tipos de Source** a seguir:

   * **Documentos** — documentos carregados no espaço selecionado
   * **Pesquisa na Web** — pesquisa na Web externa
   * **CJA** — Adobe Customer Journey Analytics

1. Clique em **Salvar**.

1. Clique no ícone da **Ajuda** ![Ícone da Ajuda](assets/more-information-icon.png) para examinar os atalhos de teclado que você pode usar para navegar pelo espaço de ideação ou selecionar um valor de zoom diferente.

   Escolha entre os seguintes níveis de zoom:

   * Nível de zoom 100%
   * Nível de Zoom 200%
   * Zoom para ajustar

   Ou use um dos seguintes atalhos para navegar na página:

   | Ação | Atalho |
   |---|---|
   | Aumentar/diminuir o zoom | Ctrl/⌘ + / - |
   | Zoom para ajustar / ajustar a seleção | — |
   | Aplicar zoom ao cursor | Ctrl/⌘ + rolagem |
   | Deslocar a tela | Espaço pressionado + arrastar |
   | Mostrar/ocultar grade de pontos | G |

1. Clique no ícone Pesquisar para pesquisar itens no espaço de ideação e clique em quando ele for exibido na lista para navegar até ele.








