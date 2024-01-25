---
title: Atividade de lançamento do Adobe Maestri
description: O Adobe Maestri está disponível atualmente para clientes selecionados do Workfront. Leia este artigo com frequência para saber mais sobre os recursos recém-lançados para o Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 54c6adf51ab8ef4e7968e8fdeeb0025e42deecc5
workflow-type: tm+mt
source-wordcount: '3564'
ht-degree: 0%

---

# Atividade de lançamento do Adobe Maestri

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro/maestro-overview.md).

Este artigo lista os recursos que foram lançados após o lançamento do programa beta fechado do Maestro, em 22 de maio de 2023.

Os recursos lançados são listados na ordem de lançamento, com o mais recente primeiro. Os clientes que estão participando do programa beta fechado Maestro podem acessar todos os recursos em seus ambientes de produção.

>[!IMPORTANT]
>
>Entre maio e dezembro de 2023, todos os recursos deste artigo foram lançados para o ambiente de Pré-visualização e Produção. Os recursos do Maestro foram temporariamente removidos dos ambientes de Pré-visualização e Sandbox desde janeiro de 2024. Todos os recursos lançados após essa data estão disponíveis atualmente na Produção.

Este artigo lista os recursos e patches que foram lançados após o lançamento do programa beta fechado do Maestro, em 22 de maio de 2023.

Os recursos são lançados semanalmente e são listados na ordem de lançamento, com o mais recente primeiro. Os clientes que estão participando do programa beta fechado Maestro podem acessar todos os recursos em seus ambientes de Pré-visualização e Produção.

>[!IMPORTANT]
>
>A documentação referenciada nas seções abaixo estará disponível algum tempo depois que os recursos forem lançados para produção.

## Semana de 22 de janeiro de 2024

### A nova seção Histórico exibe a atividade do sistema para registros Maestri

Produção: 25 de janeiro de 2024

Visualização: a ser determinado

Para melhorar os recursos de auditoria, introduzimos uma nova seção no painel direito de um registro, onde você pode revisar as alterações feitas no registro gravado pelo sistema.

Maestri registra as seguintes informações na nova seção História:

* Quaisquer alterações de campo

* Os valores antigos e novos dos campos, quando os valores são alterados

* O nome completo do usuário que fez a alteração

* Uma data e carimbo de data e hora de quando a alteração ocorreu.

Para obter mais informações, consulte [Gerenciar comentários de registro](/help/quicksilver/maestro/records/manage-record-comments.md).

### Novo rótulo para novo link de registro

Produção: 25 de janeiro de 2024

Visualização: a ser determinado

Para criar consistência ao criar registros, renomeamos o link + Novo para criar registros como &quot;+ Novo registro&quot;.  Antes dessa atualização, o link continha o nome do tipo de registro. O novo link agora está disponível ao criar registros operacionais e de taxonomia. Para obter informações, consulte [Criar registros](/help/quicksilver/maestro/records/create-records.md).

## Semana de 8 de janeiro de 2024

### Os recursos do Maestri são removidos dos ambientes Pré-visualização e Sandbox

Pré-visualização e sandbox: 11 de janeiro de 2024

A área do Maestro e todos os recursos do Maestro foram removidos temporariamente dos ambientes de Pré-visualização e Sandbox. O Maestri será adicionado a esses ambientes em uma data posterior, que será comunicada nas notas de atividade da versão.

### Permissões principais para espaços de trabalho e visualizações

Produção: 11 de janeiro de 2024

Visualização: a ser determinado

Agora você pode compartilhar um espaço de trabalho ou uma visualização com usuários e grupos. É possível definir as permissões em diferentes níveis, dependendo das informações que eles precisam exibir ou editar.

Quando você compartilha um espaço de trabalho, os usuários têm permissões para os tipos de registro, registros e campos nesse espaço.

Quando você compartilha um espaço de trabalho, os usuários não recebem permissões de compartilhamento para as exibições associadas aos tipos de registro do espaço de trabalho. Você deve conceder permissões separadas para exibições.

A seguir estão os níveis de permissões para espaços de trabalho Maestro:

* Exibir: os usuários podem exibir espaços de trabalho compartilhados com eles. Eles também podem exibir tipos de registro e registros do espaço de trabalho compartilhado.

* Contribute: os usuários podem criar, editar ou excluir registros no espaço de trabalho que é compartilhado com eles.  Eles não podem criar ou editar tipos de registro ou espaços de trabalho compartilhados com eles.

* Gerenciar: Os usuários podem criar, editar e excluir espaços de trabalho, tipos de registro, registros e campos em espaços de trabalho que são compartilhados com eles.

A seguir estão os níveis de permissões para exibições de registro:

* View: Os usuários podem selecionar a view no menu drop-down Exibir de uma página do tipo de registro.
* Gerenciar: Os usuários podem editar, compartilhar e excluir a exibição.

Para obter mais informações, consulte [Visão geral do Access](/help/quicksilver/maestro/access/access-overview.md) e [Visão geral das permissões de compartilhamento no Adobe Maestro](../maestro/access/sharing-permissions-overview.md).

### Novo tipo de campo Fórmula

Produção: 11 de janeiro de 2024

Visualização: a ser determinado

Agora é possível adicionar um campo do tipo Fórmula a um tipo de registro.

Os campos de fórmula geram um novo valor usando valores existentes de outros campos em um tipo de registro e uma função que indica como os valores existentes devem ser calculados.

Você não pode usar campos de pesquisa de tipos de registro vinculados em um cálculo de fórmula. Essa funcionalidade estará disponível posteriormente.

Para obter informações, consulte [Visão geral dos campos de fórmula](/help/quicksilver/maestro/fields/formula-fields.md).

### Desfazer/ Refazer ações ao gerenciar registros na visão de tabela

Produção: 11 de janeiro de 2024

Visualização: a ser determinado

Agora é possível desfazer ou refazer as alterações ao executar as seguintes ações na exibição de tabela:

* Copiar/ colar dados
* Editar registro
* Adicionar registro
* Excluir registro

Você pode usar os seguintes pressionamentos de tecla para desfazer ou refazer ações:

* Desfazer: CTRL/ CMD + Z
* Refazer: CTRL/ CMD + Shift + Z

Para obter mais informações, consulte os seguintes artigos:

* [Editar registros](/help/quicksilver/maestro/records/edit-records.md)

* [Excluir registros](/help/quicksilver/maestro/records/delete-records.md)

* [Criar registros](/help/quicksilver/maestro/records/create-records.md)

## Semana de 25 de dezembro de 2023

### Pesquisar na exibição de linha do tempo

Pré-visualização e produção: 27 de dezembro de 2023

Agora é possível pesquisar uma palavra-chave para localizar rapidamente um registro na exibição de linha do tempo. Você pode usar palavras-chave e caracteres especiais de qualquer campo visível na tela para localizar um registro. Para obter informações, consulte [Gerenciar a exibição de linha do tempo](../maestro/views/manage-the-timeline-view.md).

## Semana de 18 de dezembro de 2023

### Adicionar comentários nos registros da página Detalhes

Pré-visualização e produção para todos os clientes: 18 de dezembro de 2023

>[!NOTE]
>
>Os seguintes recursos estarão disponíveis na Produção com a versão de janeiro de 2024:
>
>* Pesquisar comentários
>
>* Copiar e colar imagens
>
>* Arrastar e soltar imagens
>
>Para obter mais informações, consulte [Visão geral da versão do primeiro trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

Agora é possível colaborar com outras pessoas em registros individuais adicionando comentários ou respondendo a outras pessoas ao visualizar um registro na página Detalhes.

A experiência de comentários para registros do Maestro corresponde à nova experiência de comentários para objetos do Workfront.

Para obter mais informações, consulte [Gerenciar comentários de registro](/help/quicksilver/maestro/records/manage-record-comments.md).

### Conector Maestri (beta) para Adobe Workfront Fusion

Produção: 21 de dezembro de 2023

>[!IMPORTANT]
>
>Sua organização deve comprar o Adobe Workfront Fusion para criar conexões com o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/workfront-fusion-overview.md).

Agora, você pode usar o Adobe Workfront Fusion para se conectar ao Maestro. Com a nova conexão Adobe Maestro Fusion, você pode:

* Criar, ler, atualizar e excluir registros

* Obter uma lista de registros por tipo de registro

* Excluir ou obter uma lista de tipos de registros

* Pesquisar registros

* Fazer uma chamada de API

* Acionar um cenário quando uma alteração for feita no Maestro

Para obter mais informações, consulte [Módulos do Adobe Maestri](/help/quicksilver/workfront-fusion/apps-and-their-modules/maestro-modules.md).

## Semana de 11 de dezembro de 2023

### Atualizar o campo principal em uma exibição de tabela de um tipo de registro

Pré-visualização e produção: 14 de dezembro de 2023

Agora você pode escolher o campo que deseja exibir na primeira coluna de uma exibição de tabela do Maestro. Esse campo agora é chamado de campo primário.

Antes desse aprimoramento, o campo Nome de um registro sempre era exibido na primeira coluna da exibição de tabela e não podia ser colocado em outra posição.

Com essa melhoria, observe o seguinte:

* A coluna ou o campo Name ainda é a primeira coluna de uma tabela, por padrão.

* Você pode escolher qualquer campo dos seguintes tipos para ser um campo principal e substituir o campo Name na primeira coluna:

   * Texto de linha única

   * Número

   * Fórmula

* O campo principal de uma exibição de tabela é sempre congelado e não pode ser movido, a menos que você defina outro campo como campo principal.

* Você pode alterar o campo primário de um cabeçalho de coluna não primário.

* Todas as exibições de tabela de um tipo de registro têm o mesmo campo principal selecionado.

Para obter mais informações, consulte [Gerenciar exibição de tabela](/help/quicksilver/maestro/views/manage-the-table-view.md).


### Conectar registros do Maestri com o Adobe Experience Manager Assets

Versão de pré-visualização: 14 de dezembro de 2023

Versão de produção: 21 de dezembro de 2023

>[!IMPORTANT]
>
>A instância da Workfront de sua organização deve ser integrada à Plataforma de negócios Adobe ou à Adobe Admin Console para poder conectar os registros Maestri à Adobe Experience Manager Assets.
>
>Em caso de dúvidas sobre a integração com a Adobe Admin Console, consulte [Perguntas frequentes sobre a experiência unificada do Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).


Agora você pode estabelecer uma conexão entre os tipos de registros Maestro e Adobe Experience Manager Assets.

Após estabelecer a conexão, a seguinte funcionalidade estará disponível com esta atualização:

* Você pode vincular ativos e pastas do Experience Manager a um registro Maestro de um repositório específico no Experience Manager Assets ao qual eles têm acesso. Você pode conectar campos de ativos a campos Principais neste processo.

* Os usuários do Maestro podem exibir o nome dos ativos conectados, bem como os valores dos campos conectados no Maestro

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Maestro after you establish the connection. Connected assets are visible in the Maestro table and timeline views of this new record type.  
-->

* Você pode clicar no nome do ativo na exibição de tabela do registro Mestre no campo de registro conectado e exibir uma janela pop-up com a miniatura do ativo e vários campos-chave. Na janela pop-up, você pode navegar até o visualizador de ativos no Experience Manager e visualizar todos os detalhes sobre ele.

Para obter mais informações, consulte [Conectar tipos de registro](/help/quicksilver/maestro/architecture/connect-record-types.md).

## Semana de 4 de dezembro de 2023

### Copiar e colar informações de um campo para outro na exibição de tabela Mestre para campos de registro vinculados e do tipo Pessoas

Pré-visualização e produção: 5 de dezembro de 2023

Agora você pode copiar e colar informações de um campo para outro campo do mesmo tipo em uma exibição de tabela do tipo de registro Maestri. Essa funcionalidade agora é compatível com os seguintes tipos de campos:

* Pessoas
* Campos de registro vinculados

Considere o seguinte:

* Copiar e colar valores de campo de um campo para outro é compatível com campos que exibem vários valores.

* Você não pode copiar informações de outra fonte, que não seja um campo Maestro do mesmo tipo do campo no qual você cola as informações.

* Não é possível copiar e colar valores de campo para campos exibidos na área Detalhes de um registro.

Para obter mais informações, consulte [Editar registros](../maestro/records/edit-records.md).

Para obter informações sobre campos vinculados, consulte [Conectar tipos de registro](../maestro/architecture/connect-record-types.md).

## Semana de 27 de novembro de 2023

### Copiar e colar informações de um campo para outro na exibição de tabela do Maestro

Pré-visualização e produção: 28 de novembro de 2023

Agora você pode copiar e colar informações de um campo para outro campo do mesmo tipo em uma exibição de tabela do tipo de registro Maestri.

Considere o seguinte:

* Você não pode copiar informações de outra fonte, que não seja um campo Maestro do mesmo tipo do campo no qual você cola as informações.

* Não é possível copiar e colar valores de campo para campos exibidos na área Detalhes de um registro.

* Não é possível copiar e colar valores de campo para os seguintes tipos de campo:

   * Pessoas

   * Campos do sistema

   * Campos vinculados criados como resultado da conexão de registros

Para obter mais informações, consulte [Editar registros](../maestro/records/edit-records.md).

## Semana de 6 de novembro de 2023

### Agrupamento para exibição de tabela

Pré-visualização e produção: 7 de novembro de 2023

Agora é possível agrupar registros na exibição de tabela de uma página do tipo de registro. Você pode agrupar por três campos únicos na interface do Maestro <!--checking into this for now: and by four fields when using the API-->.

Para obter mais informações, consulte [Gerenciar a exibição de tabela](../maestro/views/manage-the-table-view.md).

## Semana de 30 de outubro de 2023

### Novos tipos de campo para usuários e campos de data para capturar quem criou ou modificou um registro pela última vez ou em qual data

Pré-visualização e produção: 30 de outubro de 2023

Introduzimos os seguintes tipos de campos para registros Maestro:

* Criado por

* Data de criação

* Modificado pela última vez por

* Data da última modificação

Os valores de campo dos campos criados a partir desses tipos de campo são somente leitura e capturam o nome do usuário que criou ou modificou um registro pela última vez ou a data em que o registro foi criado ou modificado pela última vez.

Para obter mais informações, consulte [Criar campos](../maestro/fields/create-fields.md).

### Navegar para objetos do Workfront a partir de um registro Maestro

Pré-visualização e produção: 31 de outubro de 2023

Agora você pode abrir as páginas de objetos do Workfront nas seguintes áreas no Maestri:

* A exibição da tabela de registro de objeto vinculada ao Workfront somente leitura

* A página Detalhes do registro de objeto do Workfront somente leitura

Para obter mais informações, consulte [Conectar registros](../maestro/records/connect-records.md).

### Navegação aprimorada na exibição de tabela

Pré-visualização e produção: 2 de novembro de 2023

Melhoramos a navegação na exibição de tabela de uma página do tipo de registro.

Estas são algumas das melhorias:

* Use a tecla Tab do teclado para navegar pelas colunas e linhas da tabela

* Adicione um novo registro a partir de qualquer posição da coluna. Antes dessa melhoria, você poderia adicionar um registro somente da primeira coluna.

* Use a combinação de teclado Shift + Enter para adicionar um novo registro (ou linha) à tabela.

Para obter mais informações, consulte [Criar registros](../maestro/records/connect-records.md).

## Semana de 16 de outubro de 2023

### Novo tipo de campo Pessoas

Pré-visualização e produção: 16 de outubro de 2023

Agora você pode adicionar um campo do tipo Pessoas aos tipos de registro Maestro. Você pode usar campos do tipo Pessoas para associar usuários existentes a um registro. Para obter informações, consulte [Criar campos](../maestro/fields/create-fields.md).

### Formato Rich Text para campos de parágrafo

Pré-visualização e produção: 16 de outubro de 2023

Adicionamos controles de formato Rich Text para campos do tipo Parágrafo. É possível formatar campos de parágrafo usando Rich Text na exibição de Tabela de um tipo de registro ou na página Detalhes de um registro. Para obter mais informações, consulte [Editar registros](../maestro/records/edit-records.md).


### Registrar e agrupar codificação por cores para a exibição de Linha do tempo

Pré-visualização e produção: 19 de outubro de 2023

Agora é possível codificar por cores as barras de registro e os agrupamentos na exibição Linha do tempo.

A seguir estão opções para as cores que você pode escolher exibir para as barras de registro e agrupamentos na exibição Linha do tempo:

* Os agrupamentos podem corresponder às seguintes cores:

   * Cinza (o padrão)

   * A cor do campo pelo qual você agrupa

* As barras podem corresponder às seguintes cores:

   * A cor do tipo de registro

   * A cor de um campo selecionado

   * A cor do agrupamento

   * Sem cor (o padrão)

Ao corresponder cores a um determinado campo, é possível selecionar apenas campos com opções codificadas por cores.

Para obter mais informações, consulte [Gerenciar a exibição de linha do tempo](../maestro/views/manage-the-timeline-view.md).

## Semana de 9 de outubro de 2023

### Pesquisar na exibição de tabela

Pré-visualização e produção: 9 de outubro de 2023

Agora é possível pesquisar uma palavra-chave para localizar rapidamente um registro na exibição de tabela. Você pode usar palavras-chave e caracteres especiais de qualquer campo visível na tela para localizar um registro. Para obter informações, consulte [Gerenciar a exibição de tabela](../maestro/views/manage-the-table-view.md).

## Semana de 18 de setembro de 2023

### Reordenar linhas

Pré-visualização e produção: 20 de setembro de 2023

Agora é possível reordenar uma ou várias linhas (ou registros) na exibição Tabela de uma página do tipo de registro. Para obter informações, consulte [Gerenciar a exibição de tabela](../maestro/views/manage-the-table-view.md).

## Semana de 4 de setembro de 2023

### Conectar registros do Maestri com empresas e grupos da Workfront

Pré-visualização e produção: 5 de setembro de 2023

Agora você pode conectar um registro Maestro com empresas e grupos Workfront. Primeiro, você deve criar uma conexão entre um tipo de registro Maestro e os tipos de objeto de empresas e grupos do Workfront. Em seguida, você pode conectar um único registro Maestro do tipo de registro selecionado a empresas e grupos individuais da Workfront.

Considere o seguinte:

* Você deve criar uma conexão entre os tipos de registro Maestro e os tipos de objeto Empresa e Grupo do Workfront para cada Espaço de trabalho.

* Não é possível conectar tipos de registro de taxonomia a tipos de objeto do Workfront.

* Você pode conectar vários registros do Maestro à mesma empresa ou grupo da Workfront, e várias empresas ou grupos ao mesmo registro do Maestro.

* Você não pode editar empresas ou grupos no Maestro. Todas as alterações de empresa ou grupo realizadas no Workfront são visíveis no Maestro, ao revisar os registros vinculados ao Maestro.

  Para obter mais informações, consulte os seguintes artigos:

   * [Conectar tipos de registro](../maestro/architecture/connect-record-types.md)
   * [Conectar registros](../maestro/records/connect-records.md)

### Suporte de URL para campos de texto de linha única

Pré-visualização e produção: 7 de setembro de 2023

Para melhor visibilidade ao trabalhar com links na visualização Tabela, adicionamos suporte para URLs em campos de texto de linha única. Usar URLs para outros sites ou unidades externas ao atualizar um campo de texto de linha única, agora os identifica como links e permite clicar neles na tabela. Antes desse aprimoramento, os links eram exibidos como texto.

## Semana de 28 de agosto de 2023

### Menu de visibilidade de campo da barra de ferramentas Exibição em tabela

Pré-visualização e produção: 31 de agosto de 2023

Para exibir as informações certas em um determinado conjunto de registros, especialmente se você pretende compartilhar a exibição com outras pessoas que precisam ver alguns, mas não todos os campos de um tipo de registro, agora é possível selecionar quais campos (ou colunas) exibir e quais ocultar na exibição Tabela.

Você pode ocultar ou mostrar campos individuais de cada cabeçalho das colunas de campo ou gerenciar todos os campos do tipo de registro de uma configuração na barra de ferramentas da exibição de tabela.

Para obter mais informações, consulte [Gerenciar a exibição de tabela](../maestro/views/manage-the-table-view.md).

## Semana de 21 de agosto de 2023

### Conectar registros do Maestro a programas e portfólios

Pré-visualização e produção: 24 de agosto de 2023

Agora você pode conectar um registro do Maestro com programas e portfólios da Workfront. Você deve criar uma conexão entre um tipo de registro Maestro e um programa ou portfólio que cria um campo conectado. Em seguida, você pode conectar qualquer registro Maestro de todos os outros tipos de registro no mesmo espaço de trabalho a programas e portfólios específicos que criam um tipo de registro de Portfolio Workfront ou Programa Workfront somente leitura no mesmo espaço de trabalho. Considere o seguinte:

* Os tipos de registro do conector do Workfront são exclusivos para cada espaço de trabalho.
* Você pode conectar vários registros do Maestro ao mesmo programa ou portfólio do Workfront, e vários programas e portfólios ao mesmo registro do Maestro.
* Não é possível editar programas e portfólios no Maestro. Todas as alterações de programa e portfólio realizadas no Workfront são visíveis no Maestro, ao revisar os registros vinculados.

### Nova funcionalidade de classificação para a exibição de tabela

Pré-visualização e produção: 24 de agosto de 2023

Agora é possível classificar registros na exibição de tabela de uma página do tipo de registro.
Os seguintes recursos estão disponíveis:

* Classificação no nível da tabela, em que é possível classificar por vários campos ao mesmo tempo.
* Classificação no nível da coluna ou do campo, em que é possível classificar por um campo individual de cada vez.

### Melhorias na visualização da linha do tempo: nova aparência para agrupamentos e a opção de visualização Compacta/Padrão

Pré-visualização e produção: 24 de agosto de 2023

Introduzimos as seguintes melhorias na visualização da linha do tempo:

* Agora é possível exibir a exibição de linha do tempo nos seguintes modos:

   * Standard: exibe registros em linhas separadas.
   * Compacto: exibe os registros cujas datas não se cruzam na mesma linha.

* Alteramos a aparência das linhas de agrupamento na exibição de linha do tempo para exibição acima da linha do tempo dos registros que elas contêm. Antes dessa melhoria, as linhas de agrupamento eram exibidas em toda a extensão da linha do tempo.

## Semana de 14 de agosto de 2023

### Reordenar colunas na exibição de tabela

Agora você pode reordenar colunas na exibição de tabela Maestri. Considere o seguinte ao reordenar colunas:

* O campo Nome é sempre o primeiro campo na exibição de tabela de uma página do tipo registro

* Não é possível mover o campo Nome para outra posição

* O campo Nome está congelado e não faz parte da rolagem horizontal.

### Rolagem horizontal para exibição da linha do tempo

Agora é possível rolar horizontalmente na exibição de linha do tempo de um tipo de registro.

## Semana de 7 de agosto de 2023

### Importar tipos de registro de um arquivo do Excel

Pré-visualização e produção: 10 de agosto de 2023

Agora você pode importar um arquivo do Excel para criar tipos de registro em um espaço de trabalho. As folhas do arquivo se tornam os tipos de registro e as colunas do arquivo se tornam seus respectivos campos.

### Experiência aprimorada para conectar tipos de registro e projetos

Pré-visualização e produção: 10 de agosto de 2023

Melhoramos a maneira como você conecta tipos de registros, incluindo a conexão com projetos do Workfront. Como parte dessa melhoria, fizemos as seguintes alterações ao adicionar um campo para um tipo de registro na exibição de tabela:

* O campo Tipo de relação foi removido da guia &quot;Novo campo&quot;.

* Adicione uma guia &quot;New connection&quot; onde você pode selecionar diretamente o tipo de registro ou objeto ao qual deseja se conectar, eliminando a necessidade de um campo do tipo Relacionamento.

## Semana de 10 de julho de 2023

### Atualizar a aparência de um tipo de registro

Pré-visualização e produção: 13 de julho de 2023

Agora é possível selecionar um ícone personalizado para um tipo de registro e uma cor personalizada para o ícone de tipo de registro.

### Novo tipo de campo da caixa de seleção

Pré-visualização e produção: 13 de julho de 2023

Agora você pode adicionar um tipo de campo Caixa de seleção aos tipos de registro Mestre. Você pode usar um campo do tipo Caixa de seleção para adicionar uma única opção de caixa de seleção a um registro. Você pode usar esse campo para indicar um atributo ou status específico para esse registro específico. Por exemplo, você pode usá-lo como um sinalizador para rastrear a conclusão, a aprovação ou qualquer outro atributo binário para cada registro.

## Semana de 26 de junho de 2023

### Ativação rápida do menu contextual em uma tabela

Pré-visualização e produção: 28 de junho de 2023

Ativamos a capacidade de ativar o menu contextual clicando com o botão direito do mouse em qualquer lugar em uma linha de registro, ao visualizar os registros na exibição de tabela ou em um tipo de registro. Agora é possível visualizar, excluir ou copiar rapidamente um link para a página Detalhes do registro ao acessar o menu contextual de qualquer lugar na exibição de tabela de um tipo de registro. Antes desse aprimoramento, o menu contextual era acessível somente pelo menu Mais na coluna Nome de um registro.

## Semana de 19 de junho de 2023

### Os nomes dos campos de registro são exclusivos

Introduzimos um requisito agora que os nomes de campos de um tipo de registro Maestri devem ter nomes únicos. Os campos que pertencem a tipos de registro diferentes não precisam ter nomes exclusivos.

## Semana de 5 de junho de 2023

### Conectar registros do Maestri com projetos da Workfront

Pré-visualização e produção: 5 de junho de 2023

Agora você pode conectar um registro Maestro com projetos Workfront. Você deve criar um tipo de registro conector Maestri para estabelecer a conexão entre os registros Maestri e os projetos Workfront. Em seguida, é possível conectar qualquer registro Maestro de todos os outros tipos de registro ao registro conector usando o campo Relacionamento. Considere o seguinte:

* Você deve ter um tipo de registro de conector para o Workfront para cada Espaço de trabalho.
* Você pode conectar vários registros do Maestro ao mesmo projeto do Workfront, e vários projetos ao mesmo registro do Maestro.
* Não é possível editar projetos no Maestro. Todas as alterações de projeto realizadas no Workfront são visíveis no Maestro, ao revisar os registros vinculados.

## Semana de 29 de maio de 2023

### Requisito de duas datas para criar uma exibição de Linha do tempo

Pré-visualização e produção: 31 de maio de 2023

Você deve ter pelo menos dois campos de data associados a um tipo de registro para criar um modo de exibição de Linha do Tempo.
