---
title: Práticas recomendadas de planejamento do Adobe Workfront
description: Como líder em operações de marketing, você pode usar o Adobe Workfront Planning para organizar trabalhos em todo o ciclo de vida de marketing para todas as suas equipes. Estas são algumas das práticas recomendadas que recomendamos ao iniciar o Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
source-git-commit: 1926500c76e4f9cfdac829f8d9f0cdfa6231e31d
workflow-type: tm+mt
source-wordcount: '3304'
ht-degree: 0%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Práticas recomendadas do Adobe Workfront Planning

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

Como líder em operações de marketing, você pode usar o Adobe Workfront Planning para organizar trabalhos em todo o ciclo de vida de marketing para todas as suas equipes.

Este artigo documenta algumas perguntas frequentes e práticas recomendadas que recomendamos ao iniciar o Workfront Planning.

## Práticas recomendadas de configuração

### Espaços de trabalho

Os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho. Um espaço de trabalho é uma coleção de tipos de registro usados por uma equipe e representa o ciclo de vida do trabalho da equipe.

Veja a seguir algumas perguntas frequentes sobre a configuração do Workfront Planning.

#### Como devo começar?

* ✅ Ao fazer logon no Planning pela primeira vez, siga nosso processo de integração no aplicativo que comunica claramente o valor do Planning e o orienta sobre como navegar e utilizar o produto de maneira eficaz. Isso garante que você entenda seus recursos e como começar seu trabalho com facilidade.
* ✅ Comece explorando nossos modelos de espaço de trabalho predefinidos para ideias de casos de uso semelhantes existentes. Você pode usar os tipos de registro e campos predefinidos incluídos em um modelo ou pode adicionar os seus próprios.
* ✅ Identifique os principais casos de uso que deseja resolver com o Workfront Planning. Por exemplo, a maioria das organizações quer melhorar a visibilidade das atividades estratégicas, o que pode incluir a criação de um &quot;Calendário de campanha&quot; melhor. Portanto, nesse caso de uso, você deve começar respondendo algumas perguntas:

   * Quem está pedindo isso?
   * Como eles chamam as coisas que querem colocar no calendário?
Campanhas? Táticas? Iniciativas? Atividades? Eventos?
   * Que tipos de perguntas eles desejam responder com este calendário?
   * Temos campanhas sobrepostas para o mesmo público-alvo?
   * Qual é o nosso orçamento para essa campanha, tática, atividade ou evento?

  As respostas a essas perguntas ditariam o que é necessário criar dentro do Workfront Planning.

  Além disso, considere que pode haver outros planejadores que não sejam usuários do Workfront no momento. Esses planejadores podem operar a partir de planilhas do Excel, documentos do Word, PowerPoints, etc. Considere como eles podem acessar suas informações no Workfront Planning.

* ✅ Para aproveitar ao máximo o Workfront Planning, considere substituir o uso de Portfólios e Programas no Workfront Workflow por alguma outra estrutura de nível superior no Workfront Planning.

  Atualmente, os clientes da Workfront representam seu trabalho estratégico por meio de portfólios e programas, em alguns casos como projetos de diferentes tipos. Com a introdução do Planning, todo esse trabalho estratégico deve ser tratado por meio de tipos de registro personalizados no Workfront Planning, enquanto o Workfront será centralizado em torno da fase de execução do trabalho representado como projetos e tarefas.


#### Quando devo criar um novo espaço de trabalho em vez de modificar um existente?

* ✅ Design para o menor volume de espaços de trabalho de nível de organização. Você pode criar espaços de trabalho para unidades de organização operacionais específicas, para corresponder à maneira exclusiva como cada unidade funciona.

  Ter as informações em uma única Workspace, para garantir que as relações entre todos os dados possam ser facilmente gerenciadas.

  Por exemplo, tente criar um único espaço de trabalho para todo o Marketing.

  Não há problema em criar um novo espaço de trabalho para uma equipe que tenha uma estrutura operacional completamente diferente:

  Por exemplo, um espaço de trabalho de **Desenvolvimento de Produto** deve ser diferente de um espaço de trabalho de **Marketing**.

* ⛔ Não crie espaços de trabalho exclusivos para cada equipe ou processo dentro de uma organização.

  A organização de marketing deve se esforçar para manter apenas um espaço de trabalho para manter a visibilidade e permitir que os dados sejam acumulados no nível de planejamento global.

  Evite criar espaços de trabalho semelhantes ou duplicados para equipes que seguem processos semelhantes (por exemplo, Marketing da EMEA versus Marketing da APAC), especialmente onde essas equipes podem realizar trabalhos que se enquadram em campanhas estratégicas comuns.

#### Como devo usar as Seções do Workspace?

* ✅ Crie e rotule seções para ajudar seus usuários a entender como você organiza seu ciclo de vida operacional.

  Por exemplo, você pode criar uma seção chamada **Registros principais**, na qual você coloca suas Campanhas, Táticas e Entregas no seu espaço de trabalho.
* ✅ Agrupe os tipos de registros &quot;curtir&quot;.

  Por exemplo, você pode criar uma seção chamada **Geografias**, que contém tipos de registros como: Região, País e Cidade.

### Tipos de registro

Os tipos de registro são os blocos de construção de uma Workspace do Workfront Planning. Você pode definir como os tipos de registro são interconectados.


#### Como devo definir tipos de registros no meu espaço de trabalho?

* ✅ Reserve algum tempo para identificar quais informações você precisa acompanhar (quais tipos de registros eu preciso) e como essas informações precisam estar conectadas. Converse com as partes interessadas que usarão o espaço de trabalho para considerar todas as suas necessidades. Você também pode criar seções personalizadas com diferentes tipos de registro para apresentar as informações de uma maneira muito útil.


* ⛔ Não duplique os tipos de registro por um período diferente (por exemplo, não crie tipos de registro separados para **Campanhas 2024** e **Campanhas 2025**).

  A criação de diferentes tipos de registro interrompe o fluxo de dados sempre que você deseja comparar dados em vários anos. As exibições de hoje são por tipo de registro; portanto, assim que o ano terminar, a exibição desse tipo de registro não mostrará mais os itens futuros. A prática recomendada é ter um tipo de registro para o tipo de trabalho e segmentar os dados usando filtros ou arquivando-os, se necessário.

#### Quando devo usar um campo de seleção única ou múltipla em vez de um tipo de registro vinculado?

* ✅ Adicione um novo tipo de registro se o objeto for usado em conexão com vários outros tipos de registro

  Por exemplo, uma Campanha pode ter uma conexão com vários Públicos do Target, e uma Tática pode ter uma conexão com um único Público do Target. Portanto, Campaign, Tactic e Audience devem ser tipos de registro em vez de campos de seleção múltipla.

* ✅ Adicione um novo tipo de registro se o objeto precisar armazenar valores de metadados adicionais que possam ser úteis em pesquisas

  Por exemplo, um tipo de registro de canal como **Email** pode armazenar uma lista de produtos finais de suporte, como metadados nativos ou como uma conexão com um tipo de registro **Produtos** independente.
* ⛔ Não adicione um novo tipo de registro se os dados armazenados forem relevantes apenas para um único tipo de registro.

  Por exemplo, um tipo de registro **Campanha** pode ter um campo de seleção única chamado **Tamanho da Campanha**, que só é relevante quando diretamente associado a uma campanha específica.

#### Como devo rotular meus tipos de registros?

* ✅ Crie e rotule tipos de registros que representem uma única construção ou substantivo, como **Campanhas**.
* ⛔ Não crie um tipo de registro que seja melhor representado como uma exibição.

  Por exemplo, **Calendário** é uma má opção para um tipo de registro, pois não é o tipo de registro em si, mas uma exibição de registros.

### Gerenciamento de campo

Os campos são atributos de tipos de registro e são exibidos como colunas na exibição de tabela. Você pode criar campos personalizados para tipos de registro e, em seguida, associar os campos aos registros do Workfront Planning para aprimorar as informações de registro.


#### Qual campo é recomendado para ser definido como Campo primário?


* ✅ Use valores de campo primário exclusivos para facilitar a localização e a &quot;seleção&quot; desses registros ao fazer conexões. 

  Ao fazer uma conexão, os usuários pesquisarão pelos valores no campo Primário e, se não forem exclusivos, os usuários não saberão qual escolher. 
* ⛔ Evite usar valores não exclusivos como campo principal, pois isso pode criar confusão para usuários que precisam pesquisar no campo principal ao usar o menu do seletor de conexões. 

#### Como devo usar fórmulas?

* ✅ Use os tipos de campo de Fórmula para reduzir a entrada manual. Quando você estiver inserindo informações com base em dados que já estão na sua visualização de tabela, talvez possa economizar algum esforço calculando essas informações automaticamente usando fórmulas.

#### Como devo começar a conectar os dados no meu espaço de trabalho?

* ✅ Criar conexões é um dos recursos mais eficientes do Workfront Planning. É possível conectar tipos de registro uns aos outros ou tipos de registro com tipos de objeto de outros aplicativos, como o Adobe Workfront (conexão com Projetos, Portfólios, Programas, Empresas e Grupos) e o Adobe Experience Manager Assets (conexão com ativos e pastas).

  Conectar tipos de objeto e registro fornece uma visão geral completa de como tudo em sua empresa está conectado.

  Por exemplo, você tem um tipo de registro **Campanha** e um tipo de registro **Táticas**, e pode criar uma conexão entre esses dois tipos de registro para ver quais **Táticas** estão associadas a uma **Campanha** específica.

  Após definir a conexão, todas as pessoas no espaço de trabalho podem começar a adicionar valores para **Campanhas** clicando duas vezes no campo de conexão, onde verão uma lista de todas as **Táticas** disponíveis. Isso permite descobrir rapidamente quais táticas precisam ser associadas às suas campanhas.

#### Como devo usar campos de pesquisa?

* ✅ Depois de estabelecer a conexão entre registros ou tipos de objeto, você pode conectar registros individuais uns aos outros e exibir campos do registro vinculado ou tipos de objeto em um registro do Workfront Planning. Você reduzirá o número de locais necessários para atualizar a mesma informação e garantir que eles correspondam perfeitamente.

  Por exemplo, uma vez que você tenha uma conexão entre um tipo de registro **Campanha** e um tipo de registro **Táticas**, você verá as informações do campo principal, mas quando adicionar campos de pesquisa, você poderá obter informações adicionais desse tipo de registro, como a **Data de inicialização** para essa **Tática**. Os dados desses campos de pesquisa são preenchidos automaticamente após a adição dos registros.

#### Qual tipo de campo é recomendado para URLs? 

* ✅ Use um campo de texto de linha única para adicionar dados de URL a um registro.

### Visualizações

#### Como decido o que deve ser uma visualização em vez de um tipo de registro?

* ✅Para itens que representam uma única construção ou substantivo (como **Campanhas**), crie um tipo de registro. 

* ⛔ Não crie um tipo de registro que seja melhor representado como uma exibição.

  Por exemplo, **Calendário** é uma má opção para um tipo de registro, pois não é o tipo de registro em si, mas uma exibição de registros. 

#### Devo ocultar ou excluir os campos que não são relevantes para mim?

* ✅ Ocultar a coluna em vez de excluí-la quando essas informações puderem ser relevantes para uma pessoa diferente usando o mesmo tipo de registro. Se você excluir o campo em uma exibição de tabela específica, esse campo também será excluído no restante das exibições desse registro, bem como em todos os outros locais dos quais esse tipo de registro está vinculado.

#### Como devo usar filtros e agrupamentos nas visualizações de tabela e linha do tempo?

* ✅ Use modos de exibição com filtros e agrupamentos para exibir um instantâneo do que você precisa ver. Você pode filtrar e agrupar os dados para ter uma maneira mais utilizável de entender o que está planejado. Você pode agrupar os registros por campos de metadados.

  Por exemplo, você pode ter uma exibição de linha do tempo para o seu tipo de registro de **Campanha**, que pode ser agrupada por **Públicos-alvo** e filtrada por **Data** para mostrar apenas o ano atual.

#### Por que não vejo todos os registros na minha exibição de linha do tempo?

* ✅ Lembre-se de definir dois campos de data para seus registros. Você pode criar uma visualização de linha do tempo somente quando tiver pelo menos dois campos de data associados a um tipo de registro. Alguns registros talvez não sejam exibidos na exibição de linha do tempo quando as datas de Início ou Término ou ambas não tiverem valores e quando a data de Início for posterior à data de Término.

#### Como devo usar as configurações de exibição da linha do tempo

* ✅ Defina as configurações do modo de exibição de linha do tempo, como o **Estilo de barra** e a **Cor**, para obter um modo de exibição mais visualmente enriquecedor. Você pode personalizar o **Estilo de barra** definindo se deseja ver uma miniatura com uma imagem significativa e adicionar mais campos para exibir na barra (por exemplo, **Proprietário** ou **Status**).

  Por padrão, você só vê o campo principal. Você também pode definir a cor da barra por valores de campo (por exemplo, é possível personalizar as cores das barras correspondendo-as ao campo Status ) ou pelo agrupamento aplicado. Por padrão, a cor corresponde à cor do tipo de registro.

  Somente as cores do tipo de registro ou os campos com opções associadas às cores podem afetar as cores das barras de registro na linha do tempo.

### Permissões e compartilhamento

Use o recurso de compartilhamento para conceder permissões apropriadas aos funcionários para exibições e espaços de trabalho.

#### Como devo gerenciar permissões para espaços de trabalho?

* ✅ Ao criar um **espaço de trabalho**, ele só estará disponível para você. Qualquer outra pessoa além dos Administradores do sistema não poderá encontrá-lo. Depois que o espaço de trabalho estiver definido e você estiver pronto para trazer sua equipe para iniciar a colaboração, será necessário compartilhá-lo com ela e definir seu nível de permissão.

  Você pode escolher entre os seguintes níveis de permissão:

   * **Gerenciar**: as pessoas podem editar, excluir e compartilhar o espaço de trabalho.
   * **Contribute**: as pessoas podem criar, editar e excluir registros.
   * **Exibir**: as pessoas podem exibir registros.

* ✅ Embora muitos clientes tenham a impressão de que concederiam permissões de **Gerenciar** para espaços de trabalho à maioria das pessoas, restrinja as permissões de **Gerenciar** a um grupo selecionado de pessoas confiáveis que não excluirão acidentalmente um tipo de registro ou criarão campos e tipos de registro desnecessários. Eles podem editar, compartilhar e até mesmo excluir o espaço de trabalho. Esse nível de permissões concede a eles acesso administrativo total à Workspace.

  É necessária uma licença de usuário Standard para que alguém tenha permissões de gerenciamento em um espaço de trabalho.

* ✅ Conceda aos usuários permissões de **Contribute** se você quiser apenas que eles possam criar, editar e excluir registros, mas não quiser que eles alterem a estrutura e o esquema do espaço de trabalho. Com permissões do **Contribute**, não é possível criar tipos de registro ou alterar os campos nos tipos de registro existentes.

  É necessária uma licença de usuário Standard para que alguém tenha permissões do **Contribute** para um espaço de trabalho.

* ✅ Conceda aos usuários permissões de **Visualização**, se você quiser que eles apenas visualizem registros.

  >[!NOTE]
  >
  >No momento, não temos permissões específicas para tipos de registros ou registros, portanto, isso significa que todos os registros em qualquer um dos tipos de registros estarão visíveis se você conceder acesso a alguém **Exibir** ao espaço de trabalho.


#### Como devo gerenciar permissões para tipos de registros?

* ✅ Lembre-se de que os usuários com permissões para Gerenciar espaços de trabalho não podem ter suas permissões reduzidas para o tipo de registro. Eles também herdarão as permissões Gerenciar para o tipo de registro. Você não pode conceder a um usuário permissões de Gerenciar no espaço de trabalho, mas permissões do Contribute ou de Visualização no tipo de registro.
* ✅ Se você quiser que os usuários tenham um nível de permissão mais baixo (por exemplo, permissões de Exibição) para o tipo de registro do que eles têm para o espaço de trabalho, recomendamos dar a eles permissões do Contribute para o espaço de trabalho. Em seguida, você pode conceder a eles permissões de Exibição para o tipo de registro.
* Remover um usuário das permissões do tipo de registro ainda dá a ele pelo menos permissões de Exibição para o espaço de trabalho.

#### Como devo gerenciar permissões para exibições?

* ✅ Restrinja as permissões de **Gerenciar** às pessoas que você deseja que possam editar, excluir e compartilhar o modo de exibição. Isso significa que eles podem alterar os filtros, agrupar campos ou alguma configuração da visualização. Essas alterações afetarão a configuração principal da exibição para todos os outros que também estão usando a exibição.

  Uma licença de usuário Padrão é necessária para que alguém tenha permissões de gerenciamento para uma exibição.

* ✅ Conceda aos usuários acesso de **Visualização** para poder aplicar a visualização. Eles poderão alterar alguns dos filtros ou agrupamentos e classificação, mas essas alterações serão apenas temporárias; as alterações não são salvas para todos os outros usuários que acessarem a visualização. Essas alterações não afetarão a configuração principal da exibição para todos os outros que também estiverem usando a exibição.  Suas alterações só são visíveis para o usuário que está aplicando as configurações modificadas. Após atualizar a tela, as alterações são redefinidas para o padrão.

* ✅ Conceda **Todos no espaço de trabalho podem exibir** permissões quando desejar que todos os que podem exibir o espaço de trabalho vejam os registros e seus campos nesse modo de exibição específico. Dessa forma, não é necessário adicionar ninguém manualmente à caixa de permissão de compartilhamento da exibição.

  >[!NOTE]
  >
  >Se uma exibição não tiver sido compartilhada e você compartilhar um link com outras pessoas, elas poderão ver os registros na **Exibição de Tabela Padrão**. Se eles tiverem uma licença Standard Workfront, poderão criar sua própria visualização.


#### Qual a diferença entre o **compartilhamento de Workspace** e o **compartilhamento de exibição**?

* **O compartilhamento do Workspace** define o acesso das pessoas ao espaço de trabalho, seus tipos de registro, registros e seus campos.

* **Compartilhamento de exibição** define se o usuário pode ver o modo de exibição que você criou e se pode alterar o filtro, campos de agrupamento ou alguma outra configuração do modo de exibição. A visibilidade dos registros exibidos na Exibição é controlada pelo compartilhamento do Workspace, e não pelo compartilhamento de Exibição.

#### Como os tipos de licença do Workfront afetam as permissões do Workfront Planning?

* Para **compartilhamento no Workspace**: os usuários de licenças do Light e do Contribute só podem obter acesso de visualização a um espaço de trabalho. Para conceder permissão de Contribute ou Gerenciar a um espaço de trabalho, é necessário ter uma licença Standard.

* **Compartilhamento de exibições**: os usuários de licença padrão que têm permissões de gerenciamento para um espaço de trabalho poderão criar uma exibição. Os usuários de licença do Light e do Contribute só podem utilizar as exibições que os usuários do Standard criaram e compartilharam com eles. Caso contrário, se nada tiver sido compartilhado, os usuários poderão ver a **Exibição de Tabela Padrão**.


#### O que devo fazer quando um proprietário do Workspace mudar?

* O Workfront define o criador do espaço de trabalho como proprietário, mas em termos de funcionalidade, o proprietário tem as mesmas permissões que qualquer usuário com permissões de gerenciamento.
* Se o proprietário estiver desativado, outros membros poderão continuar seu trabalho no espaço de trabalho sem interrupções.
* Os administradores do sistema têm acesso a qualquer espaço de trabalho; portanto, se o proprietário for a única pessoa com permissões de gerenciamento, os administradores poderão adicionar outra pessoa e conceder a ela permissões de gerenciamento para lidar com o gerenciamento do espaço de trabalho.

### Submetendo solicitações no Workfront Planning

Você pode criar um formulário de solicitação para cada tipo de registro quando quiser que os usuários adicionem registros fora da página de um tipo de registro. O envio do formulário adiciona um novo registro ao tipo de registro.

#### Quando devo começar a criar um formulário de solicitação para um tipo de registro?

* ✅ Verifique se a estrutura do tipo de registro foi configurada primeiro adicionando os campos necessários à tabela. Esses campos descrevem seus registros e estarão acessíveis no construtor de formulários.

  Idealmente, crie o formulário de solicitação ou de entrada depois que a estrutura do tipo de registro for finalizada para evitar a falta de campos-chave.

#### Quem pode criar formulários de solicitação?

* ✅ Qualquer usuário com acesso de Gerenciar ao espaço de trabalho pode criar ou editar um formulário de solicitação. Verifique se as permissões do usuário foram atribuídas corretamente para permitir essa funcionalidade.

#### Como devo criar ou editar um formulário de solicitação para um tipo de registro?

* ✅ Qualquer usuário com acesso de Gerenciar ao espaço de trabalho pode seguir as etapas descritas no artigo [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


#### Quem poderá enviar novos registros usando o formulário de solicitação?

* ✅ As permissões de envio dependem das configurações que você definir para cada formulário.

  No construtor de formulários, depois de publicar o formulário, você pode gerenciar permissões para controlar quem pode enviar solicitações.

  Você pode escolher entre as três opções de compartilhamento a seguir:

   * **Qualquer pessoa com acesso de exibição ou superior ao espaço de trabalho:** Permite que todos os usuários com permissões de exibição ou superiores ao espaço de trabalho enviem uma solicitação que crie um registro.
   * **Qualquer pessoa com acesso de contribuir ou superior ao espaço de trabalho**: restringe os envios a usuários com permissões do Contribute ou superiores ao espaço de trabalho.
   * **Qualquer pessoa com o link:** Permite que qualquer pessoa com o link do formulário envie uma solicitação.
   * **Data de expiração:** Verifique se você definiu uma data de expiração para o link público para aprimorar a segurança.

### Práticas recomendadas para gerenciar formulários de solicitação

Veja a seguir recomendações para gerenciar formulários de solicitação:

* Planejar com antecedência: defina claramente quais informações são necessárias ou necessárias dos solicitantes antes antes de criar o formulário para evitar revisões excessivas posteriormente.
* Usar rótulos claros: certifique-se de que os rótulos e as descrições dos campos sejam claros e compreensíveis para todos os usuários.
* Formulários de teste: antes de implantar novos formulários para um público-alvo maior, teste-os usando a opção de visualização de link e formulário de formulário para garantir que todos os campos e a lógica funcionem conforme esperado.
* Manter formulários atualizados: revisa formulários periodicamente e os atualiza para corresponder a qualquer alteração na estrutura de tipo de registro ou nos processos operacionais.

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/pt-br/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/pt-br/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/pt-br/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->
