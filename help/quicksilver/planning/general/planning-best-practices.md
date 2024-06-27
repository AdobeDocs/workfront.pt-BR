---
title: 'Práticas recomendadas do Adobe Workfront Planning'
description: Como líder em operações de marketing, você pode usar o Adobe Workfront Planning para organizar trabalhos em todo o ciclo de vida de marketing para todas as suas equipes. Estas são algumas das práticas recomendadas que recomendamos ao iniciar o Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d1da3ee59b074dec3e161cf1e0134aba39ad90a4
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---


# Práticas recomendadas do Adobe Workfront Planning

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

Como líder em operações de marketing, você pode usar o Adobe Workfront Planning para organizar trabalhos em todo o ciclo de vida de marketing para todas as suas equipes.

Este artigo documenta algumas práticas recomendadas que recomendamos ao iniciar o Workfront Planning.

## O que é o Workfront Planning?

O módulo de planejamento do Workfront é um dos três recursos distintos, mas conectados, do Workfront que, juntos, criam um sistema de marketing de registro. Os três recursos são:

* **Planejamento**: os novos recursos avançados incluídos no Workfront Planning.

* **Fluxo de trabalho**: os recursos de gerenciamento de trabalho colaborativo que você usa atualmente no Workfront (gerenciamento de projetos, gerenciamento de recursos etc.)

* **Automação e integração**: os recursos abrangentes de integração e automação fornecidos pelo Workfront Fusion.

O Workfront Planning é altamente personalizável. Para obter mais informações sobre a terminologia e o conceito-chave do Workfront Planning, consulte [Visão geral do Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

## Perguntas a serem feitas antes de configurar o Workfront Planning

Depois de se familiarizar com a terminologia e arquitetura do Workfront Planning, você pode começar a configurar seu novo ambiente.

Algumas perguntas que você pode fazer a si mesmo ao configurar o Planning são:

* **Desejo usar espaços de trabalho para grupos organizacionais maiores? Ou devo encorajar as pessoas a fazer programas pessoais?**

  Você pode achar que há um bom uso para ambos. Recomendamos não ter muitos espaços de trabalho, pois eles podem se tornar difíceis de gerenciar e seus fluxos de trabalho podem estar muito fragmentados.

  >[!TIP]
  >
  >    Você pode ter mil espaços de trabalho em uma instância do Workfront.

* **Quais tipos de registro personalizado devo criar em cada espaço de trabalho?**

  Os tipos de registro são como os tipos de objeto do Workfront. Pense nos fluxos de trabalho e decida quais tipos de registro (objetos de trabalho, objetos de pessoas, taxonomias etc.) cada workflow pode precisar de.

  Para obter informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md)

* **Como criarei meus registros? Existe uma lista ou planilha externa que já contém os registros que preciso adicionar ao Planning e que posso usar? Os registros serão adicionados gradualmente, dependendo da necessidade? Ou eles serão importados usando um Fusion ou uma integração de API personalizada?**

  Para obter informações, consulte:

   * [Criar registros](/help/quicksilver/planning/records/create-records.md)
   * [Módulos do Adobe Workfront Planning](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **Quais campos preciso criar para meus registros?**

  Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

* **Quais tipos de objeto do Workfront ou do AEM Assets são necessários para me conectar aos tipos de registro do Workfront Planning para poder mostrar dependências e criar um fluxo de trabalho contínuo para minha organização?**

  Para obter informações, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md)

* **Quais calendários e visualizações de marketing serão necessários para contar a história das minhas campanhas? E a que partes interessadas eu poderia disponibilizar essas visualizações para uma colaboração contínua?**

  Para obter informações, consulte [Gerenciar exibições de registro](/help/quicksilver/planning/views/manage-record-views.md).


## Práticas recomendadas do Workfront Planning

Esta seção lista várias diretrizes de práticas recomendadas e do DOS ao configurar o Workfront Planning.

As diretrizes são organizadas dependendo do objeto ou da área que você está configurando.

### Espaços de trabalho

#### Os itens de fazer e não fazer dos espaços de trabalho

* Realizar o design para o volume mais baixo de espaços de trabalho de nível de organização

  Por exemplo, tente criar uma única Workspace para todo o Marketing

* Prepare seus espaços de trabalho periodicamente. Você pode achar que pode modificar um existente em vez de criar um novo do zero.

* Crie um novo Workspace para uma equipe que tenha um movimento operacional completamente diferente.

  Um espaço de trabalho de &quot;Desenvolvimento de produto&quot; deve ser diferente de um espaço de trabalho de &quot;Marketing&quot;

* Não crie um espaço de trabalho exclusivo para cada pequena coisa. Pense nos espaços de trabalho mais como um sistema de registro que pode beneficiar uma organização inteira e permitir que todos mapeiem fluxos de trabalho e colaborem, em vez de um espaço privado para acompanhar solicitações pessoais.

* Não crie espaços de trabalho exclusivos para cada equipe ou processo em uma organização.

  A organização de marketing deve se esforçar para manter apenas um espaço de trabalho para manter a visibilidade e permitir que os dados sejam acumulados no nível de planejamento global.

  Evite criar espaços de trabalho semelhantes ou duplicados para equipes que seguem processos semelhantes (por exemplo, marketing EMEA VS marketing APAC), especialmente onde essas equipes podem realizar trabalhos que se acumulam em uma campanha estratégica comum.

#### Como devo usar as seções do espaço de trabalho?

* Crie e rotule seções para ajudar os usuários a entender como você organiza o ciclo de vida operacional.

  Por exemplo, você pode criar uma seção chamada &quot;Registros principais&quot; em que você coloca suas Campanhas, Táticas e Entregáveis.

* Agrupe os tipos de registro &quot;curtir&quot;.

  Você pode criar uma seção chamada &quot;Geografias&quot; que contém tipos de registro como: Região, País e Cidade.

#### Como devo gerenciar as permissões do espaço de trabalho?

* Restrinja o acesso &quot;Gerenciar&quot; a um grupo selecionado de pessoas confiáveis, que não excluirão acidentalmente um tipo de registro ou criarão tipos e campos de registro desnecessários.

  >[!TIP]
  >
  >Durante nosso programa beta, descobrimos que muitos clientes acham que concederiam acesso de &quot;Gerenciamento&quot; a administradores de grupo.

* Adicione a área do Planning ao modelo de layout de usuários com uma licença Standard.

* Permitir que usuários com uma licença Standard criem espaços de trabalho pessoais. Isso lhes dá um espaço seguro para aprender a ferramenta e se familiarizarem com ela. Isso não prejudicará a experiência para outros e poderá melhorar a produtividade pessoal do usuário.

  >[!TIP]
  >
  >    Recomenda que eles não compartilhem seus espaços de trabalho pessoais como prática recomendada.


### Tipos de registro

#### Um campo de seleção única ou múltipla em comparação a um tipo de registro vinculado

* Criar um novo tipo de registro se o objeto for usado em vários outros tipos de registro

  Por exemplo, uma Campanha pode ter uma conexão com vários Públicos-alvo, e uma Tática pode ter uma conexão com um único Público-alvo.

* Crie um novo tipo de registro se o objeto precisar armazenar valores de metadados adicionais que possam ser úteis em pesquisas.

  Por exemplo, um tipo de registro Canal, como &quot;Email&quot;, pode armazenar uma lista de Materiais de entrega compatíveis, como metadados nativos ou como uma conexão com o tipo de registro &quot;Materiais de entrega&quot; independente.

* Não adicione um novo tipo de registro se os dados que você estiver armazenando precisarem ser limitados a um único tipo de registro. Em vez disso, use um campo de seleção.

  Por exemplo, um tipo de registro de Campanha pode ter um campo de seleção única chamado Tamanho da campanha que só é relevante quando diretamente associado a uma campanha específica.

#### Como devo rotular meus tipos de registros?

Crie e rotule tipos de registro que representam uma única construção ou substantivo, como &quot;Campanhas&quot;

:no_entry_sign: Não crie um tipo de registro que seja melhor representado como uma camada de visualização. Por exemplo, &quot;Calendário&quot; é uma escolha ruim para um tipo de registro, pois não é o tipo de registro em si, mas uma exibição de registros.

### Quantas camadas de hierarquia devo criar?

Visualizações

..

Fluxo de trabalho (WRK)

..

### Gerenciamento de campo

Campo principal

Use valores de campo primário exclusivos para facilitar a localização e a &quot;seleção&quot; desses registros ao fazer conexões.

Ao fazer uma conexão, os usuários pesquisarão pelos valores no campo Primário e, se não forem exclusivos, os usuários não saberão qual escolher.

Evite usar valores não exclusivos como o campo principal, pois ele pode criar confusão para usuários que precisam pesquisar no campo principal ao usar o menu do seletor de conexões.



De Chris O&#39;Neal:

Outra área que pode ser/não deve ser considerada são os casos de uso que são (ou não são) os melhores usos do Planning. Por exemplo, a discussão sobre gestão de recursos que tivemos hoje.



Alina observa:

Exemplo de artigo &quot;Práticas recomendadas&quot; do ExL: https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views

Informações adicionais de Field Readiness da Lauren S.: https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346