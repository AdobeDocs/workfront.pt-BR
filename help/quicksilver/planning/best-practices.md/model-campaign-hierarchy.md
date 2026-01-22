---
title: 'A estrutura do sucesso: Modelar a hierarquia da campanha'
description: Saiba como traduzir seus complexos processos de negócios em uma hierarquia de campanha escalável e controlada usando "Centros de gravidade" e uma arquitetura com vários espaços de trabalho.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 54a6e633e903c73a78b36e90fb27edb445dc8d47
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---


# A estrutura para o sucesso: modelar a hierarquia da campanha

<!--see the file again for additional comments from Seth and others-->

## Meta

Saiba como traduzir seus complexos processos de negócios em uma hierarquia de campanha escalável e controlada usando &quot;Centros de gravidade&quot; e uma arquitetura com vários espaços de trabalho.



## Visão geral

À medida que suas operações de marketing aumentam, a complexidade dos dados também aumenta. Sem um blueprint claro, seu Sistema de Registro de Marketing (MSOR) pode se tornar rapidamente uma &quot;gaveta de lixo&quot; de registros desconectados, terminologia conflitante e silos de relatórios.



O &quot;Blueprint of Success&quot; é uma estrutura para modelagem da hierarquia de campanha no Workfront Planning. Ela muda seu sistema de &quot;caos nas planilhas&quot; para um modelo governado e orientado a objetos que garante que todas as equipes falem a mesma linguagem, mantendo a agilidade que precisam para executar.



## A Hierarquia: Localizando Seus Níveis de Intenção

Para manter a clareza e a escalabilidade, recomendamos começar com um **Caminho principal** comprovado. Embora as organizações possam expandir essa hierarquia à medida que suas necessidades operacionais evoluem, começar com esses três níveis garante uma ponte forte entre a estratégia e a execução.



### O caminho principal: estratégia para ação

A maioria das implementações bem-sucedidas prospera com um modelo limpo de três níveis que abrange o planejamento e o fluxo de trabalho:



1. **Nível 1: Campanhas (Módulo de Planejamento)**

   * **Foco:** pilares estratégicos de longo prazo e iniciativas anuais (por exemplo, &quot;Reconhecimento Global da Marca no Ano Fiscal 26&quot;).

   * **Pessoa:** CMO, VP de Marketing, Líderes estratégicos.

2. **Nível 2: Táticas de Canal (Módulo de Planejamento)**

   * **Foco:** Os resumos operacionais que definem o &quot;quê&quot; de canais específicos (por exemplo, &quot;Q1 Social Media Blitz&quot;). Esta é a camada final de intenção estratégica antes do início do trabalho.

   * **Pessoa:** Operações De Marketing, Clientes Potenciais De Canal, Gerentes De Campanha.

3. **Nível 3: Projetos de Fluxo de Trabalho (Módulo de Fluxo de Trabalho)**

   * **Foco:** A execução real de &quot;Experiências&quot; ou &quot;Atividades&quot; (por exemplo, postagens sociais específicas, emails, páginas da Web).

   * **Implementação:** as táticas em planejamento vinculam-se diretamente aos **Projetos** no módulo de Fluxo de Trabalho, onde os resultados individuais são gerenciados como tarefas e problemas.

   * **Pessoa:** Criativos, Colaboradores Individuais.



### Expansão Estratégica: Adicionar Mais Níveis

Depois que o caminho principal é estabelecido, as organizações podem optar por adicionar mais camadas após uma consideração cuidadosa de sua complexidade de negócios específica:



* **Planos de canal:** Uma camada entre *Campanhas* e *Táticas* para agrupar estratégias multifuncionais (por exemplo, &quot;Estratégia Digital&quot;).

* **Atividades de planejamento do Workfront:** em ambientes de volume inferior (normalmente &lt;5.000 entregas/ano), algumas equipes preferem rastrear &quot;Experiências&quot; individuais como registros do Workfront Planning antes de se tornarem projetos.


>[!TIP]
>
>**Dica Crucial: O Limite De 5.000 Entregáveis**
>
>Se sua organização produz mais de 5.000 atividades por ano, você deve **sempre** descarregar o rastreamento de entrega individual para o **módulo de fluxo de trabalho**. O gerenciamento de registros de &quot;Experiência&quot; de alto volume no Planning pode levar a um acúmulo de dados que obscurece sua visibilidade estratégica. Use o Planning para o &quot;Por que&quot; e &quot;O que&quot; e o módulo Workflow para o &quot;Como&quot; de alto volume.



## Arquitetura: Centros de gravidade

Um MSOR de nível empresarial não está integrado a um único espaço de trabalho. Ele usa uma arquitetura &quot;Hub-and-Spoke&quot; onde os tipos de registros são gerenciados em seus **Centros de Gravidade** naturais.



### &#x200B;1. O Hub de Taxonomia (Classificações)

Estabeleça um espaço de trabalho centralizado para suas &quot;Classificações globais&quot; (por exemplo, Marcas, Regiões, Produtos, Personalidades).

* **Local Principal:** Este espaço de trabalho é a &quot;Source da Verdade&quot; para esses objetos.

* **O benefício:** ao agregar essas definições ao restante da empresa, você soluciona o &quot;Desvio semântico&quot;, garantindo que &quot;Região: EMEA&quot; tenha o mesmo significado para todas as equipes.



### &#x200B;2. O Workspace de Planejamento Estratégico (Centro Executivo)

Aqui é onde residem as **Campanhas** de alto nível (e quaisquer **Planos de Canal**).

* **Local principal:** este é o centro de gravidade executivo, proporcionando um ambiente sem ruídos para a tomada de decisões estratégicas.

* **O benefício:** A liderança pode gerenciar o portfólio sem ver a bagunça tática do dia a dia.



### &#x200B;3. Raios funcionais (espaços de trabalho de equipe)

As unidades funcionais (Social, Creative, Email) têm seus próprios espaços de trabalho para gerenciar suas **Táticas**.

* **Local Principal:** Esses espaços de trabalho são o centro de gravidade para a execução da equipe local.

* **O benefício:** as equipes &quot;consomem&quot; as campanhas e classificações globais dos hubs, enquanto mantêm seus próprios objetos locais (como *Meios de Comunicação* ou *Direitos de Uso*).



## Governança baseada em substantivos: fale um idioma

Para garantir que seu blueprint se mantenha pressionado, siga o princípio de **Governança baseada em substantivos**.



* **Usar substantivos, não verbos:** Nomeie os tipos de registro após as &quot;coisas&quot; que você está rastreando (`Campaign`, `Tactic`), não as &quot;ações&quot; (`Campaigning`, `Planning`).

* **Nomenclatura Padronizada:** Use os mesmos nomes em todos os espaços de trabalho. Isso permite agregar dados em todo o portfólio para a geração de relatórios executivos.



## E os portfólios e programas existentes?

Uma pergunta comum para organizações maduras é como lidar com os Portfólios e Programas que elas já criaram no **módulo de Fluxo de Trabalho**. No passado, esses objetos eram frequentemente usados para imitar o planejamento estratégico.



### &#x200B;1. Portfólios e programas → Tipos de registros

Em muitas organizações, os **Portfólios** são usados para representar marcas ou unidades de negócios (BUs) de alto nível, enquanto os **Programas** representam temas estratégicos.

* **O Turno:** São melhor modelados como **Tipos de Registro** no **Hub de Taxonomia**. Ao tratar &quot;Marca&quot; ou &quot;Unidade de negócios&quot; como um tipo de registro, é possível vinculá-los a qualquer campanha ou tática em toda a empresa, fornecendo relatórios muito mais flexíveis do que uma estrutura estática de Portfolio/Programa.



### &#x200B;2. Estratégia &quot;Reporting Bridge&quot;

Embora o Workfront Planning seja o futuro da intenção estratégica, seus relatórios nativos por meio dos **Painéis do Canvas** ainda estão amadurecendo. Muitas organizações ainda dependem dos recursos robustos de relatórios vinculados às estruturas herdadas do Portfolio e do Programa no módulo Fluxo de trabalho.

* **A recomendação:** não exclua seus Portfólios e Programas ainda. Em vez disso, use as **Automações de fusão** para criar uma ponte.

* **Como funciona:** Quando uma Tática ou Campanha é criada no Workfront Planning, o Fusion pode espelhar automaticamente esse registro em um Portfolio ou Programa correspondente no módulo de Fluxo de Trabalho. Isso permite:

   1. Aproveite a **visualização estratégica** superior do Workfront Planning (Linhas do tempo/Calendários).

   2. Mantenha seus **relatórios herdados** no módulo de fluxo de trabalho para os participantes que ainda não estão prontos para ir para o Canvas.

## Práticas recomendadas e dicas

### Faça:

* **Primeiro, mantenha o Caminho Principal.** Estabeleça o fluxo de Campanha para Tática para Projeto antes de adicionar mais complexidade.

* **Designar Espaços de Trabalho Primários.** Verifique se cada tipo de registro tem um espaço de trabalho &quot;inicial&quot; (seu centro de gravidade) que atue como agregador para relatórios.

* **Priorizar Forms para Entrada.** Use formulários de registro para grupos com menos sofisticação no Workfront Planning para garantir a integridade dos metadados. Embora os usuários avançados possam se beneficiar da entrada direta de dados nas visualizações de tabela, isso deve ser abordado com cuidado, pois alterações em massa em uma tabela podem facilmente criar problemas de dados para outras partes interessadas.


### Não:

* **Não diga &quot;principal&quot;.** Consulte especificamente os objetos **Módulo de fluxo de trabalho** e **Projeto** ao falar sobre execução.

* **Não complique demais.** Cada nível adicional de hierarquia adiciona um &quot;imposto de gerenciamento&quot;. Adicione apenas níveis que respondam a uma pergunta comercial que você não pode responder no momento.

* **Não criar silos.** Verifique se os tipos de registro são compartilhados entre espaços de trabalho para que as equipes não redigitem os mesmos dados.




