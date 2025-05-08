---
navigation-topic: search
title: Pesquisar [!DNL Adobe Workfront]
description: Você pode localizar itens facilmente em  [!DNL Adobe Workfront]  procurando por eles quando não conseguir se lembrar de sua localização exata.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: b04d09d1244a7d7abef8aaddb62dbdf7124bfde8
workflow-type: tm+mt
source-wordcount: '1673'
ht-degree: 1%

---

# Pesquisar [!DNL Adobe Workfront]

Você pode localizar itens facilmente em [!DNL Adobe Workfront] procurando por eles quando não conseguir se lembrar da localização exata.

Você pode ver a caixa [!UICONTROL Pesquisa] no canto superior direito de qualquer página em [!DNL Workfront].

![Ícone de pesquisa na barra de navegação](assets/search-globalnavigationbar-350x62.png)

Você deve ter permissões para Exibir um objeto antes de encontrá-lo em uma pesquisa. Por esse motivo, os resultados da pesquisa variam de usuário para usuário.

## Requisitos de acesso

+++ Expanda esta seção para exibir o acesso necessário para executar as etapas deste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Acesso de [!UICONTROL View] ao tipo de objeto </p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Você deve ter permissões para Exibir um objeto antes de encontrá-lo em uma pesquisa.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

+++

## Entender a pesquisa

* [[!UICONTROL Objetos disponíveis para pesquisa]](#objects-available-for-search)
* [[!UICONTROL Campos disponíveis para pesquisa]](#fields-available-for-search)

### Objetos disponíveis para pesquisa

Você pode pesquisar os seguintes objetos no Workfront:

* Projetos
* Tarefas
* Problemas
* Relatórios
* Usuários
* Modelos
* Documentos
* Portfólios
* Programas
* Painéis
* Empresas
* Notas

### Campos disponíveis para pesquisa

Os campos disponíveis para pesquisa são baseados no tipo de pesquisa: Básica ou [!UICONTROL Pesquisa Avançada].

* **Pesquisa Básica**: ao procurar objetos em uma Pesquisa Básica, o [!DNL Workfront] procura texto que possa conter suas palavras-chave nos seguintes campos:

   * Nomes de objetos
   * Descrições
   * Campos de dados personalizados
   * Atualizações
   * Nomes de documentos (em pesquisas de documentos específicas e em uma Pesquisa básica)

  Para obter mais informações sobre a Pesquisa Básica no [!DNL Workfront], consulte [Pesquisa Básica](#basic-search) neste artigo.

* **[!UICONTROL Pesquisa avançada]**: em uma [!UICONTROL Pesquisa avançada], você pode configurar filtros para campos de pesquisa não disponíveis na Pesquisa básica. Portanto, a [!UICONTROL Pesquisa Avançada] permite pesquisar qualquer campo no objeto.

  Para obter mais informações sobre a [!UICONTROL Pesquisa Avançada], consulte a [Pesquisa Avançada](#advanced-search) neste artigo.

>[!NOTE]
>
>Para executar uma [!UICONTROL Pesquisa Avançada], você deve selecionar a opção [!UICONTROL Pesquisa Avançada] ao iniciar sua pesquisa. Você não pode refinar uma Pesquisa Básica em uma [!UICONTROL Pesquisa Avançada].

## Compreender as limitações de [!DNL Workfront] pesquisas

Considere as seguintes limitações ao usar a [!UICONTROL Pesquisa] em [!DNL Workfront]:

* As pesquisas não diferenciam maiúsculas de minúsculas
* [!DNL Workfront] não corrige ou entende erros de digitação
* A pesquisa em [!DNL Workfront] não oferece suporte a Curingas
* A pesquisa em [!DNL Workfront] oferece suporte a pesquisas de palavras parciais, mas não oferece suporte a pesquisas de subsequências de caracteres.\
   Por exemplo, a palavra-chave de pesquisa &quot;stand&quot; retornaria resultados incluindo a palavra &quot;standard&quot;, mas não retornaria resultados incluindo a palavra &quot;understand&quot;.

## Pesquisar por várias palavras

Quando você inclui várias palavras em uma pesquisa e deseja localizar somente objetos que correspondam a todas as palavras na caixa Pesquisar, é possível digitar as palavras em qualquer ordem.

Por exemplo, pesquisar por &quot;Demonstração de marketing&quot; (sem aspas) encontra objetos com os seguintes nomes:

* Demonstração de marketing
* Marketing de demonstração
* Demonstração da análise de mercado de janeiro

Ele também encontra objetos que podem ter &quot;Marketing&quot; no nome e &quot;Demo&quot; na descrição.

No entanto, você pode fazer o seguinte na caixa [!UICONTROL Pesquisar] para ajustar os resultados da pesquisa exibidos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Incluir aspas</td> 
   <td> <p>Inserir palavras na ordem correta entre aspas duplas permite localizar somente objetos que possuem uma correspondência exata.<br>Por exemplo, pesquisar por "Demonstração de marketing" (com aspas) localiza objetos com os seguintes nomes:</p> 
    <ul> 
     <li> Demonstração de marketing</li> 
     <li> Demonstração de marketing de janeiro</li> 
     <li>Plano de demonstração de marketing</li> 
    </ul> <p>No entanto, essa pesquisa não localizaria um objeto com o nome "Demo Marketing".</p> </td> 
  </tr> 
  <tr> 
   <td>Incluir OR</td> 
   <td> <p>A conexão de palavras por "OR" (sem aspas) permite localizar somente objetos que correspondam a pelo menos uma das palavras na caixa [!UICONTROL Pesquisa]. Essas palavras podem ser inseridas em qualquer ordem.<br>Por exemplo, pesquisar por "Marketing OU Demonstração" (sem aspas) localiza objetos com os seguintes nomes:</p> 
    <ul> 
     <li> Demonstração da análise de mercado</li> 
     <li>Demonstração da análise de mercado de janeiro</li> 
     <li>Demonstração</li> 
     <li>Análise de mercado</li> 
    </ul> <p>Observação: "OR" deve estar em maiúsculas. Caso contrário, será interpretada como outra palavra na frase que você está procurando.</p> </td> 
  </tr> 
  <tr> 
   <td>Incluir E</td> 
   <td> <p>A conexão de palavras por "AND" (sem aspas) permite localizar somente objetos que correspondam a todas as palavras na caixa [!UICONTROL Search]. Essas palavras podem ser inseridas em qualquer ordem.<br>Por exemplo, pesquisar por "Marketing E Demonstração" (sem aspas) localiza objetos com os seguintes nomes:</p> 
    <ul> 
     <li>Demonstração de marketing</li> 
     <li>Marketing de demonstração</li> 
     <li>Demonstração da análise de mercado de janeiro</li> 
    </ul> <p>Observação: "AND" deve estar em maiúsculas. Caso contrário, será interpretada como outra palavra na frase que você está procurando. Da mesma forma, incluir "&amp;" (sem aspas) pesquisa somente os objetos que incluem o caractere E comercial.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Usar Pesquisa em [!DNL Workfront]

O [!DNL Workfront] apresenta dois tipos de pesquisas: básica e avançada. Use a Pesquisa básica se quiser encontrar palavras-chave em campos de objeto comuns, como nome ou descrição. Use a [!UICONTROL Pesquisa Avançada] se desejar usar filtros para pesquisar outros campos de objeto.

* [Pesquisa Básica](#basic-search)
* [Busca Avançada](#advanced-search)

### Pesquisa Básica

Uma Pesquisa básica permite procurar palavras-chave em todos os objetos no sistema ou em apenas um objeto por vez (como projetos). [!DNL Workfront] procura essas palavras-chave em alguns campos específicos. Você pode refinar os resultados da pesquisa com base em outros campos específicos de objeto selecionados por [!DNL Workfront].

Para obter uma lista dos campos específicos pesquisados na Pesquisa Básica, consulte [Campos disponíveis para pesquisa](#fields-available-for-search) neste artigo.

>[!NOTE]
>
>Para executar uma [!UICONTROL Pesquisa Avançada], você deve selecionar a opção [!UICONTROL Pesquisa Avançada] ao iniciar sua pesquisa. Você não pode refinar uma Pesquisa Básica em uma [!UICONTROL Pesquisa Avançada].

* [Executar uma pesquisa básica](#perform-a-basic-search)
* [Refinar uma pesquisa básica](#refine-a-basic-search)

#### Executar uma pesquisa básica

Você pode fazer uma Pesquisa básica de uma das seguintes maneiras:

* Em todos os objetos do sistema (pesquisa geral).
* Em apenas um objeto por vez (pesquisa específica de objeto).

Para executar uma Pesquisa Básica:

1. Clique no ![ícone de Pesquisa](assets/search-icon.png) da lupa, no canto superior direito da página. Você também pode digitar **[!UICONTROL ALT + /]** ou **[!UICONTROL Option + /]** para abrir o menu [!UICONTROL Search].

1. (Opcional) Para procurar um objeto específico, clique no menu suspenso **[!UICONTROL Todos]** e selecione o objeto que deseja procurar.

   ![Pesquisar por tipo de objeto](assets/search-objecttype.png)

1. Na caixa **[!UICONTROL Pesquisar]**, comece digitando as informações que você está procurando.
Para obter informações sobre quais campos são pesquisados em [!DNL Workfront], consulte [Entender a Pesquisa](#understand-search).
   ![Lista suspensa de pesquisa](assets/qs-search-drop-down-highlighted-350x234.png)

   À medida que você começa a digitar na barra de pesquisa, o [!DNL Workfront] faz recomendações com base no seu histórico de exibição e destaca a palavra-chave que você está procurando em azul.

1. Se o item que você está procurando for exibido no menu [!UICONTROL digitação antecipada], clique nele.

   Ou

   Pressione **[!UICONTROL Enter]** para executar uma pesquisa abrangente. Esta pesquisa consulta todo o banco de dados em vez dos itens visualizados mais recentemente.

   A página [!UICONTROL Resultados da Pesquisa] é aberta a partir da esquerda e cobre a maior parte da página anterior.

   Se você tiver realizado uma pesquisa geral, [!DNL Workfront] retornará resultados para qualquer objeto que corresponda ao termo de pesquisa em qualquer um dos campos pesquisados, conforme descrito em [Entender a Pesquisa](#understand-search). Os objetos que correspondem à pesquisa são exibidos em uma lista.

   >[!NOTE]
   >
   >Às vezes, as variações de uma palavra são exibidas na lista de itens encontrados.\
   >Por exemplo, pesquisar por &quot;marketing&quot; exibe objetos que contêm &quot;marketing&quot; ou &quot;marketing&quot; no nome.

1. (Opcional) Se sua pesquisa gerou muitos resultados, refine sua pesquisa conforme descrito em [Refinar uma Pesquisa Básica](#refine-a-basic-search).
1. (Opcional) Para retornar à página em que você estava antes da pesquisa, clique em **[!UICONTROL Fechar]** no canto superior direito.

>[!NOTE]
>
>A página [!UICONTROL Resultados da Pesquisa] permanece aberta apenas quando está em foco. Clicar fora da página ou abrir outra página fecha a página [!UICONTROL Resultados da Pesquisa].

#### Refinar uma pesquisa básica

Após executar uma Pesquisa Básica, conforme descrito em [[!UICONTROL Executar uma Pesquisa Básica]](#perform-a-basic-search), você pode refinar a pesquisa.

Use a barra de ferramentas à esquerda dos resultados da pesquisa para restringir as informações que você está procurando.

Para refinar uma pesquisa:

1. (Condicional) Se você tiver realizado uma pesquisa geral, selecione o objeto que estava procurando na lista de objetos no canto superior esquerdo dos resultados.
1. Localize os campos disponíveis para os objetos exibidos na pesquisa na barra de ferramentas à esquerda dos resultados.
Os valores de cada campo são exibidos, classificados por contagem, até dez valores para cada campo.
1. Clique dentro de qualquer um dos campos disponíveis para encurtar a lista de resultados.
As seleções feitas são destacadas em azul e os valores de campo que você não selecionar ficam ocultos.
Após selecionar cada novo valor, os resultados à direita são atualizados dinamicamente.

   ![Guia Pesquisa básica](assets/basic-search.png)

1. (Opcional) Clique nos valores selecionados para desmarcá-los e exibir todos os valores para cada campo novamente.

### [!UICONTROL Pesquisa avançada]

A [!UICONTROL Pesquisa Avançada] permite pesquisar usando campos e filtros não disponíveis para a Pesquisa Básica. Por exemplo, você pode pesquisar por projetos com uma Prioridade ou um Nome de proprietário de documento específico.

>[!NOTE]
>
>Para executar uma [!UICONTROL Pesquisa Avançada], você deve selecionar a opção [!UICONTROL Pesquisa Avançada] ao iniciar sua pesquisa. Você não pode refinar uma Pesquisa Básica em uma [!UICONTROL Pesquisa Avançada].

* [Usar [!UICONTROL Pesquisa Avançada]](#use-advanced-search)

#### Usar [!UICONTROL Pesquisa Avançada]

Você pode usar a [!UICONTROL Pesquisa avançada] para filtrar sua pesquisa com base em critérios específicos.\
Esse tipo de pesquisa é útil quando você não consegue se lembrar de uma palavra-chave associada a um objeto, mas conhece algumas informações específicas sobre esse objeto (por exemplo: Prioridade do projeto, Nome do proprietário do documento etc.).

Para executar uma pesquisa avançada:

1. No canto superior direito de qualquer página em [!DNL Workfront], clique no ícone **[!UICONTROL Pesquisar]** ![ícone Pesquisar](assets/search-icon.png). O menu [!DNL Search] é exibido.

1. Na parte inferior do menu [!UICONTROL Pesquisa], clique em **[!UICONTROL Pesquisa Avançada]**.\
   ![Pesquisa avançada](assets/qs-advanced-search-350x224.png)\
   A página [!UICONTROL Pesquisa Avançada] é aberta a partir da direita e cobre a maior parte da página anterior.

1. Selecione o tipo de objeto que você está procurando.\
   **[!UICONTROL Tarefas]** é selecionado por padrão.

   ![Objetos de pesquisa avançada](assets/advanced-search.png)

1. (Opcional) Digite uma palavra-chave no campo na parte superior da lista.
1. (Opcional) Ative **[!UICONTROL Filtrar os resultados]** para criar um filtro e refinar a pesquisa. Clique em **Aplicar** quando terminar.

1. Clique em **[!UICONTROL Pesquisar]**.\
   Uma lista de itens que correspondem à sua pesquisa é exibida à direita da barra de ferramentas [!UICONTROL Pesquisa avançada].

1. (Opcional) Para retornar à página em que você estava antes da pesquisa, clique em **[!UICONTROL Fechar]** no canto superior direito.

>[!NOTE]
>
>A página [!UICONTROL Resultados da Pesquisa] permanece aberta apenas quando está em foco. Clicar fora da página ou abrir outra página fecha a página [!UICONTROL Resultados da Pesquisa].
