---
title: 'A Bridge: Conectando intenções estratégicas a projetos'
description: Saiba como criar uma "thread estratégica" entre seus planos de alto nível no Adobe Workfront Planning e sua execução diária de workflows no Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---


# A ponte: conectando intenção estratégica a projetos


## Meta

Saiba como criar uma &quot;thread estratégica&quot; entre seus planos de alto nível no Workfront Planning e sua execução diária no módulo Fluxo de trabalho.



## Visão geral

Conectar sua estratégia ao seu trabalho diário transforma a visão em realidade. Quando planos de alto nível estão sincronizados com a execução, você cria um **thread estratégico** que garante que cada projeto e tarefa dê andamento aos negócios.



Para alcançar esse alinhamento, é necessário um conjunto de links técnicos e medidas de proteção de processo que conectem os esforços no **módulo de Fluxo de Trabalho** com registros estratégicos no **Workfront Planning (WFP)**. Ao reduzir a distância entre o planejamento e a ação, você garante que a energia de sua equipe esteja sempre focada em suas metas de maior prioridade.



## A base: estabelecer a conexão

Antes de interligar o planejamento e a execução, um gerenciador de espaço de trabalho deve definir quais tipos de registro são elegíveis para uma conexão.



### O campo de conexão: o handshake técnico

A ponte começa com um **campo de conexão**. Este tipo de campo é o mecanismo por trás de todos os relacionamentos no WFP. É uma expressão de intenção, na medida em que estabelece que um tipo de registro específico (como uma *tática de canal*) pode ser vinculado a outros objetos, quer eles residam no módulo de fluxo de trabalho ou dentro do próprio planejamento.



### Decidir conectar

O estabelecimento dessa permissão é uma decisão no nível da configuração que normalmente ocorre antes que qualquer trabalho seja criado. Ao adicionar um campo de conexão, você está arquitetando seu ambiente para oferecer suporte a um &quot;segmento estratégico&quot;, independentemente de como os registros individuais são criados no final.



## Estratégia e execução em sincronia

Para manter o foco da camada estratégica, recomendamos que você concentre os registros de planejamento em intenções de alto nível ao usar o módulo de Fluxo de trabalho para execução tática. Essa abordagem usa os pontos fortes exclusivos de ambos os módulos:



* **Planejamento do Workfront (A camada estratégica):** Permanece de alto nível. Ele rastreia a *Campanha*, a *Tática do Canal* e o *Orçamento*. Ele não emite ruídos e está pronto para os executivos.

* **Módulo de fluxo de trabalho (a camada de execução):** gerencia os detalhes táticos. &quot;Experiências&quot; ou &quot;Atividades&quot; individuais são gerenciadas aqui como **projetos, tarefas e problemas**.



## Ativação da ponte: da intenção à ação

Depois que a conexão for configurada, você deverá decidir como ativar o link entre um registro estratégico específico e um projeto de execução.



### Triagem profissional: o caminho guiado por tabela

Estrategistas e usuários avançados geralmente usam a **exibição de tabela** como &quot;bancada&quot; para refinar planos ao longo do tempo.

* **Entrega deliberada:** por padrão, a criação de um registro em uma tabela não estabelece um link para o módulo de Fluxo de Trabalho. A conexão com um projeto de execução é estabelecida quando um usuário decide ativar o link. Isso pode ser feito criando manualmente um projeto conectado downstream diretamente do campo de conexão no WFP ou uma **página de exibição de conexão** opcional na exibição detalhada do registro. Observe que a criação manual resulta em um projeto em branco sem formulários personalizados específicos; para necessidades mais complexas, você pode usar uma **automação nativa do WFP**. Essas automações estão disponíveis quando você seleciona uma linha em uma tabela, aparecendo como botões na barra de ação azul na parte inferior da tela. Isso permite a supervisão humana ou a criação de espaços reservados, garantindo que os projetos sejam gerados somente em seu ambiente de fluxo de trabalho quando forem realmente necessários.



### Ativação automatizada

Para organizações com solicitações de alto volume ou necessidades de automação avançada, a ponte pode ser ativada automaticamente com base em eventos específicos ou valores de campo.

* **Disparadores de envio:** como os formulários fornecem um &quot;evento de envio&quot; único e limpo, eles podem ser usados como disparadores para **Automações de fusão**. Um cenário pode detectar um envio de formulário e gerar imediatamente um projeto vinculado no módulo de fluxo de trabalho.

* **Acionadores de valor de campo:** Para uma automação mais profunda, você pode configurar o **Fusion** para monitorar campos específicos. Por exemplo, uma caixa de seleção simples chamada &quot;pronto para execução&quot; pode servir como catalisador, estabelecendo a ponte automaticamente no momento em que é marcada.



## Visibilidade de superfície: Campos de pesquisa

Depois que um projeto é vinculado, você pode exibir dados em tempo real do módulo Fluxo de trabalho diretamente no registro WFP.



Um gerente de espaço de trabalho pode configurar **campos de pesquisa** para obter qualquer campo nativo ou personalizado do projeto vinculado (como *data de conclusão real* ou *lead criativo*) no tipo de registro WFP. Uma vez capturados, esses dados podem ser acumulados em vários níveis de sua hierarquia estratégica, até mesmo o nível da campanha. Isso fornece relatórios agregados avançados para as partes interessadas em todo o ciclo de vida do marketing, mantendo-as informadas sem a necessidade de sair do ambiente de planejamento.



## Visibilidade da estratégia para a ação

O valor final da ponte é **visibilidade em tempo real**. Conectando intenção à ação, você pode responder rapidamente a perguntas críticas de negócios:



* &quot;Nossa campanha &quot;Percepção da Marca no Ano Fiscal 26&quot; está gerando resultados ativamente neste momento?&quot;

* &quot;Onde nossas táticas estratégicas precisam de mais suporte criativo para permanecer no cronograma?&quot;

* &quot;Como estamos alinhando nossos recursos com nossos pilares estratégicos de maior prioridade?&quot;



## Práticas recomendadas e dicas



### Faça:

* **Use a metáfora de &quot;thread estratégico&quot;.** Lembre às equipes que cada projeto deve ser um &quot;conta&quot; em uma sequência estratégica.

* **Automatize a entrega.** Use automações para acionar a criação de projetos e economizar tempo e esforço, além de melhorar a conectividade e a governança de dados.

* **Link, não duplicar.** Use campos de pesquisa para exibir dados de execução em tempo real (como status ou datas de conclusão) em seus registros estratégicos. Isso garante que suas visualizações estratégicas sejam sempre precisas, sem precisar de atualizações manuais da equipe.



### Não:

* **Não trate registros de planejamento como listas de tarefas.** A ponte foi projetada para conectar intenção estratégica a projetos de execução. Mantenha seus registros de planejamento focados no &quot;o que&quot; e no &quot;por quê&quot; e permita que o módulo de fluxo de trabalho lide com o &quot;como&quot; detalhado de tarefas e problemas.

* **Não sincronize em excesso.** Você não precisa sincronizar todos os detalhes no nível do projeto novamente com o Planning. Mantenha a camada estratégica de alto nível e sem ruído.

* **Não ignore a ponte.** Se o trabalho começa no módulo Fluxo de Trabalho sem um link para o Planning, você criou um &quot;Plano Sombra&quot; que é invisível para a liderança.




